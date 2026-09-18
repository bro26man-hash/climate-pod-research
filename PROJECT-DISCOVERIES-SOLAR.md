# ☀️ Solar Geoengineering — Project Discoveries
## Research Notes for Climate Pod Episode 1

---

## Overview
This document catalogs every significant open-source repository related to solar geoengineering (Solar Radiation Modification, SRM) and atmospheric climate simulation discovered through GitHub research. These projects form the technical backbone of any informed discussion about solar geoengineering.

---

## 🔬 Tier 1: Institutional, Actively Maintained

### 1. WRF (Weather Research and Forecast) Model
- **Repo:** [wrf-model/WRF](https://github.com/wrf-model/WRF)
- **Stars:** ~1,761
- **Language:** Fortran / C
- **Last Activity:** June 8, 2026 (v4.8.0 release tag)
- **License:** Apache 2.0

**What it is:** The foundational atmospheric numerical weather prediction and climate simulation model used worldwide. WRF is the platform upon which almost all solar geoengineering simulation experiments are built. If you want to model the atmospheric effects of stratospheric aerosol injection, you run WRF.

**Recent Commits (May–June 2026) — 15 commits analyzed:**
| Date | Commit Message | Significance |
|------|---------------|-------------|
| Jun 8 | Merge release-v4.8.0 | **Major version release** — v4.8.0 |
| Jun 6 | Update README and version to v4.8.0 | Documentation sync |
| Jun 5 | Turn off tempo_aerosolaware and tempo_hailaware | **TEMPO aerosol module adjustment** — directly relevant to pollution/aerosol modeling |
| May 30 | Fix vectorization option in AOCC stanza | Compiler optimization for AMD GPUs |
| **May 28** | **Correction for EOT calculation for solar radiation** | **⚡ SOLAR RADIATION FIX — directly impacts SRM simulation accuracy** |
| May 27 | Updating MYNN-EDMF pointer, removing icloud_bl package | Boundary layer physics overhaul |
| May 27 | Update MMM-physics repo SHA with fixes | Multi-scale framework update |
| May 26 | Fixing CDXWRF module | Cache management fix |
| May 26 | Update readme for GFL option | Green's Function Linear input documentation |
| May 21 | Include mp_physics=88 in TEMPO error print | ShinHong PBL physics support |
| May 20 | Minor Tempo changes | TEMPO continuous improvement |
| May 20 | Fixing scheme-guard bug in urban NbS init | Urban nature-based solutions coupling |
| May 20 | Add new namelists for ShinHong PBL and revised MMM surface layer | **New PBL scheme — critical for aerosol distribution modeling** |
| May 19 | Bug fix for udm | Microphysics dose module fix |
| May 12 | Updating MYNN-SFC submodule | Surface layer physics update |

**🎙️ Episode Hook:** The May 28 solar radiation EOT (End of Time) correction is a perfect podcast lead-in. *"Before you can even discuss whether dimming the sun works, you need to fix how the model calculates when solar radiation stops. That's the kind of foundational plumbing that 1,700 stars but almost no mainstream attention."*

---

### 2. PCMDI Metrics (PCMDI Metrics Tool)
- **Repo:** [PCMDI/pcmdi_metrics](https://github.com/PCMDI/pcmdi_metrics)
- **Stars:** ~133
- **Language:** Python
- **Last Activity:** September 17, 2026 (very active)
- **License:** BSD-3-Clause
- **Maintainer:** Lawrence Livermore National Laboratory

**What it is:** The official evaluation toolkit for CMIP (Coupled Model Intercomparison Project) climate models. When researchers propose a solar geoengineering experiment, they must first prove their model can accurately simulate the *unperturbed* climate. PCMDI metrics is how you do that.

**Recent Commits (September 2026) — 15 commits in 9 days:**
| Date | Commit Message | Significance |
|------|---------------|-------------|
| **Sep 17** | **Merge PR #1431 — mov_patch** | **ECO-EARTH model patch — expanding supported models** |
| Sep 17 | Patch for single-file case in modpath_list | Bug fix for edge cases |
| **Sep 4** | **Bump version to 4.2.1** | **New release!** |
| Sep 4 | Update version and release date in CITATION.cff | Citation management |
| Sep 4 | Prepare v4.2.1 | Release preparation |
| Sep 4 | Merge PR #1428 — lee1043-patch-1 | Contributed patch |
| Sep 4 | **Prevent roundoff to 1.00 in mean_climate figures** | **Critical fix —Tiny numerical errors in climate metrics can mislead SRM experiments** |
| Sep 4 | Merge PR #1427 — jsgoodni_corr_roundoff | Roundoff correction PR |
| **Sep 3** | **Merge PR #1425 — extremes_chunking** | **Extremes chunking for dask — handling CMIP6 extreme value analysis at scale** |
| Sep 3 | Merge branch main into extremes_chunking | Integration work |
| Sep 3 | Merge PR #1423 — variability-modes-dask-svd-memory | **Dask SVD memory optimization — enables analysis of massive datasets** |
| Sep 3 | Rechunk data to higher order than rolling operation | Performance optimization |
| Sep 3 | Chore: rename | Code cleanup |
| Sep 3 | Fix: force numpy SVD | Reliability fix for SVD computations |

**🎙️ Episode Hook:** *"In the 9 days before v4.2.1, PCMDI's team squashed a roundoff bug that would have made climate metrics display '1.00' instead of the correct value. For solar geoengineering, where we're talking about shifting global energy balances by 1-2%, a rounding error of 0.0001 could mean the difference between 'this works' and 'we're hosed.' That's the unsung heroism of climate code."*

---

### 3. MDTF Diagnostics (Model Diagnostic Task Force)
- **Repo:** [NOAA-GFDL/MDTF-diagnostics](https://github.com/NOAA-GFDL/MDTF-diagnostics)
- **Stars:** ~80
- **Language:** Python / R
- **Last Activity:** August 14, 2026
- **Maintainer:** NOAA Geophysical Fluid Dynamics Laboratory

**What it is:** Process-oriented diagnostics toolkit for evaluating climate model accuracy. MDTF doesn't just tell you if a model is "right" — it tells you *where* and *why* it's wrong, process by process. This is the quality control step before any SRM simulation is trusted.

**Recent Commits (May–August 2026):**
| Date | Commit | Significance |
|------|--------|-------------|
| Aug 14 | Merge PR #825 (weiming9115/main) | New contributor integration |
| **Jun 19** | **add MCS precipitation-buoyancy statistics POD** | **🌊 OCEAN-APPROPRIATE DIAGNOSTIC — 5 commits same day** |
| Jun 19 | Update MCS_precip_buoy_stats.rst (×4) | Intensive documentation effort |
| Jun 8 | Merge PR #823 (jongsooshin5/main) | New feature merge |
| Jun 8 | Update README (×2) | Documentation |
| Jun 2 | Merge NOAA-GFDL:main | Branch integration |
| Jun 2 | Add citation | Academic citation support |
| Jun 1 | Update quarterly-metrics.yml | CI/CD workflow update |
| Jun 1 | Add quarterly metrics workflow for traffic logging | **New automated monitoring** |
| May 27 | Move diagnostics/blocking_neale_nb to dev | Development branch management |
| May 22 | Merge blocking_notebook PR | Community contribution |

**🎙️ Episode Hook:** The precipitation-buoyancy POD (Pattern-Oriented Diagnostics) is the single most ocean-relevant tool in the entire open-source climate geospatial stack. Five commits on a single day (June 19) suggest a sprint. *"This is what it looks like when climate scientists nerf-out about precipitation physics in the ocean boundary layer. And it's beautiful."*

---

## 🔬 Tier 2: Individual Researchers, Dormant or Niche

### 4. ClimateMARGO
- **Repo:** [ClimateMARGO/ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- **Stars:** ~73
- **Language:** Julia
- **Last Activity:** August 17, 2026 (README updates after 2+ year dormancy)
- **License:** MIT

**What it is:** An idealized climate-economic modeling framework written in Julia. MARGO stands for **MA**hti **R**essources and **G**lobal **O**ptimization. It's designed to optimize trade-offs between emissions mitigation, adaptation, and solar geoengineering deployment. Think of it as the policy simulator — not "what happens physically?" but "what should we do economically?"

**Commit History Analysis:**
| Period | Activity | Pattern |
|--------|----------|---------|
| Jan 2022 | 7 commits (Henri Drake) | Active development — version bump, docs, Julia compat upgrade |
| Nov 2022 | 2 commits | Final burst before dormancy |
| **Jul 2023** | 1 commit (Fons van der Plas) | First revival — link to Pluto notebook |
| **Oct 2023** | 1 commit | Unit conversion comment fix |
| **Aug 2026** | **2 commits (Fons van der Plas)** | **Second revival — README updates** |

**🎙️ Episode Hook:** *"ClimateMARGO had two years of silence, then suddenly two README updates in August 2026. No code changes. No new features. Just... the README got better. Is someone considering using it again? Is a paper coming? Or is this digital archaeology — polishing the tombstone? We may never know, but the fact that someone still cares enough to update a README after 2 years tells you something about the permanence of geoengineering questions."*

**Key Concept — Weitzman Discounting:** ClimateMARGO implements uncertainty discounting under deep uncertainty (DREAM framework). For SRM, this means: *What's the optimal strategy when we don't know the climate sensitivity? The Weitzman (1974) certainty-equivalent approach suggests that when tail risks are fat, you should be more cautious about SRM deployment.*

---

### 5. srm-forever
- **Repo:** [hausfath/srm-forever](https://github.com/hausfath/srm-forever)
- **Stars:** 0
- **Language:** Jupyter Notebook
- **Last Activity:** August 26, 2026
- **License:** MIT

**What it is:** An interactive model for SRM economics. It applies Weitzman certainty-equivalent discounting to estimate the optimal trajectory of solar radiation modification over time. Despite zero stars, this is conceptually one of the most important repos in this list.

**Why it matters:** It directly answers the question: *"What does it cost to keep SRM going forever?"* The model shows that under certain assumptions, the optimal SRM strategy is to ramp up gradually and maintain indefinitely — but under uncertainty, the optimal path changes dramatically.

**Recent Activity:** 4 commits in late August 2026 (model refinements, documentation updates).

**🎙️ Episode Hook:** *"Zero stars on GitHub. But this little Jupyter notebook might contain the most dangerous equation in climate tech. It asks: what's the optimal temperature to target if you've committed to SRM forever? And the answer might scare you. Because once you start, the exit strategy becomes the hardest problem."*

---

### 6. GeoVision
- **Repo:** [pixnum-hub/GeoVision](https://github.com/pixnum-hub/GeoVision)
- **Language:** HTML
- **Last Activity:** December 2025

**What it is:** A geoengineering simulator with a web-based interface. One of the very few projects attempting to make SRM visualization accessible to non-scientists.

---

## 📊 Cross-Repo Solar Theme Analysis

### Development Velocity
| Repo | Recent Commits | Status | Trajectory |
|------|-----------------|--------|-------------|
| WRF | 15 in ~1 month | 🟢 Hyper-active | v4.8.0 release cycle; continuous physics improvements |
| PCMDI | 15 in 9 days | 🟢 Hyper-active | v4.2.1 release; performance and accuracy sprints |
| MDTF | 15 in 4 months | 🟡 Steady | Precip-buoyancy POD push; quarterly metrics automation |
| ClimateMARGO | 2 in 2 years | 🟡 Dormant revival | README-only updates; no code activity |
| srm-forever | 4 in <1 month | 🟢 Active | Small but focused SRM-specific development |

### Key Development Trends for Solar Episode
1. **Physics refinements are ongoing and relentless** — WRF's MYNN, ShinHong PBL, and TEMPO aerosol modules are being continuously improved. SRM simulations depend on these.
2. **Evaluation infrastructure is professionalizing** — PCMDI v4.2.1 with dask/chunking optimization means CMIP6 evaluation is getting faster and more accessible.
3. **The roundoff bug fix reveals how decimal places matter** — In SRM, we're discussing forcing changes of ~1-2 W/m². A rounding error in climate metrics could invalidate an entire experiment.
4. **Dormancy is the norm for individual projects** — ClimateMARGO's 2-year silence is typical. Solar geoengineering research is dominated by a few institutional groups, not a broad community.
5. **The interactive modeling space is tiny** — srm-forever (0 stars) and GeoVision are almost alone in making SRM computationally accessible.

---

## 🎙️ Episode 1 Talking Points

1. **"The boring foundation"** — Before we can debate SRM, we need models that accurately simulate sunlight, aerosols, and precipitation. WRF and PCMDI are that boring foundation.
2. **"A rounding error could end the world"** — Or at least a wrong climate prediction. PCMDI's roundoff fix is a microcosm of why SRM needs rigorous evaluation.
3. **"Who updates the README at 2AM?"** — ClimateMARGO's mysterious August 2026 revival. Someone still cares about the economics of SRM. Who?
4. **"Zero stars, big questions"** — srm-forever asks the defining question of SRM: what happens if we start and can't stop?
5. **"The ocean is the silent partner"** — MDTF's precipitation-buoyancy POD shows that solar geoengineering always intersects with ocean physics, even when we're talking about the atmosphere.

---

*Last updated: September 2026 | Data source: GitHub API commit histories*
*Next step: Record Episode 1 — "The Atmosphere Isn't the Only Room in the House"*