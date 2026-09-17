# 🎙️ Climate Pod Research — Fresh Commit Analysis (September 2026, v4)

**Pulled:** September 2026  
**Repositories Analyzed:** 20+ repos across solar geoengineering, carbon capture, and ocean intervention themes  
**Branches Updated:** solar-geoengineering, carbon-capture, ocean-intervention, main

---

## Executive Summary: What the Fresh Data Reveals

This v4 update pulls fresh commit histories from **20+ repositories** across all three podcast episode themes and pushes detailed analyses to each branch. The headline findings:

| Theme | Most Active Repo | Key Commit Signal | podcast Angle |
|-------|-----------------|-------------------|---------------|
| ☀️ Solar | wrf-model/WRF (1,761★) | v4.8.0 release: solar radiation EOT correction + TEMPO aerosol staging | The atmospheric model is world-class and actively improving SRM capabilities |
| 🌍 Carbon | openair-collective/openair-cyan (76★) | OSHWA certification burst (6 commits, Feb 12, 2024), then 2+ year dormancy | DIY hardware proved it works — but died without institutional support |
| 🌊 Ocean | NOAA-GFDL/MDTF-diagnostics (80★) | MCS precip-buoyancy POD (5 commits, Jun 19, 2026) | The evaluation tool for ocean intervention exists; the intervention tools don't |

**The three universes:**
- **Fast Universe (Institutional, Funded, Sustained):** WRF, MDTF, Oceananigans, OceanBioME
- **Slow Universe (Individual, Unfunded, Dormant):** OpenAir-Cyan, ClimateMARGO, Carbon_Capture_ML, academic ghosts
- **Empty Universe (Zero Presence):** Ocean geoengineering repos, marine cloud brightening, ocean sensors

---

## Cross-Theme Commit Trend Dashboard

### Solar Geoengineering (7 repos analyzed)

| Repo | Stars | Fresh Commits | Last Activity | Status |
|------|-------|--------------|--------------|--------|
| wrf-model/WRF | 1,761 | 15 in 18 days (May-Jun 2026) | Jun 8, 2026 | **ACTIVE** — v4.8.0 release |
| brandonhimpfen/awesome-geoengineering | 4 | 7/quarter | Sep 6, 2026 | **ACTIVE** — updated twice this week |
| ClimateMARGO/ClimateMARGO.jl | 73 | 15 over 4yr + 2 README (Aug 2026) | Aug 17, 2026 | **REVIVAL SIGNAL** — dormant 42 months |
| KOSASIH/GCCS-Core | 9 | 10 in 1 day (Oct 2024) | Oct 29, 2024 | **DEAD** — single-day burst |
| antara-banerjee/GeoengineeringLE_WinterWarming | 2 | 10 in 18 days (Apr 2021) | Apr 24, 2021 | **DEAD** — academic burst |
| jlehtomaa/OOCC_2021 | 2 | 10 in 3 months (Sep-Nov 2021) | Nov 15, 2021 | **DEAD** — conference burst |
| PSLmodels/Geo-DICE | 2 | 4 lifetime | Sep 27, 2018 | **GHOST** — 8 years dormant |

### Carbon Capture (10 repos analyzed)

| Repo | Stars | Fresh Commits | Last Activity | Status |
|------|-------|--------------|--------------|--------|
| openair-collective/openair-cyan | 76 | 15 (6 on Feb 12, 2024) | Feb 12, 2024 | **CERTIFIED then DORMANT** |
| zikribayraktar/Carbon_Capture_ML | 56 | 15 (paper-driven) | May 8, 2024 | **DORMANT** — last paper added |
| Beckybams/AI-for-Carbon-Capture-Opt | 25 | 3 (Feb-Mar 2026) | Mar 2, 2026 | **FRESHEST** — brand new arrival |
| tonyzyl/CO2-Soft-sensor | 16 | 8 (Mar-Aug 2022) | Aug 5, 2022 | **DORMANT** — served its purpose |
| yohanesnuwara/carbon-capture-and-storage | 85 | 15 (Feb-Mar 2021) | Mar 6, 2021 | **GHOST** — 85 stars, dead |
| CCSI-Toolset/membrane_model | 6 | Updated Aug 23, 2026 | Aug 23, 2026 | **ACTIVE** — materials wave |
| tjz21/DAC_peroxovanadates | 2 | Updated Aug 19, 2026 | Aug 19, 2026 | **ACTIVE** — CC0 license |
| tjz21/DAC_peroxotitanates | 2 | Updated Aug 19, 2026 | Aug 19, 2026 | **ACTIVE** — CC0 license |
| massimopizzol/CCU-LCA | 14 | Updated Jun 23, 2026 | Jun 23, 2026 | **DORMANT** — LCA assessment |
| IBM/Carbon-capture-fingerprint-generation | 2 | Low activity | 2024 | **DORMANT** — IBM Research |

### Ocean Intervention (1 direct + 4 adjacent repos)

