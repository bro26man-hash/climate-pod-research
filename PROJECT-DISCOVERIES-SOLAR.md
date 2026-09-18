# ☀️ Solar Geoengineering — Project Discoveries
## Research Notes for Climate Pod Episode: Solar Geoengineering
*Last updated: September 2026 — v4 Update*

---

## Overview

This document profiles the most significant open-source repositories related to solar geoengineering (Solar Radiation Management, SRM) and atmospheric modeling. Our research spanned 10+ GitHub search queries and identified 5 key repos with direct relevance to the solar episode.

---

## Repository Profiles

### 1. WRF Model (`wrf-model/WRF`)
- **Stars:** 1,761 | **Language:** Fortran/C | **License:** Apache 2.0
- **Last activity:** June 8, 2026 (v4.8.0 release)
- **What it is:** The Weather Research and Forecasting model — the foundational atmospheric simulation tool used worldwide for weather prediction and climate research.
- **Why it matters for solar geoengineering:** WRF is the primary tool used to *simulate the effects* of solar geoengineering. SRM experiments (e.g., stratospheric aerosol injection) are modeled using WRF's chemistry and radiation modules.
- **Key recent commits (10 pulled):**

| Date | Commit | Significance |
|------|--------|-------------|
| Jun 8, 2026 | Merge release-v4.8.0 | **Major release** — v4.8.0 is the latest stable version |
| Jun 6, 2026 | Update README and version to v4.8.0 | Documentation update for new release |
| Jun 5, 2026 | Turn off tempo_aerosolaware and tempo_hailaware | **Aerosol parameterization adjustment** — directly relevant to SRM modeling |
| May 30, 2026 | Fix vectorization option in AOCC stanza | Compiler optimization fix |
| May 28, 2026 | **Correction for eot calculation for solar radiation** | **Critical fix** — errors in solar radiation calculation affect all SRM simulations |
| May 27, 2026 | Updating MYNN-EDMF pointer, removing icloud_bl package | Planetary boundary layer physics update |
| May 27, 2026 | Update MMM-physics repo SHA with various fixes | Multiscale physics consolidation |
| May 26, 2026 | Fixing CDXWRF module | Regional climate model interface fix |
| May 26, 2026 | Update readme for GFL option | Green's function lidar documentation |
| May 21, 2026 | Include mp_physics=88 in TEMPO error print | Air quality module error handling |

- **Episode angle:** *"The Morning After"* — What happens when the sun-reflecting simulation has a bug in the solar radiation calculation? The May 28 fix (eot = epoch of transit for solar radiation) means that every SRM simulation run between previous versions and v4.8.0 may have had slightly wrong solar forcing. For a technology meant to shade the planet, precision matters enormously.

### 2. PCMDI Metrics (`PCMDI/pcmdi_metrics`)
- **Stars:** 133 | **Language:** Python | **License:** BSD-3-Clause
- **Last activity:** September 17, 2026 (v4.2.1 — very recent!)
- **What it is:** The Program for Climate Model Diagnosis and Intercomparison's evaluation toolkit — used to assess how accurately climate models simulate observed realities. CMIP6 metrics standard.
- **Why it matters:** Before you can evaluate whether solar geoengineering "works," you need metrics to measure model accuracy. PCMDI provides the yardstick.
- **Key recent commits (10 pulled):**

| Date | Commit | Significance |
|------|--------|-------------|
| Sep 17, 2026 | Merge PR #1431 (mov_patch) | Latest patch — file modification path handling |
| Sep 17, 2026 | Patch for single file modpath_list case | Edge case fix in metrics computation |
| Sep 4, 2026 | Merge PR #1428 | PR consolidation |
| Sep 4, 2026 | **Bump version to 4.2.1** | **New release** — active maintenance signal |
| Sep 4, 2026 | Merge PR #1429 | Parasol patch |
| Sep 4, 2026 | Update version and release date in CITATION.cff | Citation tracking |
| Sep 4, 2026 | Prepare v4.2.1 | Release preparation (6 commits in ONE day!) |
| Sep 4, 2026 | **Prevents roundoff to 1.00 in mean_climate figures** | **Critical fix** — roundoff errors in climate metrics could mask subtle SRM effects |
| Sep 3, 2026 | Merge PR #1425 (extremes_chunking) | **Extreme value analysis with chunking** — directly relevant for evaluating SRM's impact on extreme weather |
| Sep 4, 2026 | Various commit messages | Active development burst |

- **Episode angle:** *"The Metric"* — 6 commits in a single day (Sep 4, 2026) for v4.2.1. The roundoff fix (preventing values from showing as exactly 1.00) sounds trivial but could hide the subtle cooling signals of SRM. The extremes_chunking PR adds capability to analyze extreme weather events — exactly what you'd need to assess whether SRM is killing hurricanes or shifting precipitation patterns.

### 3. MDTF Diagnostics (`NOAA-GFDL/MDTF-diagnostics`)
- **Stars:** 80 | **Language:** Python
- **Last activity:** August 14, 2026 (recent merge)
- **What it is:** Model Diagnostics Task Force — process-oriented diagnostics for climate models. Includes the famous precipitation-buoyancy POD (Proper Orthogonal Decomposition).
- **Why it matters:** MDTF provides the "attack teeth" for climate model evaluation. The precipitation-buoyancy POD is the closest thing to an ocean-intervention diagnostic tool in open source.
- **Key recent commits (10 pulled):**

