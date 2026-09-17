# Solar Geoengineering — Detailed Commit Trend Analysis

> This file contains the raw commit-level analysis from 5 GitHub repositories relevant to the solar geoengineering episode.

---

## Repository 1: wrf-model/WRF — Weather Research & Forecasting
⭐ **1,761 stars | Fortran | Active (June 2026)**

### Recent Commits (8 most recent)

| Commit | Author | Date | Summary |
|--------|--------|------|---------|
| `06d4240` | Anthony Islas | Jun 8, 2026 | Merge release-v4.8.0 branch |
| `0708348` | Anthony Islas | Jun 6, 2026 | Update README and version declaration to new v4.8.0 |
| `6a289e1` | weiwangncar | Jun 5, 2026 | Turn off tempo_aerosolaware and tempo_hailaware in Registry |
| `4466746` | weiwangncar | May 30, 2026 | Fix a vectorization option in AOCC stanza |
| `e836cd6` | weiwangncar | May 28, 2026 | Correction for eot calculation for solar radiation |
| `8299919` | Joseph Olson | May 27, 2026 | Updating MYNN-EDMF pointer and removing icloud_bl package |
| `4fab0e2` | Anthony Islas | May 27, 2026 | Update MMM-physics repo SHA with various fixes |
| `75ad1f9` | Lluís Fita | May 26, 2026 | Fixing CDXWRF module |

### Trend Insights
- **Release-driven development:** v4.8.0 release cycle dominated May–June 2026
- **Aerosol physics focus:** Multiple commits modify aerosol-aware modules (tempo_aerosolaware) — directly relevant to SRM aerosol injection modeling
- **Solar radiation corrections:** Commit `e836cd6` fixes solar radiation calculation — foundational for any SRM radiative transfer work
- **Institutional contributors:** NCAR (weiwangncar), NSSL (Anthony Islas), NSSL/CIWRO (Joseph Olson), Girona (Lluís Fita)
- **Development velocity:** 8 commits in ~2 weeks, all by core contributors

---

## Repository 2: ClimateMARGO/ClimateMARGO.jl
⭐ **73 stars | Julia | Active (Aug 2026)**

### Recent Commits (8 most recent)

