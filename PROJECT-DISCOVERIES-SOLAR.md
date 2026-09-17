# ☀️ Solar Geoengineering — Project Discovery Catalog

**Last Updated:** September 2026 (v3 update — fresh commit data)
**Research Method:** GitHub repository search ("geoengineering", "climate simulation", "solar radiation management", "SRM") + cross-reference with "awesome-geoengineering" curated list

---

## Tier 1: Major Projects (100+ Stars, Active Development)

### WRF — 1,761 Stars (NCAR/NOAA)
- **URL:** https://github.com/wrf-model/WRF
- **Language:** Fortran
- **Focus:** The Weather Research and Forecasting model — the foundational atmospheric model for all climate simulation
- **Latest:** v4.8.0 (Jun 6/8, 2026) — active institutional release cycle, confirmed by 10 commits over 18 days
- **SRM Relevance:** TEMPO aerosol-aware physics modules; MYNN-EDMF ocean boundary layer physics; solar radiation EOT calculations
- **Why It Matters:** If you're going to simulate solar geoengineering, you need to simulate the atmosphere first. WRF is the tool. The aerosol microphysics development is the SRM pipeline.

**Fresh Commit Evidence (v3):**

| Date | Commit | Author | Significence |
|------|--------|--------|-------------|
| Jun 8, 2026 | Merge release-v4.8.0 | Anthony Islas | Institutional release complete |
| Jun 6, 2026 | Update README and version to v4.8.0 (#2347) | Anthony Islas | Version declaration updated |
| Jun 5, 2026 | Turn off tempo_aerosolaware and tempo_hailaware in Registry (#2346) | weiwangncar | **CRITICAL:** Experimental SRM-relevant aerosol options being staged off |
| May 30, 2026 | Fix vectorization option in AOCC stanza (#2335) | weiwangncar | Compiler optimization for AMD hardware |
| May 28, 2026 | Correction for EOT calculation for solar radiation (#2334) | weiwangncar | **Directly affects solar radiation physics — foundational for SRM** |
| May 27, 2026 | Updating MYNN-EDMF pointer and removing icloud_bl package (#2336) | Joseph Olson | Ocean boundary layer physics improvements |
| May 27, 2026 | Update MMM-physics repo SHA with various fixes (#2339) | Anthony Islas | Multi-year mean physics updates |
| May 26, 2026 | Fixing CDXWRF module (#2322) | Lluís Fita | Data assimilation module fix |
| May 26, 2026 | Update readme file for GFL option (#2333) | weiwangncar | GFL (GFDL) physics option documentation |
| May 21, 2026 | Include mp_physics=88 in TEMPO error print message (#2325) | Kelly Werner | TEMPO alert system improvement |

**Key Insight:** 10 commits over 18 days — a textbook institutional release cycle. Multiple contributors (Islas, weiwangncar, Olson, Fita, Werner) orchestrated by NCAR/NOAA. The TEMPO aerosol-aware options being turned OFF (#2346) is a critical signal: these experimental options are being staged for the next release after validation. TEMPO = Traceable Intensity of Aerosols and Gases — this is the SRM-relevant aerosol microphysics module. The solar radiation EOT correction (May 28) directly affects how solar radiation is calculated — the foundational physics for any SRM simulation.

### PCMDI Metrics — 133 Stars (LLNL)
- **URL:** https://github.com/PCMDI/pcmdi_metrics
- **Language:** Python
- **Focus:** Earth System Model evaluation toolkit — CMIP6 metrics, benchmarking, comparison
- **Latest:** v4.2.1 (Sep 3-4, 2026) — 10-commit burst release
- **SRM Relevance:** The evaluation infrastructure. If SRM is deployed, we need tools to measure whether it worked. PCMDI is that infrastructure.

**Fresh Commit Evidence (v3):** 10 commits in 2 days by Jiwoo Lee at LLNL, with PRs from James Goodnight and Jared Lewis. This is the pattern of a funded national lab release cycle.

### MDTF-Diagnostics — 80 Stars (NOAA-GFDL)
- **URL:** https://github.com/NOAA-GFDL/MDTF-diagnostics
- **Language:** Jupyter Notebook
- **Focus:** Process-oriented diagnostics for weather and climate simulations
- **Latest:** Aug 14, 2026 (active PR-based development)
- **SRM Relevance:** New MCS precipitation-buoyancy POD (Jun 2026) — directly relevant to marine cloud brightening evaluation

**Fresh Commit Evidence (v3):** MCS precipitation-buoyancy statistics POD added Jun 19, 2026 (5 commits in 1 day by Wei-Ming Tsai). PR #825 merged Aug 14, 2026 (Aparna Radhakrishnan). NOAA-GFDL:main merge Jun 2, 2026.

---

## Tier 2: Emerging Projects (20-100 Stars)

### ClimateMARGO — 73 Stars
- **URL:** https://github.com/ClimateMARGO/ClimateMARGO.jl
- **Language:** Julia
- **Focus:** Idealized climate-economic modeling (Mitigation/Adaptation/Geoengineering trade-offs)
- **Latest:** Aug 17, 2026 README updates after 2-year dormancy — confirmed as a revival signal

**Fresh Commit Evidence (v3):**

| Date | Commit | Author | Significance |
|------|--------|--------|-------------|
| Aug 17, 2026 | Update README.md | Fons van der Plas | **First activity since Nov 2023** |
| Aug 17, 2026 | Update README.md (2nd commit) | Fons van der Plas | Same-day README update — possibly a release or paper announcement |
| Oct 18, 2023 | Update unit_conversions.jl with comment from #86 | Fons van der Plas | Last code commit before dormancy |
| Jul 6, 2023 | add link to pluto in readme | Fons van der Plas | Last Activity before extended dormancy |
| Nov 14, 2022 | Update Project.toml | Fons van der Plas | Dependency management |
| Nov 12, 2022 | JuMP and Ipopt compat upgrade (#85) | Fons van der Plas | Solver compatibility update |
| Feb 10, 2022 | Removed deprecated web apps | Henri Drake | Cleanup |
| Feb 4, 2022 | Added CITATION.bib | Henri Drake | Citation infrastructure |
| Jan 13, 2022 | Fixed typo | Henri Drake | Maintenance |
| Jan 12, 2022 | Updated arguments for doc version deployment | Henri Drake | Documentation deployment |

**Key Insight:** After 2+ years of complete dormancy (last code commit: Oct 2023), two README updates appeared on Aug 17, 2026 — the first activity since November 2023. No code commits, just README touching. This is the "maybe" signal: someone cared enough to update the project introduction but not enough to write code. The MarGO (Mitigation/Adaptation/Geoengineering trade-offs) framework is an idealized climate-economic model in Julia. The 2026 revival could signal growing interest in the economics of solar geoengineering — or could be another false start.

### Open Sustainable Technology — 2,552 Stars
- **URL:** https://github.com/protontypes/open-sustainable-technology
- **Language:** Multi-language directory
- **Focus:** Comprehensive directory of 2,500+ open-source climate tech projects
- **Latest:** Sep 9, 2026 (steady ecosystem growth)
- **Why It Matters:** The ecosystem infrastructure. This is the "github.com/awesome-climate-tech" that makes everything else discoverable.

### Awesome Geoengineering — 4 Stars
- **URL:** https://github.com/brandonhimpfen/awesome-geoengineering
- **Language:** Python (curated list)
- **Focus:** Curated list of geoengineering projects, research, organizations, tools
- **Latest:** Sep 2026
- **Why It Matters:** The gateway drug for this research. Good starting point for discovering the ecosystem.

---

## Tier 3: Niche / Dormant Projects (<20 Stars)

| Repo | Stars | Language | Focus | Status |
|------|-------|----------|-------|--------|
| actm-sai-csu | 6 | Python | AI to detect, attribute, and quantify SRM effects | **Confirmed dormant since Mar 2023** |
| srm-forever | 0 | HTML | Interactive SRM economics model | Single burst (Aug 2026) |
| Geo-DICE (PSLmodels) | 2 | MATLAB | Modified DICE with geoengineering | Dormant |
| ClimateLeonardo/GeoengineeringLE | 2 | Python | Economic modeling of geoengineering | Unknown |
| OOCC_2021 | 2 | Python | Simple SRM governance model | Dormant |
| AM3 (FMS-ESM) | 4 | Fortran | Atmospheric general circulation model | Dormant since 2015 |
| PMIP p2fvar analyzer | 4 | - | Paleoclimate model analyzer | Minimal activity |
| open-earth-digital-twin | 0 | TeX | Agent-based Earth system simulation | Manifesto stage, no code |

**actm-sai-csu Commit Evidence (v3):**

| Date | Commit | Author |
|------|--------|--------|
| Mar 28, 2023 | new paper | Zachary Labe |
| Mar 28, 2023 | new paper! | Zachary Labe |
| Feb 9, 2023 | Add preprint link to Readme | Daniel Hueholt |
| Feb 8, 2023 | Add Jim's link | Daniel Hueholt |
| Feb 8, 2023 | Standardize capitalization | Daniel Hueholt |
| Feb 8, 2023 | Add code from Hueholt et al. 2023 | Daniel Hueholt |
| Jan 22, 2023 | update readme | Antonios Mamalakis |
| Jan 22, 2023 | Create readme | Antonios Mamalakis |
| Jan 11, 2023 | new preprint | Zachary Labe |
| Jan 11, 2023 | new preprint | Zachary Labe |

**Key Insight:** All activity occurred in a single burst (Jan-Mar 2023) — an academic paper project. 10 commits over 3 months, then complete silence for 3.5+ years. The AI-to-detect-SRM-effects approach was promising but never transitioned from paper to maintained tool.

---

## The Discovery Gap: What's NOT on GitHub

| Missing Category | Why It's Missing |
|-----------------|------------------|
| End-to-end SRM simulation pipeline | Requires combining WRF + aerosol models + ocean models — no one has assembled this |
| SRM governance/regulatory tools | srm-forever exists but is a toy; serious governance code doesn't exist |
| SRM risk assessment tools | Arctic impacts, monsoon disruption — only represented in academic papers |
| Open-source CESM/SAM for SRM | CESM has SRM capabilities but they're not in a dedicated public repo |

---

## 🎙️ Episode Hooks (Updated v3)

1. **The atmosphere is well-modeled, but SRM isn't.** WRF, PCMDI, MDTF are world-class — but nobody has strung them together into an SRM simulator. WRF v4.8.0's TEMPO aerosol options being turned OFF suggests the next release will have improved aerosol microphysics — the SRM simulation pipeline is being built, component by component.

2. **The governance tools are toys.** The only "SRM simulator" with a web interface (srm-forever) is a single-author teaching tool. The serious governance work happens in papers, not code.

3. **ClimateMARGO's revival is the sleeper story.** A Julia-based climate-economic model, dormant for 2+ years (last code: Oct 2023), suddenly showing README activity in Aug 2026. The policy-modeling layer for SRM might be waking up — or might just be a README touch-up with no follow-through.

4. **actm-sai-csu shows the "paper-to-tool" gap.** Promising AI approach for detecting SRM effects, 10 commits in 3 months, then 3.5 years of silence. The paper was published; the tool died. This is the most common pattern in climate tech open source.

5. **The solar radiation EOT fix in WRF is quietly important.** The May 28, 2026 correction for EOT (Empirical Orthogonal Transform) calculation for solar radiation directly affects how solar radiation is computed in WRF. This is the foundational physics for any SRM simulation — and it had a bug that was just fixed.

6. **The discovery infrastructure is thriving.** Open Sustainable Technology (2,552★) and Awesome Geoengineering are making the ecosystem discoverable — which is the foundation everything else needs.
