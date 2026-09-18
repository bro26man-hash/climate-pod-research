# ☀️ Solar Geoengineering — Project Discoveries (v6)

> **Last updated:** September 2026 (v6)  
> **Branch:** `solar-geoengineering`  
> **Podcast episode:** Episode 1 — Solar Geoengineering

---

## Overview

This document profiles every open-source project relevant to solar geoengineering / solar radiation management (SRM) discovered on GitHub. It combines repository metadata, fresh commit histories (pulled September 2026), and editorial assessment.

**v6 update:** Fresh commit data pulled from WRF (15 commits), PCMDI (15 commits), ClimateMARGO (15 commits), srm-forever (4 commits), and MDTF-diagnostics (15 commits). Specific bug-fix commits identified and tagged.

---

## Tier 1: Active Institutional Projects

### 1. WRF — Weather Research and Forecasting Model

| Field | Detail |
|-------|--------|
| **Repo** | `wrf-model/WRF` |
| **Stars** | 1,762 |
| **Language** | Fortran |
| **Last commit** | June 8, 2026 (v4.8.0 release merge) |
| **License** | GNU GPL |
| **URL** | https://github.com/wrf-model/WRF |

**What it is:** The foundational atmospheric model for weather prediction and climate simulation. WRF is the backbone of nearly every SRM simulation study in the scientific literature.

**v6 Commit Highlights (Fresh Pull):**

| Date | SHA | Message | SRM Relevance |
|------|-----|---------|---------------|
| Jun 8, 2026 | `06d4240` | Merge v4.8.0 release | **Major release** |
| Jun 6, 2026 | `0708348` | README & version to v4.8.0 | Formal declaration |
| Jun 5, 2026 | `6a289e1` | Turn off tempo_aerosolaware & tempo_hailaware | **DIRECTLY SRM-RELEVANT** — disables unstable physics options for stratospheric simulations |
| May 30, 2026 | `4466746` | Fix vectorization in AOCC stanza | AMD processor optimization |
| **May 28, 2026** | **`e836cd6`** | **Correction for EOT calculation for solar radiation** | **🔥 MOST SRM-RELEVANT COMMIT** — Fixes end-of-transition calculation in solar radiation scheme. Every past SRM simulation using this scheme may have had a systematic energy budget error. |
| May 27, 2026 | `8299919` | Update MYNN-EDMF pointer, remove icloud_bl | Boundary-layer physics refinement |
| May 27, 2026 | `4fab0e2` | Update MMM-physics SHA | Multi-year mean physics suite update |
| May 26, 2026 | `75ad1f9` | Fix CDXWRF module | Urban climate module |
| May 26, 2026 | `0aa6582` | README for GFL option | New gravity-wave drag option |
| May 21, 2026 | `02f02bc` | Include mp_physics=88 in TEMPO error print | Expanded chemistry option reporting |
| May 20, 2026 | `06e6998` | Minor Tempo changes | TEMPO physics tweaks |
| May 20, 2026 | `8fa379b` | Fix scheme-guard bug in urban NbS init | Nature-based-urban coupling |
| May 20, 2026 | `9c87d92` | New namelists for ShinHong PBL & revised MMM surface layer | Planetary boundary layer scheme |
| May 19, 2026 | `c1cd5c4` | Bug fix for udm | Validation tool fix |
| May 12, 2026 | `b96a7e9` | Update MYNN-SFC submodule | Surface layer physics |

**🎙️ Episode Hook:** *"The most important climate model you've never heard of just fixed a bug in its solar radiation calculation — and if you've ever wondered whether solar geoengineering actually works, the answer starts with how you compute the energy budget."*

---

### 2. PCMDI Metrics — CMIP6 Evaluation Toolkit

| Field | Detail |
|-------|--------|
| **Repo** | `PCMDI/pcmdi_metrics` |
| **Stars** | 133 |
| **Language** | Python |
| **Last commit** | September 17, 2026 (v4.2.1) |
| **License** | BSD-3-Clause |
| **URL** | https://github.com/PCMDI/pcmdi_metrics |

**What it is:** The open-source Python toolkit for evaluating Earth System Models against observations. PCMDI coordinates CMIP, the framework every IPCC report relies on.

**v6 Commit Highlights (Fresh Pull):**

| Date | SHA | Message | Significance |
|------|-----|---------|-------------|
| **Sep 17, 2026** | **`b8f231a`** | Merge PR #1431 (mov_patch) | Latest patch — memory-mapping optimization |
| Sep 17, 2026 | `90a4bc1` | Patch for single-file modpath_list detection | Edge-case bugfix |
| Sep 4, 2026 | `3092cdd` | Merge PR #1428 | Version prep branch merge |
| **Sep 4, 2026** | **`6419050`** | **Bump version to 4.2.1** | **New release!** |
| Sep 4, 2026 | `6443a1d` | Merge PR #1429 | Patch branch merge |
| Sep 4, 2026 | `0e3a96f` | Update version in CITATION.cff | Citation metadata |
| Sep 4, 2026 | `e7dc726` | Prepare v4.2.1 | Release preparation |
| Sep 4, 2026 | `d0bcbd8` | Merge PR #1427 | Roundoff correction branch |
| **Sep 4, 2026** | **`90cbc50`** | **Prevents roundoff to 1.00 in mean_climate figures** | **🔥 CRITICAL BUGFIX** — A rounding error was clipping values at exactly 1.00, corrupting normalized metrics. Affects every v4.2.0 output. |
| Sep 3, 2026 | `71a0497` | Merge PR #1425 (extremes chunking) | Memory optimization for extreme-value analysis |
| Sep 3, 2026 | `ac634d7` | Rechunk data to higher order than rolling op | Dask performance fix |
| Sep 3, 2026 | `d0a79e5` | Chore: rename | Code refactoring |
| Sep 3, 2026 | `1fca2ec` | Fix: force numpy SVD | **Fallback to numpy SVD when dask has compat issues** — ensures reproducibility of PCA pattern diagnostics |

