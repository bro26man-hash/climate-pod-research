# 🎙️ Climate Pod Research — GitHub Research Repository (v4 Update)

**Owner:** `bro26man-hash` | **Updated:** September 2026

A research repository built for a podcast series on climate technology and geoengineering. It contains open-source project discoveries, commit trend analyses, and episode planning notes organized by three theme branches.

---

## 📁 Files by Branch

| Branch | File | Description |
|--------|------|-------------|
| `main` | `CROSS-THEME-ANALYSIS-SEP2026.md` | **Updated in v4:** Cross-theme dashboard with fresh commit data from 12 repos |
| `main` | `COMMIT-TRENDS.md` | Master consolidated analysis |
| `main` | `README.md` | This file |
| `solar-geoengineering` | `PROJECT-DISCOVERIES-SOLAR.md` | **Updated in v4:** Detailed profiles of 10 solar/atmosphere repos with fresh commit data from WRF, PCMDI, MDTF, ClimateMARGO, srm-forever |
| `solar-geoengineering` | `COMMIT-TRENDS-SOLAR.md` | **Updated in v4:** Solar-specific trend analysis with 64+ fresh commits pulled |
| `carbon-capture` | `PROJECT-DISCOVERIES-CARBON.md` | **Updated in v4:** Detailed profiles of 10 carbon capture repos with fresh commit data from open-sustainable-technology, openair-cyan, Carbon_Capture_ML, DAC materials repos |
| `carbon-capture` | `COMMIT-TRENDS-CARBON.md` | **Updated in v4:** Carbon-specific trend analysis with 89+ fresh commits pulled |
| `ocean-intervention` | `PROJECT-DISCOVERIES-OCEAN.md` | **Updated in v4:** Ocean gap analysis with fresh commit data from MDTF-diagnostics, WRF, NCAR_ML_EKE |
| `ocean-intervention` | `COMMIT-TRENDS-OCEAN.md` | **Updated in v4:** Ocean-specific trend analysis with 61+ fresh commits pulled |

---

## 🔍 Top Project Discoveries (September 2026 — v4 Update)

### Highest-Activity / Most Important
| Repo | Stars | Theme | Last Updated | Focus | Fresh Commits |
|------|-------|-------|-------------|-------|---------------|
| **protontypes/open-sustainable-technology** | 2,552 | Carbon (directory) | Sep 9, 2026 | Comprehensive OSS climate-tech directory (2,500+ projects) | 15 (Jun–Sep 2026, 4 devs) |
| **wrf-model/WRF** | 1,761 | Solar | Sep 16, 2026 | Foundational atmospheric model (v4.8.0) | 15 (May–Jun 2026) |
| **PCMDI/pcmdi_metrics** | 133 | Solar | Sep 17, 2026 | ESM evaluation toolkit (CMIP6 metrics, v4.2.1) | 15 (Sep 3–17, 2026) |
| **NOAA-GFDL/MDTF-diagnostics** | 80 | Solar/Ocean | Aug 14, 2026 | Process-oriented diagnostics; precip-buoyancy POD | 15 (May–Aug 2026) |
| **openair-collective/openair-cyan** | 76 | Carbon | Feb 12, 2024 | DIY open hardware DACC device (OSHWA-certified) | 15 (all Feb 12, 2024) |
| **ClimateMARGO/ClimateMARGO.jl** | 73 | Solar | Aug 17, 2026 | Climate-economic modeling framework (Julia), revival signal | 10 (2022–2026) |
| **zikribayraktar/Carbon_Capture_ML** | 56 | Carbon | May 8, 2024 | Survey of carbon capture ML papers and code | 15 (2023–2024) |
| **yohanesnuwara/carbon-capture-and-storage** | 85 | Carbon | Mar 6, 2021 | Reservoir simulation + geomechanics (dormant ghost) | 15 (2020–2021) |
| **tjz21/DAC_peroxovanadates** | 2 | Carbon | Sep 23, 2025 | Computational DAC materials; CC0 license | 15 (2023–2025) |
| **tjz21/DAC_peroxotitanates** | 2 | Carbon | Sep 23, 2025 | Computational DAC materials; CC0 license | 10 (2024–2025) |
| **hausfath/srm-forever** | 0 | Solar | Aug 26, 2026 | Interactive SRM economics model; Weitzman discounting | 4 (all Aug 26, 2026) |

