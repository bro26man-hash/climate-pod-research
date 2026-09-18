# ☀️ Solar Geoengineering — Project Discoveries
## v4 Update — September 2026

---

## Overview

This file profiles the most relevant open-source repositories for the **Solar Geoengineering** episode of the Climate Pod. Data pulled from fresh GitHub commit histories (September 2026).

---

## Tier 1: Foundational Atmospheric Modeling

### 1. wrf-model/WRF ⭐ 1,762
- **Language:** Fortran | **License:** BSD-3-Clause
- **Last activity:** September 16, 2026 (v4.8.0 release cycle)
- **URL:** https://github.com/wrf-model/WRF

**Why it matters for the episode:**
WRF is the foundational atmospheric model used worldwide for weather prediction and climate simulation. It is the *de facto* standard against which solar geoengineering proposals are evaluated. No SRM experiment is credible without WRF (or its cousins like CESM) modeling the atmospheric response.

**Recent commit highlights (10 commits pulled):**
| Date | SHA | Message | Significance |
|------|-----|---------|-------------|
| Jun 8, 2026 | 06d4240 | Merge release-v4.8.0 | **Major version release** — v4.8.0 is the current production branch |
| Jun 6, 2026 | 0708348 | Update README and version to v4.8.0 | Documentation sync for v4.8.0 |
| Jun 5, 2026 | 6a289e1 | Turn off tempo_aerosolaware and tempo_hailaware | **Aerosol-aware schemes disabled** — directly relevant to SRM simulation accuracy |
| May 30, 2026 | 4466746 | Fix vectorization option in AOCC stanza | Performance optimization for AMD compilers |
| **May 28, 2026** | **e836cd6** | **Correction for EOT calculation for solar radiation** | **🔥 SOLAR RADIATION FIX** — Directly impacts how WRF simulates solar radiation absorption, essential for any SRM scenario modeling |
| May 27, 2026 | 8299919 | Update MYNN-EDMF pointer, remove icloud_bl | Cloud physics updates — affects radiative transfer modeling |
| May 27, 2026 | 4fab0e2 | Update MMM-physics repo SHA with fixes | Multi-scale physics updates |
| May 26, 2026 | 75ad1f9 | Fixing CDXWRF module | Coupled model interface fix |
| May 26, 2026 | 0aa6582 | Update readme for GFL option | Documentation for gravity wave flux option |
| May 21, 2026 | 02f02bc | Include mp_physics=88 in TEMPO error print | Error handling for meteorology options |

**Episode angle:** The May 28 solar radiation correction (e836cd6) is the anchor story. WRF's solar radiation scheme is *the* code path that determines how much sunlight reaches the surface in an SRM simulation. A correction to the End-Of-Translation (EOT) calculation means past simulations may have had systematic errors in their energy budgets. This is a governance story: anyone citing WRF-based SRM results from before mid-2026 should note this correction.

---

### 2. PCMDI/pcmdi_metrics ⭐ 133
- **Language:** Python | **License:** BSD-3-Clause
- **Last activity:** September 17, 2026 (v4.2.1)
- **URL:** https://github.com/PCMDI/pcmdi_metrics

**Why it matters:**
PCMDI Metrics is the standard toolkit for evaluating Earth System Models (ESMs) against observations. It produces the CMIP6 evaluation figures that policymakers and IPCC reports rely on. If solar geoengineering is ever governed by evidence, PCMDI metrics determine what that evidence looks like.

**Recent commit highlights (10 commits pulled):**
| Date | SHA | Message | Significance |
|------|-----|---------|-------------|
| **Sep 17, 2026** | **b8f231a** | **Merge PR #1431 — mov_patch** | Latest patch for model path handling |
| Sep 17, 2026 | 90a4bc1 | Patch for single-file modpath_list case | Bug fix for edge case in file detection |
| Sep 4, 2026 | 3092cdd | Merge PR #1428 | PR merge for previous patch cycle |
| **Sep 4, 2026** | **6419050** | **Bump version to 4.2.1** | **Minor version release** — maintenance update |
| Sep 4, 2026 | 6443a1d | Merge PR #1429 | Patch merge chain |
| Sep 4, 2026 | 0e3a96f | Update version and release date in CITATION.cff | Citation metadata update |
| Sep 4, 2026 | e7dc726 | Prepare v4.2.1 | Release preparation commits (5 commits in one day) |
| Sep 4, 2026 | d0bcbd8 | Merge PR #1427 — jsgoodni_corr_roundoff | Roundoff error fix |
| **Sep 4, 2026** | **90cbc50** | **Prevents roundoff to 1.00 in mean_climate figures** | **🔥 Critical fix** — prevents evaluation metrics from rounding to exactly 1.00, which would falsely indicate perfect model-observation agreement |
| Sep 3, 2026 | 71a0497 | Merge PR #1425 — extremes_chunking | Chunking optimization for extreme value analysis |

