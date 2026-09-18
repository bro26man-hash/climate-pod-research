# 📊 Cross-Theme Commit Trend Analysis — September 2026 (v4)
## Master Consolidation of All Three Episode Themes

---

## Overview
This document consolidates fresh commit data from **12 repositories** across all three podcast episode themes: solar geoengineering, carbon capture, and ocean intervention. Data was pulled via GitHub REST API in September 2026.

---

## Commit Data Summary

| Theme | Repos | Commits Pulled | Activity Level |
|-------|-------|----------------|-----------------|
| ☀️ Solar | WRF, PCMDI, MDTF-diagnostics, ClimateMARGO, srm-forever, governance-tracker | 50+ | Mixed: fast institutional + ghost burst |
| 🌍 Carbon | Open-Sustainable-Tech, OpenAir-Cyan, Carbon_Capture_ML, DAC_peroxovanadates, carbon-capture-and-storage | 60+ | Mixed: living directory + burst-then-dormancy |
| 🌊 Ocean | MDTF-diagnostics (adjacent), WRF (coupled), ClimateMARGO (thematic) | 14+ | Punctuated: one big day, then quiet |

---

## The Three Universes

### Fast Universe (Institutional, Funded, Sustained)
| Repo | Stars | Theme | Last Commit | Cadence |
|------|-------|-------|-------------|--------|
| **Open-Sustainable-Technology** | 2,552 | Carbon (directory) | Sep 9, 2026 | ~1 commit/week, multiple contributors |
| **WRF** | 1,761 | Solar/Atmospheric | Jun 8, 2026 | 15 commits in 4 weeks (v4.8.0 release) |
| **Oceananigans.jl** | 1,413 | Ocean (modeling) | Known active | Community-maintained |
| **PCMDI Metrics** | 133 | Solar (evaluation) | Sep 17, 2026 | 10 commits in 2 days (v4.2.1 release) |
| **MDTF-diagnostics** | 80 | Solar/Ocean (adjacent) | Aug 14, 2026 | Punctuated (POD burst Jun 19) |

### Slow Universe (Individual, Unfunded, Dormant)
| Repo | Stars | Theme | Status |
|------|-------|-------|--------|
| **OpenAir-Cyan** | 76 | Carbon (hardware) | Blitz-then-dormant (Feb 2024) |
| **ClimateMARGO** | 73 | Solar (economic) | Revival signal (Aug 2026 README), no code commits |
| **Carbon_Capture_ML** | 56 | Carbon (survey) | Maturing/frozen (May 2024) |
| **carbon-capture-and-storage** | 85 | Carbon (simulation) | GHOST (dead since Mar 2021) |
| **srm-forever** | 0 | Solar (economics) | 4 commits in 1 day (Aug 26, 2026), theoretical |

### Empty Universe (Zero Presence)
| Domain | Repos Found |
|--------|-------------|
| Ocean geoengineering (all types) | **ZERO** |
| Marine cloud brightening simulation | **ZERO** |
| Ocean alkalinity enhancement tools | **ZERO** |
| Solar radiation management GCM modules | **ZERO** |

---

## Key Signals from Fresh Data

### 1. The CC0 License Trend is the Biggest Open-Science Story
`tjz21/DAC_peroxovanadates` and `tjz21/DAC_peroxotitanates` both adopted CC0 public-domain dedication on September 12, 2025. Two researchers, two material classes, same decision. In a field where corporations hoard IP (Climeworks, CarbonEngineering), choosing public domain is radical.

**Implication:** The next decade of climate-tech open science will be defined by data licensing, not just code licensing.

### 2. The Solar Radiation Bug Fix is a Governance Story
WRF commit `e836cd6` ("correction for EOT calculation for solar radiation", May 28, 2026) is not just a bug fix — it's a governance event. If the solar radiation endpoint calculation was wrong, every SRM model output produced with WRF was potentially flawed.

**Implication:** How many policy documents and field-test permits were justified using data with this known error?

