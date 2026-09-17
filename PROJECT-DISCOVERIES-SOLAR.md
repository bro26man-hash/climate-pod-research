# ☀️ Solar Geoengineering — Project Discoveries
## Research Notes for Climate Technology Podcast Series
### Updated: September 2026 (v4 — fresh commit data)

---

## Overview

Solar geoengineering (SRM — Solar Radiation Management) is the least active area of open-source climate tech on GitHub, despite being the most politically charged. The repositories we found fall into two categories: **atmospheric modeling tools** (used to simulate SRM scenarios) and **governance/economics frameworks** (used to model the policy and cost dimensions).

---

## Tier 1: High-Impact, Active Development

### 1. WRF (Weather Research and Forecasting Model)
- **Repo:** [wrf-model/WRF](https://github.com/wrf-model/WRF)
- **Stars:** 1,761 | **Language:** Fortran | **License:** Apache-2.0
- **Last commit:** June 8, 2026 (v4.8.0 release merge)
- **Focus:** The foundational atmospheric model for weather and climate simulation. Used globally by NOAA, NCAR, and dozens of national weather services.

**Recent Commit Signals (8 commits pulled):**
| Date | Commit | Significance |
|------|--------|-------------|
| Jun 8, 2026 | Merge release-v4.8.0 | Major version release — ongoing institutional maintenance |
| Jun 6, 2026 | Update README and version to v4.8.0 | Documentation synchronization |
| Jun 5, 2026 | Turn off tempo_aerosolaware and tempo_hailaware | **Aerosol-aware physics modules being disabled — could relate to SRM aerosol injection uncertainty** |
| May 30, 2026 | Fix vectorization option in AOCC stanza | Performance optimization for AMD processors |
| May 28, 2026 | Correction for EOT calculation for solar radiation | **Directly relevant — solar radiation scheme fix improves accuracy of solar forcing simulations** |
| May 27, 2026 | Update MYNN-EDMF pointer, remove icloud_bl package | Planetary boundary layer physics update |
| May 27, 2026 | Update MMM-physics repo SHA | Coupled physics package update |
| May 26, 2026 | Fixing CDXWRF module | Build system fix |

**🎙️ Episode Hook:** The disabling of aerosol-aware schemes (tempo_aerosolaware) in WRF v4.8.0 is a double-edged sword. It may reflect improvements in how aerosol effects are handled elsewhere, or it may signal that aerosol-Radiation interactions are still not well-resolved. Either way, it's a core SRM-relevant physics question happening inside the world's most-used climate model.

---

### 2. ClimateMARGO.jl
- **Repo:** [ClimateMARGO/ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- **Stars:** 73 | **Language:** Julia | **License:** MIT
- **Last commit:** August 17, 2026 (README update)
- **Focus:** Idealized climate-economic modeling framework for optimizing trade-offs between emissions mitigation, adaptation, and geoengineering.

**Recent Commit Signals (8 commits pulled):**
| Date | Commit | Significance |
|------|--------|-------------|
| Aug 17, 2026 | Update README.md (x2) | **Revival signal — first activity since Oct 2023** |
| Oct 18, 2023 | Update unit_conversions.jl with comment from #86 | Last code change before dormancy |
| Jul 6, 2023 | Add link to Pluto in README | Documentation improvement |
| Nov 14, 2022 | Update Project.toml | Dependency update |
| Nov 12, 2022 | JuMP and Ipopt compat upgrade (#85) | Solver compatibility update |
| Feb 10, 2022 | Removed deprecated web apps | Cleanup |
| Feb 4, 2022 | Added CITATION.bib | Citation infrastructure |

**🎙️ Episode Hook:** ClimateMARGO's two README updates in August 2026 after 2+ years of dormancy are ambiguous. No code commits — just documentation. Is someone preparing for a new release, or is this a housekeeping update? The Julia ecosystem for climate-economics is small but growing; this is the best tool for modeling "what's the optimal SRM deployment strategy given economic constraints?"

---

## Tier 2: Active but Smaller / Niche

### 3. awesome-geoengineering
- **Repo:** [brandonhimpfen/awesome-geoengineering](https://github.com/brandonhimpfen/awesome-geoengineering)
- **Stars:** 4 | **Language:** Python | **License:** MIT
- **Last commit:** September 6, 2026
- **Focus:** Curated list of geoengineering projects, research, organizations, tools, and resources. The best starting point for researchers entering the field.

**Recent Commit Signals (7 commits pulled):**
| Date | Commit | Significance |
|------|--------|-------------|
| Sep 6, 2026 | Update README.md | **Still actively maintained — latest commit** |
| Sep 5, 2026 | Update README.md | Rapid double-update pattern |
| May 5, 2026 | Update to v2.0.0 | Major version bump — expanded resource list |
| Mar 12, 2026 | Update README.md | Ongoing maintenance |
| Jan 16, 2026 | Update README.md | Ongoing maintenance |
| Jun 28, 2025 | Update README.md | Initial maintenance phase |
| Jun 28, 2025 | Initial commit | Project start |

**🎙️ Episode Hook:** In just over a year, this tiny repo has gone from initial commit to v2.0.0 with 7 updates. The pace accelerated dramatically in 2026. This tells us the geoengineering discourse is accelerating — more tools, more papers, more organizations to track. It's the best bibliography for our episode.

---

### 4. GeoVision
- **Repo:** [pixnum-hub/GeoVision](https://github.com/pixnum-hub/GeoVision)
- **Stars:** 0 | **Language:** HTML | **License:** Not specified
- **Last commit:** December 6, 2025
- **Focus:** Geoengineering Simulator. A web-based interactive tool for visualizing geoengineering scenarios.

**Recent Commit Signals (4 commits pulled):**
| Date | Commit | Significance |
|------|--------|-------------|
| Dec 6, 2025 | Update README.md | Post-creation documentation |
| Dec 6, 2025 | Create LICENSE | License addition |
| Dec 6, 2025 | Add files via upload | Initial content upload |
| Dec 6, 2025 | Initial commit | Single-day project creation |

**🎙️ Episode Hook:** All 4 commits happened on a single day. This is a "burst then silence" pattern — someone built a simulator, pushed it, and then stopped. The 0-star count confirms it never found a community. But the concept (interactive SRM visualization) is exactly what the Governance community has been calling for. Is there an opportunity here?

---

## Tier 3: Dormant / Historical

### 5. Geo-DICE (Modified DICE with Geoengineering)
- **Repo:** [PSLmodels/Geo-DICE](https://github.com/PSLmodels/Geo-DICE)
- **Stars:** 2 | **Language:** Matlab | **License:** Not specified
- **Focus:** Modified DICE integrated assessment model with geoengineering modules. Based on the Weitzman/DICE framework.

### 6. OOCC_2021 (Solar Geoengineering Governance Model)
- **Repo:** [jlehtomaa/OOCC_2021](https://github.com/jlehtomaa/OOCC_2021)
- **Stars:** 2 | **Language:** Python | **License:** Not specified
- **Focus:** A simple model for solar geoengineering governance. Academic project.

### 7. GeoengineeringLE_WinterWarming
- **Repo:** [antara-banerjee/GeoengineeringLE_WinterWarming](https://github.com/antara-banerjee/GeoengineeringLE_WinterWarming)
- **Stars:** 2 | **Language:** Python | **License:** Not specified
- **Focus:** Solar geoengineering winter warming analysis. Very niche academic project.

### 8. cjcarlson/geomalaria
- **Repo:** [cjcarlson/geomalaria](https://github.com/cjcarlson/geomalaria)
- **Stars:** 3 | **Language:** R | **License:** Not specified
- **Focus:** Malaria risk modeling in a world with solar geoengineering. Cross-impact assessment (SRM -> climate -> disease).

---

## Cross-Theme Patterns

| Pattern | Evidence |
|---------|----------|
| **Aerosol physics is unstable in WRF** | tempo_aerosolaware disabled in v4.8.0; solar radiation EOT fix in same release |
| **Economic models are dormant but revivable** | ClimateMARGO's 2-year dormancy broken by README-only updates |
| **Curated lists are the most active niche** | awesome-geoengineering: 7 commits in 14 months, accelerating in 2026 |
| **Interactive simulators are born-dead** | GeoVision: single-day burst, 0 stars, no community |
| **Star count != Impact** | WRF (1,761) shapes policy; GeoVision (0) doesn't; ClimateMARGO (73) is the best economic SRM tool |

---

## Episode Notes — Solar Geoengineering Branch

### Key Narrative Arcs
1. **"The Aerosol Problem"** — WRF's disabling of aerosol-aware physics is a window into the technical uncertainty at the heart of SRM. If the world's best atmospheric model can't reliably simulate aerosol-Radiation interactions, how can we deploy SRM?
2. **"The Economic Ghost Town"** — ClimateMARGO's dormancy-whiplash suggests that SRM economics is a field where people publish models but nobody maintains them. The tools rot.
3. **"The Curator's Acceleration"** — awesome-geoengineering went from 0 to v2.0 in 14 months. The resource gap is closing, but slowly.
4. **"The Simulator's Tragedy"** — GeoVision was built by one person in one day, then abandoned. Interactive SRM visualization is needed but unfunded.

### Open Questions for Guests
- Should SRM models be open-source? Who regulates the code that simulates planetary reflection?
- Is the WRF aerosol scheme change a technical improvement or an avoidance of the SRM question?
- What would a maintained, community-driven SRM economic model look like?