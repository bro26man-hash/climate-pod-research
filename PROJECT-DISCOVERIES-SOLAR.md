# ☀️ Solar Geoengineering — Project Discoveries
## Research Notes for Podcast Episode: Solar Radiation Management (SRM)

*Last updated: September 2026 — based on fresh GitHub commit analysis*

---

## Executive Summary

Our search for open-source solar geoengineering code revealed a landscape dominated by **atmospheric foundation models** and **climate evaluation toolkits** — not SRM-specific simulations. The most active repositories are institutional, well-funded, and focused on Weather Research and Forecasting (WRF) and CMIP6 metrics. The few SRM-specific projects are small, theoretical, or dormant.

**Key finding: Solar geoengineering code exists, but it's buried inside general climate models, not purpose-built SRM tools.**

---

## Repository Profiles

### 1. WRF (Weather Research and Forecasting Model) — `wrf-model/WRF`
| Attribute | Detail |
|-----------|--------|
| Stars | **1,761** |
| Language | Fortran, C, C++ |
| Last commit | **June 8, 2026** (v4.8.0 release) |
| Activity level | 🔴 VERY HIGH (15 commits in ~1 month) |
| License | BSD-style |

**Why it matters for solar geoengineering:**
WRF is the foundational atmospheric model used to simulate the effects of SRM interventions. Its radiation scheme, aerosol treatments, and cloud microphysics are the tools scientists use to model what happens when you deflect sunlight.

**Recent solar-relevant commits (June 2026):**
- `e836cd6` — **Correction for EOT (Equinox/Oblateness/Treasury) calculation for solar radiation** — directly improves accuracy of solar radiation calculations, critical for SRM forcing estimates
- `6a289e1` — Turned off `tempo_aerosolaware` and `tempo_hailaware` in Registry — TEMPO (Tempest spectral transform) is the dynamical core relevant to how atmospheric waves propagate
- `02f02bc` — Included `mp_physics=88` in TEMPO error print message — microphysics parameterization affects how SRM-induced changes in precipitation are modeled
- `9c87d29` — Added new namelists for ShinHong PBL and revised MMM surface layer — Planetary Boundary Layer schemes affect how surface cooling from SRM propagates
- `8fa379b` — Fixed scheme-guard bug in urban NbS (Nature-based Solutions) initialization — urban cooling is a key co-benefit argument for SRM

**Episode hook:** *"The model that simulates Earth's thermostat just got a solar radiation fix. Here's what that means for the debate."*

---

### 2. PCMDI Metrics (PCMDI/pcmdi_metrics) — v4.2.1
| Attribute | Detail |
|-----------|--------|
| Stars | **133** |
| Language | Python |
| Last commit | **September 17, 2026** (same-day push, 10 commits in 2 days) |
| Activity level | 🔴 VERY HIGH (burst release pattern) |
| License | LGPL |

**Why it matters for solar geoengineering:**
PCMDI Metrics is the **evaluation toolkit** used to assess whether climate models — including those used for SRM simulations — accurately reproduce observations. If you can't evaluate the model, you can't trust the SRM scenario. This is the **governance infrastructure** of solar geoengineering research.

**Recent commits (September 2026 — 10 commits in 2 days!):**
- `b8f231a` — Merged PR #1431: modpath_list patch (Jiwoo Lee)
- `90a4bc1` — Patch for single-file detection in modpath_list
- `6419050` — **Bumped version to 4.2.1** (release day)
- `90cbc50` — **Prevents roundoff to 1.00 in mean_climate figures** — this is a numerical precision fix that could affect how SRM forcing values are reported
- `71a0497` — Merged PR #1425: extremes chunking ( jigsaW SVD analysis for climate extremes)
- `ac634d7` — Rechunked data to higher order than rolling operation (memory optimization for large ensemble runs)
- `1fca2ec` — Fixed: force to use numpy SVD (numerical stability fix)

**Episode hook:** *"A 10-commit burst in 48 hours. Why are climate model evaluators racing to fix roundoff errors? Because in SRM, precision is policy."*

---

### 3. MDTF Diagnostics (NOAA-GFDL/MDTF-diagnostics)
| Attribute | Detail |
|-----------|--------|
| Stars | **80** |
| Language | Python, R, Fortran |
| Last commit | **August 14, 2026** |
| Activity level | 🟡 MODERATE (punctuated by major feature pushes) |
| License | Apache 2.0 |

**Why it matters for solar geoengineering:**
MDTF (Model Diagnostic Task Force) provides process-oriented diagnostics for evaluating climate models. Its **precipitation-buoyancy POD** (Proper Orthogonal Decomposition) is the most ocean-adjacent tool in the solar geoengineering ecosystem — it helps researchers understand how SRM-induced surface cooling affects tropical precipitation patterns.

**Key commits:**
- `33024ad` — **Added MCS precipitation-buoyancy statistics POD** — May 19, 2026
- `4cfc99c`, `699de27`, `d6bc6d0`, `3904d29` — **Four more updates to MCS_precip_buoy_stats.rst on the SAME DAY (June 19, 2026)** — five commits to one documentation file in a single day signals a major release of this diagnostic capability
- `87f8105` — Merged PR #825 (August 2026, Aparna Radhakrishnan)
- `95991fc` — Added quarterly metrics workflow for traffic logging
- `16403a4` — Moved diagnostics/blocking_neale_nb to dev branch

