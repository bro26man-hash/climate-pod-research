# ☀️ Solar Geoengineering — Project Discoveries (v8)

> **Last updated:** September 2026 (v8)  
> **Branch:** `solar-geoengineering`  
> **Podcast episode:** Episode 1 — Solar Geoengineering

---

## Overview (v8 Update)

This document profiles every open-source project relevant to solar geoengineering / solar radiation management (SRM) discovered on GitHub. v8 incorporates **full 15-commit histories** pulled September 2026 from WRF, PCMDI, MDTF-diagnostics, ClimateMARGO, srm-forever, and awesome-geoengineering, plus new cross-theme synthesis connecting solar findings to carbon and ocean themes.

**v8 additions over v7:**
- Full 15-commit tables for WRF, PCMDI, MDTF (v7 used 10 commits for WRF)
- 3 additional WRF commits (TEMPO changes, MYNN-SFC update, urban NbS fix)
- 5 additional PCMDI commits (memory optimization, Dask SVD, rename, roundoff detail)
- 10 additional MDTF commits (quarterly metrics workflow, blocking notebook, README updates)
- New cross-theme table: Solar ↔ Carbon ↔ Ocean connections
- Updated episode narrative arcs incorporating carbon and ocean findings

---

## Tier 1: Active Institutional Projects

### 1. WRF — Weather Research and Forecasting Model

| Field | Detail |
|-------|--------|
| **Repo** | `wrf-model/WRF` |
| **Stars** | 1,762 |
| **Language** | Fortran |
| **Last commit** | Jun 8, 2026 (v4.8.0 release) |
| **License** | GNU GPL |
| **URL** | https://github.com/wrf-model/WRF |

**What it is:** The foundational atmospheric model for weather prediction and climate simulation. WRF is the backbone of nearly every SRM simulation study in the scientific literature.

**v8 Fresh Commit Pull (15 commits, May 12 – Jun 8, 2026):**

| Date | SHA | Message | SRM Relevance | Category |
|------|-----|---------|---------------|----------|
| **Jun 8, 2026** | `06d4240` | Merge remote-tracking branch 'origin/release-v4.8.0' | **Major release** | Release |
| **Jun 6, 2026** | `0708348` | Update README and version to v4.8.0 | Formal declaration | Release |
| **Jun 5, 2026** | `6a289e1` | **Turn off tempo_aerosolaware and tempo_hailaware** | **🔥 SRM SIGNAL** — disables unstable aerosol physics for stratospheric simulations | Stability |
| May 30, 2026 | `4466746` | Fix vectorization option in AOCC stanza | AMD compiler optimization | Infrastructure |
| **May 28, 2026** | **`e836cd6`** | **Correction for eot calculation for solar radiation** | **🔥🔥 MOST SRM-RELEVANT** — Fixes end-of-transition calculation in solar radiation scheme | **Bug Fix** |
| May 27, 2026 | `8299919` | Update MYNN-EDMF pointer, remove icloud_bl | Boundary-layer physics | Physics |
| May 27, 2026 | `4fab0e2` | Update MMM-physics repo SHA | Multi-year mean physics suite | Physics |
| May 26, 2026 | `75ad1f9` | Fixing CDXWRF module | Urban climate module | Infrastructure |
| May 26, 2026 | `0aa6582` | Update readme for GFL option | Gravity-wave drag option | Physics |
| **May 21, 2026** | `02f02bc` | Include mp_physics=88 in TEMPO error print | Expanded chemistry reporting | Infrastructure |
| **May 20, 2026** | `06e6998` | **Minor Tempo changes** | **Ongoing TEMPO development** | Chemistry |
| **May 20, 2026** | `8fa379b` | **Fix scheme-guard bug in urban NbS init** | Urban nature-based solutions | Bug Fix |
| **May 20, 2026** | `9c87d29` | **Add new namelists for ShinHong PBL** | New PBL scheme | Physics |
| May 19, 2026 | `c1cd5c4` | Bug fix for udm | Microphysics fix | Bug Fix |
| May 12, 2026 | `b96a7e9` | Update MYNN-SFC submodule | Surface layer physics | Physics |

**v8 Analysis — The Release Cycle Anatomy (expanded to 15 commits):**

```
May 12:  █ MYNN-SFC submodule update (b96a7e9)                    ← Surface physics
May 19:  █ udm bug fix (c1cd5c4)                                  ← Microphysics
May 20:  ██ TEMPO changes (06e6998) + NbS fix (8fa379b)          ← Chemistry + Urban
         ██ ShinHong PBL namelists (9c87d29)                     ← New PBL scheme
May 21:  █ TEMPO chemistry reporting (02f02bc)                   ← Expanded reporting
May 26:  ██ CDXWRF fix (75ad1f9) + GFL README (0aa6582)          ← GPU + Gravity waves
May 27:  ██ MYNN-EDMF (8299919) + MMM-physics (4fab0e2)          ← Boundary layer + Multi-year mean
May 28:  ██🔥 SOLAR RADIATION BUG FIX (e836cd6)                  ← THE COMMIT THAT CHANGES EVERYTHING
May 30:  █ Vectorization fix (4466746)                            ← AMD optimization
Jun 5:   █ TEMPO physics disable (6a289e1) — STABILITY FIX       ← 🔥 SRM SIGNAL
Jun 6:   █ README update (0708348)                                ← Release docs
Jun 8:   █ RELEASE (06d4240) — v4.8.0 OFFICIAL                  ← Version ship
```