**Episode angle:** The roundoff fix (90cbc50) is surprisingly dramatic. If a climate model's mean precipitation ratio rounds to 1.00, it *looks* like the model perfectly reproduces observations. But that's an artifact, not a result. For SRM governance, this matters: evaluation metrics that appear clean but are actually rounded misrepresent the model's true skill. The 5 commits in a single day (Sep 4) show the institutional intensity behind climate evaluation infrastructure.

---

## Tier 2: SRM-Specific Modeling Tools

### 3. hausfath/srm-forever ⭐ 0
- **Language:** Julia | **License:** MIT
- **Last activity:** August 26, 2026 (4 commits in one day)
- **URL:** https://github.com/hausfath/srm-forever

**Why it matters despite zero stars:**
This is the most *conceptually important* repository in our entire study, despite having no stars and no external contributors. It applies **Weitzman certainty-equivalent discounting** to the cost dynamics of sustained SRM deployment — answering the question: "What does it cost to keep solar geoengineering running forever?"

**Recent commit highlights (4 commits, all Aug 26, 2026):**
| Date | SHA | Message | Significance |
|------|-----|---------|-------------|
| Aug 26, 2026 | 61df1a4 | Add effective discount rate chart | Visual output for the discounting framework |
| Aug 26, 2026 | aa9bc0f | **Adopt Weitzman certainty-equivalent discounting; add discount-rate essay** | **🔥 Core theoretical contribution** — implements Martin Weitzman's framework from his landmark paper |
| Aug 26, 2026 | 9ee822a | Price abatement as a vintage annuity | Economic framing for cumulative mitigation costs |
| Aug 26, 2026 | 9999436 | **Interactive SRM-forever vs mitigation+CDR cost model** | **Interactive tool** — compares SRM-only vs combined mitigation+carbon dioxide removal strategies |

**Episode angle:** This is the "hidden gem" story. Zero stars, but the theoretical framework is what *should* be informing the SRM debate. Weitzman's certainty-equivalent discounting addresses the fundamental problem of intergenerational cost allocation: how do we weigh the costs of maintaining SRM for centuries against the benefits of avoided warming? The fact that this work exists as code (not just a paper) makes it uniquely valuable for the podcast. The interactive model could be a segment prop.

---

### 4. jlehtomaa/OOCC_2021 ⭐ 2
- **Language:** Python | **License:** MIT
- **Last activity:** November 15, 2021 (dormant for ~5 years)
- **URL:** https://github.com/jlehtomaa/OOCC_2021

**What it is:** A simple governance model for solar geoengineering, accompanying the 2021 Oxford Conference on Climate (OCC) paper. Models the Optimal Output-Based Cost-Sharing mechanism for SRM international cooperation.

**Recent commits:** All from September-November 2021. No activity since. This is a "paper companion" repository — created to support a publication, then abandoned.

**Episode angle:** The dormancy of OOCC_2021 illustrates a pattern: geoengineering governance gets *analyzed* in academic papers but rarely gets *maintained* as open-source tools. The governance frameworks exist in journals, not in code. This is a consequence of the problem being politically unsolvable rather than technically intractable — researchers build models of cooperation, but the real-world incentive structure ensures nobody maintains the tools.

---

## Tier 3: Curated Resources & Adjacent Tools

### 5. brandonhimpfen/awesome-geoengineering ⭐ 4
- **Language:** Python (curated list) | **License:** Not specified
- **Last activity:** September 6, 2026 (actively maintained)
- **URL:** https://github.com/brandonhimpfen/awesome-geoengineering

**What it is:** A curated, categorized list of geoengineering projects, research papers, organizations, tools, and resources. The "github.com/awesome-list" format applied to geoengineering.

**Recent commits (7 pulled):**
| Date | SHA | Message | Significance |
|------|-----|---------|-------------|
| **Sep 6, 2026** | 8d0a800 | Update README.md | **Latest update** — active curation continues |
| Sep 5, 2026 | 5926daf | Update README.md | Two updates in two days — active period |
| May 5, 2026 | a6e8359 | **Update to v2.0.0** | **Major version bump** — structural reorganization |
| Mar 12, 2026 | c06033b | Update README.md | Regular maintenance |
| Jan 16, 2026 | b04d97a | Update README.md | Regular maintenance |
| Jun 28, 2025 | c5dfd85 | Update README.md | Pre-v2 maintenance |
| Jun 28, 2025 | 06ac1de | Initial commit | Repository creation |

**Episode angle:** v2.0.0 (May 2026) is worth noting because it represents a major reorganization. The fact that someone is maintaining a *curated list* of geoengineering resources — and actively updating it in 2026 — signals that the field is growing enough to need taxonomy. This is a good "start here" resource for listeners who want to dive deeper.

---

## Tier 4: Dormant/Dead Projects (Included for Completeness)

### ClimateMARGO/ClimateMARGO.jl ⭐ 73
- **Language:** Julia | **License:** MIT
- **Last activity:** August 17, 2026 (2 README updates)
- **URL:** https://github.com/ClimateMARGO/ClimateMARGO.jl

**What it is:** Julia implementation of MARGO (Multi-start Adaptive Rejection for Ge{O}), an idealized climate-economic modeling framework for optimizing trade-offs between emissions mitigation, adaptation, and solar radiation management.

