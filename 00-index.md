# ☀️ Solar Geoengineering — Episode Research Notes

> **Branch:** `solar-geoengineering`  
> **Theme:** Solar Radiation Management (SRM)  
> **Last Updated:** 2026-09-16

---

## 🎙️ Episode Overview

Solar geoengineering (SRM) aims to reflect a small fraction of sunlight back to space to cool the planet. The central tension for this episode: the science is fast-moving, but the **open-source codebase is sparse** — most SRM simulation happens inside closed academic labs (GFDL, NCAR, ETH Zürich). What does it mean for governance when the code that could answer the hardest questions about SRM risks isn't publicly auditable?

---

## 🔍 Project Discoveries

### Top-Ranked Projects

| Repo | Stars | Language | Last Updated | Focus | Relevance |
|------|-------|----------|-------------|-------|-----------|
| **protontypes/open-sustainable-technology** | 2,546 | Python | Sep 2026 | Comprehensive OSS climate-tech directory | Curated index; contains SRM entries |
| **Fatema-Nur/LOD-Climate-Prediction-System** | — | Python | Nov 2025 | Physics-based climate simulation for SRM scenarios | Direct SRM modeling |
| **prashaant1926/open-earth-digital-twin-simulation** | — | Python | Oct 2025 | Earth system digital twin for climate intervention studies | System-level SRM simulation |
| **FMS-ESM/AM3** | 4 | Fortran | Mar 2015 | GFDL atmospheric model (legacy) | Foundational climate model; used in SRM studies |
| **pmip4/pmip_p2fvar_analyzer** | 4 | Python | Sep 2025 | CMIP6 climate data analysis | Analysis tooling for SRM experiment data |
| **RhondaMueller/Codes-RFG-Arctic-Impacts** | 1 | Python | Apr 2024 | Geoengineering radiative forcing on Arctic ice | Regional SRM impact assessment |
| **ClimateMARGO/ClimateMARGO.jl** | 73 | Julia | Aug 2026 | Idealized climate-economic planning framework (MARGO) | Optimizes trade-offs: mitigation vs. adaptation vs. geoengineering deployment timing |
| **PSLmodels/Geo-DICE** | 2 | MATLAB | — | Modified DICE model incorporating geoengineering cost-benefit | Integrated assessment modeling with SRM |
| **jlehtomaa/OOCC_2021** | 2 | Python | — | Simple model for solar geoengineering governance | Governance scenarios |
| **cjcarlson/geomalaria** | 3 | R | — | Malaria risk modeling in a world with solar geoengineering | Health impact of SRM |

### Key Themes

