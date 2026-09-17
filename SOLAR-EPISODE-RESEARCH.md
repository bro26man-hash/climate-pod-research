# ☀️ Solar Geoengineering — Episode Research Notes

## Episode Overview
This episode explores Solar Radiation Management (SRM) — the set of techniques designed to reflect a small fraction of incoming solar radiation back into space to reduce global temperatures. We examine the open-source simulation tools available, the key research groups, and the political and ethical questions that make SRM one of the most controversial areas of climate tech.

---

## Key Open-Source Projects

### 1. ClimateMARGO.jl (ClimateMARGO/ClimateMARGO.jl)
- **Stars:** 73 | **Language:** Julia | **Last Updated:** Aug 17, 2026
- **What it does:** Idealized climate-economic modelling framework for optimizing trade-offs between emissions mitigation, adaptation, and solar geoengineering.
- **Why it matters for the episode:** It's one of the few actively maintained tools that explicitly models SRM as a policy lever alongside mitigation and adaptation. The Julia implementation makes it accessible for interactive exploration.
- **Commit activity:** Bursty — 2 commits on Aug 17, 2026 (README update), then a long gap back to 2023. Single maintainer (Fons van der Plas), with earlier contributions from Henri Drake.
- **Episode angle:** "Can an interactive Julia model help non-scientists understand the SRM trade-off treadmill?"

### 2. OOCC_2021 (jlehtomaa/OOCC_2021)
- **Stars:** 2 | **Language:** Python | **Last Updated:** Nov 15, 2021
- **What it does:** A simple model for solar geoengineering governance — examining the political and governance dimensions of SRM deployment.
- **Why it matters:** One of the very few repos that explicitly models the *governance* of SRM, not just the physics. This is a gap in the field: we have lots of climate models but very little governance models.
- **Commit activity:** Dense initial development (July–Sept 2021), then silence. ~15 commits over 4 months, all by one author (jlehtomaa).
- **Episode angle:** "Why does SRM governance have a model but SRM deployment doesn't?"

### 3. Geo-DICE (PSLmodels/Geo-DICE)
- **Stars:** 2 | **Language:** MATLAB | **Last Updated:** Sep 27, 2018
- **What it does:** Modified DICE (Dynamic Integrated Climate-Economy) model with geoengineering components. By Soheil Shayegh and Matt Jensen at PSL.
- **Why it matters:** DICE is the most influential climate-economics model in policy. This modification adds SRM as an option within the canonical framework — making it the "gun" at the head of climate policy.
- **Commit activity:** Only 4 commits, all in 2016-2018. Effectively dormant. The code was uploaded once and never maintained.
- **Episode angle:** "The most important climate model with geoengineering was abandoned in 2018. What does that tell us about institutional support for SRM research?"

### 4. geomalaria (cjcarlson/geomalaria)
- **Stars:** 3 | **Language:** R | **Last Updated:** Feb 15, 2022
- **What it does:** Models malaria risk in a world with solar geoengineering — one of the few impact-assessment tools for SRM's side effects.
- **Why it matters:** SRM doesn't stop ocean acidification, and it may disrupt monsoons and agricultural patterns. This repo asks: what happens to disease vectors if we suddenly cool the planet?
- **Commit activity:** Intense burst in Jan-Feb 2022 (~15 commits in 6 weeks), then silence. By Colin J. Carlson.
- **Episode angle:** "If we reflect sunlight, who gets malaria? The unintended consequences no one models."

### 5. CESM2geoeng (jnickla1/CESM2geoeng_documentation)
- **Stars:** N/A | **Language:** Documentation | **Last Updated:** Nov 27, 2025
- **What it does:** Documentation for the ocean geoengineering CESM2 paper — includes both marine cloud brightening and ocean alkalinity enhancement simulations using the CESM2 model.
- **Note:** Repository currently has zero commits (empty repo). Documentation exists as paper supplementary material.
- **Episode angle:** "The CESM2 geoengineering paper is one of the most cited in the field, but the code is empty. Where is the reproducibility crisis in geoengineering?"

### 6. sai-git (JdeJong96/sai-git)
- **Stars:** N/A | **Language:** Jupyter Notebook | **Last Updated:** Aug 15, 2025
- **What it does:** Tools for analyzing CESM solar aerosol injection (SAI) climate data — including mapping, averaging, and figure generation for SAI experiments.
- **Commit activity:** Very active — 15+ commits between Feb-Aug 2025. The most recently active solar geoengineering-related repo in our search. By Jasper de Jong.
- **Episode angle:** "The one solar geoengineering repo that's actually being worked on right now — and it's just data analysis, not simulation."

---

## Commit Trend Analysis: Solar Geoengineering

| Pattern | Finding |
|---------|--------|
| **Burst-then-die cycle** | 4 of 6 repos show intense activity for weeks/months, then permanent silence. No sustained, years-long development. |
| **2022 was the peak year** | geomalaria, Geo-DICE's last touches, and most OOCC activity cluster in 2021-2022. Interest may have peaked and then declined. |
| **2025-2026 renaissance?** | ClimateMARGO.jl (Aug 2026) and sai-git (Feb-Aug 2025) show recent activity. But sai-git is data analysis, not new simulation. |
| **Governance gap** | The only governance-focused model (OOCC_2021) is dormant. No one is building decision-support tools for SRM policy. |
| **Single-maintainer risk** | Every repo has 1-2 contributors. If the lead loses interest, the code dies. No community infrastructure. |
| **Language fragmentation** | Julia, Python, MATLAB, R, Fortran — no common technical stack. This fragments the ecosystem and prevents tooling convergence. |

---

## Key Episode Questions

1. **Why is SRM simulation code so scarce compared to general climate modeling?** (WRF has 1,761 stars; the best SRM-specific tool has 73.)
2. **Is the burst-then-die pattern a symptom of academia's publish-and-move-on culture?** Most repos are tied to a single paper.
3. **What would a sustainable, community-governed SRM simulation platform look like?**
4. **The governance vacuum:** We can model SRM physics, but we have no open-source tools for modeling *whether and how* to govern it.
5. **The impact-assessment gap:** geomalaria is the only repo that models *consequences* of SRM (malaria). What about agriculture, monsoons, ozone?

---

## Sources & Links
- [ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- [OOCC_2021](https://github.com/jlehtomaa/OOCC_2021)
- [Geo-DICE](https://github.com/PSLmodels/Geo-DICE)
- [geomalaria](https://github.com/cjcarlson/geomalaria)
- [sai-git](https://github.com/JdeJong96/sai-git)
- [CESM2geoeng_documentation](https://github.com/jnickla1/CESM2geoeng_documentation)