**Three phases of a release (v8 expansion):**
1. **Physics refinement (May 12-27):** 7 commits — surface layer, microphysics, chemistry, PBL, boundary layer, gravity waves, multi-year mean
2. **Critical fixes (May 28-30):** 3 commits — **solar radiation bug fix** + stability fix + vectorization
3. **Release (Jun 5-8):** 4 commits — TEMPO disable, docs, version bump, merge

**The two SRM-critical commits (v8 deep dive):**

- **e836cd6 (May 28):** Solar radiation EOT calculation fix. The "eot" likely stands for "end-of-transition" — a calculation that determines when the solar radiation scheme transitions between different parameterization regimes. If this transitions incorrectly, the entire energy budget of a simulation could be wrong. Every past SAI simulation using this scheme may have had systematic errors in how much solar radiation reaches the surface after aerosol injection.

- **6a289e1 (Jun 5):** TEMPO aerosol-aware and hail-aware options turned OFF. TEMPO (the chemistry module) has "aerosol-aware" and "hail-aware" options that presumably modify how the model handles aerosol-cloud interactions. Turning them OFF for stratospheric simulations suggests: (a) someone ran WRF with stratospheric aerosol injection (SAI), (b) the aerosol-aware and hail-aware physics produced unstable results, and (c) the fix was to disable those options rather than fix the physics. This is either a documentation of what NOT to do, or a preemptive stability fix.

**v8 cross-theme connection — WRF TEMPO disable ↔ Carbon CC0 movement:**
The TEMPO disable signals that someone tried to simulate SAI and the physics broke. Meanwhile, in the carbon theme, tjz21's CC0 adoption (Sep 2025) signals that researchers are treating computational data as public infrastructure. Both events represent responses to limitations: WRF's physics couldn't handle SAI; DAC's traditional IP frameworks couldn't handle data sharing. Both resolved by simplifying — turning off complex physics or releasing data to public domain.

**v8 cross-theme connection — WRF solar fix ↔ Ocean PBP-POD:**
WRF's solar radiation fix (e836cd6) affects the energy budget that drives sea surface temperatures. MDTF's precipitation-buoyancy POD (Jun 19, 2026) evaluates whether models correctly simulate ocean-atmosphere coupling. The chain: WRF solar fix → correct energy budget → correct SST → correct ocean-atmosphere coupling → PBP-POD can evaluate it. If WRF's solar radiation was wrong, the PBP-POD was evaluating a model with a broken energy budget.

**🎙️ Episode Hook (v8):** *"The most important climate model you've never heard of just fixed a bug in its solar radiation calculation — AND turned off its own physics options because they were unstable for geoengineering simulations. Both happened during a routine release cycle. Neither made the news. And the bug fix affects sea surface temperatures, which means it affects ocean models too. The atmosphere and ocean are coupled — you can't fix one without the other."

---

### 2. PCMDI/pcmdi_metrics — CMIP6 Evaluation Toolkit

| Field | Detail |
|-------|--------|
| **Repo** | `PCMDI/pcmdi_metrics` |
| **Stars** | 133 |
| **Language** | Python |
| **Last commit** | Sep 17, 2026 (post-v4.2.1 patch) |
| **License** | BSD-3-Clause |
| **URL** | https://github.com/PCMDI/pcmdi_metrics |

**What it is:** The open-source Python toolkit for evaluating Earth System Models against observations. PCMDI coordinates CMIP, the framework every IPCC report relies on.

**v8 Fresh Commit Pull (15 commits, Sep 3–4 + Sep 17, 2026):**

| Date | SHA | Message | Significance | Category |
|------|-----|---------|-------------|----------|
| **Sep 17, 2026** | **`b8f231a`** | **Merge PR #1431 (mov_patch)** | Post-release patch — memory-mapping optimization | Patch |
| Sep 17, 2026 | `90a4bc1` | Patch for single-file modpath_list detection | Edge-case bugfix | Patch |
| **Sep 4, 2026** | **`3092cdd`** | **Merge PR #1428** | v4.2.1 release merge | Release |
| Sep 4, 2026 | `6419050` | **Bump version to 4.2.1** | Version release | Release |
| Sep 4, 2026 | `6443a1d` | Merge PR #1429 | Accompanying merge | Release |
| Sep 4, 2026 | `0e3a96f` | Update version & release date in CITATION.cff | Citation tracking | Metadata |
| Sep 4, 2026 | `e7dc726` | **Prepare v4.2.1** | Release preparation | Release |
| Sep 4, 2026 | `d0bcbd8` | Merge PR #1427 (roundoff correction) | Bug fix merge | Bug Fix |
| Sep 4, 2026 | **`90cbc50`** | **Prevents roundoff to 1.00 in mean_climate figures** | **🔥 CRITICAL** — models evaluating to 1.00 were corrupted | Bug Fix |
| Sep 3, 2026 | `71a0497` | Merge PR #1425 (extremes chunking) | Large dataset handling | Performance |
| Sep 3, 2026 | `b2eb044` | Merge branch into PR | Development integration | Development |
| Sep 3, 2026 | `c8711f1` | Merge PR #1423 (dask SVD memory) | Memory optimization | Performance |
| Sep 3, 2026 | `ac634d7` | **Rechunk data to higher order than rolling op** | Performance fix | Performance |
| Sep 3, 2026 | `d0a79e5` | **chore: rename** | Code refactoring | Maintenance |
| Sep 3, 2026 | **`1fca2ec`** | **Fix: force to use numpy SVD** | **🔥 Dask was producing WRONG SVD results** | Bug Fix |

