# ☀️ Solar Geoengineering — Project Discoveries

> **Episode Theme:** Solar Geoengineering (SRM / Marine Cloud Brightening / Albedo Modification)
> **Last Updated:** September 2026
> **Sources:** GitHub API commit pulls from 5 repositories

---

## Overview

Solar geoengineering on GitHub is defined by a stark divide: **massive, institutional, continuously funded atmospheric models** vs. **tiny, individual, theoretical or niche tools**. There is no mid-tier — no community-maintained SRM simulation toolkit, no open-source wave-altitude controller, no collaborativemarine cloud brightening platform.

---

## Repository Profiles

### 1. wrf-model/WRF — The Colossus

| Field | Value |
|-------|-------|
| **Stars** | 1,761 |
| **Language** | Fortran |
| **Last Commit** | June 8, 2026 (v4.8.0 release) |
| **License** | Apache 2.0 |
| **Contributors** | 50+ active |

**What it is:** The Weather Research and Forecasting model — the foundational atmospheric simulation tool used by NOAA, NASA, and virtually every national weather service on Earth. Not *specifically* a geoengineering model, but it is the **primary tool** through which SRM simulations are conducted.

**Why it matters for the podcast:** When scientists simulate stratospheric aerosol injection or marine cloud brightening, they run WRF (or its regional configuration WRF-Chem). Understanding WRF's development trajectory tells us about the *infrastructure* of solar geoengineering research.

**Recent commits (10 pulled):**
- `06d4240` — Merge release-v4.8.0 (Jun 8, 2026)
- `0708348` — README & version update to v4.8.0 (Jun 6, 2026)
- `6a289e1` — Turn off tempo_aerosolaware & tempo_hailaware in Registry (Jun 5, 2026)
- `4466746` — Fix vectorization option in AOCC stanza (May 30, 2026)
- `e836cd6` — **Correction for eOT calculation for solar radiation** (May 28, 2026)
- `8299919` — Updating MYNN-EDMF pointer, removing icloud_bl package (May 27, 2026)
- `4fab0e2` — Update MMM-physics repo SHA with fixes (May 27, 2026)
- `75ad1f9` — Fixing CDXWRF module (May 26, 2026)
- `0aa6582` — README for GFL option (May 26, 2026)
- `02f02bc` — Include mp_physics=88 in TEMPO error print (May 21, 2026)

**🎙️ Episode hook:** "TheSolar radiation correction commit (e836cd6) is a perfect metaphor for this entire field — scientists constantly adjusting how they measure the sun's energy, while politicians argue about whether to block it. WRF's maintenance rhythm — weekly physics fixes, quarterly releases — shows that solar geoengineering simulation is *engineering*, not science fiction."

---

### 2. ClimateMARGO/ClimateMARGO.jl — The Revival Signal

| Field | Value |
|-------|-------|
| **Stars** | 73 |
| **Language** | Julia |
| **Last Commit** | Aug 17, 2026 (README update after 2+ year dormancy) |
| **License** | MIT |
| **Contributors** | 2 primary (Fons van der Plas, Henri Drake) |

**What it is:** An idealized climate-economic modeling framework for optimizing trade-offs between emissions mitigation, adaptation, and solar geoengineering. Built in Julia for speed.

**Why it matters:** ClimateMARGO bridges the gap between pure climate models (WRF) and economic models (DICE). It asks: "Given that we *might* deploy SRM, what's the optimal policy response?"

**Recent commits (10 pulled):**
- `d916f36` — Update README.md (Aug 17, 2026) ⚡ **REVIVAL**
- `6d9ba7a` — Update README.md (Aug 17, 2026) ⚡ **REVIVAL**
- `57d4da7` — Update unit_conversions.jl with comment from #86 (Oct 18, 2023)
- `fbbe619` — Add link to Pluto in README (Jul 6, 2023)
- `5063c42` — Update Project.toml (Nov 14, 2022)
- `12a0ce6` — JuMP and Ipopt compat upgrade (Nov 12, 2022)
- `32e66fd` — Removed deprecated web apps (Feb 10, 2022)
- `d609d49` — Added CITATION.bib (Feb 4, 2022)
- `b2d9228` — Fixed typo (Jan 13, 2022)
- `8a7e012` — Updated arguments for doc version deployment (Jan 12, 2022)

**🎙️ Episode hook:** "Two README updates in August 2026 after two and a half years of silence. No code commits. Just documentation. Is ClimateMARGO waking up, or is someone polishing the tombstone? This is the ambiguity that defines small-team climate modeling — you can never tell if a revival is real or rhetorical."

---

### 3. PCMDI/pcmdi_metrics — The Evaluation Infrastructure

| Field | Value |
|-------|-------|
| **Stars** | 133 |
| **Language** | Python |
| **Last Commit** | Sep 4, 2026 |
| **License** | Apache 2.0 |