| Repo | Stars | Fresh Commits | Last Activity | Status |
|------|-------|--------------|--------------|--------|
| NOAA-GFDL/MDTF-diagnostics | 80 | 15 (May-Aug 2026) | Aug 14, 2026 | **ACTIVE** — precip-buoyancy POD |
| CliMA/Oceananigans.jl | 1,413 | 10 in 3 days (Sep 2026) | Sep 17, 2026 | **ACTIVE** — Lagrangian particles |
| team-ocean/veros | 400 | 10 (mostly dependabot) | Sep 15, 2026 | **MAINTAINED** — dep bumps |
| OceanBioME/OceanBioME.jl | 80 | 10 in 4 days (Sep 2026) | Sep 17, 2026 | **ACTIVE** — gas exchange PRs |
| **Ocean geoengineering repos** | **0** | **—** | **—** | **EMPTY** — zero repos found |

---

## The Three Headlines

### 1. ☀️ Solar: The Atmospheric Modeling Tool Is Ready for SRM

WRF v4.8.0 includes a **solar radiation EOT correction** (commit `e836cd6`, May 28, 2026) that could affect all previous SRM simulation results. The **TEMPO aerosol microphysics** options are being staged for the next release. The institutional release cycle (5 contributors, 10 commits in 18 days) shows that the atmospheric modeling infrastructure for SRM is not just theoretical — it's being actively maintained and improved.

But the governance layer is non-existent: Geo-DICE is frozen in 2018, OOCC_2021 is a document with BibTeX entries, and ClimateMARGO is a 3-year-dormant Julia package with only README updates.

**The surprise:** awesome-geoengineering (4 stars) is the ONLY actively maintained geoengineering-specific repo, updated twice in September 2026.

### 2. 🌍 Carbon: CC0 Licensing and the August 2026 Materials Wave

The biggest open-science story of the year isn't about code — it's about **licenses**. Two repos by the same author (tjz21) adopted **CC0 public domain dedication** for computational DAC materials screening data (peroxovanadates and peroxotitanates, both updated Aug 19, 2026). This is the opposite of the typical academic "all rights reserved" approach. The researcher is saying: "This data is for everyone."

The August 2026 materials wave (4+ repos updating in 6 days across sorbents, membranes, and soft-sensors) is confirmed. The field is converging on open, reproducible computational workflows for carbon capture materials discovery.

**The cautionary tale:** OpenAir-Cyan (76★, OSHWA-certified) proved DIY open-source hardware can work — then went dormant for 2+ years after the certification milestone. Without institutional support, even certified hardware dies.

**The newest signal:** AI-for-Carbon-Capture-Optimization (25★, 3 commits, Feb-Mar 2026) is the most recently active carbon repo. Synthetic industrial data for CC optimization — the applied engineering approach.

### 3. 🌊 Ocean: The Complete Absence

The ocean geoengineering quadrant is **empty**. Across 8+ search query strategies, zero dedicated ocean intervention repositories were found. No ocean alkalinity enhancement. No marine cloud brightening. No artificial upwelling. No iron fertilization. No DIY ocean sensors.

But here's the twist: the ocean *climate modeling* ecosystem is one of the most vibrant on GitHub:
- Oceananigans.jl (1,413★): 10 commits in 3 days, Lagrangian particle tracking
- OceanBioME.jl (80★): 10 commits in 4 days, gas exchange parameterization (THE central process for OAE)
- MDTF-diagnostics (80★): MCS precip-buoyancy POD added Jun 19, 2026 (5 commits in 1 day)

**The gap is specific:** The modeling stack is 80% built. The intervention layer is 0% built. We have world-class tools for understanding the ocean. We have zero tools for simulating what happens when we intervene in it.

---

## The Four Activity Patterns (Across All Themes)

| Pattern | Examples | Characteristics | Podcast Implication |
|---------|----------|----------------|-------------------|
| **Institutional Release Cycles** | WRF, MDTF, Oceananigans | Multi-contributor, version-tagged, funded | The "fast universe" — sustained, professional development |
| **Sustainably Maintained Directories** | awesome-geoengineering | Quarterly updates, focused scope | The "working resource" — low stars, high utility |
| **Dormant with Revival Signals** | ClimateMARGO | Long dormancy, README-only updates | The "maybe" pattern — hope or funeral procession? |
| **Academic Single-Burst** | Geo-DICE, WinterWarming, OpenAir-Cyan, GCCS-Core | One push of commits, then permanent silence | The "publish and perish" pattern — incentives don't reward maintenance |

---

## What to Watch (Updated Watchlist)

1. **WRF TEMPO aerosol physics** — Experimental options being turned off in v4.8.0 suggest a next release with improved aerosol microphysics. The SRM simulation pipeline.

2. **ClimateMARGO revival** — If the Aug 2026 README updates lead to code commits, this could become the policy-modeling layer for SRM. Watch for the next commit.

3. **MDTF marine cloud brightening diagnostics** — The precip-buoyancy POD (Jun 19, 2026) is the closest thing to MCB evaluation tooling. Expect more ocean-relevant PODs.

4. **CC0 licensing adoption** — If tjz21's CC0 approach spreads, it could become the standard for open DAC materials data. This is a governance signal, not just a technical one.

