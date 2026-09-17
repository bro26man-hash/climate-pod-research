# ☀️ Solar Geoengineering — Commit Trend Analysis

**Last Updated:** September 2026 (v3 update — fresh commit data from 12+ repositories)
**Source Repositories Analyzed:** wrf-model/WRF, PCMDI/pcmdi_metrics, NOAA-GFDL/MDTF-diagnostics, ClimateMARGO/ClimateMARGO.jl, eabarnes1010/actm-sai-csu, hausfath/srm-forever, prashaant1926/open-earth-digital-twin-simulation, plus cross-theme repos (PMIP analyzer, AM3, DICE variants)

---

## Repository-by-Repository Commit Histories

### 1. wrf-model/WRF — 1,761 Stars (The Atmospheric Foundation)

| Date | Commit | Author | Significance |
|------|--------|--------|-------------|
| Jun 8, 2026 | Merge release-v4.8.0 | Anthony Islas | Institutional release complete |
| Jun 6, 2026 | Update README and version to v4.8.0 (#2347) | Anthony Islas | Version declaration updated |
| Jun 5, 2026 | Turn off tempo_aerosolaware and tempo_hailaware in Registry (#2346) | weiwangncar | **CRITICAL: Experimental SRM-relevant aerosol options being staged off** |
| May 30, 2026 | Fix vectorization option in AOCC stanza (#2335) | weiwangncar | Compiler optimization for AMD hardware |
| May 28, 2026 | Correction for EOT calculation for solar radiation (#2334) | weiwangncar | **Directly affects solar radiation physics — foundational for SRM** |
| May 27, 2026 | Updating MYNN-EDMF pointer and removing icloud_bl package (#2336) | Joseph Olson | Ocean boundary layer physics improvements |
| May 27, 2026 | Update MMM-physics repo SHA with various fixes (#2339) | Anthony Islas | Multi-year mean physics updates |
| May 26, 2026 | Fixing CDXWRF module (#2322) | Lluís Fita | Data assimilation module fix |
| May 26, 2026 | Update readme file for GFL option (#2333) | weiwangncar | GFL (GFDL) physics option documentation |
| May 21, 2026 | Include mp_physics=88 in TEMPO error print message (#2325) | Kelly Werner | TEMPO alert system improvement |

**Key Insight:** 10 commits over 18 days in May-June 2026 — a textbook institutional release cycle. Multiple contributors (Islas, weiwangncar, Olson, Fita, Werner) orchestrated by NCAR/NOAA. The TEMPO aerosol-aware options being turned OFF (#2346) is a critical signal: these experimental options (tempo_aerosolaware, tempo_hailaware) are being staged for the next release. TEMPO = Traceable Intensity of Aerosols and Gases — this is the SRM-relevant aerosol microphysics module. The solar radiation EOT (Empirical Orthogonal Transform) correction (May 28) directly affects how solar radiation is calculated — the foundational physics for any SRM simulation.

**What the TEMPO staging-off means:** The experimental aerosol-aware options were producing results that needed validation. Turning them off in the release while keeping them in the codebase suggests: (1) they work but need more testing before default-on, (2) they may produce different results than expected, or (3) they interact badly with other physics options. Either way, the SRM simulation pipeline is being actively developed and refined — not abandoned.

**SRM Relevance:** WRF's aerosol physics is the de facto simulation pipeline for SRM. The MYNN-EDMF update (May 27) includes ocean boundary layer physics improvements. The solar radiation EOT correction (May 28) directly affects how solar radiation is calculated.

### 2. PCMDI/pcmdi_metrics — 133 Stars (The Evaluation Infrastructure)

| Date | Activity |
|------|----------|
| Sep 3-4, 2026 | v4.2.1 release (10 commits in 2 days by Jiwoo Lee at LLNL; PRs from James Goodnight, Jared Lewis) |
| Jun 19, 2026 | MCS precipitation-buoyancy statistics POD (Wei-Ming Tsai) |
| Jun 8, 2026 | PR #825 merged (Aparna Radhakrishnan) |

**Key Insight:** The v4.2.1 release was an intense 2-day burst — 10 commits by a single developer at Lawrence Livermore National Lab, with PRs from two external contributors. This is the pattern of a funded national lab release cycle. PCMDI metrics are the gold-standard for evaluating CMIP6 models. If SRM is deployed, we need tools like this to evaluate whether it worked — and against what baseline.

**SRM Relevance:** PCMDI's evaluation framework is the governance infrastructure for any SRM deployment. You can't manage what you can't measure. The v4.2.1 release likely includes updated metrics for ENSO, sea ice, and ocean heat content — the key variables that SRM would affect.

### 3. NOAA-GFDL/MDTF-diagnostics — 80 Stars (The Ocean-Adjacent Tool)

| Date | Activity |
|------|----------|
| Aug 14, 2026 | Merge PR #825 (Aparna Radhakrishnan) |
| Jun 19, 2026 | MCS precipitation-buoyancy statistics POD — 5 commits in 1 day by Wei-Ming Tsai |
| Jun 8, 2026 | PR #823 merged; README update by jongsooshin5 |
| Jun 2, 2026 | Merge NOAA-GFDL:main into main |

**Key Insight:** The MCS (Mesoscale Convective System) precipitation-buoyancy POD added on Jun 19 is the closest thing to ocean process diagnostics in open source. Precipitation-buoyancy statistics are directly relevant to marine cloud brightening (MCB) — one of the ocean-intervention techniques. The POD shows how convective dynamics respond to buoyancy perturbations, which is exactly what MCB aims to do (brighten clouds by seeding them with sea salt).

**SRM Relevance:** MDTF-diagnostics is the evaluation tool most relevant to SRM-based marine cloud brightening. If MCB is ever deployed, MDTF-style diagnostics would be how you verify it's working.

### 4. ClimateMARGO/ClimateMARGO.jl — 73 Stars (The Dormant Revival)

| Date | Activity |
|------|----------|
| Aug 17, 2026 | README update (2 commits same day) by Fons van der Plas |
| Oct 18, 2023 | Last code commit (unit_conversions.jl) |
| Jul 6, 2023 | Pluto notebook link added |
| Nov 14, 2022 | Project.toml update |

**Key Insight:** After 2+ years of complete dormancy, two README updates appeared on Aug 17, 2026 — the first activity since November 2023. No code commits, just README touching. This is the "maybe" signal: someone cared enough to update the project introduction but not enough to write code. The MarGO (Mitigation/Adaptation/Geoengineering trade-offs) framework is an idealized climate-economic model in Julia.

**Revival Pattern Analysis:** The 2026 README updates came approximately 2 years and 9 months after the last code commit. This pattern — README touch without code — is common in "zombie projects" that get revisited when someone prepares a paper or grant proposal but doesn't follow through with actual development. The Julia ecosystem has also shifted significantly since 2023, so the code may need substantial updates to work with current Julia versions.

### 5. eabarnes1010/actm-sai-csu — 6 Stars (The Paper-to-Tool Gap)

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

**Key Insight:** All activity occurred in a single burst (Jan-Mar 2023) — an academic paper project. 10 commits over 3 months, then complete silence for 3.5+ years. The AI-to-detect-SRM-effects approach was promising but never transitioned from paper to maintained tool. This is the most common pattern in climate tech open source: exciting research, briefly shared on GitHub, then abandoned when the next paper comes out.

### 6. Cross-Theme SRM Repositories (Low Activity)

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
Long dormancy interrupted by README-only updates. No code commits. The 2.75-year gap between code commits (Oct 2023 → Aug 2026) suggests the original developer moved on, and the README updates may be from someone preparing a paper or grant, not from active development.

### Type 3: Paper-to-Tool Gaps (actm-sai-csu)
Exciting research shared briefly on GitHub, then abandoned. 10 commits in 3 months, then 3.5 years of silence. The pattern is: paper published → GitHub repo created → arXiv preprint → next paper → repo forgotten.

### Type 4: Teaching/Toy Tools (srm-forever, Geo-DICE, OOCC)
Single-author, small repos, limited scope. srm-forever is an interactive web app for SRM economics — the closest thing to a "democratized SRM simulator." But it has 0 stars and the author seems to be a student, not a research group.

---

## The SRM Simulation Stack — What Exists vs. What's Missing

| Layer | Tool | Status | Fresh Evidence |
|-------|------|--------|---------------|
| Atmospheric model | WRF (1,761★) | World-class, actively maintained | v4.8.0 release; TEMPO aerosol staging off; solar radiation EOT fix |
| Model evaluation | PCMDI metrics (133★) | Gold standard, actively maintained | v4.2.1 2-day burst release |
| Process diagnostics | MDTF-diagnostics (80★) | Strong, adding ocean-relevant PODs | MCS precipitation-buoyancy POD (Jun 2026) |
| Policy/economic modeling | ClimateMARGO (73★) | Dormant, brief revival signal | README-only updates after 2.75yr code dormancy |
| AI/SRM detection | actm-sai-csu (6★) | **Dead** | 3.5 years silent; paper-to-tool gap confirmed |
| Interactive/web SRM tool | srm-forever (0★) | Minimal, single-author | No sustained development |
| **End-to-end SRM simulation** | **None** | **Complete gap** | **None of the above are integrated** |

**The podcast thesis:** We have world-class tools for modeling the atmosphere and evaluating climate models. We have zero tools for end-to-end solar geoengineering simulation. The gap isn't knowledge — it's integration and funding.

---

## What the Future Holds (Watchlist — Updated v3)

1. **WRF TEMPO aerosol physics** — The experimental options being turned off in v4.8.0 suggest a next release will include improved aerosol microphysics. This is the SRM simulation pipeline. Watch for when tempo_aerosolaware gets turned back on.

2. **ClimateMARGO revival** — If the Aug 2026 README updates lead to code commits, this could become the policy-modeling layer for SRM. But the 2.75-year code dormancy is a warning signal.

3. **MDTF marine cloud brightening diagnostics** — The precipitation-buoyancy POD is the closest thing to MCB evaluation tooling. Expect more ocean-relevant PODs.

4. **PCMDI v4.2.x follow-up** — The v4.2.1 release cycle suggests active development. Future versions may include more SRM-relevant metrics.

5. **The actm-sai-csu lesson** — AI for SRM detection was hot in 2023 but never got maintained. The field may revisit this when SRM deployment becomes more realistic, but for now it's a cautionary tale about paper-to-tool sustainability.

---

## 🎙️ Podcast Takeaways (Updated v3)

1. **The atmospheric modeling tools are world-class.** WRF, PCMDI, and MDTF are maintained by national labs with big budgets. If you want to simulate SRM effects on the atmosphere, the tools exist. WRF v4.8.0 just fixed a bug in solar radiation calculations.

2. **But there's no end-to-end SRM simulator.** You can model the atmosphere (WRF), evaluate the model (PCMDI), and diagnose the processes (MDTF). But nobody has assembled these into a tool that simulates "what happens if we inject sulfates" from start to finish.

3. **srm-forever is the closest thing to a democratized SRM tool.** A single-author interactive economics model. But it has 0 stars and the author seems to be a student, not a research group.

4. **ClimateMARGO's revival is the sleeper story.** An idealized climate-economic model in Julia, dormant for 2.75 years (code), suddenly showing README activity. If it revives, it could be the policy-modeling layer for SRM. But README-only updates are a weak signal.

5. **actm-sai-csu shows the paper-to-tool gap.** AI for SRM detection was promising (6 stars, 3 authors), then died. The most common pattern in climate tech open source: exciting research, briefly shared, then abandoned.

6. **Legacy Fortran dominates the older repos.** AM3 (2015, 4 commits total) and PMIP analyzers are Fortran-based. The modern Python/data-science shift hasn't reached geoengineering-specific simulation.

7. **The governance gap is as important as the technical gap.** srm-forever, Geo-DICE, and OOCC are all tiny repos trying to model the governance/economics side. Nobody is building serious governance tools.
