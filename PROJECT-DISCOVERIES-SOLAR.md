# ☀️ Solar Geoengineering — Project Discoveries

**Branch:** `solar-geoengineering` | **Last Updated:** September 2026 (v4)

Detailed profiles of open-source repositories relevant to solar geoengineering, atmospheric modeling, and climate-information infrastructure.

---

## Tier 1: High-Activity, Institutionally Funded

### 1. WRF — Weather Research and Forecasting Model
- **Repo:** [wrf-model/WRF](https://github.com/wrf-model/WRF)
- **Stars:** 1,762 | **Language:** Fortran | **Last commit:** June 8, 2026
- **Focus:** The foundational atmospheric model for weather and climate simulation. Version 4.8.0 recently released.
- **Why it matters for solar geoengineering:** WRF is the primary tool used to evaluate the atmospheric effects of stratospheric aerosol injection (SAI). Any simulation of solar geoengineering's climate impacts must pass through WRF's physics suite.

**Recent Commit Highlights (15 commits pulled):**
| Date | Commit | Significence |
|------|--------|-------------|
| Jun 8, 2026 | Merge v4.8.0 release | Major version milestone |
| Jun 6, 2026 | README & version update to v4.8.0 | Documentation sync |
| May 28, 2026 | **Correction for EOF calculation for solar radiation** | Direct solar radiation fix — core physics improvement |
| May 27, 2026 | MYNN-EDMF pointer update; remove icloud_bl package | Boundary layer physics refinement |
| May 26, 2026 | GFL option readme update | New gravity wave drag option |
| May 21, 2026 | Include mp_physics=88 in TEMPO error print | TEMPO chemistry option expanded |
| May 20, 2026 | Minor Tempo changes; urban NbS scheme-guard bug fix | Atmospheric chemistry + urban physics |
| May 20, 2026 | Add new namelists for ShinHong PBL and revised MMM surface layer | New PBL scheme — critical for aerosol transport |
| May 19, 2026 | Bug fix for udm | University of Delaware Module fix |
| May 12, 2026 | Update MYNN-SFC submodule | Surface layer physics |

**🎙️ Episode Hook:** The May 28 solar radiation correction is the single most solar-relevant commit. A qualitative error in EOF calculation could change how much solar energy is reflected vs. absorbed in SAI simulations. This is the kind of bug that could alter the entire cost-benefit analysis of solar geoengineering.

---

### 2. PCMDI — PCMDI Metrics (CMIP6 Evaluation Toolkit)
- **Repo:** [PCMDI/pcmdi_metrics](https://github.com/PCMDI/pcmdi_metrics)
- **Stars:** 133 | **Language:** Python | **Last commit:** September 17, 2026
- **Focus:** The official toolkit for evaluating Earth System Models against CMIP6 observational benchmarks. Used to answer: "How good are the models that we base geoengineering decisions on?"
- **Why it matters:** You can't evaluate solar geoengineering impacts if you can't evaluate the baseline models. PCMDI metrics are the quality-control infrastructure for all climate projections, including those used in SAI research.

**Recent Commit Highlights (15 commits pulled):**
| Date | Commit | Significence |
|------|--------|-------------|
| Sep 17, 2026 | Merge PR #1431 — modpath_list patch | Bug fix for path handling |
| Sep 4, 2026 | **Bump version to 4.2.1** | Latest release — 10 commits in 2 days! |
| Sep 4, 2026 | Prepare v4.2.1; roundoff fix in mean_climate | Precision fix — prevents roundoff to 1.00 |
| Sep 3, 2026 | Extremes chunking (dask/SVD memory optimization) | Handle larger datasets for extreme-event analysis |
| Sep 3, 2026 | Force numpy SVD; chore rename | Performance + code cleanup |

**🎙️ Episode Hook:** Ten commits in two days for v4.2.1. This is the "morning after" pattern — a release happens, then the community converges to fix the bugs. The roundoff fix (preventing 1.00 instead of 0.9999 in mean climate figures) is a perfect podcast anecdote: the difference between a correct model evaluation and a misleading one is literally in the last decimal place.

---

### 3. ClimateMARGO — Climate Economic Modeling Framework
- **Repo:** [ClimateMARGO/ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- **Stars:** 73 | **Language:** Julia | **Last commit:** August 17, 2026
- **Focus:** An idealized climate-economic modeling framework for optimizing trade-offs between emissions mitigation, adaptation, and solar geoengineering.
- **Why it matters:** This is one of the very few open-source tools that explicitly models the *decision problem* of solar geoengineering — not just the physics, but the economics and governance. It answers: "When is it optimal to deploy SAI vs. mitigate?"

**Recent Commit Highlights (15 commits pulled):**
| Date | Commit | Significence |
|------|--------|-------------|
| Aug 17, 2026 | **Update README.md (2 commits same day)** | Revival signal after 2+ year dormancy! |
| Oct 18, 2023 | Update unit_conversions.jl (referenced PR #86) | Last code change before dormancy |
| Jul 6, 2023 | Add Pluto notebook link | Interactive documentation |
| Nov 14, 2022 | Update Project.toml | Dependency management |
| Nov 12, 2022 | JuMP and Ipopt compat upgrade (#85) | Solver compatibility |
| Feb 10, 2022 | Removed deprecated web apps | Cleanup |
| Jan 12, 2022 | Bulk: CITATION.bib, doc deployment, version bump, README update | Last productive period |

**🎙️ Episode Hook:** ClimateMARGO went dormant from Jan 2022 to Oct 2023, then had a burst of activity (unit conversions fix, Pluto notebook), then went quiet again until Aug 2026 when the README was updated twice in one day. Is someone preparing a paper? A new version? Or is this another false start? The 2.5-year dormancy followed by a README-only revival is the perfect case study for a podcast segment on the "state of solar geoengineering modeling."

---

## Tier 2: Conceptually Important, Low Visibility

### 4. SRM Forever?
- **Repo:** [hausfath/srm-forever](https://github.com/hausfath/srm-forever)
- **Stars:** 0 | **Language:** HTML/JavaScript | **Last commit:** August 26, 2026
- **Focus:** An interactive model asking: "Could it make economic sense to decarbonize slowly while holding 1.5°C with stratospheric aerosol injection for as long as it takes, rather than mitigating rapidly and drawing temperatures back down with carbon removal?"
- **Why it matters:** This is the most directly relevant solar geoengineering tool on GitHub, despite having zero stars. It uses Weitzman certainty-equivalent discounting to compare SRM-forever vs. mitigation+CDR scenarios. The answer depends almost entirely on the discount rate choice — which is itself a deep governance question.

**Recent Commit Highlights (4 commits, all on August 26, 2026):**
| Date | Commit | Significence |
|------|--------|-------------|
| Aug 26, 2026 | Add effective discount rate chart | Visualization enhancement |
| Aug 26, 2026 | **Adopt Weitzman certainty-equivalent discounting; add essay** | Major theoretical upgrade |
| Aug 26, 2026 | Price abatement as a vintage annuity | Refined economic framing |
| Aug 26, 2026 | Initial commit: Interactive SRM-forever vs mitigation+CDR cost model | Full launch |

**🎙️ Episode Hook:** All four commits happened on a single day — this was a "big bang" release. The Weitzman discounting framework is the intellectual core: under default settings, the SRM-forever scenario is cheaper in NPV (~$42T vs. ~$55T), but the TCRE likely range straddles the verdict. The breakeven mean discount rate is ~0.9% — squarely inside the range experts actually debate. This is a perfect "tension" for a podcast narrative.

---

## Tier 3: Adjacent — Atmospheric Chemistry & Air Quality

### 5. WRF Extended (via submodules and chemistry options)
- TEMPO (Trace Atmospheric Gas Instrument) chemistry option being actively developed
- Urban Nature-based Solutions (NbS) module with scheme-guard bug fixes
- MYNN PBL and surface layer physics — critical for simulating aerosol injection

### 6. PCMDI-extremes (via PCMDI metrics chunking work)
- Dask/SVD memory optimization for extreme-event analysis
- These tools will be needed to evaluate the impacts of SAI on temperature extremes (heatwaves, cold spells)

---

## Summary Table: Solar Theme Repos

| Repo | Stars | Last Activity | Status | Episode Potential |
|------|-------|--------------|--------|------------------|
| wrf-model/WRF | 1,762 | Jun 2026 (active) | ✅ Sustained institutional development | ⭐⭐⭐ Core tool story |
| PCMDI/pcmdi_metrics | 133 | Sep 2026 (very active) | ✅ Rapid release cycle | ⭐⭐⭐ QC infrastructure story |
| ClimateMARGO/ClimateMARGO.jl | 73 | Aug 2026 (dormant→revival) | ⚠️ Ambiguous revival | ⭐⭐⭐ Governance modeling story |
| hausfath/srm-forever | 0 | Aug 2026 (new) | 🆕 Single-day launch | ⭐⭐⭐ Economics/philosophy story |

---

## 🎙️ Cross-Cutting Narrative Threads for Solar Episode

1. **The Bug That Changes Everything** — The May 28 solar radiation EOF correction in WRF. A qualitative error in core physics. How do you trust SAI simulations when the fundamental radiation code gets corrected?

2. **The Decimal Place That Matters** — PCMDI's roundoff fix (preventing 1.00 instead of 0.9999). Model evaluation is in the precision. If you can't evaluate the baseline, you can't evaluate the intervention.

3. **The Dormant Giant** — ClimateMARGO's 2.5-year silence followed by a README-only update. What does it mean when the best solar geoengineering economic model stops being developed? Is it a funding problem, a field problem, or a political problem?

4. **The Zero-Star Time Machine** — SRM-forever has 0 stars but is arguably the most directly relevant tool. It asks the question that matters: "Is it cheaper to run SRM forever, or to mitigate + remove?" The answer depends on a discount rate that experts can't agree on.

5. **The Institutional Paradox** — WRF and PCMDI are well-funded, fast-moving institutions. ClimateMARGO and srm-forever are individual, unfunded, and fragile. Solar geoengineering science depends on infrastructure, but the decisions about whether to deploy it are being made by people who build tools in their spare time.
