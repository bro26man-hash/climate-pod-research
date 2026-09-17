# ☀️ Solar Geoengineering — Project Discoveries

**Research Date:** September 2026  
**Podcast Episode:** Solar Geoengineering — Episode 1

---

## Overview

This document catalogs the open-source solar geoengineering and climate simulation projects discovered through GitHub research, along with commit trend analysis from the most active repositories.

---

## Top Projects by Activity & Relevance

### 1. ClimateMARGO/ClimateMARGO.jl ⭐ 73
- **Language:** Julia
- **Focus:** Idealized climate-economic modelling framework for optimizing trade-offs between emissions mitigation, adaptation, and geoengineering
- **Last Updated:** Aug 17, 2026 (see commit analysis below)
- **Key Feature:** Julia-based optimization framework that models SRM trade-offs
- **Podcast Angle:** The revival of this 2+ year dormant project in Aug 2026 could signal growing policy-modeling interest
- **Commit Insight:** Two README updates on Aug 17, 2026 after no activity since Oct 2023 — potential false start or genuine revival?

### 2. wrf-model/WRF ⭐ 1,761
- **Language:** Fortran
- **Focus:** The Weather Research and Forecasting model — foundational atmospheric simulation
- **Last Updated:** Sep 16, 2026
- **Key Feature:** The de facto standard atmospheric model; v4.8.0 released Jun 2026
- **Podcast Angle:** WRF's aerosol physics module is the simulation pipeline that SRM research depends on. Without WRF, there's no SRM modeling.
- **Commit Insight:** Institutional funding drives release cycles; massive codebase maintained by NCAR/NOAA

### 3. NOAA-GFDL/MDTF-diagnostics ⭐ 80
- **Language:** Jupyter Notebook
- **Focus:** Process-oriented diagnostics for weather and climate simulations
- **Last Updated:** Aug 14, 2026
- **Key Feature:** CMIP6 evaluation toolkit; precipitation-buoyancy POD (Jun 2026) is closest thing to ocean process diagnostics in open source
- **Podcast Angle:** Evaluation infrastructure is the governance backbone — you can't deploy SRM without being able to evaluate its effects

### 4. KOSASIH/GCCS-Core ⭐ 9
- **Language:** Python
- **Focus:** Global Climate Control System — foundational framework for geoenginewithout control algorithms and data pipelines
- **Last Updated:** Oct 29, 2024
- **Key Feature:** Ambitious attempt to build an end-to-end geoengineering control system
- **Podcast Angle:** The "kitchen sink" project — tries to model the entire climate system for geoengineering purposes. 7 README-only commits in a single day suggests a bulk upload rather than careful development.

### 5. eabarnes1010/actm-sai-csu ⭐ 6
- **Language:** Python
- **Focus:** AI to detect, attribute, and quantify solar radiation management (SRM) effects and risks under geopolitical scenarios. Funded by DARPA.
- **Last Updated:** Mar 28, 2023
- **Key Feature:** Machine learning for SRM attribution — critical for governance (who deployed SRM? what are the effects?)
- **Commit Insight:** All commits are paper-related (4 preprint/paper updates, Jan–Mar 2023). The code is paper-supplementary, not a standalone tool.

### 6. pixnum-hub/GeoVision
- **Language:** HTML
- **Focus:** Geoengineering Simulator — interactive web-based visualization
- **Last Updated:** Dec 6, 2025
- **Podcast Angle:** The closest thing to an "interactive SRM simulator" that a layperson could use. Democratization tool.

---

## The Solar Geoengineering Field on GitHub: Key Patterns

### Pattern 1: Scarcity of SRM-Specific Code
Despite geoengineering being a major research topic, **there are very few dedicated SRM simulation repositories on GitHub.** Most climate simulation happens in generalized models (WRF, CESM) that can be configured for SRM experiments, but no one has built a clean, open-source SRM-specific simulator.

### Pattern 2: Institutional Dominance
Every highly active repo is institutionally funded (NCAR, NOAA, DARPA). Community-driven SRM projects are rare and small.

### Pattern 3: The Governance Gap
Projects like `actm-sai-csu` (DARPA-funded attribution AI) and `jlehtomaa/OOCC_2021` (governance model) suggest the community is thinking about governance, but the tools are lagging behind the physics.

### Pattern 4: Revival Signals
ClimateMARGO's Aug 2026 updates after 2+ years dormant may indicate renewed interest in climate-economic modeling for geoengineering policy.

---

## Commit Trend Analysis: Solar Geoengineering Repos

| Repository | Stars | Last Commit | Commit Span | Activity Level |
|------------|-------|-------------|-------------|----------------|
| ClimateMARGO.jl | 73 | Aug 17, 2026 | Jan 2022–Aug 2026 | ★★☆☆☆ (revival burst) |
| wrf-model/WRF | 1,761 | Sep 16, 2026 | Continuous | ★★★★★ (institutional) |
| MDTF-diagnostics | 80 | Aug 14, 2026 | Jun–Aug 2026 | ★★★☆☆ (release-driven) |
| GCCS-Core | 9 | Oct 29, 2024 | Single-day burst | ★☆☆☆☆ (bulk upload) |
| actm-sai-csu | 6 | Mar 28, 2023 | Jan–Mar 2023 | ★★☆☆☆ (paper-driven) |