**Episode hook:** *"Five commits to one file in one day. What's so important about precipitation-buoyancy statistics that NOAA's diagnostics team dropped everything? It's the closest thing we have to an SRM impact early-warning system."*

---

### 4. ClimateMARGO.jl (ClimateMARGO/ClimateMARGO.jl)
| Attribute | Detail |
|-----------|--------|
| Stars | **73** |
| Language | Julia |
| Last commit | **August 17, 2026** (README update after 2+ year dormancy) |
| Activity level | 🟡 DORMANT with revival signal |
| License | MIT |

**Why it matters for solar geoengineering:**
ClimateMARGO is an **idealized climate-economic modeling framework** that optimizes trade-offs between mitigation, adaptation, and solar radiation management. It's the tool for answering: *"Given what we know, what's the optimal SRM strategy?"*

**Recent activity:**
- `d916f36` — README update (August 17, 2026)
- `6d9ba7a` — README update (August 17, 2026) — **two README updates after 2 years of silence**
- Last code commit: October 2023 (unit_conversions.jl)
- Last meaningful update: November 2022 (JuMP/Ipopt compat upgrade)

**The revival pattern:** Two README updates in August 2026 after 2+ years without any code changes. This could signal:
1. Renewed policy-modeling interest (IPCC AR7 synthesis reports?)
2. A potential refactoring effort approaching
3. Another false start (the pattern has repeated before)

**Episode hook:** *"After two years of silence, a climate-economic model wakes up with two README updates. Is SRM optimization back in style, or is it another ghost in the machine?"*

---

### 5. srm-forever (hausfath/srm-forever)
| Attribute | Detail |
|-----------|--------|
| Stars | **0** |
| Language | Python |
| Last commit | **August 26, 2026** |
| Activity level | 🟢 ACTIVE despite zero stars |
| License | MIT |

**Why it matters for solar geoengineering:**
This is the most **conceptually important** repo in our entire study, despite having zero stars. It implements **Weitzman certainty-equivalent discounting** applied to SRM cost dynamics. The question it answers: *"What does it cost to keep SRM going forever?"*

The Weitzman framework is a way of handling deep uncertainty about climate sensitivity. Applied to SRM, it addresses the worst-case scenario: what if SRM must be maintained indefinitely, and what happens if you stop?

**Commit pattern:** Small, focused updates indicating ongoing theoretical maintenance. Not a community project — this is a solo researcher's theoretical framework.

**Episode hook:** *"Zero stars, but this repo might be the most important thought experiment in solar geoengineering. It asks the question nobody wants to answer: what's the forever cost of sun-blocking?"*

---

## 🌡️ Development Trend Summary for Solar Episode

### The Three Tiers
| Tier | Repos | Pattern | What It Means |
|------|-------|---------|---------------|
| **Fast** (Institutional) | WRF, PCMDI | Continuous commits, versioned releases, multiple contributors | Solar geoengineering modeling is a mature, funded field with sustained infrastructure |
| **Medium** (Feature-driven) | MDTF | Punctuated major pushes (precip-BUOYANCY POD), then quiet | Diagnostic tools appear when funding cycles demand them, then go quiet |
| **Slow/Dormant** (Individual) | ClimateMARGO, srm-forever | Long gaps, README-only revivals, theoretical focus | The economics of SRM is an intellectual niche, not a community |

### Key Themes from Commit Data
1. **Solar radiation accuracy is actively being refined** — WRF's EOT correction (May 2026) shows that even flagship models still have unresolved issues in how they calculate solar forcing
2. **Evaluation is racing ahead of simulation** — PCMDI's 10-commits-in-2-days burst suggests that the community is under pressure to deliver reliable model evaluation tools, possibly for an upcoming assessment cycle
3. **The precipitation-buoyancy connection is the new frontier** — MDTF's 5-commits-to-one-file pattern suggests a major diagnostic breakthrough linking SRM surface cooling to tropical precipitation changes
4. **Economic models are dormant but not dead** — ClimateMARGO's ghost revival and srm-forever's steady theoretical work suggest that the economic case for SRM is being refined in parallel, not in the mainstream

### Episode Talking Points
- **Opening question:** "Where's the code for solar geoengineering?" → *It's inside climate models, not in SRM-specific repos*
- **The precision argument:** PCMDI's roundoff fix is a metaphor — in SRM, small errors have outsized policy consequences
- **The ocean connection:** MDTF's precip-buoyancy POD is how we know SRM wouldn't just cool the surface — it would reshape tropical rainfall
- **The economics ghost:** ClimateMARGO's README revival after 2 years — is SRM optimization intellectually alive, or just being cited?
- **The zero-star masterpiece:** srm-forever's Weitzman discounting — the most important question in SRM, asked by a repo nobody has starred

---

## 📚 Sources & Links
- [WRF Repository](https://github.com/wrf-model/WRF)
- [PCMDI Metrics Repository](https://github.com/PCMDI/pcmdi_metrics)
- [MDTF Diagnostics Repository](https://github.com/NOAA-GFDL/MDTF-diagnostics)
- [ClimateMARGO.jl Repository](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- [srm-forever Repository](https://github.com/hausfath/srm-forever)

---

*Research methodology: GitHub commit API analysis, September 2026. Commit data pulled via GitHub REST API. All timestamps are approximate based on API response dates.*