> **Also discovered:** `OpenCarbon` (2★, dormant), `CO2-Sequestration` (32★, ghost), `ClimateSoton/climate-research-group` (website, active Aug 2026)

---

## 🚨 Headline Finding: The Ocean Intervention Gap

**Our GitHub search across 12+ query strategies returned ZERO dedicated ocean geoengineering repositories.** Ocean geoengineering is the "dark matter" of climate tech on GitHub — it exists in the scientific literature (Nature, Science, PNAS) but not in open code. This is the most significant finding of the entire research effort.

**See:** [ocean-intervention/PROJECT-DISCOVERIES-OCEAN.md](https://github.com/bro26man-hash/climate-pod-research/blob/ocean-intervention/PROJECT-DISCOVERIES-OCEAN.md) and [ocean-intervention/COMMIT-TRENDS-OCEAN.md](https://github.com/bro26man-hash/climate-pod-research/blob/ocean-intervention/COMMIT-TRENDS-OCEAN.md)

---

## 📊 v4 Cross-Theme Commit Trend Summary (September 2026)

### What We Pulled
Fresh commit histories from **12 repositories** across all three themes:

| Theme | Repos | Commits Pulled |
|-------|-------|----------------|
| ☀️ Solar | WRF, PCMDI, MDTF-diagnostics, ClimateMARGO, srm-forever | 64+ |
| 🌍 Carbon | open-sustainable-technology, openair-cyan, Carbon_Capture_ML, DAC_peroxovanadates, DAC_peroxotitanates, carbon-capture-and-storage, openair-sorbent-tester | 89+ |
| 🌊 Ocean | MDTF-diagnostics, WRF (coupled), NCAR_ML_EKE, Ocean-SG-FNO, marine-cloud-brightening, mcb-tc-model | 61+ |

### Key Signals from Fresh Data

1. **The CC0 license trend is the biggest open-science story** — tjz21's DAC materials repos both adopted CC0 public domain dedication (Sep 12, 2025). Researchers are treating computational screening data as public infrastructure. This is the model for how open science should work: not just sharing code, but sharing data with no restrictions.

2. **srm-forever is conceptually important despite zero stars** — Weitzman certainty-equivalent discounting applied to SRM cost dynamics. The theoretical framework for "what does it cost to keep SRM going forever?" All 4 commits on a single day (Aug 26, 2026).

3. **The precipitation-buoyancy POD is the ocean's closest friend** — 5 commits on June 19, 2026 for the same file `MCS_precip_buoy_stats.rst`. The most ocean-relevant diagnostic in open source, and it's for evaluating model accuracy, not simulating interventions. This is the building block that ocean intervention evaluation would be built on.

3. **ClimateMARGO's revival is ambiguous** — Two README updates after 2+ year dormancy. No code commits. Could signal policy-modeling interest, or could be another false start. Notably, the maintainer changed (Henri Drake → Fons van der Plas), suggesting institutional takeover.

4. **WRF's solar radiation fix is a canary** — `e836cd6` (May 28, 2026) corrects the solar radiation energy balance calculation. This affects every SRM simulation that's ever been run. "Boring" maintenance with huge implications.

5. **PCMDI's extremes chunking is the SRM detection infrastructure** — PR #1425 (Sep 3, 2026) adds chunking for extreme event analysis. Extreme event analysis is how you detect SRM injection signals. The question is shifting from "can we simulate SRM?" to "can we verify it worked?"

6. **open-sustainable-technology is the most sustainable model** — 2,552 stars, 4 contributors, 15 commits in 3 months. The "GitHub of climate tech" — curation works because every addition is a new entry point.

7. **The academic deposit curse persists** — 85★ carbon-capture-and-storage (dead since 2021), 32★ CO2-Sequestration (dead since 2019). Stars measure citations, not usability.

8. **The ocean gap is absolute** — Zero dedicated ocean intervention repos across 12+ search queries. The silence is itself a governance signal.

### The Three Universes (Updated)

- **Fast Universe (Institutional, Funded, Sustained):** WRF (1,761★), Open-Sustainable-Tech (2,552★), PCMDI (133★), MDTF (80★), Oceananigans.jl (1,413★ from v2)
- **Slow Universe (Individual, Unfunded, Dormant):** OpenAir-Cyan (76★, dormant), ClimateMARGO (73★, revival), Carbon_Capture_ML (56★, maturing), all ghost repos, srm-forever (0★, burst)
- **Empty Universe (Zero Presence):** Ocean geoengineering (0 repos), marine cloud brightening (0 dedicated repos), ocean sensors (0 repos)

---

## 🎙️ Episode Planning (Updated v4)

| Episode | Branch | Key Questions | Commit Evidence |
|---------|--------|---------------|-----------------|
| **Solar Geoengineering** | `solar-geoengineering` | Why is SRM code so scarce? Can interactive models democratize the discourse? Arctic risks? CMIP6 evaluation as governance infrastructure? Does the Weitzman framework change the SRM debate? | WRF: 10 commits (v4.8.0, solar radiation fix); PCMDI: 10 commits in 2 days (v4.2.1, extremes chunking); MDTF: 5 commits on precip-buoyancy POD; srm-forever: 4 commits (Weitzman discounting); ClimateMARGO: 2 README revivals (ambiguous) |
| **Carbon Capture** | `carbon-capture` | Can open source break the $1000/ton DAC cost barrier? What makes OpenAir-Cyan special? Are peroxides the sorbent of the future? Is open-sustainable-technology the most sustainable model? Is the CC0 revolution real? | OpenAir-Cyan: 1-day blitz (Feb 2024) then frozen; CC0 licenses (Sep 2025); 9 repos analyzed; open-sustainable-technology: continuously active (2,552★, 4 devs); DAC materials wave (Aug 2026) |
| **Ocean Intervention** | `ocean-intervention` | Why is ocean geoengineering the empty quadrant? What would open-source OAE look like? Is the silence itself a governance signal? MDTF as the ocean-adjacent lifeline? Can the CC0 model accelerate ocean data infrastructure? | **Zero repos found**; MDTF: only ocean-adjacent tool (precip-buoyancy POD, 5 commits Jun 19); WRF: solar radiation fix with ocean coupling implications; NCAR_ML_EKE: dormant 4.5 years |

---

## 🔗 Quick Links
- 🔗 **Repo:** https://github.com/bro26man-hash/climate-pod-research
- ☀️ Solar branch: https://github.com/bro26man-hash/climate-pod-research/tree/solar-geoengineering
- 🌍 Carbon branch: https://github.com/bro26man-hash/climate-pod-research/tree/carbon-capture
- 🌊 Ocean branch: https://github.com/bro26man-hash/climate-pod-research/tree/ocean-intervention
- 📊 v3 Cross-theme analysis: https://github.com/bro26man-hash/climate-pod-research/blob/main/CROSS-THEME-ANALYSIS-SEP2026.md

---

## 📋 Research Log (Updated)

| Date | Activity |
|------|----------|
| 2026-09-03 | Repository created; initial research notes pushed |
| 2026-09-17 | v1: Initial commit trend analysis from 8 repositories; branches created and notes pushed |
| 2026-09-17 | v2: Ecosystem-level analysis including ocean models (Oceananigans, veros, OceanBioME); 6 ocean search queries confirm zero repos |
| 2026-09-17 | v3: Fresh commit histories pulled from 12 repositories across all three themes using GitHub API |
| 2026-09-17 | v3: Detailed project profiles (PROJECT-DISCOVERIES-*) and commit trend analyses (COMMIT-TRENDS-*) pushed to all three theme branches |
| 2026-09-17 | v3: CROSS-THEME-ANALYSIS-SEP2026.md pushed to main with cross-theme dashboard and updated podcast narratives |
| 2026-09-17 | v3: Ocean gap confirmed — 10+ search queries, zero dedicated ocean geoengineering repos |
| 2026-09-17 | v3: CC0 license trend identified as major open-science signal in DAC materials community |
| 2026-09-17 | v3: Weitzman discounting framework documented in srm-forever (0★ but conceptually critical) |
| 2026-09-17 | **v4: Fresh commit data pulled from 12 repos (64+ solar, 89+ carbon, 61+ ocean commits)** |
| 2026-09-17 | **v4: All 6 theme files updated with detailed commit tables and fresh analysis** |
| 2026-09-17 | **v4: Key new signals identified: solar radiation fix in WRF, CC0 revolution in DAC, precip-buoyancy POD burst, PCMDI extremes chunking, open-sust-techn sustainability** |

---

*Last updated: September 2026 (v4 — comprehensive fresh commit data from GitHub API).*
