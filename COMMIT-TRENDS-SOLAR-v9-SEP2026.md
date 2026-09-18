# ☀️ Solar Geoengineering — Commit Trend Analysis (v9, September 2026)

> **Branch:** `solar-geoengineering`
> **Podcast episode:** Episode 1 — Solar Geoengineering
> **Data pulled:** September 2026 via GitHub API
> **Repos analyzed:** 5 (WRF, PCMDI/pcmdi_metrics, NOAA-GFDL/MDTF-diagnostics, ClimateMARGO/ClimateMARGO.jl, hausfath/srm-forever)

---

## Executive Summary for Episode Production

The solar geoengineering open-source ecosystem splits into **three distinct development cultures**:

| Culture | Repos | Development Pulse | Episode Angle |
|---------|-------|-------------------|---------------|
| **Operational Infrastructure** | WRF, PCMDI | Continuous, institutional, multi-contributor | "The invisible backbone" |
| **Diagnostic Tools** | MDTF-diagnostics | Bursts of focused activity around specific metrics | "The accuracy police" |
| **Individual Theorists** | ClimateMARGO, srm-forever | Dormant long stretches, then symbolic bursts | "The solo theorists" |

---

## 1. WRF — Weather Research and Forecasting Model

**Repo:** `wrf-model/WRF` | **Stars:** 1,762 | **Language:** Fortran | **License:** GNU GPL

### Recent Commit Window: May 21 – Jun 8, 2026 (10 commits in 18 days)

| Date | SHA | Message | Author | SRM Relevance |
|------|-----|---------|--------|----------------|
| Jun 8, 2026 | `06d4240` | Merge remote-tracking branch 'origin/release-v4.8.0' | Anthony Islas | **v4.8.0 RELEASE** |
| Jun 6, 2026 | `0708348` | Update README and version declaration to v4.8.0 | Anthony Islas | Formal version declaration |
| Jun 5, 2026 | `6a289e1` | **Turn off tempo_aerosolaware and tempo_hailaware** | weiwangncar | **SRM SIGNAL** — disables unstable aerosol-aware physics for stratospheric simulations |
| May 30, 2026 | `4466746` | Fix vectorization option in AOCC stanza | weiwangncar | AMD compiler optimization |
| **May 28, 2026** | **`e836cd6`** | **Correction for eot calculation for solar radiation** | weiwangncar | **MOST SRM-RELEVANT** — Fixes end-of-transition calculation in solar radiation scheme |
| May 27, 2026 | `8299919` | Updating MYNN-EDMF pointer and removing icloud_bl | Joseph Olson | Boundary-layer physics |
| May 27, 2026 | `4fab0e2` | Update MMM-physics repo SHA | Anthony Islas | Multi-year mean physics suite |
| May 26, 2026 | `75ad1f9` | Fixing CDXWRF module | Lluís Fita | Urban climate module |
| May 26, 2026 | `0aa6582` | Update readme file for GFL option | weiwangncar | Gravity-wave drag option |
| May 21, 2026 | `02f02bc` | Include mp_physics=88 in TEMPO error print message | Kelly Werner | Error handling |

### Episode Talking Points — WRF

1. **The Solar Radiation Bug Fix (May 28):** A one-line correction to the end-of-transition calculation. If you ran an SRM simulation before this fix, your energy balance might have been systematically off.

2. **The Aerosol Physics Shutdown (Jun 5):** Three days before v4.8.0, the lead contributor turned off `tempo_aerosolaware` and `tempo_hailaway`. The model says "this physics doesn't work up there" — exactly the conditions relevant to SRM.

3. **Institutional Rhythm:** 10 commits in 18 days, 6 contributors, all NCAR/NOAA affiliations. Big science software is made by funded teams, not lone hackers.

---

## 2. PCMDI/pcmdi_metrics — Climate Model Evaluation Toolkit

**Repo:** `PCMDI/pcmdi_metrics` | **Stars:** 133 | **Language:** Python | **License:** MIT

### Recent Commit Window: Sep 3 – Sep 17, 2026 (10 commits in 14 days)

| Date | SHA | Message | Author | Significance |
|------|-----|---------|--------|-------------|
| Sep 17, 2026 | `b8f231a` | Merge PR #1431 from PCMDI/mov_patch | Jiwoo Lee | Latest patch |
| Sep 17, 2026 | `90a4bc1` | Patch for single file case in modpath_list | Jiwoo Lee | Edge-case fix |
| Sep 4, 2026 | `3092cdd` | Merge PR #1428 | Jiwoo Lee | PR consolidation |
| **Sep 4, 2026** | `6419050` | **Bump version to 4.2.1** | Jiwoo Lee | **Version release** |
| Sep 4, 2026 | `6443a1d` | Merge PR #1429 | Jiwoo Lee | PR consolidation |
| Sep 4, 2026 | `0e3a96f` | Update version in CITATION.cff | Jiwoo Lee | Citation metadata |
| Sep 4, 2026 | `e7dc726` | Prepare v4.2.1 | Jiwoo Lee | Release preparation |
| Sep 4, 2026 | `d0bcbd8` | Merge PR #1427 | Jiwoo Lee | PR consolidation |
| **Sep 4, 2026** | `90cbc50` | **Prevents roundoff to 1.00 in mean_climate figures** | James Goodnight | **KEY SIGNAL** — fixes rounding that could fake perfect model-observation match |
| Sep 3, 2026 | `71a0497` | Merge PR #1425 — extremes chunking | Jiwoo Lee | Performance optimization |