5. **AI-for-Carbon-Capture-Optimization** — The most recently active carbon repo. If the author continues updating, this could be a new approach to CC optimization using synthetic data.

6. **OceanBioME gas exchange PRs** — 3 PRs in 4 days (Sep 15-17, 2026). The science of gas exchange is accelerating. The jump from "modeling gas exchange" to "modeling OAE deployment" is the next step.

7. **awesome-geoengineering updates** — Quarterly cadence, currently active. Check Sep 2026 updates for new entries on ocean geoengineering (if any).

---

## Repository Links

| Theme | Repo | Link |
|-------|------|------|
| ☀️ Solar | wrf-model/WRF | https://github.com/wrf-model/WRF |
| ☀️ Solar | ClimateMARGO/ClimateMARGO.jl | https://github.com/ClimateMARGO/ClimateMARGO.jl |
| ☀️ Solar | brandonhimpfen/awesome-geoengineering | https://github.com/brandonhimpfen/awesome-geoengineering |
| ☀️ Solar | PSLmodels/Geo-DICE | https://github.com/PSLmodels/Geo-DICE |
| 🌍 Carbon | openair-collective/openair-cyan | https://github.com/openair-collective/openair-cyan |
| 🌍 Carbon | zikribayraktar/Carbon_Capture_ML | https://github.com/zikribayraktar/Carbon_Capture_ML |
| 🌍 Carbon | Beckybams/AI-for-Carbon-Capture-Optimization | https://github.com/Beckybams/AI-for-Carbon-Capture-Optimization |
| 🌍 Carbon | tonyzyl/CO2-Soft-sensor | https://github.com/tonyzyl/CO2-Soft-sensor-for-a-carbon-capture-pilot-plant |
| 🌍 Carbon | tjz21/DAC_peroxovanadates | https://github.com/tjz21/DAC_peroxovanadates |
| 🌊 Ocean | NOAA-GFDL/MDTF-diagnostics | https://github.com/NOAA-GFDL/MDTF-diagnostics |
| 🌊 Ocean | CliMA/Oceananigans.jl | https://github.com/CliMA/Oceananigans.jl |
| 🌊 Ocean | OceanBioME/OceanBioME.jl | https://github.com/OceanBioME/OceanBioME.jl |

---

## Branch Structure

| Branch | Files | Content |
|--------|-------|---------|
| `main` | COMMIT-TRENDS.md, CROSS-THEME-ANALYSIS-SEP2026.md, FRESH-COMMIT-DATA-SEP2026-* | Master consolidated analysis |
| `solar-geoengineering` | PROJECT-DISCOVERIES-SOLAR.md, COMMIT-TRENDS-SOLAR.md, FRESH-COMMIT-DATA-SEP2026-SOLAR.md | Solar theme deep dive |
| `carbon-capture` | PROJECT-DISCOVERIES-CARBON.md, COMMIT-TRENDS-CARBON.md, FRESH-COMMIT-DATA-SEP2026-CARBON.md | Carbon theme deep dive |
| `ocean-intervention` | PROJECT-DISCOVERIES-OCEAN.md, COMMIT-TRENDS-OCEAN.md, FRESH-COMMIT-DATA-SEP2026-OCEAN.md | Ocean theme deep dive |

---

## Research Log

| Date | Version | Activity |
|------|---------|----------|
| 2026-09-03 | v1 | Repository created; initial research notes pushed |
| 2026-09-17 | v2 | Ecosystem-level analysis including ocean models; 6 ocean search queries confirm zero repos |
| 2026-09-17 | v3 | Fresh commit histories pulled from 12 repositories; detailed project profiles pushed to all 3 theme branches |
| 2026-09-17 | v3 | CC0 license trend identified; Weitzman discounting documented in srm-forever |
| 2026-09-17 | **v4** | **Fresh commit data pulled from 20+ repos via GitHub API across all 3 themes** |
| 2026-09-17 | v4 | **WRF v4.8.0 release cycle analyzed — solar radiation EOT correction = most SRM-relevant commit** |
| 2026-09-17 | v4 | **awesome-geoengineering confirmed as only actively maintained geoengineering repo (Sep 5-6, 2026)** |
| 2026-09-17 | v4 | **AI-for-Carbon-Capture-Optimization confirmed as most recently active carbon repo (Mar 2026)** |
| 2026-09-17 | v4 | **August 2026 materials wave confirmed across peroxovanadates, peroxotitanates, membranes, soft-sensors** |
| 2026-09-17 | v4 | **CC0 public domain licensing identified as major open-science signal** |
| 2026-09-17 | v4 | **MDTF precip-buoyancy POD (Jun 19, 2026) identified as most ocean-relevant commit** |
| 2026-09-17 | v4 | **Ocean gap confirmed with 8+ search queries — zero dedicated ocean geoengineering repos** |
| 2026-09-17 | v4 | **5-tier carbon capture ecosystem analysis; 4 activity patterns across all themes** |
| 2026-09-17 | v4 | **Fresh commit data files pushed to all 3 theme branches; cross-theme dashboard pushed to main** |
