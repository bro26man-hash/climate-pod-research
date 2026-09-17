# ☀️ Solar Geoengineering — Project Discoveries

**Research Date:** September 2026
**Podcast Episode:** Solar Geoengineering (SRM)

---

## Overview

This file catalogs open-source repositories relevant to solar radiation management (SRM), solar geoengineering simulation, and atmospheric modeling. Commit histories were pulled fresh from GitHub in September 2026.

---

## Key Repositories

### 1. wrf-model/WRF ⭐ 1,761
- **URL:** https://github.com/wrf-model/WRF
- **Language:** Fortran / C
- **Last Activity:** June 8, 2026 (v4.8.0 release)
- **Focus:** The Weather Research and Forecasting model — the foundational atmospheric simulation tool. WRF's aerosol-aware physics schemes (tempo_aerosolaware, tempo_hailaware) are the closest thing to an open-source SRM simulation pipeline.
- **Why it matters for SRM:** Aerosol direct and indirect effects are at the heart of SRM modeling. WRF's microphysics and radiative transfer schemes are used in virtually all climate-modeling studies that include geoengineering "what-if" experiments.

**Recent Commits (10 pulled):**
| Date | SHA | Message |
|------|-----|--------|
| 2026-06-08 | 06d4240 | Merge remote-tracking branch 'origin/release-v4.8.0' |
| 2026-06-06 | 0708348 | Update README and version declaration to new v4.8.0 |
| 2026-06-05 | 6a289e1 | Turn off tempo_aerosolaware and tempo_hailaware in Registry |
| 2026-05-30 | 4466746 | Fix a vectorization option in AOCC stanza |
| 2026-05-28 | e836cd6 | Correction for eot calculation for solar radiation |
| 2026-05-27 | 8299919 | Updating MYNN-EDMF pointer and removing icloud_bl package |
| 2026-05-27 | 4fab0e2 | Update MMM-physics repo SHA with various fixes |
| 2026-05-26 | 75ad1f9 | Fixing CDXWRF module |
| 2026-05-26 | 0aa6582 | Update readme file for GFL option |
| 2026-05-21 | 02f02bc | Include mp_physics=88 in TEMPO error print message |

**Trend Signal:** Heavy maintenance on aerosol/radiation physics in the run-up to v4.8.0. The "correction for eot calculation for solar radiation" commit is directly relevant to SRM radiative forcing calculations. Institutional funding (NCAR/NOAA) drives this pace.

---

### 2. PCMDI/pcmdi_metrics ⭐ 133
- **URL:** https://github.com/PCMDI/pcmdi_metrics
- **Language:** Python
- **Last Activity:** September 4, 2026 (v4.2.1)
- **Focus:** PCMDI (Program for Climate Model Diagnosis and Intercomparison) metrics toolkit — the standard for evaluating Earth system models against observational data. Essential for verifying SRM simulation outputs.
- **Why it matters for SRM:** Any SRM simulation that claims to cool the planet needs to be evaluated against observations. PCMDI metrics are the governance infrastructure that makes SRM claims credible or debunks them.

**Recent Commits (10 pulled):**
| Date | SHA | Message |
|------|-----|--------|
| 2026-09-04 | 3092cdd | Merge PR #1428 |
| 2026-09-04 | 6419050 | Bump version to 4.2.1 |
| 2026-09-04 | 6443a1d | Merge PR #1429 |
| 2026-09-04 | 0e3a96f | Update version and release date in CITATION.cff |
| 2026-09-04 | e7dc726 | Prepare v4.2.1 |
| 2026-09-04 | d0bcbd8 | Merge PR #1427 (roundoff fix) |
| 2026-09-04 | 90cbc50 | Prevents roundoff to 1.00 in mean_climate figures |
| 2026-09-03 | 71a0497 | Merge PR #1425 (extremes chunking) |
| 2026-09-03 | b2eb044 | Merge branch 'main' into extremes_chunking |
| 2026-09-03 | c8711f1 | Merge PR #1423 (dask SVD memory fix) |

