# ☀️ Solar Geoengineering — Research Notes
**Podcast Episode: Solar Geoengineering | Last updated: September 2026**

---

## 📋 Episode Anchor Question
**Why is solar radiation management (SRM) code living inside climate models rather than in dedicated SRM repositories?**

---

## 🔬 Project Discoveries

### 1. ClimateMARGO.jl — `ClimateMARGO/ClimateMARGO.jl`
- **Stars:** 73 | **Language:** Julia | **Updated:** 2026-08-17
- **Description:** Julia implementation of MARGO, an idealized climate-economic modelling framework for optimizing trade-offs between emissions mitigation, adaptation, and geoengineering.
- **Why it matters for the episode:** This is one of the few open-source frameworks that explicitly couples climate physics with economic optimization and geoengineering decision-making. It's the kind of tool that could shape how policymakers think about SRM trade-offs.
- **Link:** https://github.com/ClimateMARGO/ClimateMARGO.jl

### 2. regional-geo — `Sustainable-Solutions-Lab/regional-geo`
- **Stars:** Low (niche) | **Language:** Python | **Updated:** 2026-09-18
- **Description:** Regional climate effects of sulfate aerosol injection in WRF simulations. From Ken Caldeira's lab (Carnegie Science / Permanente Associates).
- **Why it matters:** This is the most *directly* SRM-focused code we found — it simulates the actual regional climate impacts of stratospheric aerosol injection. The fact that it's a small, personal research repo rather than a major institution project is telling.
- **Link:** https://github.com/Sustainable-Solutions-Lab/regional-geo

### 3. awesome-geoengineering — `brandonhimpfen/awesome-geoengineering`
- **Stars:** 4 | **Language:** Python/Markdown | **Updated:** 2026-09-06
- **Description:** A curated list of projects, research, organizations, tools, and resources related to geoengineering. Now at v2.0.0.
- **Why it matters:** A good starting point for the episode's "where to go deeper" segment. actively maintained with 7 recent commits.
- **Link:** https://github.com/brandonhimpfen/awesome-geoengineering

### 4. Geo-DICE — `PSLmodels/Geo-DICE`
- **Stars:** 2 | **Language:** MATLAB | **Updated:** 2018 (dormant)
- **Description:** Modified DICE (Dialogue on Earth's Internal Climate) model with geoengineering components. By Matteo Degasperi and Soheil Shayegh.
- **Why it matters:** DICE is the canonical integrated assessment model in climate economics. The geoengineering variant is essentially defunct — last commit was 2018. This illustrates how SRM modeling tends to be absorbed back into mainstream climate-econ frameworks rather than sustaining its own codebase.
- **Link:** https://github.com/PSLmodels/Geo-DICE

### 5. OOCC_2021 — `jlehtomaa/OOCC_2021`
- **Stars:** 2 | **Language:** Python | **Updated:** 2021 (dormant)
- **Description:** A simple model for solar geoengineering governance. Published as part of the 2021 Conference on Open Collaboration.
- **Why it matters:** This is a governance *model* — it's not about the physics of SRM but about how to govern it. The fact that it's dormant since 2021 suggests the governance conversation may have moved to academic papers rather than code.
- **Link:** https://github.com/jlehtomaa/OOCC_2021

---

## 📊 Commit Trend Analysis

### Commit Velocity by Repo (last 12 months)

| Repo | 12-mo Commits | Pattern | Last Commit |
|------|---------------|---------|-------------|
| ClimateMARGO.jl | 2 | Burst-then-dormant | 2026-08-17 |
| regional-geo | 10 | Cluster-burst (research sprint) | 2026-02-15 |
| awesome-geoengineering | 7 | Steady maintenance | 2026-09-06 |
| Geo-DICE | 0 | Dormant since 2018 | 2018-09-27 |
| OOCC_2021 | 0 | Dormant since 2021 | 2021-11-15 |

### Key Observations

1. **The "burst then vanish" pattern dominates.** Both ClimateMARGO.jl and regional-geo show research-sprint patterns — a cluster of commits followed by long dormancy. This is characteristic of academic code: built for a paper, not for a community.

2. **The only continuously maintained repo is awesome-geoengineering** — a curated list, not a simulation. This means the *metadata layer* of geoengineering open source is alive, while the *simulation layer* is not.

3. **Solar radiation fix in WRF is notable.** The WRF model (the giant at 1,763 stars) recently merged a commit (2026-05-28) titled "correction for eot calculation for solar radiation." SRM physics lives inside the general climate modeling infrastructure — you can't find it by searching for "geoengineering."

4. **DORMANCY IS THE NORM.** 3 out of 5 solar geoengineering repos are completely dormant. This is a structural finding for the episode: solar geoengineering research on GitHub is *ephemeral* — it appears, serves its paper, then stops.

---

## 🎙️ Episode Talking Points

- **The WRF Problem:** The most important SRM simulation code in the world lives inside the WRF weather model, not in any SRM-specific repo. How do you discuss governance of technology that's hidden inside general-purpose infrastructure?
- **The DORMANCY SIGNAL:** Why do SRM repos die after publication? Is it a governance problem (no one maintains it) or a philosophical one (the code served its purpose for the paper)?
- **ClimateMARGO.jl as the exception:** One repo is trying to build an ongoing community around climate-economic-geoengineering modeling. Is this the future, or the outlier?
- **The governance gap:** OOCC_2021 shows that governance *models* for SRM are even rarer than the physics models — and they're dying too.

---

## 🔗 Cross-References
- See `main/CROSS-THEME-ANALYSIS-v4.md` for the unified dashboard across all three themes.
- See `carbon-capture/RESEARCH-NOTES-CARBON-v5.md` for the carbon capture comparison.
- See `ocean-intervention/RESEARCH-NOTES-OCEAN-v5.md` for the ocean intervention gap analysis.

*Methodology: GitHub Repository & List Commits APIs, September 2026. Search queries: "geoengineering", "solar geoengineering", "solar radiation management", "stratospheric aerosol injection", "regional climate effects sulfate aerosol".*