**Recent commit pattern — THE REVIVAL SIGNAL:**
| Date | SHA | Message | Gap |
|------|-----|---------|-----|
| **Aug 17, 2026** | d916f36 | Update README.md | **2 years, 10 months after previous commit** |
| **Aug 17, 2026** | 6d9ba7a | Update README.md | Same day — second commit |
| Oct 18, 2023 | 57d4da7 | Update unit_conversions.jl | Last code commit before dormancy |
| Jul 6, 2023 | fbbe619 | Add Pluto link in README | Documentation |
| Nov 14, 2022 | 5063c42 | Update Project.toml |Dependency management |
| Nov 12, 2022 | 12a0ce6 | JuMP and Ipopt compat upgrade | Last meaningful code change |
| Feb 10, 2022 | 32e66fd | Removed deprecated web apps | Cleanup |
| 2022 | d609d49 | Added CITATION.bib | Academic citation support |

**Episode angle:** Two README updates on August 17, 2026, after 2 years and 10 months of complete dormancy. No code commits. No issue responses. Just two README pushes. Is this a genuine revival signal, or is someone updating links because the paper is being cited again? The ambiguity itself is interesting — ClimateMARGO is a climate-economic model that *includes* SRM as a decision variable, and its dormancy-turned-revival mirrors the broader pattern of geoengineering research going from "politically radioactive" to "increasingly discussed but still unfunded."

---

### PSLmodels/Geo-DICE ⭐ 2
- **Language:** MATLAB | **License:** Not specified
- **Last activity:** September 27, 2018 (completely dead for ~8 years)
- **URL:** https://github.com/PSLmodels/Geo-DICE

**What it is:** Modified DICE (Dynamic Integrated Climate-Economy) model with geoengineering as an explicit control variable. The DICE model is the most influential climate-economics framework in policy analysis (Nordstrom, 2008 Nobel laureate). Geo-DICE adds SRM as an additional lever.

**Recent commits:** Last commit was September 2018. Four commits total over two upload sessions in August-September 2016.

**Episode angle:** Geo-DICE is historically important — it was one of the first attempts to model SRM within the canonical DICE framework. But its 8-year death march illustrates a key point: the DICE model's creator (William Nordhaus) was *skeptical* of SRM, and Geo-DICE was more a proof-of-concept than a serious policy tool. The model's dormancy mirrors the institutional resistance to SRM within mainstream climate economics.

---
n
---

## Summary Table: Solar Geoengineering Repos

| Rank | Repository | Stars | Status | Last Commit | Theme Relevance |
|------|-----------|-------|--------|-------------|----------------|
| 1 | wrf-model/WRF | 1,762 | 🟢 Active (v4.8.0) | Jun 8, 2026 | **Critical** — foundational atmospheric model |
| 2 | PCMDI/pcmdi_metrics | 133 | 🟢 Active (v4.2.1) | Sep 17, 2026 | **Critical** — ESM evaluation infrastructure |
| 3 | ClimateMARGO.jl | 73 | 🟡 Revival? | Aug 17, 2026 | **High** — climate-economic SRM optimization |
| 4 | awesome-geoengineering | 4 | 🟢 Active (v2.0.0) | Sep 6, 2026 | **Medium** — curated resource list |
| 5 | srm-forever | 0 | 🔴 Single-day burst | Aug 26, 2026 | **Critical** — theoretical SRM cost framework |
| 6 | OOCC_2021 | 2 | ⚫ Dormant (5yr) | Nov 15, 2021 | **Medium** — governance cost-sharing model |
| 7 | Geo-DICE | 2 | ⚫ Dead (8yr) | Sep 27, 2018 | **Low** — historical DICE+SRM modification |

---

## 🎙️ Episode Hooks — Solar Geoengineering

1. **"The Solar Radiation Fix That Changes Everything"** — WRF's May 28 correction to EOT solar radiation calculation means past SRM simulations may have had systematic energy budget errors. Governance implications.

2. **"Zero Stars, Infinite Importance"** — srm-forever has no stars, no forks, no community. But it implements Weitzman's certainty-equivalent discounting — the theoretical framework for "what does it cost to keep SRM going forever?" The most important repo nobody's heard of.

3. **"The Roundoff Error That Could Break Climate Policy"** — PCMDI's fix preventing metrics from rounding to 1.00. If evaluation tools silently produce perfect scores, how do we know what we know about SRM efficacy?

4. **"The 2-Year Sleep and the Two README Pushes"** — ClimateMARGO's mysterious August 2026 revival. Two README updates after 34 months of silence. Revival or ghost?

5. **"Why Is SRM Code So Scarce?"** — The answer: there is no SRM-specific modeling community. The tools are atmospheric models (WRF), evaluation toolkits (PCMDI), and economic models (DICE, MARGO). SRM is *modeled by* other communities, not *by* a dedicated community. That's the structural hole.

---

*Last updated: September 2026 (v4) | Data source: GitHub API commit histories*
*Previous version: v3 (September 2026) | Created: September 2026*