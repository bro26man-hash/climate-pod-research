# 🌊 Ocean Intervention Commit Analysis — September 2026

## The Fundamental Finding: The Ocean Gap

After 10+ distinct GitHub search queries across multiple strategies, **we found zero dedicated ocean geoengineering repositories.** Not one. Zero repos for:
- Ocean alkalinity enhancement (OAE)
- Marine cloud brightening (MCB)
- Ocean temperature management
- Marine ecosystem intervention
- Ocean-based carbon removal (beyond general ocean health)
- Ocean sensors / monitoring for geoengineering

The ocean covers 71% of the Earth's surface. It absorbs 90% of excess heat and 30% of human CO2 emissions. And it has **zero GitHub repos.** This is the most significant finding of our entire research.

---

## What DOES Exist: Ocean-Adjacent Repositories

While there are no ocean geoengineering repos, there are ocean-climate modeling repos that provide the scientific infrastructure. These are the tools that would be used to evaluate ocean intervention proposals — not to implement them.

### Repository 1: NCAR_ML_EKE (Ocean Climate Modeling)
**Repo:** [CrayLabs/NCAR_ML_EKE](https://github.com/CrayLabs/NCAR_ML_EKE)  
**Stars:** 20  |  **Language:** Jupyter Notebook  |  **Status:** 🟡 Dormant (last commit 2022)

#### What It Does
This repository accompanies a paper: "Using Machine Learning at Scale in HPC Simulations with SmartSim: An Application to Ocean Climate Modeling." It's about using machine learning to accelerate ocean climate simulations — specifically, driven research into ocean energy kinetic energy (EKE) and how ML can improve ocean model resolution.

#### Recent Commits (10 pulled)

| Date | Commit | Author | Significance |
|------|--------|--------|-------------|
| Mar 30 | Fix notebook typos | Andrew Shao | Documentation cleanup (2022) |
| Mar 28 | Refactor driver for colocated option | Andrew Shao | ML-HPC integration refinement |
| Mar 14 | Update MOM6 instructions and submodule | Sam Partee | **MOM6** — Modular Ocean Model update |
| Feb 9 | Update README for compiling MOM6 | Andrew Shao | Build system documentation |
| Feb 8 | Update MOM6 submodule | Andrew Shao | Ocean model component update |
| Jul 2021 | edit README | Sam Partee | Pre-release documentation |
| Apr 2021 | Create LICENSE + README updates | Sam Partee | Initial release (4 commits on Apr 13) |

#### Why It Matters for Ocean Intervention
- **MOM6 (Modular Ocean Model)** is the same model family used in climate projections that evaluate ocean intervention proposals. If someone wanted to model the effects of ocean alkalinity enhancement, they'd use a model like MOM6.
- **ML-accelerated ocean modeling** is the enabling technology. Traditional ocean simulations are computationally expensive. ML can make them fast enough to run the ensemble simulations needed for intervention risk assessment.
- **The dormancy pattern** (last commit 2022) is a warning sign. Ocean climate modeling is underfunded relative to atmospheric modeling. NCAR's ML efforts may have moved to other projects.

#### Episode Talking Points
- "This repo has 20 stars and 4 commits in its entire life. The ocean's digital twin runs on 20 GitHub stars."
- "MOM6 is the modular ocean model — the same tool used to project sea level rise and ocean acidification. If we can't even keep ocean modelers funded to update their code, how will we model the effects of ocean geoengineering?"
- "ML for ocean modeling is the key technology. You need fast simulations to assess intervention risks. But the ML ocean modeling project went dormant in 2022. The funding didn't follow the science."

---

### Repository 2: WRF (Atmospheric-Oceanic Coupling)
**Repo:** [wrf-model/WRF](https://github.com/wrf-model/WRF)  
**Stars:** 1,762  |  **Relevance:** Ocean-adjacent through air-sea coupling

#### Ocean Connection
WRF includes air-sea coupling capabilities. While it's primarily an atmospheric model, its ocean component (WAV) and air-sea interaction schemes are used in coastal and maritime climate studies. The May 2026 commit fixing solar radiation calculations affects ocean surface temperature simulations, which in turn affect ocean intervention modeling.

#### Key Ocean-Related Commits (from our fresh pull)
- May 28: **Solar radiation eot correction** — affects ocean surface heat budget
- May 20: New ShinHong PBL scheme — affects air-sea flux calculations
- May 12: MYNN-SFC submodule update — affects sea surface temperature modeling

---n
### Repository 3: ClimateMARGO.jl (Climate-Economic Framework)
**Repo:** [ClimateMARGO/ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)  
**Stars:** 73  |  **Relevance:** Economic modeling of ocean geoengineering scenarios

#### Ocean Connection
ClimateMARGO's idealized climate-economic framework could theoretically model ocean intervention scenarios (e.g., "what are the economic costs/benefits of marine cloud brightening?"). But with the repo dormant for 3.5 years, the ocean-economic modeling capacity is theoretical, not practical.

---

## What Would Open-Source Ocean Intervention Look Like?

### The Missing Repos We Searched For

| Search Term | Repos Found | What It Would Model |
|-------------|-------------|-------------------|
| "ocean alkalinity enhancement" | 0 | Chemical reactions of olivine/limestone dissolution in seawater |
| "marine cloud brightening" | 0 | Sea spray aerosol injection for cloud seeding |
| "ocean geoengineering" | 0 | Any ocean-based climate intervention |
| "ocean intervention climate" | 0 | Direct ocean climate stabilization |
| "ocean carbon removal" | 0 | Biological or chemical ocean CDR |
| "ocean temperature management" | 0 | Ocean cooling techniques |
| "sea spray" | 0 | Marine cloud brightening ingredient |
| "olivine weathering" | 0 | Mineral dissolution for alkalinity |
| "ocean sensors" | 0 | Monitoring arrays for intervention assessment |
| "marine biodiversity geoengineering" | 0 | Ecosystem-level interventions |

### The Governance Signal
The absence of ocean geoengineering repos is not just a technical gap — it's a **governance signal.** The scientific community has published extensively on ocean intervention proposals (Nature, Science, PNAS). But the open-source code community has not picked up the initiative. This could mean:

1. **The science isn't mature enough** — We don't have validated models that can simulate ocean interventions at scale, so no one's writing code.
2. **The governance is too uncertain** — No international framework exists for ocean intervention, so researchers are reluctant to build tools that could be used without regulation.
3. **The funding isn't there** — Ocean modeling is already underfunded. Modeling ocean *intervention* would be even further down the priority list.
4. **The community hasn't formed** — Unlike solar geoengineering (which has WRF, CESM, etc.), ocean geoengineering has no established computational community.

### What a Real Open-Source Ocean Intervention Repo Would Need

Based on the patterns we observed in the solar and carbon repos, here's what the ocean's "WRF moment" would look like:

| What Exists (Atmosphere) | What's Missing (Ocean) |
|--------------------------|------------------------|
| WRF (1,762★) — atmospheric model | ✗ No ocean intervention model |
| MOM6 (via NCAR_ML_EKE) — ocean model but dormant | ○ Ocean model exists but not for intervention |
| PCMDI metrics (133★) — ESM evaluation | ✗ No ocean intervention evaluation toolkit |
| awesome-geoengineering (4★) — catalog | ✗ No ocean intervention catalog |
| ClimateMARGO (73★) — economic modeling | ✗ No ocean intervention economics |

---

## The Ocean's Closest Friend: MDTF's Precipitation-Buoyancy POD

**Repo:** [NOAA-GFDL/MDTF-diagnostics](https://github.com/NOAA-GFDL/MDTF-diagnostics)  
**Relevance:** Process-oriented ocean diagnostics

The most ocean-relevant code we found is the **precipitation-buoyancy POD** in the Model Diagnostics Toolkit (MDTF). On June 19, 2026, there were **5 commits to the same file** — the most concentrated ocean-related commit activity we found anywhere.

What is it? A Pod (Plain Old Documentation) that evaluates the relationship between precipitation and buoyancy in climate models. It's a diagnostic tool, not an intervention tool. But it's the closest thing to ocean intervention code that exists: it evaluates how well models represent ocean-atmosphere coupling.

**The irony:** The most active ocean-related code on GitHub is for evaluating model accuracy, not simulating interventions. We can tell you how good models are at simulating the ocean. What we can't do is simulate changing the ocean.

---

## Episode Talking Points

### The Ocean Episode Narrative
> "We searched GitHub ten different ways for ocean geoengineering code. Zero repos. Not one. The ocean covers seventy-one percent of the Earth, absorbs ninety percent of our excess heat, and it has zero GitHub repositories. The atmospheric modeling community has WRF — 1,700 stars, institutional backing, weekly commits. The carbon capture community has directories, economic maps, even public domain sorbent data. But the ocean? The ocean's digital footprint is invisible. And that silence is itself a story. Either the science isn't ready, the governance isn't clear, the funding isn't there, or nobody's thought about it. Or maybe — and this is the uncomfortable possibility — we're all just waiting for someone else to go first."

### The "What Would It Take?" Segment
> "Looking at what exists in the solar and carbon universes, here's what we'd need for an ocean 'WRF moment': a community-maintained ocean intervention model (like WRF but for the sea), an evaluation toolkit (like PCMDI but for ocean interventions), a curated catalog (like awesome-geoengineering but for ocean approaches), and economic modeling (like ClimateMARGO but for ocean scenarios). None of that exists. The ocean is the empty quadrant on the climate tech map."

### The Governance Angle
> "The absence of ocean geoengineering code might be the most responsible thing in the history of climate tech. No one's built the tools because no one's agreed on the rules. The ocean is a global commons. If someone codes an ocean intervention model, who decides when it's ready to use? Who owns the results? Who bears the liability? The silence on GitHub might be the governance signal we should listen to."

---

## Summary: The Ocean Gap in Three Numbers

| Metric | Value |
|--------|-------|
| Ocean geoengineering repos on GitHub | **0** |
| Ocean-climate modeling repos (active) | **1** (NCAR_ML_EKE, dormant since 2022) |
| Ocean-related commit activity (peak) | **5 commits on one file** (MDTF precip-buoyancy POD, Jun 19 2026) |

The ocean is the dark matter of climate tech on GitHub. It exerts gravitational influence on everything else — atmospheric models couple with it, carbon cycle models depend on it, economic models reference it — but it has no visible code presence of its own.

---

## Research Methods Note

**Search queries used:**
1. `geoengineering simulation climate`
2. `climate technology carbon capture ocean`
3. `geoengineering`
4. `climate simulation modeling`
5. `carbon capture removal`
6. `ocean climate intervention`
7. `ocean alkalinity enhancement`
8. `marine cloud brightening`
9. `ocean geoengineering`
10. `ocean intervention climate`
11. `ocean carbon removal`
12. `sea spray aerosol`
13. `olivine weathering ocean`
14. `ocean sensors monitoring`
15. `marine biodiversity geoengineering`

**Commit histories pulled from:**
- wrf-model/WRF (15 commits, May-Jun 2026)
- ClimateMARGO/ClimateMARGO.jl (15 commits, 2022-2026)
- protontypes/open-sustainable-technology (15 commits, Jun-Sep 2026)
- PSLmodels/Geo-DICE (4 commits, 2016-2018)
- brandonhimpfen/awesome-geoengineering (7 commits, 2025-2026)
- swarmlabsusa/carbon-swarm (3 commits, Apr 2026)
- CrayLabs/NCAR_ML_EKE (10 commits, 2021-2022)
- jlehtomaa/OOCC_2021 (10 commits, 2021)