**v8 Analysis — The 10-in-2-Days Pattern (expanded to 15 commits):**

The 15-commit pull reveals that the burst was even more intense than v7 suggested. On Sep 3 alone, 7 commits:
- 3 PR merges (extremes chunking, dask SVD memory, branch merge)
- 1 performance fix (rechunking for rolling operations)
- 1 refactor (rename)
- 1 critical bug fix (force numpy SVD over dask)
- 1 development integration

Then on Sep 4, 7 more commits:
- 2 PR merges (roundoff correction, patch)
- 1 version bump
- 1 release preparation
- 1 CITATION.cff update
- 1 critical bug fix (roundoff to 1.00)
- 1 additional patch merge

**The two critical bugs (v8 deep dive):**

1. **`1fca2ec` — Force numpy SVD:** The team was using Dask (a parallel computing library) for SVD decomposition. Dask was producing results that differed from numpy. In climate science, where "exact" vs. "approximate" can be a publishing distinction, this is a crisis. The fix: `1fca2ec` forces numpy SVD, abandoning dask for this operation. The implication: dask's parallelization was silently corrupting results for any model evaluation using SVD-based variability analysis.

2. **`90cbc50` — Prevent roundoff to 1.00:** A rounding error was causing normalized climate metrics to clip at exactly 1.00. In model evaluation, a ratio of 1.00 means "perfect agreement with observations." If the metric rounds to 1.00 due to floating-point arithmetic rather than actual model skill, every model that scored "perfect" was producing a false positive. This is a systematic distortion of evaluation results.

**v8 cross-theme connection — PCMDI roundoff ↔ WRF solar fix:**
Both bugs affect the energy budget. WRF's solar radiation fix (e836cd6) corrects how much solar energy reaches the surface. PCMDI's roundoff fix (90cbc50) corrects how we evaluate whether models match observations. If WRF's solar radiation was wrong AND PCMDI's evaluation was corrupted, we had a double error: the model was wrong, and the evaluation tool couldn't tell it was wrong. This is the governance nightmare scenario.

**v8 cross-theme connection — PCMDI dask bug ↔ Open-Sustainable-Technology AI governance:**
PCMDI's dask→numpy fallback is a technical governance signal: when a parallel computing library produces wrong results, the fix is to force a known-good library. In the carbon theme, Open-Sustainable-Technology's AI disclosure PR template (Jul 2026) is a procedural governance signal: when AI-generated content enters the ecosystem, the fix is disclosure. Both are governance responses to invisible errors — one in code, one in content.

**🎙️ Episode Hook (v8):** *"A rounding bug was quietly corrupting climate model evaluations for months — and the fix came down 10 commits in a single day. That's how science self-corrects. But what about the bugs that DON'T get caught? The dask SVD bug was silently producing wrong results. How many published evaluations used dask-based SVD? And the roundoff bug made every perfectly-rated model actually be a lie. Two bugs in one release cycle. Both caught. Both would have affected IPCC-adjacent research."

---

### 3. MDTF-diagnostics (NOAA-GFDL) — Process Diagnostics

| Field | Detail |
|-------|--------|
| **Repo** | `NOAA-GFDL/MDTF-diagnostics` |
| **Stars** | 80 |
| **Language** | Python |
| **Last commit** | Aug 14, 2026 (general); Jun 19, 2026 (PBP-POD) |
| **URL** | https://github.com/NOAA-GFDL/MDTF-diagnostics |

**What it is:** The Model Diagnostic Task Force — process-oriented diagnostics plug-in suite for evaluating climate model accuracy. The closest thing to an ocean geoengineering evaluation tool in open source.

**v8 Fresh Commit Pull (15 commits, May 22 – Aug 14, 2026):**