| Commit | Author | Date | Summary |
|--------|--------|------|---------|
| `d916f36` | Fons van der Plas | Aug 17, 2026 | Update README.md |
| `6d9ba7a` | Fons van der Plas | Aug 17, 2026 | Update README.md |
| `57d4da7` | Fons van der Plas | Oct 18, 2023 | Update unit_conversions.jl with comment from #86 |
| `fbbe619` | Fons van der Plas | Jul 6, 2023 | Add link to Pluto in README |
| `5063c42` | Fons van der Plas | Nov 14, 2022 | Update Project.toml |
| `12a0ce6` | Fons van der Plas | Nov 12, 2022 | JuMP and Ipopt compat upgrade (#85) |
| `32e66fd` | Henri Drake | Feb 10, 2022 | Removed deprecated web apps |
| `d609d49` | Henri Drake | Feb 4, 2022 | Added CITATION.bib |

### Trend Insights
- **Single maintainer:** Fons van der Plas drives ~75% of all commits
- **Recovery pattern:** Long quiet periods (2022–2023) interrupted by README/docs updates in 2026 — suggests renewed academic interest
- **Dependency modernization:** 2022 commits focused on JuMP/Ipopt compatibility — optimization solver upgrades
- **Two eras:** Henri Drake era (2022: initial setup, deprecations) → Fons van der Plas era (2022–present: maintenance, docs, updates)

---

## Repository 3: pixnum-hub/GeoVision — Geoengineering Simulator
⭐ **~0 visible stars | HTML | Brand new (Dec 2025)**

### Recent Commits (4 total)

| Commit | Author | Date | Summary |
|--------|--------|------|---------|
| `831ef39` | Manik Roy | Dec 6, 2025 | Update README.md |
| `e219148` | Manik Roy | Dec 6, 2025 | Create LICENSE |
| `a5bf50f` | Manik Roy | Dec 6, 2025 | Add files via upload |
| `20ccd35` | Manik Roy | Dec 6, 2025 | Initial commit |

### Trend Insights
- **All commits in one day:** Complete initial project skeleton in a single push
- **No stars yet, no forks:** Not yet discovered by community
- **HTML-only:** Frontend visualization simulator, no backend model — likely interactive/educational tool
- **Potential:** Could evolve into a serious SRM visualization tool if maintained; currently a proof-of-concept

---

## Repository 4: PSLmodels/Geo-DICE
⭐ **2 stars | MATLAB | Dormant (2016–2018)**

### Recent Commits (4 total)

| Commit | Author | Date | Summary |
|--------|--------|------|---------|
| `82a0370` | Soheil Shayegh | Sep 27, 2018 | Add files via upload |
| `fe8da8e` | Soheil Shayegh | Aug 15, 2016 | Add files via upload |
| `b2f65e6` | Soheil Shayegh | Aug 15, 2016 | Add files via upload |
| `82e4f18` | Matt Jensen | Aug 15, 2016 | Initial commit |

### Trend Insights
- **All activity 2016–2018:** No commits in ~8 years — abandoned
- **Two contributors:** Matt Jensen (initial) → Soheil Shayegh (all substantive work)
- **DICE model extension:** DICE is the standard integrated assessment model; geoengineering extension was forward-thinking for 2016
- **Uploaded as datasets:** "Add files via upload" suggests direct file pushes rather than Git LFS or proper structured commits

---

## Repository 5: NCAR_ML_EKE (CrayLabs)
⭐ **20 stars | Jupyter Notebook | Dormant (2021–2022)**

### Recent Commits (8 total)

| Commit | Author | Date | Summary |
|--------|--------|------|---------|
| `5b2d6cf` | Andrew Shao | Mar 30, 2022 | Fix notebook typos (#10) |
| `c4028e5` | Andrew Shao | Mar 28, 2022 | Refactor driver for colocated option (#9) |
| `aa0abc8` | Sam Partee | Mar 14, 2022 | Update MOM6 instructions and submodule |
| `6586405` | Andrew Shao | Feb 9, 2022 | Update README.md for compiling MOM6 |
| `962e6c6` | Andrew Shao | Feb 8, 2022 | Update MOM6 submodule |
| `b30698f` | Sam Partee | Jul 23, 2021 | Edit README |
| `b300602` | Sam Partee | Apr 13, 2021 | Create LICENSE |
| `90b0430` | Sam Partee | Apr 13, 2021 | Update README.md |

### Trend Insights
- **Machine Learning + Ocean Climate:** Applies ML (via SmartSim) at scale in HPC simulations for ocean climate modeling
- **MOM6 submodule:** Uses MITgcm's MOM6 ocean model — directly relevant to ocean-based geoengineering simulation
- **Two contributors:** Andrew Shao (ML/driver code) + Sam Partee (documentation, MOM6)
- **NCAR collaboration:** CrayLabs = NCAR's supercomputing division
- **Trend sign:** While not SRM-specific, this represents the ML-for-climate-simulation trend that will eventually extend to SRM modeling

---

## Summary: Solar Geoengineering Codebase Health

| Dimension | Assessment |
|-----------|------------|
| Open-source simulation depth | ⭐⭐☆☆☆ — Repurposed weather models (WRF), purpose-built SRM code is scarce |
| Institutional backing | ⭐⭐⭐⭐⭐ — NCAR, GFDL, PSL pivot heavily invested in closed-code versions |
| Community maintenance | ⭐⭐☆☆☆ — ClimateMARGO.jl is the best case; most projects are institutional or dormant |
| Recent momentum | ⭐⭐⭐☆☆ — GeoVision (new), MARGO (renewed), WRF (continuously active) |
| Governance modeling | ⭐☆☆☆☆ — Almost no open-source SRM governance tools exist |
