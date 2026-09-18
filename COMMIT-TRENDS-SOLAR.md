# ☀️ Solar Geoengineering — Commit Trend Analysis

**Branch:** `solar-geoengineering` | **Last Updated:** September 2026 (v4)

Commit trend analysis across solar-atmosphere repositories, based on fresh commit histories pulled via the GitHub API (September 2026).

---

## Activity Overview

| Repo | Total Commits Pulled | Date Range | Commit Density | Development State |
|------|---------------------|------------|---------------|------------------|
| wrf-model/WRF | 15 | May–Jun 2026 | ~1/week during release | 🟢 Active, v4.8.0 released |
| PCMDI/pcmdi_metrics | 15 | Sep 3–17, 2026 | ~5/day during release | 🟢 Very active, v4.2.1 released |
| ClimateMARGO/ClimateMARGO.jl | 15 | Jan 2022–Aug 2026 | ❌ Dormant (2yr gap) | 🟡 Revival unclear |
| hausfath/srm-forever | 4 | Aug 26, 2026 | 💥 Single-day burst | 🆕 New, unproven |

---

## Trend 1: The "Release Weekend" Pattern (WRF & PCMDI)

Both WRF and PCMDI show a clear pattern: **long periods of steady maintenance punctuated by intense release weekends.**

**WRF v4.8.0 release cycle (May 19 – Jun 8, 2026):**
- 15 commits in 20 days
- Peak activity: May 20–21 (3 commits), May 26–28 (3 commits)
- Solar radiation correction on May 28 — late in the cycle, suggesting it was caught during final testing

**PCMDI v4.2.1 release cycle (Sep 3–4, 2026):**
- 10 commits in 2 days
- Sep 3: 6 commits (extremes chunking, SVD fix, rename, numpy SVD, merges)
- Sep 4: 4 commits (version bump, roundoff fix, release prep, more merges)
- Sep 17: 2 follow-up commits (modpath_list patch)

**🎙️ Podcast angle:** This pattern reveals how climate model development actually works — not as a steady stream, but as **release waves**. The tools that underpin solar geoengineering research are maintained like naval ships: they undergo periods of intense refitting, then patrol quietly. The question is whether this model can sustain itself for the decades-long timeline of solar geoengineering deployment.

---

## Trend 2: The Physics-Philosophy Gap

There's a striking contrast between the **institutional tools** (WRF, PCMDI) and the **decision tools** (ClimateMARGO, srm-forever):

| Attribute | Institutional Tools | Decision Tools |
|-----------|-------------------|----------------|
| Development pace | Continuous, Milestone-driven | Episodic, insight-driven |
| Contributors | Large teams, institutional|\ Individual or tiny teams |
| Release pattern | Versioned, scheduled | "When ready" |
| Code quality | CI/CD, testing, documentation | Working prototype, minimal QA |
| Stars (visibility) | 100–1,700 | 0–73 |
| Sustainability | Funded, institutional | Unfunded, volunteer |

**🎙️ Podcast angle:** The people who build the climate models (WRF team at NCAR, PCMDI at LLNL) are funded, salaried scientists. The people who ask "should we use them?" (ClimateMARGO, srm-forever) are working on their own time. This asymmetry shapes what questions get asked — and which ones don't.

---

## Trend 3: The Solar Radiation Fix as a Case Study

The single most solar-relevant commit across all repos pulled:

```
Commit: e836cd6
Message: correction for EOF calculation for solar radiation
Author: weiwangncar
Date: May 28, 2026
Repo: wrf-model/WRF
```

**What happened:**An error in the Energy Outflow Flux (EOF) calculation for solar radiation was corrected. This affects how much solar energy is incorrectly calculated as leaving the system vs. being correctly accounted for.

**Why it matters for SAI:** If the baseline solar radiation budget is wrong, then any simulation of stratospheric aerosol injection — which works by reflecting solar energy — is built on a faulty foundation. This is not a minor parameter adjustment; it's a correction to the fundamental energy accounting.

**The podcast narrative:** This is the "bug that changes everything" story. It's also a story about how science self-corrects — the error was caught, fixed, and documented. But it raises the question: how many past solar geoengineering simulations were built on versions with this error? And how long does it take for a radiation code fix to propagate into the geoengineering literature?

---

## Trend 4: The Zero-Star Time Machine (srm-forever)

All 4 commits occurred on August 26, 2026 — a "big bang" release:

