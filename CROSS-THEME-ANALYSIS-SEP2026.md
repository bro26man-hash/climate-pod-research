# 📊 Cross-Theme Commit Trend Analysis — September 2026 (v4)

**Updated:** September 2026 — v4 (fresh commit histories from 14 repositories across all themes)

## Methodology

Fresh commit histories from 14 key repositories across all three podcast themes, retrieved from GitHub's API on September 18, 2026.

| Theme | Repos | Commits | New in v4 |
|-------|-------|---------|----------|
| ☀️ Solar | WRF, PCMDI, MDTF, ClimateMARGO, srm-forever, awesome-geo, Geo-DICE, OOCC_2021 | 60+ | awesome-geo, Geo-DICE, OOCC_2021 |
| 🌍 Carbon | open-sustain-tech, OpenCarbon, openair-cyan, Carbon_Capture_ML, DAC_peroxovanadates, DAC_peroxotitanates, carbon-cc-andsim, **differentiable-flowsheets**, CO2-Soft-Sensor, membrane_model | 80+ | **differentiable-flowsheets (Claude-authored)** |
| 🌊 Ocean | MDTF, WRF, **Oceananigans.jl**, **veros**, **OceanBioME.jl**, **awesome-climate-science** | 50+ | **Lagrangian particles + gas exchange PRs** |

## Fresh Commit Data — By Theme

### ☀️ Solar Geoengineering

| Repo | Stars | Commits | Window | Key Signal |
|------|-------|---------|--------|------------|
| WRF | 1,761 | 10 | May-Jun 2026 | v4.8.0; TEMPO staging off; solar radiation EOT fix |
| PCMDI | 133 | 10 | Sep 3-4, 2026 | v4.2.1; dask/SVD extremes chunking |
| MDTF-diagnostics | 80 | 10 | Jun-Aug 2026 | MCS precip-buoyancy POD (5 commits Jun 19) |
| ClimateMARGO | 73 | 2 | Aug 17, 2026 | README revival; no code commits |
| srm-forever | 0 | 4 | Aug 26, 2026 | Weitzman discounting; interactive SRM economics |
| awesome-geoengineering | 4 | 1 | Sep 6, 2026 | Curated list updated |
| Geo-DICE | 2 | 4 | Sep 2018 | Dormant ghost |
| OOCC_2021 | 2 | 10 | Sep-Nov 2021 | Paper-linked governance; then silence |

### 🌍 Carbon Capture

| Repo | Stars | Commits | Window | Key Signal |
|------|-------|---------|--------|------------|
| open-sustainable-technology | 2,552 | 10 | Jul-Sep 2026 | claude-carbon; MUIO/MUIOGO DAC units |
| **differentiable-flowsheets** | **13** | **10** | **Sep 13-17** | **🔥 Claude writing production code** |
| openair-cyan | 76 | 10 | Feb 2022-2024 | OSHWA cert; dormant |
| Carbon_Capture_ML | 56 | 10 | Feb 2023-May 2024 | OpenDAC paper; maturing |
| DAC_peroxovanadates | 2 | 10 | Dec 2023-Sep 2025 | **CC0 (Sep 12, 2025)** |
| DAC_peroxotitanates | 2 | 10 | May 2024-Sep 2025 | **CC0 (Sep 12, 2025)** |
| carbon-capture-and-storage | 85 | 10 | Feb-Mar 2021 | Ghost since 2021 |
| CO2-Soft-Sensor | 16 | 1 | Aug 18, 2026 | DAE-LSTM DAC plant control |
| membrane_model | 6 | 1 | Aug 23, 2026 | Hollow fiber membrane |

### 🌊 Ocean Intervention