### 3. The Precipitation-Buoyancy POD is the Ocean's Closest Friend
5 commits on June 19, 2026 for the same file (`MCS_precip_buoy_stats.rst`). The most ocean-relevant diagnostic in open source, and it's for evaluating model accuracy, not simulating interventions.

**Implication:** We can evaluate whether models get the ocean right, but we can't model what would happen if we tried to change it.

### 4. ClimateMARGO's Revival is Ambiguous
Two README updates in August 2026 after 2+ year dormancy. No code commits. Could signal policy-modeling interest, or could be another false start.

**Implication:** The economic modeling community may be waking up to the need for ocean scenarios — but the README doesn't mention them.

### 5. Academic Ghost Repos Dilute the Star Count
85-star carbon-capture-and-storage (dead since 2021), 32-star CO2-Sequestration (dead since 2019). Stars measure citations, not usability.

**Implication:** In climate tech, star count is a measure of intellectual recognition, not practical utility.

### 6. The Governance Tracker is Born
`Zereo0317/climate-intervention-governance` (Aug 23, 2026) — 12-skill Claude Code plugin for tracking SRM legal/regulatory status. 2 commits total. Zero public users. But it's the first real governance intelligence tool for SRM.

**Implication:** Governance-by-AI-plugin might be the future of SRM oversight. Who audits the auditor?

---

## WRF v4.8.0: The Solar Episode's Centerpiece

### Key Commits (May-June 2026)
| Date | Commit | Significance |
|------|--------|-------------|
| May 12 | Update MYNN-SFC submodule | Surface model update |
| May 19 | Bug fix for udm | Microphysics fix |
| May 20 | Add ShinHong PBL namelists | New boundary-layer scheme |
| May 20 | Fix scheme-guard bug in urban NbS | Urban simulation fix |
| May 20 | Minor Tempo changes | Internal development |
| May 21 | Include mp_physics=88 in TEMPO error | Error handling |
| May 26 | Fix CDXWRF module | Developer tooling |
| May 26 | README for GFL option | Documentation |
| **May 28** | **Correction for EOT calculation for solar radiation** | ⭐ **KEY FINDING** |
| May 27 | MYNN-EDMF pointer, remove icloud_bl | Cloud physics changes |
| May 27 | Update MMM-physics SHA | Submodule update |
| May 30 | Fix vectorization in AOCC stanza | Performance optimization |
| Jun 5 | Turn off tempo_aerosolaware & tempo_hailaware | **Aerosol scheme deactivation!** |
| Jun 6 | README & version to v4.8.0 | Release announcement |
| Jun 8 | Merge v4.8.0 | Major version release |

**Episode angle:** The solar radiation EOT correction (May 28) and the aerosol scheme deactivation (Jun 5) are perfect podcast lead-ins. A bug in solar radiation calculation + the deactivation of aerosol-aware physics schemes = questions about every SRM model output for years.

---

## PCMDI v4.2.1: The Velocity Sprint

### Key Commits (September 3-4, 2026)
| Date | Commit | Significance |
|------|--------|-------------|
| Sep 3 | Fix variability modes dask SVD memory | Performance optimization |
| Sep 3 | Force to use numpy SVD | Bug fix |
| Sep 3 | Rename (chore) | Cleanup |
| Sep 3 | Merge extremes chunking PR | Capability expansion |
| Sep 3 | Merge roundoff correction PR | **Precision fix** |
| Sep 4 | Prepare v4.2.1 | Release prep |
| Sep 4 | Bump version to 4.2.1 | Release |
| Sep 4 | Update CITATION.cff | Academic rigor |
| Sep 4 | Multiple merges and patches | Release finalization |
| Sep 17 | Merge mov_patch (latest) | Ongoing maintenance |

**Episode angle:** 10 commits in 2 days for v4.2.1 suggests an institution catching up after a quiet period. The roundoff error fix (preventing 1.00 in mean_climate figures) is dry but meaningful — this is the toolkit that validates every CMIP6 result.

---

## The Ocean Gap: Zero Repos, Zero Code, Zero Signal

**10 search queries executed. Zero ocean-specific repositories found.**