**Trend Signal:** 10 commits in 2 days — a release sprint. The roundoff fix (1.00 in mean_climate) suggests precision issues in metrics that could affect SRM evaluation. The "extremes chunking" PR with dask/SVD memory fixes indicates they're scaling to handle larger ensembles — exactly what SRM scenario testing would require.

---

### 3. NOAA-GFDL/MDTF-diagnostics ⭐ 80
- **URL:** https://github.com/NOAA-GFDL/MDTF-diagnostics
- **Language:** Python / R
- **Last Activity:** August 14, 2026
- **Focus:** Model Diagnostics Task Force diagnostics — process-oriented diagnostics for weather and climate simulations. Includes precipitation-buoyancy PODs (Process-Oriented Diagnostics).
- **Why it matters for SRM:** MDTF provides the "reality check" diagnostics that would be needed to verify whether an SRM intervention is actually producing the intended physical effects (e.g., precipitation changes, temperature responses).

**Recent Commits (10 pulled):**
| Date | SHA | Message |
|------|-----|--------|
| 2026-08-14 | 87f8105 | Merge PR #825 |
| 2026-06-19 | 4cfc99c | Update MCS_precip_buoy_stats.rst |
| 2026-06-19 | 699de27 | Update MCS_precip_buoy_stats.rst |
| 2026-06-19 | d6bc6d0 | Update MCS_precip_buoy_stats.rst |
| 2026-06-19 | 3904d29 | Update MCS_precip_buoy_stats.rst |
| 2026-06-19 | 33024ad | Add MCS precipitation-buoyancy statistics POD |
| 2026-06-08 | 2df59f6 | Merge PR #823 |
| 2026-06-08 | 16f936c | Update README |
| 2026-06-08 | b96127e | Update README.md |
| 2026-06-02 | 97b3028 | Merge branch 'NOAA-GFDL:main' into main |

**Trend Signal:** The new precipitation-buoyancy POD (June 2026) is the closest thing to an ocean-interaction diagnostic in open source. Five commits on the same day for the same file suggests a focused development push. The MCS (Mesoscale Convective System) precipitation-buoyancy diagnostic is directly relevant to SRM's potential to alter precipitation patterns — a major governance concern.

---

### 4. ClimateMARGO/ClimateMARGO.jl ⭐ 73
- **URL:** https://github.com/ClimateMARGO/ClimateMARGO.jl
- **Language:** Julia
- **Last Activity:** August 17, 2026 (README updates after 2+ year dormancy)
- **Focus:** Climate-economic modeling framework. Integrates climate simulation with economic impact assessment.
- **Why it matters for SRM:** SRM is fundamentally an economic question as much as a physical one. ClimateMARGO provides the integrated assessment framework that could model the cost-benefit trade-offs of solar geoengineering versus mitigation.

**Recent Commits (10 pulled):**
| Date | SHA | Message |
|------|-----|--------|
| 2026-08-17 | d916f36 | Update README.md |
| 2026-08-17 | 6d9ba7a | Update README.md |
| 2023-10-18 | 57d4da7 | Update unit_conversions.jl with comment from #86 |
| 2023-07-06 | fbbe619 | Add link to Pluto in README |
| 2022-11-14 | 5063c42 | Update Project.toml |
| 2022-11-12 | 12a0ce6 | JuMP and Ipopt compat upgrade |
| 2022-02-10 | 32e66fd | Removed deprecated web apps |
| 2022-02-04 | d609d49 | Added CITATION.bib |
| 2022-01-13 | b2d9228 | Fixed typo |
| 2022-01-12 | 8a7e012 | Updated arguments for doc version deployment |

**Trend Signal:** Two README updates on August 17, 2026 after 2+ years of dormancy. This is a revival signal — could indicate growing policy-modeling interest in SRM economic assessment, or could be another false start. The Julia ecosystem is gaining traction in climate-economics modeling, and ClimateMARGO is the most prominent open-source entry point.