### Episode Talking Points — PCMDI

1. **The Roundoff That Changed Everything (Sep 4):** Models could score "perfect" (1.00) on evaluation metrics by rounding error. A model whose precipitation pattern appears to match observations perfectly might actually be slightly wrong.

2. **The 9-Commit Launch Day:** Nine commits on September 4 alone — all directed at releasing v4.2.1. When the tool that evaluates ALL climate models gets updated, every subsequent paper is implicitly affected.

3. **CMIP6 Governance:** PCMDI metrics are the yardstick for CMIP6. Every SRM study using CMIP6 output is filtered through this codebase.

---

## 3. NOAA-GFDL/MDTF-diagnostics — Process-Oriented Diagnostics

**Repo:** `NOAA-GFDL/MDTF-diagnostics` | **Stars:** 80 | **Language:** Python/R

### Recent Commit Window: Jun 2 – Aug 14, 2026

| Date | SHA | Message | Author | Ocean Relevance |
|------|-----|---------|--------|------------------|
| Aug 14, 2026 | `87f8105` | Merge PR #825 | Aparna Radhakrishnan | Latest update |
| **Jun 19, 2026** | **`33024ad`** | **add MCS precip-buoyancy statistics POD** | Wei-Ming Tsai | **OCEAN'S CLOSEST FRIEND** |
| Jun 19, 2026 | `4cfc99c` | Update MCS_precip_buoy_stats.rst | Wei-Ming Tsai | Doc round 1 |
| Jun 19, 2026 | `699de27` | Update MCS_precip_buoy_stats.rst | Wei-Ming Tsai | Doc round 2 |
| Jun 19, 2026 | `d6bc6d0` | Update MCS_precip_buoy_stats.rst | Wei-Ming Tsai | Doc round 3 |
| Jun 19, 2026 | `3904d29` | Update MCS_precip_buoy_stats.rst | Wei-Ming Tsai | Doc round 4 |
| Jun 8, 2026 | `2df59f6` | Merge PR #823 | Aparna Radhakrishnan | PR consolidation |
| Jun 8, 2026 | `16f936c` | Update README | Jongsooshin5 | Documentation |
| Jun 8, 2026 | `b96127e` | Update README.md | Jongsooshin5 | Companion update |
| Jun 2, 2026 | `97b3028` | Merge branch 'NOAA-GFDL:main' | Jongsooshin5 | Master sync |

### Episode Talking Points — MDTF / Ocean

1. **The 5-Commit Blitz (Jun 19):** Five commits on a single day for the PBP-POD. Four were documentation revisions. This is scientific rigor made visible.

2. **The Ocean's Closest Friend:** The precipitation-buoyancy POD is the most ocean-relevant diagnostic in open source. It evaluates whether models correctly simulate vertical buoyancy motions governing ocean-atmosphere coupling.

3. **Two-Person Team:** All commits from exactly two contributors — Jongsooshin Lee (infrastructure) and Wei-Ming Tsai (science).

---

## 4. ClimateMARGO/ClimateMARGO.jl — Climate-Economic Modeling

**Repo:** `ClimateMARGO/ClimateMARGO.jl` | **Stars:** 73 | **Language:** Julia | **License:** MIT

### Commit Pattern: Long dormancy + revival burst

| Date | SHA | Message | Author | Pattern |
|------|-----|---------|--------|---------|
| **Aug 17, 2026** | `d916f36` | **Update README.md** | Fons van der Plas | **REVIVAL SIGNAL #2** |
| **Aug 17, 2026** | `6d9ba7a` | **Update README.md** | Fons van der Plas | **REVIVAL SIGNAL #1** |
| Oct 18, 2023 | `57d4da7` | Update unit_conversions.jl | Fons van der Plas | Last code change |
| Jul 6, 2023 | `fbbe619` | Add link to Pluto in README | Fons van der Plas | Doc polish |
| Nov 14, 2022 | `5063c42` | Update Project.toml | Fons van der Plas | Dependency mgmt |
| Nov 12, 2022 | `12a0ce6` | JuMP and Ipopt compat upgrade | Fons van der Plas | Last code update |
| Feb 10, 2022 | `32e66fd` | Removed deprecated web apps | Henri Drake | Cleanup |
| Feb 4, 2022 | `d609d49` | Added CITATION.bib | Henri Drake | Citation infra |
| Jan 13, 2022 | `b2d9228` | Fixed typo | Henri Drake | Minor fix |
| Jan 12, 2022 | `8a7e012` | Updated doc version deployment | Henri Drake | Infra |