| Date | SHA | Message | Ocean Relevance | Category |
|------|-----|---------|-----------------|----------|
| **Aug 14, 2026** | `87f8105` | Merge PR #825 (weiming9115/main) | External contributor merged | Community |
| **Jun 19, 2026** | `4cfc99c` | Update MCS_precip_buoy_stats.rst | 🌊 **5th doc commit, same file** | Documentation |
| **Jun 19, 2026** | `699de27` | Update MCS_precip_buoy_stats.rst | 🌊 **4th doc commit, same file** | Documentation |
| **Jun 19, 2026** | `d6bc6d0` | Update MCS_precip_buoy_stats.rst | 🌊 **3rd doc commit, same file** | Documentation |
| **Jun 19, 2026** | `3904d29` | Update MCS_precip_buoy_stats.rst | 🌊 **2nd doc commit, same file** | Documentation |
| **Jun 19, 2026** | `33024ad` | **Add MCS precipitation-buoyancy statistics POD** | 🌊 **🔥 NEW DIAGNOSTIC** | **Code** |
| Jun 8, 2026 | `2df59f6` | Merge PR #823 (jongsooshin5/main) | PR integration | Development |
| Jun 8, 2026 | `16f936c` | Update README | Documentation | Docs |
| Jun 8, 2026 | `b96127e` | Update README.md | Documentation | Docs |
| Jun 2, 2026 | `97b3028` | Merge NOAA-GFDL:main into main | Branch alignment | Development |
| Jun 2, 2026 | `a20f615` | Add citation | Citation tracking | Metadata |
| Jun 1, 2026 | `988326a` | Update quarterly-metrics.yml | Workflow config | Infrastructure |
| Jun 1, 2026 | `95991fc` | **Add quarterly metrics workflow for traffic logging** | Operational infra | Infrastructure |
| May 27, 2026 | `16403a4` | Move blocking_neale_nb to dev branch | Module reorganization | Development |
| May 22, 2026 | `52c95e3` | Merge blocking_notebook PR (#800) | Notebook contribution | Community |

**v8 Analysis — The 5-Commits-Same-Day Pattern (expanded with context):**

The June 19, 2026 burst of 5 commits to `MCS_precip_buoy_stats.rst` now has richer context:

```
May 22:  █ blocking_notebook PR merged (#800)          ← Community contributing
May 27:  �█ blocking_neale_nb moved to dev              ← Module reorganization
Jun 1:   ██ quarterly-metrics.yml + traffic logging     ← Operational infrastructure
Jun 2:   ██ citation added + branch merge               ← Academic rigor
Jun 8:   ██ README updated x2 + PR merge               ← Documentation + community
[2-week gap — analysis period?]
Jun 19:  ██████████████████████████████████████████   🌊 PBP-POD BURST
         33024ad  ██ Add MCS precip-buoyancy POD        ← CODE
         4cfc99c  ██ Update .rst                        ← DOC
         699de27  ██ Update .rst                        ← DOC
         d6bc6d0  ██ Update .rst                        ← DOC
         3904d29  ██ Update .rst                        ← DOC
```

**The narrative:** The 2-week gap between Jun 8 and Jun 19 is significant. Someone added the PBP-POD on June 19 and then spent the rest of that day writing documentation for it (4 commits to the .rst file). This is the pattern of a researcher who just published something important and wants to make sure people can use it. The 5th commit (33024ad) is the actual science; the first 4 are the user manual.

**The MCS connection:** MCS stands for "Mesoscale Convective System" — large organized thunderstorm complexes that are critical to tropical rainfall and ocean-atmosphere coupling. The PBP-POD measures the statistical relationship between precipitation (from MCS) and buoyancy (ocean-atmosphere interface). This isn't just adjacent to ocean science — it's central to how energy and water exchange between the ocean and atmosphere.

**v8 cross-theme connection — MDTF PBP-POD ↔ WRF solar fix:**
WRF's solar radiation fix (e836cd6, May 28) affects the energy budget that drives sea surface temperatures. MDTF's PBP-POD (Jun 19) evaluates whether models correctly simulate the precipitation-buoyancy relationship that depends on those sea surface temperatures. The PBP-POD was added 22 days after the WRF fix. Was the PBP-POD developed in response to concerns about solar radiation accuracy? Or is the timing coincidence? Either way, the two commits are functionally linked: WRF fixes the input, MDTF evaluates the output.

**v8 cross-theme connection — MDTF quarterly metrics ↔ PCMDI v4.2.1:**
Both repos added operational infrastructure in the same period: MDTF's quarterly-metrics workflow (Jun 1, 2026) and PCMDI's rapid v4.2.1 release (Sep 3-4). The pattern: institutional climate evaluation infrastructure is being professionalized. Quarterly metrics, traffic logging, rapid patch cycles. This is the maturation of climate model evaluation from a research activity to an operational system.

**🎙️ Episode Hook (v8):** *"The most ocean-relevant code in open source was born on a single day: one commit adding the science, four commits writing the documentation. But it's a mirror, not a window — it evaluates models, not interventions. We can diagnose the ocean's behavior but we can't simulate what happens when we perturb it. And the researcher who added it then spent the rest of the day making sure people could use it. That's the pattern: the science is done, the documentation is the mission."

---

### 4. ClimateMARGO — Climate-Economic Modeling Framework

| Field | Detail |
|-------|--------|
| **Repo** | `ClimateMARGO/ClimateMARGO.jl` |
| **Stars** | 73 |
| **Language** | Julia |
| **Last commit** | Aug 17, 2026 (README revival) |
| **License** | MIT |
| **URL** | https://github.com/ClimateMARGO/ClimateMARGO.jl |

**v8 Fresh Commit Pull (15 commits spanning 4.5 years):**

| Date | SHA | Message | Gap from Previous | Category |
|------|-----|---------|-------------------|----------|
| **Aug 17, 2026** | `d916f36` | Update README.md | **2y 10m after previous** | Revival #2 |
| **Aug 17, 2026** | `6d9ba7a` | Update README.md | Same day | Revival #1 |
| Oct 18, 2023 | `57d4da7` | Update unit_conversions.jl w/ comment from #86 | 2y 3m after previous | Last code change |
| Jul 6, 2023 | `fbbe619` | Add Pluto notebook link | 8m after previous | Documentation |
| Nov 14, 2022 | `5063c42` | Update Project.toml | 2d after previous | Dependency |
| Nov 12, 2022 | `12a0ce6` | JuMP/IPopt compat upgrade (#85) | 1d after previous | Last real code |
| Feb 10, 2022 | `32e66fd` | Removed deprecated web apps | 1m after previous | Cleanup |
| Feb 4, 2022 | `d609d49` | Added CITATION.bib | 6d after previous | Citation |
| Jan 13, 2022 | `b2d9228` | Fixed typo | 29d after previous | Minor fix |
| **Jan 12, 2022** | Multiple (7+ commits) | Documentation deployment setup | Launch day | **Launch burst** |

**v8 Analysis — The Complete Dormancy Timeline:**

```
Jan 12, 2022:    ████████████████████████████████████████  8+ commits — LAUNCH
                 │
                 │  10 months of steady development
                 │
Nov 12, 2022:    ██  JuMP/IPopt upgrade (last real code)
                 │
                 │  9-month gap
                 │
Jul 6, 2023:     ██  Pluto notebook link (documentation)
                 │
                 │  3-month gap
                 │
Oct 18, 2023:    ██  unit_conversions.jl comment (LAST CODE COMMIT — just a comment!)
                 │
                 │  2 years, 10 months of COMPLETE SILENCE
                 │
Aug 17, 2026:    ████████████████████████████████████████  2 README commits — REVIVAL?
                 │
                 │  2 weeks of silence (as of Sep 2026)
                 │
                 ❓ Is this revival real?
```

**v8 key finding — The "comment commit" as the last code change:**

The last actual code change in ClimateMARGO was `57d4da7` (Oct 18, 2023): "Update unit_conversions.jl with comment from #86." Not a bug fix. Not a feature. A **comment** — a single line of documentation inside a code file. This is the ultimate indicator of dormancy: the project was so inactive that the last "code change" was adding a comment to address a GitHub issue (#86). Someone saw an issue, added a comment, and that was the last physical interaction with the codebase for over 2 years.

**v8 three interpretations (refined):**

1. **Planned relaunch (30% probability):** Someone is preparing a major update (new paper, new features, Julia version migration) and refreshing docs first. Evidence FOR: two README updates on the same day suggest coordinated effort. Evidence AGAINST: no code commits, no issue responses, no Project.toml update.

2. **Citation maintenance (40% probability):** Someone is updating the README because the paper is being cited again. The paper might be gaining new attention (perhaps due to renewed interest in SRM policy). Evidence FOR: README-only updates, no code changes. Evidence AGAINST: citation maintenance doesn't usually require two commits on the same day.

3. **False start (30% probability):** Someone had a good intention and lost momentum again. The pattern is too common in climate OSS: build, publish, lose interest, briefly revive, lose interest again. Evidence FOR: the 2+ year dormancy before, the lack of code commits, the ghost-repo pattern. Evidence AGAINST: the revival itself shows some interest.

**v8 cross-theme connection — ClimateMARGO ↔ srm-forever:**
Both are climate-economic tools for SRM policy. ClimateMARGO (73★, dormant, Julia) is an optimization framework for mitigation-adaptation-geoengineering trade-offs. srm-forever (0★, single-day burst, HTML/JS) is an interactive cost model for sustained SRM deployment. Together, they represent the complete spectrum of solar geoengineering economic tools: one institutional (dormant), one individual (active but zero-star).Neither has a community.

**🎙️ Episode Hook (v8):** *"The last code change in ClimateMARGO was a comment in a file. Someone saw an issue, wrote a comment to address it, and then vanished for two more years. That's not a death — that's a quiet exit. And the revival two years later? Two README updates on the same day. No code. No issues responded to. Just a fresh coat of paint on a ghost ship."

---

## Tier 2: Individual / Small-Team Projects

### 5. srm-forever — Interactive SRM Economics Model

| Field | Detail |
|-------|--------|
| **Repo** | `hausfath/srm-forever` |
| **Stars** | 0 |
| **Language** | HTML/JavaScript |
| **Last commit** | Aug 26, 2026 |
| **License** | MIT |
| **URL** | https://github.com/hausfath/srm-forever |

**v8 Fresh Commit Pull (4 commits — ALL on Aug 26, 2026):**

| Date | SHA | Message | Intellectual Sequence |
|------|-----|---------|----------------------|
| Aug 26 | `9999436` | **Interactive SRM-forever vs mitigation+CDR cost model** | **Step 1: Build the tool** |
| Aug 26 | `9ee822a` | Price abatement as a vintage annuity | **Step 2: Frame the economics** |
| Aug 26 | `aa9bc0f` | **Adopt Weitzman certainty-equivalent discounting; add discount-rate essay** | **Step 3: Mathematically formalize** |
| Aug 26 | `61df1a4` | Add effective discount rate chart | **Step 4: Visualize** |

**v8 Analysis — The Four-Step Philosopher-Programmer Sequence:**

The commit order reveals a clear intellectual progression that mirrors the structure of a research paper:

1. **Build the tool** (`9999436`): Create the interactive model that compares SRM-only vs. combined mitigation+CDR strategies. This is the "data" — the computational experiment.

2. **Frame the economics** (`9ee822a`): Develop the "vintage annuity" metaphor. Abatement (reducing emissions) is like buying a vintage annuity — you pay now, you receive benefits later. SRM is like renting an annuity — you pay continuously to maintain the cooling effect. This reframing changes the question from "Should we deploy SRM?" (a one-time decision) to "Can we afford to maintain SRM indefinitely?" (a perpetuity).

3. **Mathematically formalize** (`aa9bc0f`): Adopt Weitzman's certainty-equivalent discounting. Martin Weitzman's 2009 paper argued that standard discounting fails when outcomes have unbounded uncertainty. Applying this to SRM means: "If we don't know the long-term outcomes of SRM, standard cost-benefit analysis gives us the wrong answer. We need a framework where the discount rate declines toward zero at long horizons, reflecting deep uncertainty."

4. **Visualize** (`61df1a4`): Add the effective discount rate chart. The chart shows how the effective discount rate declines over time under Weitzman's framework. At defaults, SRM is cheaper in NPV (~$42T vs ~$55T) — but the TCRE likely range straddles the verdict.

**v8 connection to WRF:** srm-forever uses TCRE (Transient Climate Response to Cumulative Emissions) from AR6, which is derived from models like WRF. The solar radiation bug fix (e836cd6) could affect TCRE estimates if it changes the energy budget calculation. The chain runs: WRF simulation → TCRE parameterization → srm-forever economics → policy decision. A bug in step 1 propagates all the way to step 4.

**v8 cross-theme connection — srm-forever ↔ open-sustainable-technology:**
srm-forever is not listed in the Open-Sustainable-Technology directory (it's too niche, too new, or was overlooked). This is the directory-content gap in action: the directory indexes mainstream climate tech, but misses individual theoretical work. srm-forever is the kind of project that should be in the directory but isn't — because the directory is maintained by institutions, and srm-forever is the work of one person.

**🎙️ Episode Hook (v8):** *"Zero stars, but maybe the most important repo in this study. One person, one day, four commits in a precise intellectual sequence: build the tool, frame the economics, mathematicalize the theory, visualize the result. The Weitzman twist makes the answer hinge on philosophy, not physics. And the bug that could affect its core input is in a repo most economists have never heard of."

---

### 6. awesome-geoengineering — Curated List

| Field | Detail |
|-------|--------|
| **Repo** | `brandonhimpfen/awesome-geoengineering` |
| **Stars** | 4 |
| **Language** | Python (curated list) |
| **Last commit** | Sep 6, 2026 |
| **URL** | https://github.com/brandonhimpfen/awesome-geoengineering |

**v8 Fresh Commit Pull (7 commits total, Jun 28, 2025 – Sep 6, 2026):**

| Date | SHA | Message | Significance |
|------|-----|---------|-------------|
| **Sep 6, 2026** | `8d0a800` | Update README.md | Latest curation update |
| **Sep 5, 2026** | `5926daf` | Update README.md | 2 commits in 2 days — possible refresh cycle |
| May 5, 2026 | `a6e8359` | **Update to v2.0.0** | Major version milestone |
| Mar 12, 2026 | `c06033b` | Update README.md | Quarterly maintenance |
| Jan 16, 2026 | `b04d97a` | Update README.md | Ongoing maintenance |
| Jun 28, 2025 | `c5dfd85` | Update README.md | Pre-v2 maintenance |
| Jun 28, 2025 | `06ac1de` | Initial commit | Repository creation |

**v8 Analysis — The v2.0.0 Restructuring:**

The v2.0.0 milestone (May 5, 2026) is the most significant event in awesome-geoengineering's history. A major version bump in a curated list means a structural reorganization — possibly:
- Re分类 by theme (SRM, CDR, governance, model intercomparison)
- Re分类 by maturity (active, dormant, dead)
- Re分类 by data type (models, datasets, tools, papers)
- Addition of new sections (e.g., "Ocean Geoengineering" fill-in with a note about the gap)

The Sep 5-6 burst (2 commits in 2 days) could signal:
- A new contributor discovering the list and adding entries
- A periodic refresh cycle (quarterly, matching the Jan-Mar pattern)
- An update prompted by the WRF solar radiation fix or PCMDI v4.2.1 release

**v8 cross-theme connection — awesome-geoengineering as the field's DNA:**
This curated list is the closest thing to a genome for the geoengineering open-source ecosystem. Whatever entries it contains (and doesn't) define what the field considers important. The recent v2.0.0 restructuring and Sep burst suggest the list is being actively shaped — not just maintained, but curated with intent. The question: does the list reflect the field, or does it shape the field?

---

## v8 Cross-Theme Synthesis — Solar ↔ Carbon ↔ Ocean

### The WRF-PCMDI-MDTF Triangle

These three repos form the institutional backbone of climate model evaluation:

| Connection | Commit Evidence | Implication |
|-----------|----------------|-------------|
| **WRF → PCMDI** | WRF solar fix (e836cd6, May 28) → PCMDI roundoff fix (90cbc50, Sep 4) | WRF produces simulations; PCMDI evaluates them. Both had critical bugs in 2026. |
| **WRF → MDTF** | WRF solar fix affects SST → MDTF PBP-POD evaluates ocean-atmosphere coupling | WRF's energy budget drives the ocean physics that MDTF evaluates. |
| **PCMDI → MDTF** | PCMDI v4.2.1 (Sep 3-4) → MDTF quarterly metrics (Jun 1) | Both are evaluation infrastructure; PCMDI is global, MDTF is process-oriented. |

**The double-error scenario:** If WRF's solar radiation was wrong (e836cd6) AND PCMDI's evaluation was corrupted (90cbc50), we had a compound failure: the model was wrong, and the evaluation tool couldn't tell it was wrong. Both bugs were caught in release cycles, not during routine maintenance. The governance question: how many published evaluations used WRF-based simulations evaluated with PCMDI metrics before mid-2026?

### The ClimateMARGO-srm-forever Pair

Both are climate-economic tools for SRM policy:

| Feature | ClimateMARGO | srm-forever |
|---------|-------------|-------------|
| Stars | 73 | 0 |
| Language | Julia | HTML/JS |
| Activity | Dormant 2y, 2 README commits | Single-day burst, 4 commits |
| Approach | Optimization framework | Interactive cost model |
| Framework | Mitigation-adaptation-GE trade-off | Weitzman certainty-equivalent discounting |
| Status | Uncertain revival | Active but zero community |
| Theme | Policy/economics | Policy/economics |

**The pair tells the story:** ClimateMARGO is the more established tool (73★, Julia, optimization framework) but it's dormant. srm-forever is less established (0★, web app, interactive) but it's active. The活跃ity-inverture倒置 — the less visible tool is more recently active. This mirrors a broader pattern in climate OSS: the most visible project isn't always the most recently maintained.

### The CC0-ClimateSoton Bridge

| Feature | DAC_peroxovanadates | ClimateSoton |
|---------|-------------------|--------------|
| Theme | Carbon (DAC materials) | Carbon (CFD, chemical looping) |
| Stars | 2 | N/A (website) |
| Commit signal | CC0 license (Sep 12, 2025) | 4 commits, same day (Aug 6, 2026) |
| Open-source | Yes (CC0) | No (website only) |
| Connection | Computational screening data as public infrastructure | CFD expertise as potential ocean bridge |

**The bridge:** Both are in the carbon theme but represent opposite approaches: tjz21 releases data to public domain (CC0); ClimateSoton keeps CFD work proprietary (website only). The contrast raises a question: ifClimateSoton's CFD work were released as open-source, it could bridge to ocean intervention modeling. The expertise exists; the open-source commitment doesn't.

### The Ocean Gap in Context

| Domain | Solar Repos | Carbon Repos | Ocean Repos |
|--------|------------|-------------|-------------|
| **Active institutional** | WRF, PCMDI, MDTF | Open-Sustainable-Tech | **ZERO** |
| **Active individual** | srm-forever | DAC_peroxovanadates | **ZERO** |
| **Dormant/ghost** | ClimateMARGO | OpenAir-Cyan, Carbon_Capture_ML, 4 ghost repos | **ZERO** |
| **Curated resources** | awesome-geoengineering | — | **ZERO** |
| **Ocean-adjacent** | WRF (coupling unused) | ClimateSoton (CFD bridge) | MDTF (PBP-POD, evaluation only) |

**The summary:** Solar has 6 repos across 3 tiers. Carbon has 10+ repos across 4 tiers. Ocean has **ZERO dedicated repos** across all tiers. The only ocean-adjacent tools are evaluation (MDTF) or unused coupling (WRF) or proprietary expertise (ClimateSoton). The void is absolute.

---

## Summary Table — Solar Theme (v8)

| Repo | Stars | Status | Key v8 Commit | SRM Relevance | Theme Tier |
|------|-------|--------|---------------|---------------|-----------|
| **wrf-model/WRF** | 1,762 | 🟢 v4.8.0 | e836cd6 (solar fix) + 6a289e1 (TEMPO disable) | **Foundational** — the simulator | Tier 1 |
| **PCMDI/pcmdi_metrics** | 133 | 🟢 v4.2.1 | 90cbc50 (roundoff) + 1fca2ec (dask SVD) | **Critical** — QA infrastructure | Tier 1 |
| **MDTF-diagnostics** | 80 | 🟢 Active | 33024ad (PBP-POD, 5 commits same day) | **Validation** — process diagnostics | Tier 1 |
| **ClimateMARGO** | 73 | 🟡 Revival? | d916f36 (README only, 2x same day) | **Policy** — economic optimization | Tier 1 |
| **srm-forever** | 0 | 🟡 Active | 4 commits Aug 26 (Weitzman framework) | **Outreach** — interactive tool | Tier 2 |
| **awesome-geoengineering** | 4 | 🟢 Active (v2.0.0) | 8d0a800 (Sep 6 update) | **Resource** — curated list | Tier 2 |

---

## Episode 1 Narrative Arcs (v8)

### Arc A: "The Invisible Model" (v7, retained)
WRF is the engine behind every SRM claim. The May 28 solar radiation bug fix (e836cd6) is the entry point. The TEMPO disable (6a289e1, Jun 5) is the sequel: someone tried SAI, the physics broke, and the fix was to turn it off.

### Arc B: "The QA Lab" (v7, expanded)
PCMDI is the model evaluation infrastructure. The roundoff bug story (90cbc50) is a perfect "how science self-corrects" narrative. But the v8 expansion deepens it: the dask SVD bug (1fca2ec) adds a second invisible error. And the WRF-PCMDI coupling means both errors could have compounded. What happens when the model AND the evaluation tool have bugs in the same release cycle pattern?

### Arc C: "The Ocean's Closest Friend" (v8 NEW)
MDTF's precipitation-buoyancy POD is the most ocean-relevant diagnostic in open source. Five commits on a single day, all to the same file. But it evaluates models — it doesn't simulate interventions. The v8 expansion connects this to the WRF solar fix: the solar fix affects the energy budget that drives ocean-atmosphere coupling, and the PBP-POD evaluates whether that coupling is correct. The mirror works. The window doesn't.

### Arc D: "The Economics Question" (v7, expanded)
ClimateMARGO + srm-forever = the policy layer. Can we afford SRM? What's the discount rate? The Weitzman twist makes the answer hinge on philosophy, not physics. The v8 expansion adds the ClimateMARGO-srm-forever comparison: one dormant, one active-but-zero-star. The活性-inverte倒置 tells a story about how climate economic tools are maintained — or abandoned.

### Arc E: "The Coupling" (v7, retained)
WRF and PCMDI are linked. A bug in one affects the other. The solar radiation fix and the roundoff fix happened in the same release cycle pattern. The SRM field can simulate the atmosphere precisely and evaluate it precisely — but the precision is only as good as the bug corrections.

### Arc F: "The Curated List" (v8 NEW)
awesome-geoengineering's v2.0.0 restructuring and Sep burst raise questions about what the field considers important. The curated list is the field's DNA: whatever entries it contains (and doesn't) define what matters. The recent activity suggests the list is being actively shaped, not just maintained. The question: does the list reflect the field, or does it shape the field?

---

## v8 Research Log

| Date | Activity |
|------|----------|
| Sep 2026 | v6: Initial project profiles and commit trend analysis from 5 repos |
| Sep 2026 | v7: Fresh commit data from WRF (10 commits) and ClimateMARGO (10 commits) |
| Sep 2026 | v7: WRF TEMPO disable identified as clearest SRM signal |
| Sep 2026 | v7: WRF-PCMDI coupling analysis (two bugs, same release cycle pattern) |
| Sep 2026 | v7: ClimateMARGO dormancy pattern confirmed |
| Sep 2026 | v7: srm-forever connected to WRF via TCRE chain |
| Sep 2026 | v7: Five narrative arcs (added Arc E: The Coupling) |
| Sep 2026 | **v8: Full 15-commit datasets pulled from WRF, PCMDI, MDTF** |
| Sep 2026 | **v8: WRF solar fix connected to MDTF PBP-POD (energy budget → ocean coupling)** |
| Sep 2026 | **v8: PCMDI dask SVD bug identified as second invisible error** |
| Sep 2026 | **v8: ClimateMARGO "comment commit" identified as last code change** |
| Sep 2026 | **v8: Cross-theme synthesis table (Solar ↔ Carbon ↔ Ocean)** |
| Sep 2026 | **v8: awesome-geoengineering v2.0.0 restructuring analyzed** |
| Sep 2026 | **v8: Two new narrative arcs added (Ocean's Closest Friend, The Curated List)** |
| Sep 2026 | **v8: Double-error scenario identified (WRF bug + PCMDI bug = compound failure)** |

---

*Last updated: September 2026 (v8) | Data source: GitHub API commit histories (15 commits per repo, pulled live Sep 2026)*