---

## Detailed Commit Histories

### ClimateMARGO.jl — Recent Commits
| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| Aug 17, 2026 | `d916f36` | Fons van der Plas | Update README.md |
| Aug 17, 2026 | `6d9ba7a` | Fons van der Plas | Update README.md |
| Oct 18, 2023 | `57d4da7` | Fons van der Plas | Unit conversions update (issue #86) |
| Jul 6, 2023 | `fbb619` | Fons van der Plas | Added Pluto notebook link |
| Nov 14, 2022 | `5063c42` | Fons van der Plas | Updated Project.toml |
| Nov 12, 2022 | `12a0ce6` | Fons van der Plas | JuMP/Ipopt compat upgrade (#85) |
| Feb 10, 2022 | `32e66fd` | Henri Drake | Removed deprecated web apps |
| Feb 4, 2022 | `d609d49` | Henri Drake | Added CITATION.bib |
| Jan 13, 2022 | `b2d9228` | Henri Drake | Fixed typo |
| Jan 12, 2022 | `8a7e012` | Henri Drake | Updated doc deployment args |

**Trend:** Two distinct developer eras (Henri Drake → Fons van der Plas). 2+ year gap between 2023 and 2026 activity. The 2026 README-only updates are unexplained — could be a revival or just maintenance.

### GCCS-Core — Recent Commits (All Oct 29, 2024)
| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| Oct 29, 2024 | `99bf84f` | KOSASIH | Update README.md |
| Oct 29, 2024 | `7cad777` | KOSASIH | Update README.md |
| Oct 29, 2024 | `4350445` | KOSASIH | Update README.md |
| Oct 29, 2024 | `b6e44cc` | KOSASIH | Update README.md |
| Oct 29, 2024 | `cfaa741` | KOSASIH | Update README.md |
| Oct 29, 2024 | `bef35ee` | KOSASIH | Update README.md |
| Oct 29, 2024 | `cc92644` | KOSASIH | Update README.md |
| Oct 29, 2024 | `fc3553b` | KOSASIH | Create requirements.txt |
| Oct 29, 2024 | `f6da191` | KOSASIH | Create setup.py |
| Oct 29, 2024 | `4a068bc` | KOSASIH | Create data_collection.sh |

**Trend:** 7 README commits + 3 infrastructure commits all on a single day. This is a bulk upload pattern, not organic development. The project has infrastructure scaffolding but no visible modeling code commits.

### actm-sai-csu — Recent Commits
| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| Mar 28, 2023 | `b25f0a8` | Zachary Labe | New paper |
| Mar 28, 2023 | `e4e4d57` | Zachary Labe | New paper! |
| Feb 9, 2023 | `203c4ed` | Daniel Hueholt | Add preprint link to README |
| Feb 8, 2023 | `6b3fdc2` | Daniel Hueholt | Add Jim's link |
| Feb 8, 2023 | `163f927` | Daniel Hueholt | Standardize capitalization |
| Feb 8, 2023 | `7038625` | Daniel Hueholt | Add code from Hueholt et al. 2023 |
| Jan 22, 2023 | `a155ce9` | Antonios Mamalakis | Update README |
| Jan 22, 2023 | `16ff5c5` | Antonios Mamalakis | Create README |
| Jan 11, 2023 | `45e47b7` | Zachary Labe | New preprint |
| Jan 11, 2023 | `28314c9` | Zachary Labe | New preprint |

**Trend:** Purely paper-driven repository. All commits map to publication events. No standalone tool development. Joins the growing body of research that SRM attribution is an active DARPA-funded area.

---

## 🎙️ Podcast Episode Notes: Solar Geoengineering

### Key Questions for the Episode
1. Why is dedicated SRM simulation code so scarce compared to the volume of SRM research papers?
2. Can interactive models like GeoVision democratize the SRM discourse, or do they oversimplify?
3. Is ClimateMARGO's 2026 revival a signal of growing policy-modeling interest?
4. WRF's aerosol physics as the SRM simulation pipeline — what does it take to configure WRF for SRM experiments?
5. The governance gap: DARPA is funding SRM attribution AI (actm-sai-csu). What does militarized SRM monitoring mean for climate governance?
6. Arctic risks: How do SRM models handle polar amplification?

### Sources
- https://github.com/ClimateMARGO/ClimateMARGO.jl
- https://github.com/wrf-model/WRF
- https://github.com/NOAA-GFDL/MDTF-diagnostics
- https://github.com/KOSASIH/GCCS-Core
- https://github.com/eabarnes1010/actm-sai-csu
- https://github.com/pixnum-hub/GeoVision
- https://github.com/jlehtomaa/OOCC_2021