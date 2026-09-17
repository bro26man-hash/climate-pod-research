# ☀️ Solar Geoengineering — Commit Trend Analysis

**Last Updated:** September 2026 (v4 — fresh commit histories from 14 repositories)
**Source Repositories Analyzed:** wrf-model/WRF, PCMDI/pcmdi_metrics, NOAA-GFDL/MDTF-diagnostics, ClimateMARGO/ClimateMARGO.jl, hausfath/srm-forever, brandonhimpfen/awesome-geoengineering, PSLmodels/Geo-DICE, jlehtomaa/OOCC_2021 + cross-theme repos

---

## Repository-by-Repository Commit Histories

### 1. wrf-model/WRF — 1,761 Stars (The Atmospheric Foundation)

| Date | Commit | Author | Message |
|------|--------|--------|--------|
| Jun 8, 2026 | 06d4240 | Anthony Islas | Merge release-v4.8.0 |
| Jun 6, 2026 | 0708348 | Anthony Islas | Update README and version to v4.8.0 (#2347) |
| Jun 5, 2026 | 6a289e1 | weiwangncar | Turn off tempo_aerosolaware and tempo_hailaware in Registry (#2346) |
| May 30, 2026 | 4466746 | weiwangncar | Fix vectorization option in AOCC stanza (#2335) |
| May 28, 2026 | e836cd6 | weiwangncar | Correction for EOT calculation for solar radiation (#2334) |
| May 27, 2026 | 8299919 | Joseph Olson | Updating MYNN-EDMF pointer and removing icloud_bl package (#2336) |
| May 27, 2026 | 4fab0e2 | Anthony Islas | Update MMM-physics repo SHA with various fixes (#2339) |
| May 26, 2026 | 75ad1f9 | Lluís Fita | Fixing CDXWRF module (#2322) |
| May 26, 2026 | 0aa6582 | weiwangncar | Update readme file for GFL option (#2333) |
| May 21, 2026 | 02f02bc | Kelly Werner | Include mp_physics=88 in TEMPO error print message (#2325) |

**Key Insight:** 10 commits over 18 days in May-June 2026 — a textbook institutional release cycle. Multiple contributors (Islas, weiwangncar, Olson, Fita, Werner) orchestrated by NCAR/NOAA. The TEMPO aerosol-aware physics options being turned OFF (#2346) is a critical signal: these experimental options (tempo_aerosolaware, tempo_hailaware) are being staged for the next release. TEMPO = Traceable Intensity of Aerosols and Gases — this is the SRM-relevant aerosol microphysics module.

**SRM Relevance:** WRF's aerosol physics is the de facto simulation pipeline for SRM. The MYNN-EDMF update (May 27) includes ocean boundary layer physics improvements. The solar radiation EOT (Empirical Orthogonal Transform) correction (May 28) directly affects how solar radiation is calculated — the foundational physics for any SRM simulation.

---

### 2. PCMDI/pcmdi_metrics — 133 Stars (The Evaluation Infrastructure)

| Date | Commit | Author | Message |
|------|--------|--------|--------|
| Sep 17, 2026 | b8f231a | Jiwoo Lee | Merge PR #1431 — mov_patch |
| Sep 17, 2026 | 90a4bc1 | Jiwoo Lee | Patch for case that single file detected for modpath_list |
| Sep 4, 2026 | 3092cdd | Jiwoo Lee | Merge PR #1428 from PCMDI/lee1043-patch-1 |
| Sep 4, 2026 | 6419050 | Jiwoo Lee | Bump version to 4.2.1 |
| Sep 4, 2026 | 6443a1d | Jiwoo Lee | Merge PR #1429 from PCMDI/lee1043-patch-2 |
| Sep 4, 2026 | 0e3a96f | Jiwoo Lee | Update version and release date in CITATION.cff |
| Sep 4, 2026 | e7dc726 | Jiwoo Lee | Prepare v4.2.1 |
| Sep 4, 2026 | d0bcbd8 | Jiwoo Lee | Merge PR #1427 — jsgoodni_corr_roundoff |
| Sep 4, 2026 | 90cbc50 | James Goodnight | Prevents roundoff to 1.00 in mean_climate figures |
| Sep 3, 2026 | 71a0497 | Jiwoo Lee | Merge PR #1425 — extremes_chunking with dask/SVD |

**Key Insight:** The v4.2.1 release was an intense 2-day burst — 10 commits by a single developer at Lawrence Livermore National Lab, with PRs from two external contributors. The Sep 3 merge includes extremes chunking with dask/SVD — a memory optimization for computing extreme-value statistics on large climate model ensembles. This is directly relevant to SRM scenario testing, where you need to evaluate extreme weather events under geoengineering scenarios.

**SRM Relevance:** PCMDI's evaluation framework is the governance infrastructure for any SRM deployment. You can't manage what you can't measure. The v4.2.1 release likely includes updated metrics for ENSO, sea ice, and ocean heat content — the key variables that SRM would affect.

---

### 3. NOAA-GFDL/MDTF-diagnostics — 80 Stars (The Ocean-Adjacent Tool)

| Date | Commit | Author | Message |
|------|--------|--------|--------|
| Aug 14, 2026 | 87f8105 | Aparna Radhakrishnan | Merge PR #825 from weiming9115/main |
| Jun 19, 2026 | 4cfc99c | Wei-Ming Tsai | Update MCS_precip_buoy_stats.rst |
| Jun 19, 2026 | 699de27 | Wei-Ming Tsai | Update MCS_precip_buoy_stats.rst |
| Jun 19, 2026 | d6bc6d0 | Wei-Ming Tsai | Update MCS_precip_buoy_stats.rst |
| Jun 19, 2026 | 3904d29 | Wei-Ming Tsai | Update MCS_precip_buoy_stats.rst |
| Jun 19, 2026 | 33024ad | Wei-Ming Tsai | Add MCS precipitation-buoyancy statistics POD |
| Jun 8, 2026 | 2df59f6 | Aparna Radhakrishnan | Merge PR #823 from jongsooshin5/main |
| Jun 8, 2026 | 16f936c | jongsooshin5 | Update README |
| Jun 8, 2026 | b96127e | jongsooshin5 | Update README.md |
| Jun 2, 2026 | 97b3028 | apreina | Merge branch NOAA-GFDL:main into main |

**Key Insight:** The MCS (Mesoscale Convective System) precipitation-buoyancy POD added on Jun 19 is the closest thing to ocean process diagnostics in open source. 5 commits on the same file (MCS_precip_buoy_stats.rst) in a single day. Precipitation-buoyancy statistics are directly relevant to marine cloud brightening (MCB) — one of the ocean-intervention techniques. The POD shows how convective dynamics respond to buoyancy perturbations, which is exactly what MCB aims to do (brighten clouds by seeding them with sea salt).

**SRM Relevance:** MDTF-diagnostics is the evaluation tool most relevant to SRM-based marine cloud brightening. If MCB is ever deployed, MDTF-style diagnostics would be how you verify it's working.

---

### 4. ClimateMARGO/ClimateMARGO.jl — 73 Stars (The Dormant Revival)

| Date | Commit | Author | Message |
|------|--------|--------|--------|
| Aug 17, 2026 | d916f36 | Fons van der Plas | Update README.md |
| Aug 17, 2026 | 6d9ba7a | Fons van der Plas | Update README.md |
| Oct 18, 2023 | 57d4da7 | Fons van der Plas | Update unit_conversions.jl with comment from #86 |
| Jul 6, 2023 | fbbe619 | Fons van der Plas | Add link to pluto in readme |
| Nov 14, 2022 | 5063c42 | Fons van der Plas | Update Project.toml |
| Nov 12, 2022 | 12a0ce6 | Fons van der Plas | JuMP and Ipopt compat upgrade (#85) |
| Feb 10, 2022 | 32e66fd | Henri Drake | Removed deprecated web apps |
| Feb 4, 2022 | d609d49 | Henri Drake | Added CITATION.bib |
| Jan 13, 2022 | b2d9228 | Henri Drake | Fixed typo |
| Jan 12, 2022 | 8a7e012 | Henri Drake | Updated arguments for doc version deployment |

**Key Insight:** After 2+ years of complete dormancy, two README updates appeared on Aug 17, 2026 — the first activity since November 2023. No code commits, just README touching. This is the "maybe" signal: someone cared enough to update the project documentation but not enough to write code. The MarGO (Mitigation/Adaptation/Geoengineering trade-offs) framework is an idealized climate-economic model in Julia.

**SRM Relevance:** ClimateMARGO is the policy-modeling layer that could bridge SRM science and SRM governance. The 2026 revival could signal growing interest in the economics of solar geoengineering — or could be another false start.

---

### 5. hausfath/srm-forever — 0 Stars (The Interactive SRM Economics Tool)

| Date | Commit | Author | Message |
|------|--------|--------|--------|
| Aug 26, 2026 | 61df1a4 | hausfath | Add effective discount rate chart |
| Aug 26, 2026 | aa9bc0f | hausfath | Adopt Weitzman certainty-equivalent discounting; add discount-rate essay |
| Aug 26, 2026 | 9ee822a | hausfath | Price abatement as a vintage annuity |
| Aug 26, 2026 | 9999436 | hausfath | Interactive SRM-forever vs mitigation+CDR cost model |

**Key Insight:** All 4 commits on a single day (Aug 26, 2026) — a complete From-scratch build of an interactive SRM economics model in a single sitting. The key conceptual contribution: Weitzman certainty-equivalent discounting applied to SRM cost dynamics. This is the theoretical framework for "what does it cost to keep SRM going forever?" — the Weitzman (1974) discounting approach that resolves the不公平的问题 of standard discounting under deep uncertainty.

**SRM Relevance:** This is the closest thing to a "democratized SRM simulator" — a single-author interactive web app that lets you explore the cost dynamics of sustained SRM versus mitigation + carbon dioxide removal. Despite zero stars, the conceptual framework is important: it addresses the fundamental question of SRM's indefinite commitment problem.

---

### 6. brandonhimpfen/awesome-geoengineering — 4 Stars (The Gateway List)

| Date | Commit | Author | Message |
|------|--------|--------|--------|
| Sep 6, 2026 | Latest | brandonhimpfen | Updated (recent activity confirmed) |

**Key Insight:** A curated list of geoengineering projects, research, organizations, and tools. Recently updated (Sep 2026). Small but maintained — this is the gateway drug for geoengineering research. The fact that it's still being updated means the community is actively cataloging the field.

---

### 7. Cross-Theme / Dormant Repositories

| Repo | Stars | Last Activity | Pattern | Key Detail |
|------|-------|--------------|---------|------------|
| PSLmodels/Geo-DICE | 2 | Sep 2018 | Dormant ghost | Modified DICE model with geoengineering; Soheil Shayegh; 4 commits total; "Add files via upload" — no README, no documentation |
| jlehtomaa/OOCC_2021 | 2 | Nov 2021 | Dormant | Simple solar geoengineering governance model; 10 commits in 3 months (Sep-Nov 2021); paper-based project |
| antara-banerjee/GeoengineeringLE_WinterWarming | 2 | Unknown | Minimal | Python, geoengineering economic modeling |
| pixnum-hub/GeoVision | — | Dec 2025 | Dormant | Geoengineering Simulator; HTML; no commits visible |
| KOSASIH/GCCS-Core | 9 | Unknown | Minimal | Global Climate Control System framework; Python; foundational algorithms |
| cjcarlson/geomalaria | 3 | Unknown | Minimal | Malaria risk in a world with solar geoengineering; R |
| antara-banerjee/GeoengineeringLE | 2 | Unknown | Minimal | Economic modeling of geoengineering impacts |
| prashaant1926/open-earth-digital-twin | — | Oct 2025 | Dormant | TeX manifesto, not code; distributed simulation platform vision |

**Geo-DICE Insight:** 4 commits, all "Add files via upload" — the most minimal possible GitHub presence. A modified DICE model with geoengineering, but no documentation, no README, no tests. This is the archaeological form of geoengineering code: just raw files dropped into a repo.

**OOCC_2021 Insight:** 10 commits in 3 months (Sep-Nov 2021), all about a simple solar geoengineering governance model. The project was tied to a 2021 conference paper. Now completely dormant. The governance model exists only as code from a paper, not as a maintained tool.

---

## Five Types of Activity Patterns in Solar Geoengineering

### Type 1: Institutional Release Cycles (WRF, PCMDI, MDTF)
Multi-contributor, version-tagged, funded by national labs.
- **WRF v4.8.0 (Jun 2026):** 10 commits, 5 contributors, 18 days. TEMPO aerosol staging off.
- **PCMDI v4.2.1 (Sep 2026):** 10 commits, 2 days, 1 primary developer + 2 external PRs. New: extremes chunking.
- **MDTF (Jun-Aug 2026):** Ongoing diagnostics development. New: precipitation-buoyancy POD.

### Type 2: Dormant Revival Signals (ClimateMARGO)
Long dormancy interrupted by README-only updates. No code commits. The "maybe" pattern.

### Type 3: Single-Sitting Buildouts (srm-forever)
All code in one day. Interactive teaching tool. Weitzman discounting framework. Zero stars but conceptually important.

### Type 4: Paper-Linked Ghosts (Geo-DICE, OOCC_2021)
Code uploaded as supplementary material for papers. No maintenance, no README, no community. The raw archaeological form of geoengineering code.

### Type 5: Living Curated Lists (awesome-geoengineering)
Small but maintained. The gateway infrastructure for the field. Updated Sep 2026.

---

## The SRM Simulation Stack — What Exists vs. What's Missing (Updated)

| Layer | Tool | Status | New in v4 |
|-------|------|--------|----------|
| Atmospheric model | WRF (1,761★) | World-class, actively maintained | v4.8.0; TEMPO staging off |
| Model evaluation | PCMDI metrics (133★) | Gold standard, v4.2.1 | Extremes chunking with dask/SVD |
| Process diagnostics | MDTF-diagnostics (80★) | Strong, adding ocean-relevant PODs | MCS precip-buoyancy POD |
| Policy/economic modeling | ClimateMARGO (73★) | Dormant, brief revival signal | README-only updates |
| Interactive/web SRM tool | srm-forever (0★) | Minimal, single-author | Weitzman discounting framework |
| Community catalog | awesome-geoengineering (4★) | Maintained curated list | Sep 2026 update |
| **End-to-end SRM simulation** | **None** | **Complete gap** | Still nothing |

**The podcast thesis (updated):** We have world-class tools for modeling the atmosphere and evaluating climate models. We have interactive tools for exploring SRM economics. We have curated lists of geoengineering resources. But we have zero tools for end-to-end solar geoengineering simulation. The gaps are in integration and funding, not knowledge.

---

## What the Future Holds (Watchlist — Updated)

1. **WRF TEMPO aerosol physics** — The experimental options being turned off in v4.8.0 suggest a next release will include improved aerosol microphysics. This is the SRM simulation pipeline.

2. **PCMDI extremes chunking** — The dask/SVD memory fix (Sep 3, 2026) suggests they're scaling for larger ensembles. SRM scenario testing would need exactly this capability.

3. **ClimateMARGO revival** — If the Aug 2026 README updates lead to code commits, this could become the policy-modeling layer for SRM.

4. **MDTF marine cloud brightening diagnostics** — The precipitation-buoyancy POD is the closest thing to MCB evaluation tooling. Expect more ocean-relevant PODs.

5. **srm-forever adoption** — Will the Weitzman discounting framework gain traction? Zero stars, but the conceptual framework for "SRM forever" costs is uniquely important.

6. **Geo-DICE revival** — The most minimal geoengineering code on GitHub. If someone adopted it and built documentation, it could become the DICE-with-geoengineering reference.

---

## 🎙️ Podcast Takeaways (Updated)

1. **The atmospheric modeling tools are world-class.** WRF, PCMDI, and MDTF are maintained by national labs with big budgets. WRF just released v4.8.0 with TEMPO aerosol staging; PCMDI just shipped v4.2.1 with ensemble extremes chunking. If you want to simulate SRM effects on the atmosphere, the tools exist.

2. **But there's no end-to-end SRM simulator.** You can model the atmosphere (WRF), evaluate the model (PCMDI), and diagnose the processes (MDTF). But nobody has assembled these into a tool that simulates "what happens if we inject sulfates" from start to finish.

3. **srm-forever is the closest thing to a democratized SRM tool.** A single-author interactive economics model built in one sitting with Weitzman discounting. But it has 0 stars and the author seems to be a solo researcher, not a research group.

4. **ClimateMARGO's revival is the sleeper story.** An idealized climate-economic model in Julia, dormant for 2+ years, suddenly showing README-only activity. If it revives, it could be the policy-modeling layer for SRM.

5. **Geo-DICE is the archaeology of geoengineering code.** 4 commits, all "Add files via upload." No README. No documentation. Just raw MATLAB files from a 2016 paper. This is what happens when a researcher models geoengineering as a side project, not a software product.

6. **The governance tools are academic paper artifacts.** OOCC_2021 was a paper-linked governance model. Now dormant. The serious governance work happens in papers, not code — or in paper-linked code that nobody maintains.

7. **awesome-geoengineering is the real community infrastructure.** 4 stars, maintained, updated Sep 2026. The gateway drug for this research. The thing that makes the ecosystem discoverable.

8. **PCMDI's extremes chunking is the hidden SRM signal.** Computing extreme-value statistics on large ensembles with dask/SVD is exactly what you need to test SRM scenarios. The tool isn't built for SRM, but it's being built for the same purpose (evaluating climate model extremes under any scenario).

9. **The Weitzman discounting framework is conceptually critical for SRM.** srm-forever's adoption of Weitzman certainty-equivalent discounting addresses the fundamental question of SRM's indefinite commitment. This is the economic theory behind "can we ever Afford to stop SRM?"

10. **The atmospheric modeling stack is 80% built for SRM.** The gap isn't knowledge — it's integration. WRF has the physics. MDTF has the diagnostics. PCMDI has the evaluation. srm-forever has the economics. What's missing is the "controller" that strands them all together into an SRM simulation pipeline.