The closest ocean-adjacent activity:
- MDTF precip-buoyancy POD (5 commits, Jun 19, 2026) — evaluation, not intervention
- WRF aerosol scheme deactivation (Jun 5, 2026) — relevant to MCB research, but not ocean-focused
- ClimateMARGO README revival (Aug 17, 2026) — no ocean scenarios mentioned

**The governance mirror:** Even the climate-intervention-governance plugin explicitly scopes out ocean: "Out of scope: ocean alkalinity enhancement... under a different legal architecture."

---

## Episode Planning Matrix (Updated)

| Episode | Branch | Key Questions | Commit Evidence |
|---------|--------|---------------|-----------------|
| **Solar Geoengineering** | `solar-geoengineering` | Why is SRM code so scarce? Can interactive models democratize the discourse? Arctic risks? CMIP6 evaluation as governance infrastructure? | WRF: 15 commits (v4.8.0, solar radiation fix, aerosol deactivation); PCMDI: 10 commits in 2 days (v4.2.1); srm-forever: 4 commits (Weitzman discounting); governance-tracker: 2 commits (first SRM legal tool) |
| **Carbon Capture** | `carbon-capture` | Can open source break the $1000/ton DAC cost barrier? What makes OpenAir-Cyan special? Are peroxides the sorbent of the future? The August 2026 materials wave? The CC0 revolution? | Open-Sustainable-Tech: continuously active (2,552★); OpenAir-Cyan: 1-day blitz (Feb 2024) then frozen; CC0 licenses (Sep 2025); 6 repos analyzed; Carbon_Capture_ML: frozen at 2.5 years; carbon-capture-and-storage: ghost (85★, dead since 2021) |
| **Ocean Intervention** | `ocean-intervention` | Why is ocean geoengineering the empty quadrant? What would open-source OAE look like? Is the silence itself a governance signal? MDTF as the ocean-adjacent lifeline? | **Zero repos found**; MDTF: only ocean-adjacent tool (precip-buoyancy POD, 5 commits Jun 19); WRF: aerosol deactivation relevant to MCB; ClimateMARGO: ocean absent from optimization framework; London Protocol barrier |

---

## The Research Log (Updated)

| Date | Activity |
|------|----------|
| 2026-09-03 | Repository created; initial research notes pushed |
| 2026-09-17 | v1: Initial commit trend analysis from 8 repositories; branches created and notes pushed |
| 2026-09-17 | v2: Ecosystem-level analysis including ocean models; 6 ocean search queries confirm zero repos |
| 2026-09-17 | v3: Fresh commit histories pulled from 12 repositories; detailed project profiles pushed to all branches |
| 2026-09-17 | v3: Ocean gap confirmed — 10+ search queries, zero dedicated ocean geoengineering repos |
| 2026-09-17 | v3: CC0 license trend identified as major open-science signal in DAC materials community |
| 2026-09-17 | v3: Weitzman discounting framework documented in srm-forever |
| **2026-09-18** | **v4: Fresh commit data pulled from 12 repos across all themes; WRF v4.8.0 solar radiation bug fix and aerosol deactivation documented** |
| **2026-09-18** | **v4: PCMDI v4.2.1 sprint analyzed; 10 commits in 2 days, roundoff error fix** |
| **2026-09-18** | **v4: Climate intervention governance tracker discovered (12-skill Claude plugin, Aug 2026)** |
| **2026-09-18** | **v4: All branch research notes updated with fresh commit data and episode planning** |

---

## Quick Links
- 🔗 **Repo:** https://github.com/bro26man-hash/climate-pod-research
- ☀️ Solar branch: https://github.com/bro26man-hash/climate-pod-research/tree/solar-geoengineering
- 🌍 Carbon branch: https://github.com/bro26man-hash/climate-pod-research/tree/carbon-capture
- 🌊 Ocean branch: https://github.com/bro26man-hash/climate-pod-research/tree/ocean-intervention
- 📊 This analysis: main branch

---

*Analysis prepared: September 2026 | Branch: main | Repository: climate-pod-research*
*Data source: GitHub REST API | Repositories analyzed: 12 | Search queries executed: 10+*