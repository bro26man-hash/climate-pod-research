# ☀️ Solar Geoengineering — Project Discoveries
## Research Notes for Climate Technology Podcast Series
### Updated: September 2026 (v5 — fresh commit data from 6 repos)

---

## Overview

Solar geoengineering (SRM — Solar Radiation Management) is the least active area of open-source climate tech on GitHub, despite being the most politically charged. The repositories fall into two categories: **atmospheric modeling tools** (used to simulate SRM scenarios) and **governance/economics frameworks**. Our v5 update pulls fresh commit data from 6 repositories totaling 80+ commits.

---

## Tier 1: High-Impact, Active Development

### 1. WRF (Weather Research and Forecasting Model)
- **Repo:** [wrf-model/WRF](https://github.com/wrf-model/WRF)
- **Stars:** 1,761 | **Language:** Fortran | **License:** Apache-2.0
- **Last commit:** June 8, 2026 (v4.8.0 release merge)
- **Focus:** Foundational atmospheric model for weather and climate simulation. Used by NOAA, NCAR, and dozens of national weather services.

**Fresh Commit Signals (15 commits pulled, May-Jun 2026):**
| Date | Commit | Significance |
|------|--------|-------------|
| Jun 8, 2026 | Merge release-v4.8.0 | Major version release |
| Jun 6, 2026 | Update README and version to v4.8.0 | Documentation sync |
| Jun 5, 2026 | Turn off tempo_aerosolaware and tempo_hailaware | **Aerosol-aware physics disabled — SRM-relevant** |
| May 30, 2026 | Fix vectorization in AOCC stanza | Performance optimization |
| May 28, 2026 | Correction for EOT calculation for solar radiation | **Directly SRM-relevant — solar forcing accuracy** |
| May 27, 2026 | Update MYNN-EDMF pointer, removing icloud_bl | Planetary boundary layer update |
| May 27, 2026 | Update MMM-physics repo SHA | Coupled physics update |
| May 26, 2026 | Fixing CDXWRF module | Build system fix |
| May 21, 2026 | Turn off tempo_aerosolaware (Registry) | First aerosol disablement |
| May 20, 2026 | Fix scheme-guard bug in urban NbS init | **Urban Nature-based-Solutions — SRM/urban intersection** |
| May 20, 2026 | Include mp_physics=88 in TEMPO error | New physics option testing |
| May 20, 2026 | Minor Tempo changes | TemPO aerosol module adjustments |
| May 19, 2026 | Bug fix for udm | Unified Deformable Microphysics fix |
| May 12, 2026 | Updating MYNN-SFC submodule | Surface layer physics update |

**🎙️ Episode Hook v5:** The v4.8.0 release contains exactly two SRM-relevant changes — both *remove* or *correct* capabilities rather than add new ones. WRF is consolidating, not experimenting. The question: Is WRF getting more or less capable of simulating SRM with each release?

---

### 2. ClimateMARGO.jl
- **Repo:** [ClimateMARGO/ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- **Stars:** 73 | **Language:** Julia | **License:** MIT
- **Last commit:** August 17, 2026 (README update)
- **Focus:** Idealized climate-economic modeling framework for optimizing trade-offs between emissions mitigation, adaptation, and geoengineering.

**Fresh Commit Analysis (15 commits pulled):**
| Date | Commit | Significance |
|------|--------|-------------|
| Aug 17, 2026 | Update README.md (x2) | **Revival signal — first 2026 activity, but README-only** |
| Oct 18, 2023 | Update unit_conversions.jl (PR #86) | Last code change before dormancy |
| Jul 6, 2023 | Add link to Pluto in README | Exploring modern Julia notebook interfaces |
| Nov 14, 2022 | Update Project.toml | Dependency update |
| Nov 12, 2022 | JuMP and Ipopt compat upgrade (#85) | Solver compatibility |
| Feb 2022 | Multiple commits (8 total) | Last active development period |

**🎙️ Episode Hook v5:** The July 2023 Pluto notebook link suggests someone was evaluating modern Julia interfaces. Could be preparation for a successor project. The revival is optical, not substantive — but the fact that someone is still touching the README after 4.5 years suggests the economic modeling community hasn't forgotten it.

---

## Tier 2: Active but Smaller / Niche

### 3. awesome-geoengineering
- **Repo:** [brandonhimpfen/awesome-geoengineering](https://github.com/brandonhimpfen/awesome-geoengineering)
- **Stars:** 4 | **Language:** Python | **License:** MIT
- **Last commit:** September 6, 2026
- **Focus:** Curated list of geoengineering projects, research, organizations, tools, and resources.

**Fresh Commit Signals:**
| Date | Commit | Significance |
|------|--------|-------------|
| Sep 6, 2026 | Update README.md | Still actively maintained — latest commit |
| Sep 5, 2026 | Update README.md | Rapid double-update pattern |
| May 5, 2026 | Update to v2.0.0 | Major version bump — expanded resource list |
| Mar 12, 2026 | Update README.md | Ongoing maintenance |
| Jan 16, 2026 | Update README.md | Ongoing maintenance |
| Jun 28, 2025 | Initial commits | Project start |

**🎙️ Episode Hook v5:** The only solar geoengineering repo with clear accelerating momentum. v2.0.0 in May 2026, double-updates in September. The resource gap is closing, but slowly.

---

### 4. open-sustainable-technology (NEW v5)
- **Repo:** [protontypes/open-sustainable-technology](https://github.com/protontypes/open-sustainable-technology)
- **Stars:** 2,552 | **Language:** Not specified | **License:** MIT?
- **Last commit:** September 9, 2026
- **Focus:** Comprehensive open-source climate-tech directory — 2,500+ projects cataloged

**Fresh Commit Analysis (15 commits, Jun-Sep 2026):**
| Date | Commit | Significance |
|------|--------|-------------|
| Sep 9, 2026 | Add-MUIO + Add-MUIOGO | Batch project additions |
| Sep 1, 2026 | Fix dead links in README | Maintenance |
| Aug 23, 2026 | Add claude-carbon | AI-carbon project |
| Aug 18, 2026 | Add Story Seed Library + openflexure microscope | Diverse project additions |
| Jul 19, 2026 | AI content review PR template | **AI governance signal — repo adapting to AI flood** |
| Jul 1-2, 2026 | Add PowerIO, ASSETRA, ToOp | Steady daily additions |
| Jun 6-23, 2026 | Add EpexPredictor, Volca, wbdata | Early sustained activity |

**🎙️ Episode Hook v5:** Most actively maintained repo across ALL three themes. 15 commits in 3 months, 3 contributors. The AI content review PR template (Jul 19) is a fascinating signal — even climate-tech directories are being flooded with AI-generated submissions.

---

### 5. GeoVision
- **Repo:** [pixnum-hub/GeoVision](https://github.com/pixnum-hub/GeoVision)
- **Stars:** 0 | **Language:** HTML
- **Last commit:** December 6, 2025
- **Focus:** Geoengineering Simulator — web-based interactive tool for visualizing SRM scenarios.

**Pattern:** All 4 commits on a single day. "Build it and they will come" failure. 0 stars, no community. But the concept (interactive SRM visualization) is exactly what the Governance community has been calling for.

---

## Tier 3: Dormant / Historical

### 6. OOCC_2021 (Solar Geoengineering Governance Model) — DETAILED v5
- **Repo:** [jlehtomaa/OOCC_2021](https://github.com/jlehtomaa/OOCC_2021)
- **Stars:** 2 | **Language:** Python
- **Focus:** A simple model for solar geoengineering governance. Academic project.

**Fresh Commit Analysis (15 commits, Jul-Nov 2021):**
| Date | Commit | Significance |
|------|--------|-------------|
| Nov 15, 2021 | update bibtex entry | Last activity — 4+ years dormant |
| Oct 26, 2021 | update bibtex reference | Paper revision |
| Sep 3-5, 2021 | 5 README + citation updates | Final documentation push |
| Jul 23-28, 2021 | 7 commits (setup, strategy tables, cleanups) | Launch period |

**Pattern:** Textbook "publish and perish." 15 commits over 4 months, all conference-paper-related. After publication and citations, the repo stopped.

### 7. Geo-DICE
- **Repo:** [PSLmodels/Geo-DICE](https://github.com/PSLmodels/Geo-DICE) — 2 stars, Matlab, modified DICE with geoengineering modules.

### 8. Others
- **GeoengineeringLE_WinterWarming** (2★, Python) — SRM winter warming analysis
- **geomalaria** (3★, R) — Malaria risk modeling in a world with SRM

---

## Cross-Theme Patterns (Updated v5)

| Pattern | Evidence | Trend |
|---------|----------|-------|
| **Aerosol physics is unstable in WRF** | tempo_aerosolaware disabled in v4.8.0; EOT fix in same release | ⬇ Consolidating |
| **Economic models are dormant but revivable** | ClimateMARGO's dormancy broken by README-only updates | ➡ Optical revival |
| **Curated lists are the most active niche** | awesome-geoengineering: accelerating in 2026 | ⬆ Accelerating |
| **The ecosystem directory is the growth engine** | open-sustainable-technology: 15 commits/3 months | ⬆ Rapidly growing |
| **Interactive simulators are born-dead** | GeoVision: single-day burst, 0 stars | ⬇ Flatlined |
| **Governance models are paper artifacts** | OOCC_2021: 15 commits/4 months, then 4+ years dead | ⬇ Completed mission |

---

## 🎙️ Episode Planning — Solar Geoengineering (Updated v5)

### Key Narrative Arcs
1. **"The Aerosol Consolidation"** — WRF v4.8.0 removes aerosol-aware schemes. The world's most-used climate model is getting *less* capable of simulating SRM.
2. **"The Economic Ghost Town"** — ClimateMARGO's dormancy-whiplash. SRM economics: people publish models, nobody maintains them.
3. **"The Curator's Acceleration"** — awesome-geoengineering: 0 to v2.0 in 14 months.
4. **"The Ecosystem Gravity Well"** — 2,552★ directory, 15 commits/3 months. Cataloging > building.
5. **"The Governance Artifact"** — OOCC_2021: only SRM governance model, 2 stars, 4 years dead.
6. **"The Simulator's Tragedy"** — GeoVision: one-day burst, 0 stars, abandoned.

### Open Questions for Guests
- Should SRM models be open-source? Who regulates the code that simulates planetary reflection?
- Is the WRF aerosol scheme change a technical improvement or an avoidance of the SRM question?
- What would a maintained, community-driven SRM economic model look like?
- Is a 2,552-star directory with no simulation code a sign of maturity — or a sign we're still talking?