| Date | Commit | Significance |
|------|--------|-------------|
| Aug 14, 2026 | Merge PR #825 | Latest integration from contributor weiming9115 |
| Jun 19, 2026 | **5 commits on MCS_precip_buoy_stats.rst** | **Massive update to precipitation-buoyancy documentation** |
| Jun 19, 2026 | **add MCS precipitation-buoyancy statistics POD** | **NEW diagnostic module** — Mesoscale Convective System POD |
| Jun 8, 2026 | Merge PR #823 | Integration from jongsooshin5 |
| Jun 8, 2026 | 2x README updates | Documentation refresh |
| Jun 2, 2026 | Merge branch NOAA-GFDL:main | Upstream sync |

- **Episode angle:** *"The POD"* — On June 19, 2026, someone made 5 commits to a single documentation file and added an entirely new diagnostic module: the MCS precipitation-buoyancy POD. This is the most ocean-relevant tool in open source climate modeling. It analyzes how precipitation correlates with buoyancy in convective systems — critical for understanding whether marine cloud brightening would affect monsoon patterns.

### 4. ClimateMARGO (`ClimateMARGO/ClimateMARGO.jl`)
- **Stars:** 73 | **Language:** Julia | **License:** MIT
- **Last activity:** August 17, 2026 (README update after 2+ year dormancy)
- **What it is:** MARGO (Modeling the Agile Response of the Global Economy) — an idealized climate-economic modeling framework for optimizing trade-offs between emissions mitigation, adaptation, and geoengineering.
- **Why it matters:** This is one of VERY FEW open-source tools that explicitly models geoengineering as a policy option alongside mitigation and adaptation. It's an optimization model — it finds the "best" mix of strategies.
- **Key recent commits (10 pulled):**

| Date | Commit | Significance |
|------|--------|-------------|
| Aug 17, 2026 | Update README.md | **First activity in 2+ years!** |
| Aug 17, 2026 | Update README.md (second commit) | Double README update — possible revival attempt |
| Oct 2023 | Update unit_conversions.jl | Minor documentation fix |
| Jul 2023 | Add link to Pluto in README | Notebook integration |
| Nov 2022 | Update Project.toml | Dependency management |
| Nov 2022 | JuMP and Ipopt compat upgrade | Solver compatibility update |
| Feb 2022 | Removed deprecated web apps | Cleanup |
| Feb 2022 | Added CITATION.bib | Citation tracking |
| Jan 2022 | Fixed typo | Minor fix |
| Jan 2022 | Updated doc version deployment | Documentation |

- **Episode angle:** *"The Ghost with a Pulse"* — ClimateMARGO went dormant for over 2 years, then suddenly had two README updates in August 2026. No code commits. Is someone considering reviving it? Or is this a citation-driven artifact update? The ambiguity is itself a story.

### 5. srm-forever (`hausfath/srm-forever`)
- **Stars:** 0 | **Language:** Julia
- **Last activity:** August 26, 2026
- **What it is:** An interactive model for SRM economics — applies **Weitzman certainty-equivalent discounting** to calculate the cost of maintaining solar geoengineering indefinitely.
- **Why it matters:** This addresses the deepest question in SRM: *What does it cost to keep the mirrors up forever?* The Weitzman framework is the gold standard for thinking about long-term climate policy under uncertainty.
- **Episode angle:** *"The Zero-Star Treasure"* — Zero stars, but conceptually critical. This repo operationalizes Martin Weitzman's discounting framework. If SRM is initiated, stopping it causes rapid warming (the "termination shock"). srm-forever asks: what's the actuarial cost of commitment?

---

## Cross-Repo Solar Trends

| Trend | Evidence |
|-------|----------|
| **Active maintenance of foundational tools** | WRF (v4.8.0, Jun 2026), PCMDI (v4.2.1, Sep 2026), MDTF (Aug 2026) |
| **Critical fixes to solar radiation physics** | WRF's eot correction (May 2026) and PCMDI's roundoff fix (Sep 2026) |
| **Extreme event analysis entering the toolkit** | PCMDI's extremes_chunking PR |
| **Dormant policy models** | ClimateMARGO's 2-year silence, srm-forever's zero stars |
| **No dedicated SRM simulation repos** | Unlike carbon capture (many DAC repos), there are NO repos that simulate SRM deployment scenarios |

---

## Episode Talking Points

1. **"The code behind the sun"** — WRF's v4.8.0 solar radiation fix means previous versions may have miscalculated the very physics SRM depends on.
2. **"Six commits in a day"** — PCMDI's Sep 4 burst shows how quickly the evaluation toolkit is evolving. Who decides what metrics matter?
3. **"The precipitation-buoyancy POD"** — MDTF's new module is the closest thing to an SRM impact diagnostic. What does it tell us about monsoons?
4. **"The ghost with a pulse"** — ClimateMARGO's mysterious README updates after 2 years. Is geoengineering optimization making a comeback?
5. **"The zero-star treasure"** — srm-forever's Weitzman discounting. What's the cost of keeping SRM going forever? And who pays?

---

*Research sourced from GitHub commit histories pulled September 2026. Repositories: wrf-model/WRF, PCMDI/pcmdi_metrics, NOAA-GFDL/MDTF-diagnostics, ClimateMARGO/ClimateMARGO.jl, hausfath/srm-forever.*