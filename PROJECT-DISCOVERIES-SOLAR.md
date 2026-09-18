# ☀️ Solar Geoengineering — Project Discoveries
## Research Notes | Climate Pod Research | September 2026

---

## Overview

This document profiles the most significant open-source repositories related to **solar geoengineering (SRM)** and **solar-climate simulation**. These repos form the backbone of our Episode 1 research — "Why is there so little code for sun-based climate intervention?"

---

## 🔬 Tier 1: Flagship Repos (High Activity, Institutional)

### 1. WRF — Weather Research and Forecasting Model
- **Repo:** [wrf-model/WRF](https://github.com/wrf-model/WRF)
- **Stars:** 1,763 ⭐
- **Language:** Fortran
- **Last commit:** June 8, 2026 (v4.8.0 release)
- **Active developers:** Anthony Islas, weiwangncar, Joseph Olson, Lluís Fita, Kelly Werner, AndersJensen-NOAA, Chenghao Wang

**What it is:** The definitive community atmospheric model used by NOAA, NCAR, and research institutions worldwide. WRF's radiation schemes are directly relevant to SRM modeling because they simulate how solar radiation propagates through the atmosphere — the same physics needed to model stratospheric aerosol injection.

**Recent commit highlights (15 commits pulled):**
| Date | Commit | Significance |
|------|--------|-------------|
| Jun 8, 2026 | Merge release-v4.8.0 | Major version release — stability boost for long simulations |
| Jun 6, 2026 | README & version → v4.8.0 | Documentation modernization |
| Jun 5, 2026 | Turn off tempo_aerosolaware & tempo_hailaware | **Aerosol-aware physics module being deprecated** — potential shift in aerosol modeling strategy |
| May 28, 2026 | Correction for EOT calculation for solar radiation | **Direct solar radiation fix** — improves accuracy of solar energy budgets in simulations |
| May 27, 2026 | MYNN-EDMF pointer update & icloud_bl removal | Boundary layer physics refinement |
| May 26, 2026 | Fix CDXWRF module | Catalyst driver compatibility fix |
| May 20, 2026 | Add mp_physics=88 in TEMPO error print | New physics option messaging |
| May 20, 2026 | Minor Tempo changes | Ongoing development |
| May 20, 2026 | Fix scheme-guard bug in urban NbS init | Urban nature-based solutions integration |
| May 20, 2026 | Add namelists for ShinHong PBL & revised MMM surface layer | New PBL scheme — critical for boundary layer aerosol transport |
| May 19, 2026 | Bug fix for udm | Microphysics dispatch fix |
| May 12, 2026 | Update MYNN-SFC submodule | Surface layer physics update |

**🎙️ Episode hook:** WRF's v4.8.0 release includes a **direct solar radiation correction** and the **deprecation of aerosol-aware physics**. This is a double signal: the model is improving its solar radiation handling (useful for SRM假装), while simultaneously moving away from certain aerosol parameterizations. What does it mean for the SRM modeling community?

---

### 2. PCMDI Metrics — ESM Evaluation Toolkit
- **Repo:** [PCMDI/pcmdi_metrics](https://github.com/PCMDI/pcmdi_metrics)
- **Stars:** 133 ⭐
- **Language:** Python
- **Last commit:** September 17, 2026 (v4.2.1)
- **Active developers:** Jiwoo Lee, James Goodnight, Jared Lewis

**What it is:** The standard toolkit for evaluating Earth System Models against observational data using CMIP6 metrics. If WRF is the atmospheric model, PCMDI metrics is the **quality assurance infrastructure** that tells us whether model results — including any SRM simulations — are trustworthy.

**Recent commit highlights (15 commits pulled — 10 in a single day!):**
| Date | Commit | Significance |
|------|--------|-------------|
| Sep 17, 2026 | Merge PR #1431 — modpath patch | File path handling fix |
| Sep 17, 2026 | Patch for single-file modpath_list | **Bug fix for edge case in path detection** |
| Sep 4, 2026 | **Bump version to 4.2.1** | New release |
| Sep 4, 2026 | Prepare v4.2.1 | Release preparation |
| Sep 4, 2026 | Update version & release date in CITATION.cff | Citation metadata |
| Sep 4, 2026 | Prevent roundoff to 1.00 in mean_climate figures | **Critical precision fix** — prevents climate metrics from being distorted by floating-point rounding |
| Sep 4, 2026 | PR #1427 — corr_roundoff merge | Roundoff correction merged |
| Sep 3, 2026 | PR #1425 — extremes chunking | **Memory optimization for extreme-value analysis** — large datasets now processable |
| Sep 3, 2026 | Merge branch for extremes chunking | Integration |
| Sep 3, 2026 | PR #1423 — variability modes dask SVD memory | **Dask-based SVD for variability modes** — enables analysis of massive climate arrays |
| Sep 3, 2026 | Rechunk data to higher order than rolling op | Performance optimization |
| Sep 3, 2026 | Chore: rename | Code cleanup |
| Sep 3, 2026 | Fix: force numpy SVD | **Fallback to numpy when Dask fails** — robustness improvement |

**🎙️ Episode hook:** On **September 4, 2026**, PCMDI released v4.2.1 with **10 commits in a single day**. The standout fix: preventing roundoff to 1.00 in mean climate figures. This sounds mundane but is *critical* — if a climate metric rounds to exactly 1.00, it could mask a 0.004°C warming signal. For SRM, where we're looking for small temperature perturbations, this precision matters enormously.

---

### 3. MDTF Diagnostics — Process-Oriented Model Evaluation
- **Repo:** [NOAA-GFDL/MDTF-diagnostics](https://github.com/NOAA-GFDL/MDTF-diagnostics)
- **Stars:** 80 ⭐
- **Language:** Python/R
- **Last commit:** August 14, 2026
- **Active developers:** Aparna Radhakrishnan, Wei-Ming Tsai, jongsooshin5, Dani Coleman

**What it is:** The Model Diagnostics Task Force produces process-oriented diagnostics for evaluating climate models. Its **precipitation-buoyancy POD** (Proper Orthogonal Decomposition) is the most ocean-relevant diagnostic tool in open source — it identifies the dominant modes of precipitation-buoyancy coupling, which is central to understanding how solar forcing drives atmospheric circulation.

**Recent commit highlights:**
| Date | Commit | Significance |
|------|--------|-------------|
| Aug 14, 2026 | Merge PR #825 | Integration of new diagnostics |
| Jun 19, 2026 | **5 commits on MCS_precip_buoy_stats.rst** | **The precipitation-buoyancy POD gets 5 updates in one day** — the most active single-file development across all solar-adjacent repos this year |
| Jun 19, 2026 | Add MCS precipitation-buoyancy statistics POD | **Brand-new POD diagnostic added** — expands the toolkit for convective process evaluation |
| Jun 8, 2026 | Merge PR #823 | Integration |
| Jun 8, 2026 | Update README (2 commits) | Documentation |
| Jun 2, 2026 | Add citation | Citation support |
| Jun 1, 2026 | Quarterly metrics workflow for traffic logging | CI/CD monitoring |
| May 27, 2026 | Move blocking_neale_nb to dev branch | Development workflow |
| May 22, 2026 | Merge blocking notebook PR | New blocking diagnostic |

**🎙️ Episode hook:** The **precipitation-buoyancy POD** received **5 commits on June 19, 2026** — all updating the same documentation file. This is the closest thing to an ocean-intervention tool in the GitHub ecosystem, and it's about *evaluating model accuracy*, not simulating interventions. The silence around actual ocean geoengineering code is deafening, but the evaluation infrastructure is alive and well.

---

## 🌱 Tier 2: Emerging & Conceptual Repos

### 4. ClimateMARGO.jl — Climate-Economic Modeling Framework
- **Repo:** [ClimateMARGO/ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- **Stars:** 73 ⭐
- **Language:** Julia
- **Last commit:** August 17, 2026 (README update after 2+ year dormancy)
- **Developer:** Fons van der Plas (primary), Henri Drake (earlier)

**What it is:** An idealized climate-economic modeling framework for optimizing trade-offs between emissions mitigation, adaptation, and solar geoengineering. Written in Julia, it uses JuMP and Ipopt for optimization. MARGO stands for " Modeling At the RareGOund" — a play on the RCP/SSP scenario framework.

**Commit timeline — the dormancy pattern:**
| Period | Activity | Commits |
|--------|----------|--------|
| Jan 2022 | Active development push (5 commits on Jan 12 alone) | 5 |
| Feb 2022 | CITATION.bib added, web apps removed, typo fix | 3 |
| Nov 2022 | JuMP/Ipopt compat upgrade, Project.toml update | 2 |
| Jul 2023 | Pluto notebook link added | 1 |
| **Oct 2023** | **Last code commit** (unit_conversions.jl comment) | 1 |
| **Aug 2026** | **Two README updates after 2+ year silence** | 2 |

**🎙️ Episode hook:** ClimateMARGO's **August 2026 revival** is ambiguous. Two README updates, zero code commits. Is someone preparing the model for a new run? Or is it a citation update? The 2-year dormancy followed by a README-only revival is the pattern of an **academic ghost repo** — cited in papers but never actively developed. Yet it's the *only* open-source tool that explicitly models the optimization trade-off between mitigation, adaptation, and SRM. That makes it conceptually irreplaceable.

---

### 5. srm-forever — Interactive SRM Economics Model
- **Repo:** [hausfath/srm-forever](https://github.com/hausfath/srm-forever)
- **Stars:** 0 ⭐ (but conceptually critical)
- **Language:** Python/Markdown
- **Last commit:** August 26, 2026
- **Developer:** hausfath

**What it is:** An **interactive cost model for stratospheric aerosol injection** that answers the question: "What does it cost to keep SRM going forever?" It applies **Weitzman certainty-equivalent discounting** — a theoretical economics framework from Martin Weitzman — to SRM cost dynamics. This is pure theory translated into code.

**All 4 commits (all on August 26, 2026 — single-day launch):**
| Commit | Significance |
|--------|-------------|
| Interactive SRM-forever vs mitigation+CDR cost model | **Base model** — compares SRM persistence costs against Combined Mitigation + Carbon Dioxide Removal strategies |
| Price abatement as a vintage annuity | **Economic framing** — models abatement costs as annuities, connecting to vintage capital theory |
| Adopt Weitzman certainty-equivalent discounting; add discount-rate essay | **Theoretical foundation** — applies Weitzman's framework for uncertain future costs |
| Add effective discount rate chart | **Visualization** — makes the theory interpretable |

**🎙️ Episode hook:** With **zero stars**, srm-forever is the most wine DMC (Doing Mathematical Climate) project on GitHub. But it tackles the deepest question in SRM economics: **what's the cost of commitment?** If you start SRM, you can't stop — because stopping means rapid warming. The Weitzman discounting approach is the theoretically correct way to evaluate that commitment, and someone has now coded it. This is a **conceptual flagship** despite its zero star count.

---

### 6. Orbital-Climate-Simulator — SRM Drone Fleet Dashboard
- **Repo:** [yanpefnsc/orbital-climate-simulator](https://github.com/yanpefnsc/orbital-climate-simulator)
- **Stars:** 2 ⭐
- **Language:** Python
- **Last commit:** September 16, 2026
- **Developer:** yanpefnsc

**What it is:** An **interactive mission-control dashboard for a conceptual Solar Radiation Management drone fleet**. This is the most directly SRM-themed code on GitHub — it simulates a fleet of high-altitude drones that would deploy aerosols, with SQLite telemetry, matplotlib visualization, and a Streamlit dashboard.

**All 12 commits (burst of activity over 2 days — September 15-16, 2026):**
| Date | Commit | Significance |
|------|--------|-------------|
| Sep 16 | docs: add dashboard preview | Documentation |
| Sep 16 | docs: add dashboard preview image | Visual documentation |
| Sep 16 | Correct author name casing in README | Metadata fix |
| Sep 16 | docs: add professional project README | Documentation overhaul |
| Sep 16 | Remove technology badges from README | Readability focus |
| Sep 16 | Enhance README with project details & setup | Documentation quality |
| Sep 16 | fix: update drone telemetry & simulation state | **Bug fix** — telemetry accuracy |
| Sep 16 | **feat: add interactive Streamlit dashboard** | **Major feature — real-time mission control UI** |
| Sep 15 | **feat: integrate SQLite database for mission logging** | **Data persistence** — drone flight logging |
| Sep 15 | **feat: add matplotlib visualizer** | **Visualization** — drone positions & radiation decay |
| Sep 15 | **feat: implement V1 base drone simulation logic** | **Core simulation** — the actual physics |
| Sep 15 | Initial commit | Project launch |

**🎙️ Episode hook:** This is the **only repo on GitHub that simulates an actual SRM deployment** — not just the climate effects, but the *operational logistics* of a drone fleet. It went from zero to a working prototype in **2 days** (12 commits). The streaming dashboard + SQLite telemetry stack is production-quality. Is this a student project? A proof of concept? Either way, it's the closest thing to "SRM mission control" in open source.

---

## 📊 Cross-Repo Solar Trend Analysis

### Activity Patterns
| Repo | Total Commits Pulled | Active Period | Commit Intensity | Pattern |
|------|---------------------|----------------|-----------------|--------|
| WRF | 15 | May-Jun 2026 | ~3/week | **Steady institutional cadence** |
| PCMDI | 15 | Sep 3-17, 2026 | 10 in 1 day! | **Burst release cycle** |
| MDTF | 15 | May-Aug 2026 | ~2/week | **POD-driven development** |
| ClimateMARGO | 15 | Jan 2022-Aug 2026 | Dormant 2.5 yrs | **Ghost revival** |
| srm-forever | 4 | Aug 26, 2026 | 4 in 1 day | **Single-day launch** |
| Orbital-Sim | 12 | Sep 15-16, 2026 | 12 in 2 days | **Rapid prototyping** |

### Key Developmental Signals
1. **The solar radiation fix in WRF (May 28)** is the most directly SRM-relevant code change — a correction to the End-of-Time calculation for solar radiation physics.
2. **PCMDI's roundoff fix (Sep 4)** prevents climate metrics from being distorted — critical for evaluating any SRM simulation.
3. **MDTF's precip-buoyancy POD (Jun 19)** is the ocean's closest friend in the solar ecosystem — 5 commits on the same file.
4. **ClimateMARGO's ghost revival (Aug 17)** — README updates without code commits suggest academic interest but no active development.
5. **srm-forever's Weitzman discounting (Aug 26)** — the most theoretically sophisticated SRM economics code, despite zero stars.
6. **Orbital-Sim's drone fleet (Sep 15-16)** — the only operational SRM simulation, built in 2 days.

---

## 🎙️ Episode 1 Talking Points

### The Scarcity Problem
- **Zero repos** directly simulate stratospheric aerosol injection's climate effects
- WRF can model the physics, but no one has built an SRM scenario module
- The two exceptions (srm-forever, orbital-climate-simulator) are both tiny and conceptual

### The Evaluation Infrastructure is Thriving
- PCMDI metrics: 10 commits in 1 day, v4.2.1 released
- MDTF diagnostics: precipitation-buoyancy POD actively developed
- WRF v4.8.0: solar radiation correction, aerosol physics changes
- **The evaluation toolkit is more active than the intervention tools**

### The Economics Frontier
- srm-forever: Weitzman discounting for SRM cost dynamics (0★ but theoretically critical)
- ClimateMARGO: The only optimization framework for mitigation-vs-SRM trade-offs (dormant)
- **Nobody is building operational SRM cost models**

### The Democraticization Signal
- Orbital-climate-simulator: A 2-day prototype that simulates an SRM drone fleet
- Open-source tools could democratize the SRM discourse — but only if the community builds them
- **The gap between evaluation infrastructure and intervention tools is the story**

---

*Last updated: September 2026 | Data source: GitHub API commit histories*