1. **The Simulation Gap** — Most operational SRM models (GFDL's AM3, CAM-CTM) are proprietary or locked behind institutional login. The handful of open attempts (LOD-Climate, Earth Digital Twin) are early-stage.
2. **Julia's Rising Role** — ClimateMARGO.jl (73★) shows Julia becoming the language of choice for climate-economic optimization problems that blend SRM with policy.
3. **Regional Risk is the Uncomfortable Question** — RhondaMueller's Arctic impacts code and geomalaria's health modelling are the only repos that tackle the *distributional* consequences of SRM.

---

## 📊 Commit Trend Analysis

### WRF Model (wrf-model/WRF) — 1,761★ — *Most Active Climate Simulation Codebase*
Last commits all clustered in May–June 2026:

| Commit | Author | Date | Summary |
|--------|--------|------|---------|
| `06d4240` | Anthony Islas | Jun 8, 2026 | Merge release-v4.8.0 branch |
| `0708348` | Anthony Islas | Jun 6, 2026 | Update README & version to v4.8.0 (#2347) |
| `6a289e1` | weiwangncar | Jun 5, 2026 | Turn off tempo_aerosolaware & tempo_hailaware in Registry (#2346) |
| `4466746` | weiwangncar | May 30, 2026 | Fix vectorization option in AOCC stanza (#2335) |
| `e836cd6` | weiwangncar | May 28, 2026 | Correction for eot calculation for solar radiation (#2334) |

**Trend:** WRF is in active maintenance mode, bumping versions and fixing physics modules. The aerosol-aware physics (temporarily turned off) and solar radiation corrections are directly relevant to SRM — aerosol intervention and solar flux modeling are two paths to the same goal. The fact that these fixes come from `weiwangncar` (NCAR staff) confirms that SRM-adjacent physics lives inside institutional codebases.

### ClimateMARGO.jl — 73★ — *Most Active Geo-Economic Model*

| Commit | Author | Date | Summary |
|--------|--------|------|---------|
| `d916f36` | Fons van der Plas | Aug 17, 2026 | Update README.md |
| `6d9ba7a` | Fons van der Plas | Aug 17, 2026 | Update README.md |
| `57d4da7` | Fons van der Plas | Oct 18, 2023 | Update unit_conversions.jl with comment from #86 |
| `fbbe619` | Fons van der Plas | Jul 6, 2023 | Add link to Pluto notebook in README |
| `5063c42` | Fons van der Plas | Nov 14, 2022 | Update Project.toml |

**Trend:** Single-author maintenance (Fons van der Plas). Two README updates in one day (Aug 2026) suggest a recent refresh likely tied to a new publication or version release. The long gaps between earlier commits (2022–2023) and the 2026 burst make this an interesting case study for how academic open-source climate models get sustained.

### clisops (roocs/clisops) — 25★ — *Climate Simulation Operations*

| Commit | Author | Date | Summary |
|--------|--------|------|---------|
| `a7ca1d6` | github-actions[bot] | Sep 8, 2026 | Bump httpx2 2.5.0→2.12.0 (#510) |
| `026c615` | dependabot[bot] | Sep 8, 2026 | Bump httpx2 2.5.0→2.12.0 |
| `9a3b8f2` | github-actions[bot] | Sep 8, 2026 | Bump pip 26.1.2→26.2 (#511) |
| `0c72e75` | dependabot[bot] | Sep 8, 2026 | Bump pip 26.1.2→26.2 |
| `75dc87b` | github-actions[bot] | Sep 1, 2026 | Bump pygments 2.19.1→2.20.0 (#509) |

**Trend:** Entirely dependency updates via CI bots. No scientific development commits visible in the recent window — clisops has matured into a stable operations layer. For SRM research, this means the *post-processing* infrastructure (climate data extraction, formatting) is solid, but the *modeling* layer needs to come from elsewhere.

### Xanthos (JGCRI/xanthos) — 38★ — *Global Hydrologic Framework*

| Commit | Author | Date | Summary |
|--------|--------|------|---------|
| `9ad117a` | Mengqi Zhao | Aug 21, 2023 | Update citations and publications |
| `0aaf320` | Mengqi Zhao | Jun 2, 2023 | Update quick_starter.ipynb |
| `30ac6df` | Mengqi Zhao | May 26, 2023 | Update notebook and setup.py |
| `946c0c3` | Mengqi Zhao | May 23, 2023 | Add xanthos tutorial notebook |
| `c2b11d5` | Mengqi Zhao | May 3, 2023 | Update xanthos version in install_supplement.py |

**Trend:** All commits from May–Aug 2023, all by one author (Mengqi Zhao). The cluster of commits in a single month (May–June 2023) suggests a release effort. After that, silence — Xanthos is in maintenance mode. Hydrology is critical for SRM because stratospheric aerosol injection would alter global precipitation patterns; Xanthos provides the modeling framework to study those impacts.

### GeoVision (pixnum-hub/GeoVision) — Geoengineering Simulator

| Commit | Author | Date | Summary |
|--------|--------|------|---------|
| `831ef39` | Manik Roy | Dec 6, 2025 | Update README.md |
| `e219148` | Manik Roy | Dec 6, 2025 | Create LICENSE |
| `a5bf50f` | Manik Roy | Dec 6, 2025 | Add files via upload |
| `20ccd35` | Manik Roy | Dec 6, 2025 | Initial commit |

**Trend:** All four commits on a single day (Dec 6, 2025) — looks like a one-shot push of an initial project. No maintenance momentum. GeoVision as a geoengineering simulator exists on paper but hasn't attracted contributors. Illustrates the upload-vs-sustainability problem in open-source climate tech.

---

## 🎙️ Episode Narrative Arc

1. **Hook** — The hardest SRM questions (regional precipitation disruption, ozone impacts) can *only* be answered by models that aren't publicly available.
2. **The Hub** — ClimateMARGO.jl as a case study of open climate-economic SRM planning (73★, Julia).
3. **The Gap** — Compare WRF's active aerosol/physics development (inside NCAR) vs. the handful of open SRM simulation repos.
4. **The Risk** — geomalaria and Arctic impacts codes show that SRM's redistribution of climate risk is the most politically explosive question.
5. **The Path Forward** — What would open-source SRM simulation require? Shared parameterizations, common experimental protocols, transparent governance.

---

## 🔗 Key Links
- [ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- [WRF Model](https://github.com/wrf-model/WRF)
- [Geo-DICE](https://github.com/PSLmodels/Geo-DICE)
- [LOD-Climate-Prediction-System](https://github.com/Fatema-Nur/LOD-Climate-Prediction-System)
- [Open Earth Digital Twin](https://github.com/prashaant1926/open-earth-digital-twin-simulation)
- [geomalaria](https://github.com/cjcarlson/geomalaria)
- [Codes-RFG-Arctic-Impacts](https://github.com/RhondaMueller/Codes-RFG-Arctic-Impacts)