**What it is:** CMIP6 model evaluation toolkit. It doesn't simulate geoengineering — it **grades** the models that do. Every SRM simulation study must pass through PCMDI metrics to be published.

**Why it matters:** Governance through evaluation. If you can't measure the effectiveness of a geoengineering intervention, you can't regulate it. PCMDI is the unintentional governance infrastructure.

**🎙️ Episode hook:** "The most important tool in solar geoengineering isn't a simulation — it's a rubric. PCMDI decides what 'good' looks like, and right now, there's no rubric for 'was the SRM experiment successful.'"

---

### 4. NOAA-GFDL/MDTF-diagnostics — The Process Drill-Down

| Field | Value |
|-------|-------|
| **Stars** | 80 |
| **Language** | Jupyter Notebook |
| **Last Commit** | Aug 14, 2026 |
| **Key feature** | Precipitation-buoyancy POD (Process-Oriented Diagnostic) |

**What it is:** Analysis framework for weather and climate simulations with process-oriented diagnostics. The **precipitation-buoyancy POD** (added Jun 19, 2026 — 5 commits in one day) is the most ocean-relevant diagnostic in open source.

**Recent commits (10 pulled):**
- `87f8105` — Merge PR #825 from weiming9115/main (Aug 14, 2026)
- `4cfc99c` — Update MCS_precip_buoy_stats.rst (Jun 19, 2026)
- `699de27` — Update MCS_precip_buoy_stats.rst (Jun 19, 2026)
- `d6bc6d0` — Update MCS_precip_buoy_stats.rst (Jun 19, 2026)
- `3904d29` — Update MCS_precip_buoy_stats.rst (Jun 19, 2026)
- `33024ad` — **Add MCS precipitation-buoyancy statistics POD** (Jun 19, 2026)
- `2df59f6` — Merge PR #823 (Jun 8, 2026)
- `16f936c` — Update README (Jun 8, 2026)
- `b96127e` — Update README.md (Jun 8, 2026)
- `97b3028` — Merge branch NOAA-GFDL:main (Jun 2, 2026)

**🎙️ Episode hook:** "Five commits on June 19th, 2026, all to the same file: MCS_precip_buoy_stats.rst. That's not typical open-source behavior — that's a sprint. Someone needed that diagnostic *fast*. And it's about precipitation and buoyancy, which means it's about how clouds form, how rain falls, and how the atmosphere responds to perturbation. Which is exactly what you need to predict what happens when you inject aerosols into the stratosphere."

---

### 5. hausfath/srm-forever — The Theoretical Edge Case

| Field | Value |
|-------|-------|
| **Stars** | 0 |
| **Language** | Unknown (likely Python/Julia) |
| **Last Commit** | Aug 26, 2026 |
| **License** | Likely CC0 |

**What it is:** Interactive SRM economics model applying **Weitzman certainty-equivalent discounting** to SRM cost dynamics. It asks: "What does it cost to keep solar geoengineering going *forever*?"

**Why it matters:** This is the philosophical counterpoint to WRF's engineering. While WRF simulates the atmosphere, srm-forever simulates the *commitment*. It's about the intergenerational debt of continuously maintaining an intervention.

**🎙️ Episode hook:** "Zero stars. But conceptually, this might be the most important repo in this entire episode. Weitzman discounting applied to SRM — it's not asking 'does SRM work?' It's asking 'are we willing to pay to keep it working forever?' And the answer, mathematically, might be no."

---

## 🔍 Cross-Cutting Themes for Solar Episode

| Theme | Evidence |
|-------|----------|
| **Infrastructure over innovation** | WRF (1,761★) dominates; SRM-specific tools are niche |
| **Physics corrections > new features** | WRF's most notable recent commit is a *solar radiation correction* |
| **Dormancy + revival pattern** | ClimateMARGO's 2-year silence + 2 README updates |
| **Governance-through-evaluation** | PCMDI & MDTF define what "good" means |
| **Theoretical vs. practical** | srm-forever (0★, Weitzman economics) vs. WRF (1,761★, operational) |
| **No open-source SRM controller** | Zero repos for interactive SRM decision-making tools |

---

## 📋 Episode Talking Points

1. **Opening:** "The most sophisticated solar geoengineering simulation software on Earth runs on Fortran, is maintained by a government lab, and has 1,762 stars. The most important question it can't answer is whether we should use it."

2. **The correction commit:** WRF's May 2026 solar radiation fix (e836cd6) — science is iterative, even for the tools we use to predict the future.

3. **The revival:** ClimateMARGO's August 2026 README updates after 2+ years of silence. What does it mean when a climate model wakes up?

4. **The invisible governance:** PCMDI and MDTF don't simulate geoengineering — they evaluate it. And evaluation is a form of power.

5. **The philosophical edge:** srm-forever asks the question no one wants to answer: what's the cost of *perpetual* intervention?

6. **Closing:** "We can simulate the atmosphere down to the millimeter. We can't simulate the politics. That gap is the episode."
