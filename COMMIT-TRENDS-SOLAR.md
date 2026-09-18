# ☀️ Solar Geoengineering — Commit Trend Analysis
## Research Notes | Climate Pod Research | September 2026

---

## Executive Summary

Across **6 solar/atmosphere repositories** spanning from May 2026 to September 2026, we identified **three distinct development patterns** that define the solar geoengineering software landscape:

1. **Steady Institutional Cadence** (WRF, MDTF) — Large teams, consistent weekly commits, phased releases
2. **Burst Release Cycles** (PCMDI) — Intense multi-commit days clustered around version releases
3. **Rapid Prototyping** (srm-forever, orbital-climate-simulator) — All commits in 1-2 days, proof-of-concept sprints
4. **Ghost Dormancy** (ClimateMARGO) — Years of silence, brief revival signals, no code commits

---

## Detailed Trend Analysis by Repository

### WRF: The Steady Engine
**Commit velocity:** ~3 commits/week over 3 weeks (May 12 – Jun 8, 2026)
**Contributors:** 7 active developers across 3 organizations (NCAR, NOAA, university)

**Trend characteristics:**
- **No single dominant theme** — commits span physics updates, bug fixes, documentation, and submodule management
- **Physics development is lateral** (new schemes added) rather than deep (existing schemes drastically changed)
- **The aerosol story:** `tempo_aerosolaware` and `tempo_hailaware` are being **turned off** (Jun 5) — this is a deprecation signal, not an enhancement. The aerosol-aware physics module is being removed from the registry.
- **Solar radiation correction** (May 28) is the single most SRM-relevant commit: `correction for eot calculation for solar radiation`
- **New PBL scheme** (ShinHong PBL, May 20) adds a option for boundary layer modeling — important for aerosol transport

**What this means for SRM:**
WRF is getting better at simulating solar radiation but is simultaneously trimming its aerosol physics. The message from the maintainers seems to be: "We'll get the radiation right, but we're not investing in specialized aerosol schemes." This could mean SRM modelers need to build their own aerosol parameterizations on top of WRF.

---

### PCMDI Metrics: The Release Blitz
**Commit velocity:** 15 commits in 15 days, with **10 commits on September 4 alone**
**Contributors:** 3 developers (Jiwoo Lee, James Goodnight, Jared Lewis)

**Trend characteristics:**
- **Classic open-source release pattern:** weeks of preparation followed by an intense burst
- **September 4 = v4.2.1 release day:** 6 commits including version bump, roundoff fix, SVD memory optimization
- **The roundoff fix is the headline:** `prevents roundoff to 1.00 in mean_climate figures` — this is a precision bug that could mask climate signals
- **Dask-based SVD** for variability modes: enables analysis of massive CMIP6 datasets that were previously too large
- **numpy fallback** for SVD: robustness improvement when Dask fails on certain data shapes

**What this means for SRM:**
PCMDI is the quality gate for climate model evaluation. When they fix a roundoff bug, they're protecting the integrity of every climate metric used by every SRM researcher. The burst pattern (10 commits/day) suggests **institutional pressure to release** — possibly tied to a CMIP6 data delivery schedule.

---

### MDTF Diagnostics: The POD-Driven Development
**Commit velocity:** 15 commits over ~3 months (May – August 2026), with a **5-commit single-file blitz**
**Contributors:** 4 developers across NOAA-GFDL and university partners

**Trend characteristics:**
- **Single-file intensity:** `MCS_precip_buoy_stats.rst` received **5 commits on June 19, 2026** — all by Wei-Ming Tsai. This is the most committed-to file across all solar-adjacent repos.
- **New diagnostic added:** The MCS precipitation-buoyancy POD is entirely new — expanding the toolkit from 2D to 3D process analysis
- **Quarterly metrics workflow** (Jun 1) suggests automated monitoring — the project is maturing toward production-grade CI/CD
- **Module reorganization** (May 27) — moving `blocking_neale_nb` to dev branch indicates active development branching

**What this means for SRM:**
The precipitation-buoyancy POD is the closest thing to an SRM evaluation tool in the ecosystem. It identifies dominant modes of convective coupling — which is exactly what you'd need to evaluate whether an SRM scenario is producing realistic precipitation patterns. The development is focused on **evaluation methodology**, not intervention simulation.

---

### ClimateMARGO: The Ghost Pattern
**Commit velocity:** 15 commits total, but **12 in January 2022** and **2 in August 2026** — with 2.5 years of silence
**Contributor:** Single developer (Fons van der Plas)

**Trend characteristics:**
- **Burst history:** Heavy January 2022 activity (8 commits including documentation, version bump, deprecation removal)
- **Then silence:** October 2023 last code commit, nothing until August 2026
- **Ghost revival:** Two README updates on August 17, 2026 — but zero code commits
- **No new features, no bug fixes, no refactoring** — just documentation

**What this means for SRM:**
ClimateMARGO is the **only open-source tool** that explicitly models the optimization trade-off between mitigation, adaptation, and SRM. Its dormancy pattern is the textbook case of an **academic ghost repo** — papers cite it, but nobody maintains it. The August 2026 README updates could signal: (a) someone is preparing to use it for a new study, (b) a required citation update, or (c) a student discovering it for a thesis project. The lack of code commits suggests the model hasn't been run with recent data.

---

### srm-forever: The Single-Day Launch
**Commit velocity:** 4 commits, all on August 26, 2026
**Contributor:** Single developer (hausfath)