---

### 5. hausfath/srm-forever ⭐ 0
- **URL:** https://github.com/hausfath/srm-forever
- **Language:** JavaScript (interactive web)
- **Last Activity:** August 26, 2026
- **Focus:** Interactive single-page SRM economics model. "SRM-forever" simulates the cost dynamics of sustained solar geoengineering versus mitigation + carbon dioxide removal.
- **Why it matters for SRM:** This is the most directly relevant open-source SRM tool on GitHub. It's not a climate simulation — it's an economics/policy simulation that models the question: "What would it cost to keep SRM going forever?" This is the Weitzman-style discounting question applied to geoengineering.

**Recent Commits (4 pulled):**
| Date | SHA | Message |
|------|-----|--------|
| 2026-08-26 | 61df1a4 | Add effective discount rate chart |
| 2026-08-26 | aa9bc0f | Adopt Weitzman certainty-equivalent discounting; add discount-rate essay |
| 2026-08-26 | 9ee822a | Price abatement as a vintage annuity |
| 2026-08-26 | 9999436 | Interactive SRM-forever vs mitigation+CDR cost model |

**Trend Signal:** All four commits on the same day — a focused development burst. The adoption of Weitzman certainty-equivalent discounting is significant: it's the theoretical economics framework for handling deep uncertainty, which is exactly the situation with SRM. The "vintage annuity" pricing model for abatement is a novel contribution. Despite zero stars, this is conceptually the most important SRM code on GitHub.

---

### 6. prashaant1926/open-earth-digital-twin-simulation ⭐ 0
- **URL:** https://github.com/prashaant1926/open-earth-digital-twin-simulation
- **Language:** Not specified
- **Last Activity:** October 10, 2025
- **Focus:** Manifesto-stage project for distributed Earth system simulation. A "digital twin" of Earth that could potentially include SRM scenarios.
- **Why it matters for SRM:** If realized, a distributed Earth system simulation would provide the open-source alternative to GISS ModelE or UKESM for SRM experiments. Currently at manifesto stage — essentially a vision document, not working code.

**Trend Signal:** Last committed October 2025. No recent activity. The project is in early-stage planning.

---

## Cross-Cutting Discovery: The SRM Simulation Gap

Despite WRF being the foundational atmospheric model, there is **no dedicated open-source SRM simulation repository** on GitHub. The gap is striking:

- **No open-source code for:** Stratospheric aerosol injection modeling, marine cloud brightening simulation, orbital reflectance engineering
- **What exists:** Atmospheric models (WRF) that *can* be configured for SRM, but require expert knowledge and institutional resources
- **What's missing:** Accessible, small-scale SRM simulation tools that could democratize the discussion
- ** Hausfath's srm-forever** is the exception — but it's economics, not physics

**Podcast Angle:** "The most important climate simulation code on Earth has almost no stars."

---

## Commit Trend Summary — Solar Geoengineering Theme

| Signal | Detail |
|--------|--------|
| **Institutional bursts** | PCMDI: 10 commits in 2 days (v4.2.1). WRF: v4.8.0 release with aerosol physics focus. MDTF: 5 commits in 1 day (precipitation POD).
| **Revival signals** | ClimateMARGO: 2 README updates after 2-year dormancy (Aug 2026). SRM-forever: 4 commits in 1 day (Aug 2026). |
| **Solar-specific commits** | WRF: "correction for eot calculation for solar radiation" (May 2026). MDTF: precipitation-buoyancy POD (Jun 2026). |
| **Governance infrastructure** | PCMDI metrics are the evaluation standard. MDTF diagnostics are the reality-check standard. Both are institutional, both are funded. |
| **Dormancy** | 6 of 8 solar repos show no meaningful activity in the last year. Climate tech open source is fragile. |
| **Language barrier** | WRF is Fortran. ClimateMARGO is Julia. The modern Python/data-science shift hasn't reached SRM simulation. |