# ☀️ Solar Geoengineering — Project Discoveries
## Research Notes for Podcast Episode (September 2026)

---

## Overview
This document profiles all open-source repositories discovered during GitHub research that relate to **solar geoengineering / solar radiation management (SRM)** and atmospheric climate modeling. Data was gathered via GitHub search queries and direct commit-history pulls on **September 2026**.

---

## Repo Profiles

### 1. WRF Model (`wrf-model/WRF`)
- **Stars:** ~1,761 | **Language:** Fortran/C | **Last commit:** June 8, 2026
- **Focus:** The Weather Research and Forecasting Model — the foundational atmospheric simulation model used worldwide
- **Why it matters for SRM:** WRF is the primary tool used to *evaluate* solar radiation management scenarios. Every serious SRM modeling study runs WRF (or its cousin CESM) to assess how aerosol injection would affect precipitation, temperature, and atmospheric dynamics.

#### Recent Commit Highlights (Fresh Data)
| Date | Commit | Significance |
|------|--------|-------------|
| Jun 8, 2026 | Merge v4.8.0 | **Major version release** — v4.8.0 is the latest stable |
| Jun 6, 2026 | README & version declaration update | Formal v4.8.0 announcement |
| Jun 5, 2026 | Turn off tempo_aerosolaware & tempo_hailaware | **Directly CN relevant** — aerosol-aware physics schemes being adjusted |
| May 30, 2026 | Fix vectorization option in AOCC stanza | Performance optimization for AMD processors |
| May 28, 2026 | **Correction for EOT calculation for solar radiation** | ⭐ **KEY FINDING** — bug fix in solar radiation endpoint calculation! This is the most directly SRM-relevant commit |
| May 27, 2026 | MYNN-EDMF pointer update & remove icloud_bl package | Cloud physics changes |
| May 27, 2026 | Update MMM-physics repo SHA | Submodule update for physics |
| May 26, 2026 | Fix CDXWRF module | Developer tooling fix |
| May 26, 2026 | README update for GFL option | Documentation |
| May 21, 2026 | Include mp_physics=88 in TEMPO error print | Error handling improvement |
| May 20, 2026 | Minor Tempo changes | Internal development |
| May 20, 2026 | Fix scheme-guard bug in urban NbS initialization | Urban simulation fix |
| May 20, 2026 | Add new namelists for ShinHong PBL | New boundary-layer scheme |
| May 19, 2026 | Bug fix for udm | Microphysics fix |
| May 12, 2026 | Update MYNN-SFC submodule | Surface model update |

**Episode Angle:** The solar radiation EOT correction (May 28) is a *perfect* podcast lead-in. A bug in how WRF calculates solar radiation endpoints could skew every SRM model output for years. Ask: **How many policy decisions were made on data with a known solar calculation error?** The v4.8.0 release also deactivated aerosol-aware schemes (tempo_aerosolaware, tempo_hailaware) — is this a simplification that could mask feedback effects?

---

### 2. PCMDI Metrics (`PCMDI/pcmdi_metrics`)
- **Stars:** ~133 | **Language:** Python | **Last commit:** September 17, 2026 (just days ago!)
- **Focus:** Earth System Model evaluation toolkit — the standard for assessing how well climate models reproduce observed reality (CMIP6 metrics)
- **Why it matters for SRM:** Before you can evaluate whether SRM"""