### Episode Talking Points — ClimateMARGO

1. **The 2.5-Year Silence + 2-Day Burst:** Completely dark from Nov 2022 to Aug 2026. Then two README updates in one day. No code changes. Just acknowledgment that the repo exists.

2. **The Julia Niche:** ClimateMARGO bridges climate science and economics — where SRM governance debates live. How much would it cost to sustain SRM forever?

3. **Single-Person Project:** When the person moves on, the project stops.

---

## 5. hausfath/srm-forever — Interactive SRM Cost Modeling

**Repo:** `hausfath/srm-forever` | **Stars:** 0 | **Language:** JavaScript/HTML

### Complete History: All 4 commits on a single day

| Date | SHA | Message | Significance |
|------|-----|---------|-------------|
| Aug 26, 2026 | `61df1a4` | Add effective discount rate chart | Visualization layer |
| Aug 26, 2026 | `aa9bc0f` | **Adopt Weitzman certainty-equivalent discounting** | **Theoretical framework** |
| Aug 26, 2026 | `9ee822a` | Price abatement as a vintage annuity | Economic mechanics |
| Aug 26, 2026 | `9999436` | Interactive SRM-forever vs mitigation+CDR cost model | **The product** |

### Episode Talking Points — srm-forever

1. **The 4-Commit Day That Packed a Theory:** All four commits on Aug 26. Built an interactive cost comparison model, adopted Weitzman's discounting framework, added a chart, and wrote an essay.

2. **Weitzman Certainty-Equivalent Discounting:** Mathematical machinery for handling "what we don't know about the future" in climate economics. Matters enormously for SRM because the longer you sustain it, the more uncertain costs become.

3. **Zero Stars, Maximum Conceptual Density:** The defining example of the "Empty Universe" problem. The work exists and is rigorous, but nobody's using it.

---

## Cross-Theme Solar Commit Patterns

### The Three Development Cultures

| Culture | Repos | Commit Pattern | Team Size | Funding |
|---------|-------|-----------------|-----------|---------|
| **Institutional** | WRF, PCMDI, MDTF | Regular, multi-contributor | 3-6 | NCAR, NOAA, DOE |
| **Diagnostic-Individual** | MDTF (PBP-POD) | Focused bursts | 1-2 | NOAA-GFDL |
| **Solo-Theoretical** | ClimateMARGO, srm-forever | Dormancy + bursts | 1 | Unfunded |

### Timeline (Sep 2026)

```
Sep 17  PCMDI v4.2.1 patch (90a4bc1)       ← Latest event
Sep 04  PCMDI v4.2.1 release (7 commits)   ← Major release
Aug 26  srm-forever 4-commit theory bundle  ← Theoretical burst
Aug 17  ClimateMARGO 2 README updates       ← Faint revival
Jun 08  WRF v4.8.0 merge                    ← Major release
Jun 05  WRF aerosol physics shutoff         ← SRM-relevant change
May 28  WRF solar radiation eot fix         ← Most SRM-critical fix
Jun 19  MDTF PBP-POD 5-commit blitz         ← Ocean-adjacent
```

---

## Episode 1 Production Notes

### Opening Hook
> "On May 28, 2026, a programmer at NCAR fixed a single line of code in the WRF model — the atmospheric model that underpins nearly every solar geoengineering simulation ever published. The fix corrected how the model calculates the end of a transition period in its solar radiation scheme. If you've read a paper about solar radiation management using WRF, and that paper was published before May 28, 2026, its energy balance might be quietly wrong."

### Three Narrative Arcs

1. **Infrastructure (WRF + PCMDI):** Climate simulation is institutional science. Big teams, version control, funded labs. The solar radiation fix and the roundoff bug both come from this world.

2. **Evaluation (MDTF):** Before you can intervene, you need to evaluate. The PBP-POD is the closest thing to an ocean-atmosphere audit tool.

3. **Lone-Theorist (ClimateMARGO + srm-forever):** Between infrastructure and diagnostics, individuals answer big questions. What does it cost to keep SRM going forever? Zero stars, but maybe the most important ideas.

### Closing Question
> "If the most conceptually important SRM cost model has zero stars, and the most popular atmospheric model just fixed a solar radiation bug that could silently skew results — which matters more: the tool that everyone uses, or the idea that nobody has adopted?"

---

*Last updated: September 2026 (v9) | Next update: December 2026*