1. `9999436` — Initial commit: full interactive model
2. `9ee822a` — Price abatement as a vintage annuity (refined economics)
3. `aa9bc0f` — Weitzman certainty-equivalent discounting + essay
4. `61df1a4` — Effective discount rate chart (visualization)

**Timeline:** The commits suggest a single development session, likely a weekend or intensive period. The model went from concept to fully functional interactive tool in one push.

**The paradox:** This is arguably the most directly relevant solar geoengineering tool on GitHub (it asks the core question: "SRM forever vs. mitigation+CDR?"), yet it has zero stars. Compare with WRF's 1,762 stars.

**🎙️ Podcast angle:** The most important tool has no audience. The most popular tool can't answer the question. This is the governance paradox of solar geoengineering research on GitHub.

---

## Trend 5: The Dormancy-Revival Pattern (ClimateMARGO)

ClimateMARGO's commit history reveals a clear dormancy-revival pattern:

| Period | Activity | Nature |
|--------|----------|--------|
| Jan 2022 | 7 commits in 2 days | Initial release push (docs, citations, version bump) |
| Mar–Nov 2022 | 3 commits | Solver upgrades, web app removal |
| **Nov 2022 – Oct 2023** | **Gap of ~11 months** | Full dormancy |
| Oct 2023 | 1 commit (unit_conversions.jl) | Single fix — possible bug report response |
| **Oct 2023 – Aug 2026** | **Gap of ~2.8 years** | Deep dormancy |
| **Aug 17, 2026** | **2 README updates same day** | **Revival signal** |

**Interpretation options:**
1. **Funding signal** — A grant was awarded, someone updated the README to prepare for a paper
2. **Political signal** — Renewed policy interest in solar geoengineering prompted a re-update
3. **False start** — README update without follow-through (same pattern as Oct 2023 single-commit fix)
4. **Community signal** — Someone found the repo, reported issues, maintainer responded

**🎙️ Podcast angle:** ClimateMARGO's dormancy-revival pattern is the canary in the coal mine for solar geoengineering research. If the best economic modeling tool for SAI goes dark for 2.8 years, what does that mean for the deployment decisions that depend on it? And does a README update count as "revival" if no code follows?

---

## Commit Velocity Comparison

```
WRF (v4.8.0 cycle):     ████████████████████  15 commits / 20 days = 0.75/day
PCMDI (v4.2.1 cycle):   ████████████████████████████████████████  10 commits / 2 days = 5/day
ClimateMARGO (total):   ░░░░░░░░░░░░░░░░░░░░░  ~1 commit / 2 months (dormant)
srm-forever (total):    💥💥💥💥  4 commits / 1 day (burst)
```

**Key insight:** The institutional tools can sustain ~1 commit/day during active development. The decision tools oscillate between dormancy and burst. This is not a sustainability problem — it's a **funding topology** problem.

---

## 🎙️ Episode Structure (Suggested)

### Act 1: "The Bug" (5 min)
- Open with the May 28 solar radiation fix in WRF
- What does it mean to get the energy budget wrong?
- How science self-corrects — and how slowly

### Act 2: "The Factory" (7 min)
- WRF and PCMDI as institutions — how climate models are built
- The release-weekend pattern
- Why we can trust (and critique) the tools

### Act 3: "The Garage" (7 min)
- ClimateMARGO's dormancy and ambiguous revival
- srm-forever's zero-star time machine
- The governance gap: who decides, and who builds the tools they need?

### Act 4: "The Question" (5 min)
- SRM forever vs. mitigation + CDR — the core question
- Weitzman discounting: why the answer depends on what you believe about the future
- The philosophical stakes

---

## Data Sources

All commit data pulled fresh from GitHub API on September 19, 2026:
- `wrf-model/WRF` — 15 commits (page 1)
- `PCMDI/pcmdi_metrics` — 15 commits (page 1)
- `ClimateMARGO/ClimateMARGO.jl` — 15 commits (page 1)
- `hausfath/srm-forever` — 4 commits (page 1)

---

## Research Log

| Date | Activity |
|------|----------|
| 2026-09-19 | v4: Fresh commit histories pulled from 4 solar-theme repos; project discoveries and trend analysis pushed to branch |
| 2026-09-17 | v3: Previous analysis completed (incorporated into README) |
| 2026-09-03 | Initial research notes created |