| Repo | Stars | Commits | Window | Key Signal |
|------|-------|---------|--------|------------|
| **Oceananigans.jl** | **1,413** | **10** | **Sep 15-17** | **🔥 Lagrangian particles (#6005)** |
| **OceanBioME.jl** | **80** | **10** | **Sep 14-17** | **🔥 Gas exchange PRs (#411,#399,#419)** |
| veros | 400 | 10 | Aug-Sep 2026 | 8/10 dependabot; 1 bugfix |
| MDTF-diagnostics | 80 | 10 | Jun-Aug 2026 | Precip-buoyancy POD |
| awesome-climate-science | 598 | — | Sep 2026 | Infrastructure |

## The Three Universes — v4

### Fast Universe
| Repo | Stars | Theme |
|------|-------|-------|
| open-sustainable-technology | 2,552 | 🌍 Carbon |
| WRF | 1,761 | ☀️ Solar |
| Oceananigans.jl | 1,413 | 🌊 Ocean |
| PCMDI | 133 | ☀️ Solar |
| veros | 400 | 🌊 Ocean |

### Slow Universe (Dormant)
| Repo | Stars | Theme |
|------|-------|-------|
| openair-cyan | 76 | 🌍 Carbon |
| ClimateMARGO | 73 | ☀️ Solar |
| Carbon_Capture_ML | 56 | 🌍 Carbon |
| DAC_peroxovanadates | 2 | 🌍 Carbon |
| DAC_peroxotitanates | 2 | 🌍 Carbon |
| carbon-capture-and-storage | 85 | 🌍 Carbon |
| srm-forever | 0 | ☀️ Solar |
| Geo-DICE | 2 | ☀️ Solar |
| OOCC_2021 | 2 | ☀️ Solar |

### AI-Augmented (NEW)
| Repo | Stars | Factor |
|------|-------|--------|
| differentiable-flowsheets | 13 | Claude writing code |
| claude-carbon | — | Category recognized |

### Empty Universe
| Domain | Repos | Proxy |
|--------|-------|-------|
| Ocean geoengineering | 0 | Oceananigans (particles Sep 16) |
| Marine cloud brightening | 0 | WRF + MDTF |
| Ocean sensors | 0 | None |
| Ocean governance | 0 | srm-forever (SRM only) |

## What's New in v4

1. **AI-augmented simulation wave** — Claude authored production code in differentiable-flowsheets
2. **CC0-to-AI pipeline** — tjz21 public domain data may become AI training infrastructure
3. **Lagrangian particles in Oceananigans** (Sep 16) — Tracer deployment method for OAE; nobody using it for interventions
4. **OceanBioME gas exchange PR chain** (Sep 15-17) — 3 PRs in 4 days; wind speed coupling debate = physics gate for OAE
5. **PCMDI extremes chunking** — dask/SVD for ensemble stats = SRM scenario testing
6. **claude-carbon** — New directory category; AI-for-climate recognized

## 🎙️ Podcast Narratives — v4

1. **The Institutional Divide** — Now with AI-augmented third tier
2. **The CC0 Revolution** — CC0-to-AI pipeline story
3. **The Ocean is the Silence** — 80% built; intervention layer 0%
4. **Ghost Stars** — 85★ dead since 2021; stars ≠ usage
5. **Nearest Feasible Ocean Project** — Oceananigans OAE module + particles
6. **Aug/Sep 2026 Wave** — AI now part of coordination
7. **AI Is Writing Climate Tech Code** (NEW) — Claude's merged production code

## 🔮 Watchlist

1. WRF TEMPO re-enablement 2. CC0 propagation 3. ClimateMARGO code revival 4. Oceananigans OAE module 5. OceanBioME gas exchange → OAE 6. differentiable-flowsheets + Claude 7. OpenAir-Cyan commercialization 8. PCMDI extremes for SRM 9. srm-forever adoption 10. Ocean gap into 2027 11. AI vs. institutional divide

## Research Log

| Date | Activity |
|------|----------|
| 2026-09-03 | Repository created |
| 2026-09-17 | v1-v3: Initial research, ecosystem analysis |
| 2026-09-18 | v4: 14 repos; differentiable-flowsheets + Claude; Lagrangian particles; OceanBioME gas exchange; all branches updated |