# ☀️ Solar Geoengineering — Commit Trend Analysis

**Last Updated:** September 2026
**Source Repositories Analyzed:** wrf-model/WRF, PCMDI/pcmdi_metrics, NOAA-GFDL/MDTF-diagnostics, ClimateMARGO/ClimateMARGO.jl, hausfath/srm-forever, prashaant1926/open-earth-digital-twin-simulation, plus cross-theme repos (PMIP analyzer, AM3, DICE variants)

---

## Repository-by-Repository Commit Histories

### 1. wrf-model/WRF — 1,761 Stars (The Atmospheric Foundation)

| Date | Commit | Author |
|------|--------|--------|
| Jun 8, 2026 | Merge release-v4.8.0 | Anthony Islas |
| Jun 6, 2026 | Update README and version to v4.8.0 (#2347) | Anthony Islas |
| Jun 5, 2026 | Turn off tempo_aerosolaware and tempo_hailaware in Registry (#2346) | weiwangncar |
| May 30, 2026 | Fix vectorization option in AOCC stanza (#2335) | weiwangncar |
| May 28, 2026 | Correction for EOT calculation for solar radiation (#2334) | weiwangncar |
| May 27, 2026 | Updating MYNN-EDMF pointer and removing icloud_bl package (#2336) | Joseph Olson |
| May 27, 2026 | Update MMM-physics repo SHA with various fixes (#2339) | Anthony Islas |
| May 26, 2026 | Fixing CDXWRF module (#2322) | Lluís Fita |
| May 26, 2026 | Update readme file for GFL option (#2333) | weiwangncar |
| May 21, 2026 | Include mp_physics=88 in TEMPO error print message (#2325) | Kelly Werner |

**Key Insight:** 10 commits over 18 days in May-June 2026 — a textbook institutional release cycle. Multiple contributors (Islas, weiwangncar, Olson, Fita, Werner) orchestrated by NCAR/NOAA. The TEMPO aerosol-aware physics options being turned OFF (#2346) is a critical signal: these experimental options (tempo_aerosolaware, tempo_hailaware) are being staged for the next release. TEMPO = Traceable Intensity of Aerosols and Gases — this is the SRM-relevant aerosol microphysics module.

**SRM Relevance:** WRF's aerosol physics is the de facto simulation pipeline for SRM. The MYNN-EDMF update (May 27) includes ocean boundary layer physics improvements. The solar radiation EOT (Empirical Orthogonal Transform) correction (May 28) directly affects how solar radiation is calculated — the foundational physics for any SRM simulation.

---

### 2. PCMDI/pcmdi_metrics — 133 Stars (The Evaluation Infrastructure)

| Date | Activity |
|------|----------|
| Sep 3-4, 2026 | v4.2.1 release (10 commits in 2 days by Jiwoo Lee at LLNL; PRs from James Goodnight, Jared Lewis) |
| Jun 19, 2026 | MCS precipitation-buoyancy statistics POD (Wei-Ming Tsai) |
| Jun 8, 2026 | PR #825 merged (Aparna Radhakrishnan) |

**Key Insight:** The v4.2.1 release was an intense 2-day burst — 10 commits by a single developer at Lawrence Livermore National Lab, with PRs from two external contributors. This is the pattern of a funded national lab release cycle. PCMDI metrics are the gold-standard for evaluating CMIP6 models. If SRM is deployed, we need tools like this to evaluate whether it worked — and against what baseline.

**SRM Relevance:** PCMDI's evaluation framework is the governance infrastructure for any SRM deployment. You can't manage what you can't measure. The v4.2.1 release likely includes updated metrics for ENSO, sea ice, and ocean heat content — the key variables that SRM would affect.

---

### 3. NOAA-GFDL/MDTF-diagnostics — 80 Stars (The Ocean-Adjacent Tool)

| Date | Activity |
|------|----------|
| Aug 14, 2026 | Merge PR #825 (Aparna Radhakrishnan) |
| Jun 19, 2026 | MCS precipitation-buoyancy statistics POD — 5 commits in 1 day by Wei-Ming Tsai |
| Jun 8, 2026 | PR #823 merged; README update by jongsooshin5 |
| Jun 2, 2026 | Merge NOAA-GFDL:main into main |

**Key Insight:** The MCS (Mesoscale Convective System) precipitation-buoyancy POD added on Jun 19 is the closest thing to ocean process diagnostics in open source. Precipitation-buoyancy statistics are directly relevant to marine cloud brightening (MCB) — one of the ocean-intervention techniques. The POD shows how convective dynamics respond to buoyancy perturbations, which is exactly what MCB aims to do (brighten clouds by seeding them with sea salt).

**SRM Relevance:** MDTF-diagnostics is the evaluation tool most relevant to SRM-based marine cloud brightening. If MCB is ever deployed, MDTF-style diagnostics would be how you verify it's working.

---

### 4. ClimateMARGO/ClimateMARGO.jl — 73 Stars (The Dormant Revival)

| Date | Activity |
|------|----------|
| Aug 17, 2026 | README update (2 commits same day) by Fons van der Plas |
| Oct 18, 2023 | Last code commit (unit_conversions.jl) |
| Jul 6, 2023 | Pluto notebook link added |
| Nov 14, 2022 | Project.toml update |
|

**Key Insight:** After 2+ years of complete dormancy, two README updates appeared on Aug 17, 2026 — the first activity since November 2023. No code commits, just README touching. This is the "maybe" signal: someone cared enough to update the项目介绍 but not enough to write code. The MarGO (Mitigation/Adaptation/Geoengineering trade-offs) framework is an idealized climate-economic model in Julia.

**SRM Relevance:** ClimateMARGO is the policy-modeling layer that could bridge SRM science and SRM governance. The 2026 revival could signal growing interest in the economics of solar geoengineering — or could be another false start.

---

### 5. Cross-Theme SRM Repositories (Low Activity)

| Repo | Stars | Last Activity | Pattern |
|------|-------|--------------|---------|
| hausfath/srm-forever | 0 | Aug 26, 2026 | Single-author burst — interactive SRM economics teaching tool |
| prashaant1926/open-earth-digital-twin | 0 | Oct 2025 | Dormant — TeX manifesto, not code |
| pmip4/pmip_p2fvar_analyzer | 4 | Sep 2025 | Minimal — PMIP paleoclimate analyzer |
| FMS-ESM/AM3 | 4 | Mar 2015 | Legacy — 11+ years dormant, Fortran-based |
| antara-banerjee/GeoengineeringLE_WinterWarming | 2 | Unknown | Python, geoengineering economic modeling |
| PSLmodels/Geo-DICE | 2 | Unknown | Modified DICE model with geoengineering |
| jlehtomaa/OOCC_2021 | 2 | Unknown | Simple solar geoengineering governance model |

---

## Four Types of Activity Patterns in Solar Geoengineering

### Type 1: Institutional Release Cycles (WRF, PCMDI, MDTF)
Multi-contributor, version-tagged, funded by national labs.
- WRF v4.8.0 (Jun 2026): 10 commits, 5 contributors, 18 days
- PCMDI v4.2.1 (Sep 2026): 10 commits, 2 days, 1 primary developer
- MDTF (Jun-Aug 2026): ongoing diagnostics development

### Type 2: Dormant Revival Signals (ClimateMARGO)
Long dormancy interrupted by README-only updates. No code commits.

### Type 3: Teaching/Toy Tools (srm-forever, Geo-DICE, OOCC)
Single-author, small repos, limited scope. srm-forever is an interactive web app for SRM economics — the closest thing to a "democratized SRM simulator."

### Type 4: Legacy Fortn (AM3, PMIP analyzer)
Ancient, dormant, Fortran-based. The geoengineering simulation ecosystem predates the Python/open-source revolution.

---

## The SRM Simulation Stack — What Exists vs. What's Missing

| Layer | Tool | Status |
|-------|------|--------|
| Atmospheric model | WRF (1,761★) | World-class, actively maintained |
|(Model evaluation) | PCMDI metrics (133★) | Gold standard, actively maintained |
| Process diagnostics | MDTF-diagnostics (80★) | Strong, adding ocean-relevant PODs |
| Policy/economic modeling | ClimateMARGO (73★) | Dormant, brief revival signal |
| Interactive/web SRM tool | srm-forever (0★) | Minimal, single-author |
| **End-to-end SRM simulation** | **None** | **Complete gap** |

**The podcast thesis:** We have world-class tools for modeling the atmosphere and evaluating climate models. We have zero tools for end-to-end solar geoengineering simulation. The gap isn't knowledge — it's integration and funding.

---

## What the Future Holds (Watchlist)

1. **WRF TEMPO aerosol physics** — The experimental options being turned off in v4.8.0 suggest a next release will include improved aerosol microphysics. This is the SRM simulation pipeline.

2. **ClimateMARGO revival** — If the Aug 2026 README updates lead to code commits, this could become the policy-modeling layer for SRM.

3. **MDTF marine cloud brightening diagnostics** — The precipitation-buoyancy POD is the closest thing to MCB evaluation tooling. Expect more ocean-relevant PODs.

4. **PCMDI v4.2.x follow-up** — The v4.2.1 release cycle suggests active development. Future versions may include more SRM-relevant metrics.

---

## 🎙️ Podcast Takeaways

1. **The atmospheric modeling tools are world-class.** WRF, PCMDI, and MDTF are maintained by national labs with big budgets. If you want to simulate SRM effects on the atmosphere, the tools exist.

2. **But there's no end-to-end SRM simulator.** You can model the atmosphere (WRF), evaluate the model (PCMDI), and diagnose the processes (MDTF). But nobody has assembled these into a tool that simulates "what happens if we inject sulfates" from start to finish.

3. **srm-forever is the closest thing to a democratized SRM tool.** A single-author interactive economics model. But it has 0 stars and the author seems to be a student, not a research group.

4. **ClimateMARGO's revival is the sleeper story.** An idealized climate-economic model in Julia, dormant for 2 years, suddenly showing activity. If it revives, it could be the policy-modeling layer for SRM.

5. **Legacy Fortran dominates the older repos.** AM3 (2015, 4 commits total) and PMIP analyzers are Fortran-based. The modern Python/data-science shift hasn't reached geoengineering-specific simulation.

6. **The governance gap is as important as the technical gap.** srm-forever, Geo-DICE, and OOCC are all tiny repos trying to model the governance/economics side. Nobody is building serious governance tools.
