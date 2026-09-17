# ☀️ Solar Geoengineering — Commit Trend Analysis (September 2026)

## Overview
This document captures the commit history analysis of open-source solar geoengineering and climate simulation projects, pulled from GitHub in September 2026. It covers 8 key repositories across SRM simulation, climate modeling, radiative forcing, and governance tools.

---

## 🔥 Most Active Projects

### 1. wrf-model/WRF — 1,761 ⭐ | Fortran | v4.8.0 Released Jun 2026
**The foundational atmospheric model — and it's in rapid development.**

| Date | Commit | Significance |
|------|--------|-------------|
| Jun 8, 2026 | Merge release-v4.8.0 | Major version release |
| Jun 6, 2026 | Update README and version to v4.8.0 | Documentation sync |
| Jun 5, 2026 | Turn off tempo_aerosolaware and tempo_hailaware | Aerosol physics toggle — **directly relevant to SRM simulation** |
| May 30, 2026 | Fix vectorization option in AOCC stanza | Compiler optimization |
| May 28, 2026 | Correction for eot calculation for solar radiation | **Solar radiation fix — critical for SRM accuracy** |
| May 27, 2026 | Updating MYNN-EDMF pointer, removing icloud_bl | Boundary layer physics |
| May 27, 2026 | Update MMM-physics repo SHA with fixes | Physics suite update |
| May 26, 2026 | Fixing CDXWRF module | Diagnostic tool fix |
| May 26, 2026 | Update readme for GFL option | Documentation |
| May 21, 2026 | Include mp_physics=88 in TEMPO error print | Error handling |

**🎙️ Podcast Angle:** WRF's v4.8.0 release includes a solar radiation correction and aerosol awareness toggles — these are the exact physics modules that SRM researchers depend on. The 15 commits in ~4 weeks show institutional climate software is alive and well. If you're simulating stratospheric aerosol injection, you're running WRF under the hood.

**Key Insight:** The solar radiation correction (commit e836cd6) is the most podcast-relevant commit — it means previous simulations may have had systematic errors in radiative forcing calculations.

---

### 2. NOAA-GFDL/MDTF-diagnostics — 80 ⭐ | Jupyter | Active through Aug 2026
**Process-oriented diagnostics for weather and climate simulations — the ocean-adjacent lifeline.**

| Date | Commit | Significance |
|------|--------|-------------|
| Aug 14, 2026 | Merge PR #825 from weiming9115/main | Institutional review cycle |
| Jun 19, 2026 | 5 commits: MCS_precip_buoyancy_stats.rst updates | **New precipitation-buoyancy statistics POD** |
| Jun 19, 2026 | add MCS precipitation-buoyancy statistics POD | New diagnostic tool |
| Jun 8, 2026 | Merge PR #823 from jongsooshin5/main | Code review merge |
| Jun 8, 2026 | Update README (×2) | Documentation refresh |
| Jun 2, 2026 | Merge branch NOAA-GFDL:main into main | Sync |

**🎙️ Podcast Angle:** MDTF's new precipitation-buoyancy POD is the closest thing to an ocean-intervention diagnostic tool in the GitHub ecosystem. It's designed for climate model evaluation, not geoengineering specifically — but the methodology could be adapted for ocean perturbation monitoring.

---

### 3. ClimateMARGO/ClimateMARGO.jl — 73 ⭐ | Julia | Revival signal Aug 2026
**Idealized climate-economic modeling framework for mitigation/adaptation trade-offs.**

