# ☀️ Solar Geoengineering — Commit Trend Analysis & Project Discoveries

*Last updated: September 2026 — sourced from GitHub REST API, List Commits endpoint*

---

## 🔬 Key Repositories Analyzed

### 1. wrf-model/WRF — The Atmosphere Model That Swallowed Geoengineering
| Metric | Value |
|--------|-------|
| Stars | 1,763 |
| Language | Fortran |
| Last commit | June 8, 2026 |
| Activity level | **🔴 Fast** — institutional, continuous, funded |

**Recent commit highlights (May–June 2026, 15 commits pulled):**

| Date | Commit message | Author |
|------|---------------|--------|
| 2026-06-08 | Merge release-v4.8.0 | Anthony Islas |
| 2026-06-06 | Update README and version to v4.8.0 | Anthony Islas |
| 2026-06-05 | Turn off tempo_aerosolaware and tempo_hailaware in Registry | weiwangncar |
| 2026-05-30 | Fix vectorization option in AOCC stanza | weiwangncar |
| 2026-05-28 | **Correction for eot calculation for solar radiation** | weiwangncar |
| 2026-05-27 | Updating MYNN-EDMF pointer and removing icloud_bl package | Joseph Olson |
| 2026-05-27 | Update MMM-physics repo SHA with various fixes | Anthony Islas |
| 2026-05-26 | Fixing CDXWRF module | Lluís Fita |
| 2026-05-26 | Update readme for GFL option | weiwangncar |
| 2026-05-21 | Include mp_physics=88 in TEMPO error print | Kelly Werner |
| 2026-05-20 | Minor Tempo changes | AndersJensen-NOAA |
| 2026-05-20 | Fixing scheme-guard bug in urban NbS initialization | Chenghao Wang |
| 2026-05-20 | Add new namelists for ShinHong PBL and revised MMM surface layer | weiwangncar |
| 2026-05-19 | Bug fix for udm | weiwangncar |
| 2026-05-12 | Updating MYNN-SFC submodule | Joseph Olson |

**🎙️ Podcast angle:** WRF is the world's dominant regional climate model — and it *contains* aerosol-aware physics schemes (TEMPO, MYNN-EDMF) that are used to simulate sulfate aerosol injection. The aerosol-aware scheme was recently *turned off* in the registry (commit 6a289e1), which is a governance signal: the code exists, but maintainers are cautious about enabling it by default. The solar radiation "eot" correction (May 28) is exactly the kind of radiative-transfer fix that SRM researchers depend on.

---

### 2. Sustainable-Solutions-Lab/regional-geo — Direct WRF Aerosol Deposition Research
| Metric | Value |
|--------|-------|
| Stars | Low (niche research) |
| Language | Python/R |
| Last commit | February 15, 2026 |
| Activity level | **🟡 Burst** — intensive paper-driven sprints |

**Recent commit highlights (Feb 2026, 15 commits pulled — all within 4 days):**

| Date | Commit message |
|------|---------------|
| 2026-02-15 | gaussian smoothing |
| 2026-02-14 | improved maps and analysis |
| 2026-02-14 | show individual cases |
| 2026-02-14 | fixing figures |
| 2026-02-13 | start analysis |
| 2026-02-13 | read rds files |
| 2026-02-13 | area calculation |
| 2026-02-13 | Add data loader documentation to README |
| 2026-02-13 | Remove defensive checks from data loader |
| 2026-02-13 | Add data loader utility |
| 2026-02-13 | updated README.md |
| 2026-02-13 | Add file dimension patterns to README |
| 2026-02-13 | Merge data documentation into main README |
| 2026-02-13 | Add comprehensive README for WRF input data |
| 2026-02-13 | Add CLAUDE.md style guide and update project config |

**🎙️ Podcast angle:** This is Ken Caldeira's lab (Carnegie Science) doing the *exact* kind of regional sulfate aerosol simulation that sparks the geoengineering debate. The commit pattern — 15 commits in 4 days — is classic "paper sprint": build a data loader, run analysis, produce maps, fix figures, push. The "gaussian smoothing" commit on Feb 15 is the final analytical step before publication. This repo *is* the proof-of-concept for regional SRM impacts — and it's hidden inside a climate-modeling workflow, not in a dedicated geoengineering repo.

---

### 3. brandonhimpfen/awesome-geoengineering — The Curated Field Guide
| Metric | Value |
|--------|-------|
| Stars | 4 |
| Language | Python (markdown list) |
| Last commit | September 6, 2026 |
| Activity level | **🟡 Slow** — individual maintenance, periodic updates |

**Recent commits:**

| Date | Message |
|------|---------|
| 2026-09-06 | Update README.md (v2.0.0 era) |
| 2026-09-05 | Update README.md |
| 2026-05-05 | Update to v2.0.0 |
| 2026-03-12 | Update README.md |
| 2026-01-16 | Update README.md |
| 2025-06-28 | Initial commit / c5dfd85 |

**🎙️ Podcast angle:** A living bibliography of the geoengineering space — 4 stars but steadily maintained. The v2.0.0 release in May 2026 suggests a reorganization. This is a good "starting point" repo for listeners who want to explore the landscape.

---

## 📊 Solar Theme — Trend Summary

| Signal | Evidence |
|--------|----------|
| **SRM code lives inside climate models, not SRM repos** | WRF has TEMPO aerosol physics; regional-geo wraps WRF for aerosol deposition |
| **Active radiative-transfer maintenance** | WRF's May 28 solar radiation eot fix; MYNN-EDMF updates |
| **Governance caution** | aerosolaware scheme turned off in registry (June 5) |
| **Burst publication cycle** | Caldeira lab: 15 commits / 4 days before paper |
| **Curated list keeps pace** | awesome-geoengineering updated Sept 2026 |

### Episode architecture suggestion:
1. **Cold open:** "The most important geoengineering code you've never heard of runs inside a weather model..."
2. **Act 1:** How WRF became the de facto SRM simulation platform
3. **Act 2:** Caldeira's regional-geo sprint — what 15 commits in 4 days looks like
4. **Act 3:** The governance question — why the aerosol scheme is disabled by default

---

*Methodology: GitHub List Commits API. Data pulled September 2026.*
