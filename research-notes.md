# ☀️ Solar Geoengineering — Research Notes (Updated Sep 2026)

## Project Discoveries

### 1. PSLmodels/Geo-DICE
- **URL:** https://github.com/PSLmodels/Geo-DICE
- **Language:** MATLAB
- **Stars:** 2
- **Contributors:** Soheil Shayegh, Matt Jensen
- **Description:** Modified DICE (Dynamic Integrated Climate-Economy) model incorporating geoengineering scenarios. Developed at PSL (Program in Science, Technology, and Environmental Policy), Princeton.
- **Last Activity:** September 27, 2018
- **Commit Count:** 4 total (Aug 2016 – Sep 2018)
- **Relevance:** Foundational integrated assessment model for SRM governance economics. The DICE framework is the gold standard for climate-economy modeling; this variant explicitly includes solar geoengineering as a policy lever. Last touched in 2018 — essentially a legacy snapshot of DICE + geoengineering capability.

### 2. jlehtomaa/OOCC_2021
- **URL:** https://github.com/jlehtomaa/OOCC_2021
- **Language:** Python
- **Stars:** 2
- **Description:** A simple model for solar geoengineering governance. Accompanies the 2021 paper "Sustainable Governance of Solar Geoengineering" published in Oxford Open Climate Change.
- **Last Activity:** November 15, 2021
- **Commit Count:** 10 shown (all in Sep–Nov 2021: 4 README updates, 2 citation updates, 2 README+another, 1 bibtex entry, 1 bibtex reference)
- **Relevance:** The ONLY open-source repo explicitly modeling geoengineering governance. Can-a-climate-model-democratize-the-policy-discourse? Critical for episode framing around who controls the global thermostat. All commits were in a tight publication window — classic paper-driven lifecycle.

### 3. cjcarlson/geomalaria
- **URL:** https://github.com/cjcarlson/geomalaria
- **Language:** R
- **Stars:** 3
- **Contributor:** Colin J. Carlson (Georgetown University)
- **Description:** Malaria risk modeling in a world with solar geoengineering. Examines secondary biological impacts of SRM scenarios on disease vector populations.
- **Last Activity:** February 15, 2022
- **Commit Count:** 10 shown (clustered heavily in Jan–Feb 2022 — 7 commits in 2 weeks!)
- **Relevance:** Highlights the ecological side-effects of SRM. Key episode question: if we block sunlight to cool the planet, what happens to tropical disease vectors and ecosystems? The commit burst mirrors a paper publication cycle.

### 4. ClimateMARGO/ClimateMARGO.jl
- **URL:** https://github.com/ClimateMARGO/ClimateMARGO.jl
- **Language:** Julia
- **Stars:** 73
- **Contributors:** Fons van der Plas, Henri Drake
- **Description:** Julia implementation of MARGO, an idealized climate-economic modelling framework for optimizing trade-offs between emissions mitigation, adaptation, and CDR (Carbon Dioxide Removal).
- **Last Activity:** August 17, 2026
- **Commit Count:** 10 shown (2 in Aug 2026 after 2-year dormancy; 1 in Oct 2023; 1 in Jul 2023; rest in 2021–2022)
- **Relevance:** The most active climate-economic simulation model in this set. The August 2026 burst (2 README updates after 2+ years of silence) is the only sign of renewed life across all solar geoengineering repos. Julia implementation makes it computationally efficient for ensemble runs. Potential "policy layer" for SRM governance.

---

## Commit Trend Analysis

| Repository | Commits (shown) | Active Period | Last Commit | Status |
|------------|----------------|---------------|-------------|--------|
| ClimateMARGO.jl | 10 | 2021–2026 | Aug 17, 2026 | **Active** (maintenance bursts) |
| OOCC_2021 | 10 | Sep–Nov 2021 | Nov 15, 2021 | Dormant (paper-driven) |
| geomalaria | 10 | Jan–Feb 2022 | Feb 15, 2022 | Dormant (research completion) |
| Geo-DICE | 4 total | Aug 2016–Sep 2018 | Sep 27, 2018 | **Long-dormant** (legacy) |

### Key Trends

1. **Paper-Driven Lifecycle:** OOCC_2021 and geomalaria both show commit activity concentrated tightly around publication dates, then immediate dormancy. Open-source SRM code is typically a byproduct of papers, not sustained software projects. The tools that should be most useful for governance — the OOCC model especially — are the ones most likely to be abandoned after publication.

2. **The Governance Modeling Gap:** Only ONE repository (OOCC_2021) explicitly models geoengineering governance. The rest are either impact models (geomalaria) or economic optimization (ClimateMARGO, Geo-DICE). The gap between simulation capability and governance tooling is enormous. **Episode angle:** "We can model the climate but not the politics."

3. **Dormancy Is the Norm:** 3 of 4 solar geoengineering repos haven't been touched in 3+ years. Only ClimateMARGO shows recent activity (Aug 2026). This fragility means that policy-relevant tools may not exist when they're needed most.

4. **Legacy MATLAB Persists:** Geo-DICE (2018, 4 commits) is MATLAB-based. The modern Julia/Python data-science shift hasn't reached geoengineering-specific simulation. This creates a reproducibility barrier for researchers without MATLAB licenses.

5. **The Renewed Interest Signal:** ClimateMARGO's August 2026 burst is the only sign of active life. This could indicate renewed attention from the CDR-governance community, possibly driven by recent UNFCCC discussions or the Paris Agreement Global Stocktake.

---

## Episode Questions for Solar Geoengineering

1. **Who controls the thermostat?** If governance tools like OOCC_2021 are dormant and only 4 repos exist for SRM simulation, who sets the research agenda for a technology that affects everyone?

2. **Can interactive models democratize the discourse?** The simplicity of OOCC_2021 and geomalaria suggests that low-barrier models could involve more stakeholders — but only if they're maintained. Dormant tools = no democratization.

3. **What are the ecological surprises?** geomalaria's finding that SRM could alter malaria risk patterns highlights the need for cross-disciplinary simulations. We model temperature but not disease vectors.

4. **Is ClimateMARGO's revival a signal?** The August 2026 activity burst on the most active SRM-adjacent repo — what policy event triggered it? What if it goes dormant again?

5. **Why no community-maintained SRM code?** Every existing SRM repo is either legacy (Geo-DICE), paper-driven (OOCC_2021, geomalaria), or multi-purpose (ClimateMARGO). Where is the community-maintained SRM simulator?

---

*Research compiled from GitHub repository search and commit history analysis. Sources: ClimateMARGO/ClimateMARGO.jl, PSLmodels/Geo-DICE, jlehtomaa/OOCC_2021, cjcarlson/geomalaria.*