| Date | Commit | Significance |
|------|--------|-------------|
| Aug 17, 2026 | Update README.md (×2) | **Revival after 2.5 years of silence** |
| Oct 18, 2023 | Update unit_conversions.jl with comment from #86 | Community contribution |
| Jul 6, 2023 | Add link to Pluto notebook | Interactive documentation |
| Nov 14, 2022 | Update Project.toml | Dependency management |
| Nov 12, 2022 | JuMP and Ipopt compat upgrade (#85) | Solver compatibility |
| Feb 10, 2022 | Removed deprecated web apps | Cleanup |
| Feb 4, 2022 | Added CITATION.bib | Citation support |

**🎙️ Podcast Angle:** ClimateMARGO went dormant for 2.5 years then suddenly got 2 README updates in August 2026. Is someone coming back to it? The Julia implementation of an integrated assessment model is exactly the kind of tool that could incorporate geoengineering scenarios. The Pluto notebook link suggests interactive exploration — a potential demonstration tool for the podcast.

---

### 4. brandonhimpfen/awesome-geoengineering — 4 ⭐ | Python | Actively curated v2.0.0
**The curated list — healthy ongoing activity, the most sustainable project in our survey.**

| Date | Commit | Significance |
|------|--------|-------------|
| Sep 6, 2026 | Update README.md | Ongoing curation |
| Sep 5, 2026 | Update README.md | Ongoing curation |
| May 5, 2026 | Update to v2.0.0 | Major version release |
| Mar 12, 2026 | Update README.md | Regular maintenance |
| Jan 16, 2026 | Update README.md | Regular maintenance |
| Jun 28, 2025 | Update README.md | Pre-launch activity |
| Jun 28, 2025 | Initial commit | Project creation |

**🎙️ Podcast Angle:** This is the *healthiest* project in terms of activity pattern — 7 commits in 14 months, consistently maintained. A curated list doesn't need complex code, but it shapes who finds what tools. If you're looking for geoengineering open-source projects, this list is the gateway. The v2.0.0 release in May 2026 suggests a major reorganization.

---

## ❄️ Dormant but Relevant Projects

### 5. pixnum-hub/GeoVision — Geoengineering Simulator
| Date | Commit | Significance |
|------|--------|-------------|
| Dec 6, 2025 | Update README.md | Final update |
| Dec 6, 2025 | Create LICENSE | Licensing |
| Dec 6, 2025 | Add files via upload | Initial content |
| Dec 6, 2025 | Initial commit | Project creation |

**All 4 commits on a single day (Dec 6, 2025).** A Geoengineering Simulator with zero subsequent activity. This is a "flash in the pan" — created with enthusiasm but no sustaining community. The HTML language suggests it's a web-based tool. Worth investigating whether the simulator is functional.

---

### 6. jlehtomaa/OOCC_2021 — Solar Geoengineering Governance Model
| Date | Commit | Significance |
|------|--------|-------------|
| Nov 15, 2021 | update bibtex entry | Citation update |
| Oct 26, 2021 | update bibtex reference | Citation update |
| Sep 5, 2021 | update readme (×3) | Documentation |
| Sep 4, 2021 | update citation | Citation work |
| Sep 4, 2021 | added citation file | Citation support |
| Sep 3, 2021 | update readme (×3) | Documentation |

**All activity in Sep-Nov 2021. Dormant for 5 years.** A simple model for solar geoengineering governance — exactly the governance gap we've identified. The project was created for a paper (OCF 2021 conference) and served its purpose, then was abandoned. This is the *typical* lifecycle of geoengineering research code: built for a paper, frozen after publication.

---

### 7. PSLmodels/Geo-DICE — Modified DICE with Geoengineering
| Date | Commit | Significance |
|------|--------|-------------|
| Sep 27, 2018 | Add files via upload | Final update |
| Aug 15, 2016 | Add files via upload (×2) | Content additions |
| Aug 15, 2016 | Initial commit | Project creation |

**Dormant since 2018 — 8 years of silence.** A modified DICE integrated assessment model that includes geoengineering. The original DICE model (Nordhaus) is the most influential climate-economics model ever built. Geo-DICE adds SRM scenarios. But nobody has touched it since 2018 — the codebase is frozen in the DICE2016 era.

---

### 8. antara-banerjee/GeoengineeringLE_WinterWarming — Winter Warming Ensembles
| Date | Commit | Significance |
|------|--------|-------------|
| Apr 24, 2021 | Update README.md | Final update |
| Apr 23, 2021 | updated | Minor fix |
| Apr 16, 2021 | removing netcdf / removed netcdf | File management |
| Apr 14, 2021 | Color handling consistency | Visualization fix |
| Apr 8, 2021 | Renamed ensemble and plotting modules | Code organization |
| Apr 8, 2021 | Cleaning up region selection | Code quality |
| Apr 6, 2021 | Added 95% confidence stippling | Peer review response |
| Apr 6, 2021 | Small change to PC saving | Bug fix |

**All activity in April 2021. Dormant for 5+ years.** This was a well-structured Python project for ensemble analysis of winter warming experiments (a form of SRM). The peer review response (adding confidence stippling) shows this was genuine research code. The removal of netcdf files suggests the author was trying to slim the repo — possibly moving data elsewhere.

---

## 📊 Solar Theme: Cross-Cutting Trend Summary

### Trend 1: Institutional Bursts Dominate
WRF (15 commits in 4 weeks) and MDTF-diagnostics (10 commits in 3 months) are both NOAA-GFDL / NCAR institutional products. They receive regular, funded development. Community-driven SRM simulation tools are the exception.

### Trend 2: Governance Tools are Frozen in Time
Both OOCC_2021 (2021) and Geo-DICE (2018) are dormant. The governance infrastructure for SRM has not advanced in code form. Our podcast should note: physics has outpaced policy infrastructure by a decade.

### Trend 3: The "Curation > Code" Pattern
awesome-geoengineering (actively curated) and ClimateMARGO (revival signal) show that the most sustainable projects are either lists/curation or economic models — not complex simulations. The simulation tools die after the paper; the lists and models get maintained.

### Trend 4: Solar Radiation Physics is Being Fixed
WRF's v4.8.0 includes a correction to solar radiation calculations. This is critical for SRM research because radiative forcing is the core quantity being modeled. If the baseline physics code has errors, years of SRM simulation results may be systematically off.

### Trend 5: Interactive Tools are Emerging
GeoVision (Dec 2025) attempted to build a web-based geoengineering simulator. The effort was commendable but unsustainable. The "democratization" wave of interactive SRM tools is real but still tiny and fragile.

---

## 🎙️ Episode Talking Points — SolarGeoengineering

1. **"The atmosphere model underneath everything"** — WRF v4.8.0 just fixed solar radiation physics and added aerosol toggles. If you're simulating SRM, you're standing on NOAA's shoulders.

2. **"The governance vacuum"** — The only two SRM governance code projects (OOCC_2021, Geo-DICE) are frozen from 2018 and 2021. Nobody is writing governance simulation tools.

3. **"Why simulation code dies"** — GeoVision (4 commits, one day), GeoengineeringLE_WinterWarming (10 commits, one month), Geo-DICE (4 commits, 2 years). The lifecycle of research code: paper → commits → freeze. ClimateMARGO's revival is the exception.

4. **"The curated list outlives the simulation"** — awesome-geoengineering is the most sustainably maintained project. Curation is a different kind of software — it doesn't break, it just needs updating.

5. **"The summer of SRM fixes"** — WRF's May-Jun 2026 commits includes a solar radiation correction and aerosol awareness toggles. The physics is being refined *right now* — what does that mean for past SRM simulation results?

---

*Last updated: September 2026 based on GitHub commit data pulled from 8 repositories.*