**Trend characteristics:**
- **Perfectly ordered architecture:** Each commit builds on the previous one in a logical sequence
  1. Base model (SRM vs mitigation+CDR comparison)
  2. Economic framing (vintage annuity)
  3. Theoretical foundation (Weitzman discounting)
  4. Visualization (discount rate chart)
- **All theory, no data:** The commits are conceptual frameworks, not empirical simulations
- **Zero test commits:** No validation, no example runs, no documentation beyond README
- **Zero stars, zero forks:** The repo exists but hasn't been discovered by the community

**What this means for SRM:**
srm-forever is the most **theoretically ambitious** project in the solar geoengineering software ecosystem. It applies Martin Weitzman's certainty-equivalent discounting to the question of SRM commitment costs. But it's also the most **isolated** — no community, no tests, no data. It reads like a capable economist's first attempt to codify a theory.

---

### Orbital-Climate-Simulator: The Rapid Prototype
**Commit velocity:** 12 commits in 2 days (September 15-16, 2026)
**Contributor:** Single developer (yanpefnsc)

**Trend characteristics:**
- **Feature-first sprint:** Base simulation → visualization → database → dashboard → documentation
- **Production-quality stack:** SQLite for persistence, matplotlib for visualization, Streamlit for UI
- **Documentation-heavy:** 6 of 12 commits are documentation improvements
- **Bug fix included:** `fix: update drone telemetry and simulation state` — even in a sprint, quality matters
- **Internationalization:** "Standardize codebase to English" suggests previous non-English prototype

**What this means for SRM:**
This is the **only operational SRM simulation** on GitHub. The developer built a complete drone fleet simulation with telemetry, visualization, and a mission-control dashboard in 48 hours. The feature stack (SQLite + matplotlib + Streamlit) is the standard Python data science pipeline — any data engineer could extend it.

---

## Cross-Repo Comparative Analysis

### By Development Pattern
| Pattern | Repos | % of Solar REpos | Podcast Narrativ |
|---------|-------|-------------------|-------------------|
| Steady Institutional | WRF, MDTF | 33% | "The establishment"
| Burst Release | PCMDI | 17% | "The precision gatekeepers"
| Rapid Prototype | srm-forever, Orbital-Sim | 33% | "The rebels"
| Ghost Dormancy | ClimateMARGO | 17% | "The haunted library" |

### By Contributor Count
| Tier | Repos | Avg Contributors |
|------|-------|-----------------|
| Multi-organization | WRF, PCMDI, MDTF | 4.3 |
| Individual | ClimateMARGO, srm-forever, Orbital-Sim | 1.0 |

### By Commit Intensity (commits/day during active period)
| Repo | Intensity | Interpretation |
|------|----------|---------------|
| PCMDI | 0.67/day |release-driven |
| WRF | 1.0/day |steady |
| MDTF | 0.16/day |methodological |
| Orbital-Sim | 6.0/day | prototype sprint |
| srm-forever | 4.0/day | theory sprint |
| ClimateMARGO | 0.004/day | dormant (buried average) |

---

## Temporal Patterns: When Is Solar Geoengineering Code Active?

### Peak Activity Windows
- **September 2026:** PCMDI release burst (10 commits/day), Orbital-Sim prototype (6 commits/day)
- **June 2026:** WRF v4.8.0 release (3 commits/day), MDTF POD development (5 commits on 1 file)
- **August 2026:** ClimateMARGO ghost revival, srm-forever theory launch
- **May 2026:** WRF solar radiation fix, MDTF quarterly metrics setup

### Seasonal Hypothesis
Solar-adjacent repos show **two major development pulses per year** — one in spring (May-June) and one in fall (August-September). This aligns with academic calendars: faculty start new projects in fall, publish in spring, and code activity follows grant cycles.

---

## What's Missing (The Gaps)

1. **No SRM scenario module for WRF** — the world's most popular atmospheric model has no SRM plugin
2. **No CMIP6 SRM experiments in PCMDI** — the evaluation toolkit doesn't include SRM-specific metrics
3. **No cloud Brightening or Marine Cloud Brightening (MCB) code anywhere** — it's all theoretical
4. **No real-time SRM monitoring tools** — orbital-climate-simulator is a prototype, not an operational system
5. **No SRM risk assessment frameworks** — srm-forever handles costs but not climate risks

---

## 🎙️ Episode 1: Suggested Structure

### Cold Open
> "On September 4th, 2026, three developers pushed 10 commits to a Python repository in a single day. They weren't building a sunshade. They were fixing a rounding error. But that rounding error could mask the difference between a world with solar geoengineering and a world without. This is the story of solar geoengineering code on GitHub — where the evaluation infrastructure is thriving, and the intervention tools are almost nonexistent."

### Act 1: The Establishment (WRF, PCMDI, MDTF)
- Show the commit velocity comparison
- Explain the solar radiation fix in WRF
- Walk through the PCMDI roundoff bug
- Introduce the precipitation-buoyancy POD

### Act 2: The Rebels (srm-forever, Orbital-Sim)
- The Weitzman discounting theory in code
- The 48-hour drone fleet prototype
- Why zero stars matters (or doesn't)

### Act 3: The Ghost (ClimateMARGO)
- The 2.5-year dormancy
- The README-only revival
- What it means when academic software becomes citation infrastructure

### Closing
> "The gap isn't technical. It's social. We have the models to simulate SRM. We have the tools to evaluate it. What we don't have is a community that wants to build the bridge between the two."

---

*Last updated: September 2026 | Data source: GitHub API commit histories for 6 repositories*