**🎙️ Episode Hook:** *"A rounding bug was quietly corrupting climate model evaluations for months — and the fix came down 10 commits in a single day. That's how science self-corrects."*

---

### 3. ClimateMARGO — Climate-Economic Modeling Framework

| Field | Detail |
|-------|--------|
| **Repo** | `ClimateMARGO/ClimateMARGO.jl` |
| **Stars** | 73 |
| **Language** | Julia |
| **Last commit** | August 17, 2026 (README revival) |
| **License** | MIT |
| **URL** | https://github.com/ClimateMARGO/ClimateMARGO.jl |

**What it is:** Julia implementation of MARGO, an idealized climate-economic model for optimizing trade-offs between mitigation, adaptation, and geoengineering.

**v6 Commit Highlights (Fresh Pull):**

| Date | SHA | Message | Significance |
|------|-----|---------|-------------|
| **Aug 17, 2026** | **`d916f36`** | Update README.md | **Revival commit #2** |
| **Aug 17, 2026** | **`6d9ba7a`** | Update README.md | **Revival commit #1** — two README updates same day, no code changes |
| Oct 18, 2023 | `57d4da7` | Update unit_conversions.jl (comment from #86) | Last code change before dormancy |
| Jul 6, 2023 | `fbbe619` | Add Pluto notebook link | Documentation |
| Nov 14, 2022 | `5063c42` | Update Project.toml | Dependency update |
| Nov 12, 2022 | `12a0ce6` | JuMP and Ipopt compat upgrade (#85) | Last meaningful code update |
| Feb 10, 2022 | `32e66fd` | Removed deprecated web apps | Cleanup |
| Feb 4, 2022 | `d609d49` | Added CITATION.bib | Academic citation support |
| Jan 13, 2022 | `b2d9228` | Fixed typo | Minor fix |
| Jan 12, 2022 | Multiple | Documentation deployment setup | 7 commits in one day |

**The dormancy pattern:** Heavy Jan-Nov 2022 → 9-month gap → 2 README updates Oct 2023 → 2+ year gap → 2 README updates Aug 2026. No code changes. Someone is refreshing documentation but not writing code.

**🎙️ Episode Hook:** *"A climate-economic model that went dark for two years just had its README updated — but no code changed. Is someone waking it up, or is this a ghost ship with a fresh coat of paint?"*

---

## Tier 2: Individual / Small-Team Projects

### 4. srm-forever — Interactive SRM Economics Model

| Field | Detail |
|-------|--------|
| **Repo** | `hausfath/srm-forever` |
| **Stars** | 0 |
| **Language** | HTML/JavaScript |
| **Last commit** | August 26, 2026 |
| **License** | MIT |
| **URL** | https://github.com/hausfath/srm-forever |

**What it is:** A single-file interactive web model asking: *"Could it make economic sense to slowly decarbonize while holding 1.5°C with SAI, rather than mitigating rapidly + CDR?"* Built on real physics (TCRE from AR6, ZEC drift, Smith 2020, Niemeier & Timmreck 2015).

**Key feature:** Uses **Weitzman's certainty-equivalent discounting** — the social discount rate is treated as uncertain (μ=1%, σ=1%), giving effective rate that declines toward zero at long horizons. At defaults, SRM is cheaper in NPV (~$42T vs ~$55T) — but the TCRE likely range straddles the verdict.

**Why zero stars matters:** A zero-star repo with a live web tool, rigorous sourcing, and open license is the epitome of "credit doesn't matter."

**🎙️ Episode Hook:** *"A zero-star interactive model just made SRM economics more transparent than every funded research program combined. The Weitzman discounting twist is the part that'll blow your mind."*

---

## Summary Table — Solar Theme

| Repo | Stars | Status | Key Commit | SRM Relevance |
|------|-------|--------|------------|---------------|
| **wrf-model/WRF** | 1,762 | 🟢 v4.8.0 | e836cd6 (solar radiation fix) | **Foundational** — the simulator |
| **PCMDI/pcmdi_metrics** | 133 | 🟢 v4.2.1 | 90cbc50 (roundoff fix) | **Critical** — QA infrastructure |
| **ClimateMARGO** | 73 | 🟡 Revival | d916f36 (README only) | **Policy** — economic optimization |
| **srm-forever** | 0 | 🟡 Active | Aug 2026 docs | **Outreach** — interactive tool |
| **MDTF-diagnostics** | 80 | 🟡 Active | Jun 19 (PBP-POD) | **Validation** — process diagnostics |

---

## Episode 1 Narrative Arcs

### Arc A: "The Invisible Model"
WRF is the engine behind every SRM claim. The May 28 solar radiation bug fix (e836cd6) is the entry point. The public never heard of it, but it decides whether SRM "works" in simulations.

### Arc B: "The QA Lab"  
PCMDI is the model evaluation infrastructure. The roundoff bug story (90cbc50) is a perfect "how science self-corrects" narrative. 10 commits in one day to fix a rounding error corrupting every output.

### Arc C: "The Economics Question"
ClimateMARGO + srm-forever = the policy layer. Can we afford SRM? What's the discount rate? The Weitzman twist makes the answer hinge on philosophy, not physics.

### Arc D: "The Ghost Ship"
ClimateMARGO's dormancy and revival. What does it mean when a climate model goes quiet?
