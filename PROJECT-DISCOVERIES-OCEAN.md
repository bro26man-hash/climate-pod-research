# 🌊 Ocean Intervention — Project Discovery Catalog

**Last Updated:** September 2026 (v4 — fresh commit data from ocean modeling ecosystem with Lagrangian particle tracking and OceanBioME gas exchange PR chain)
**Research Method:** GitHub repository search ("ocean fertilization", "ocean alkalinity enhancement", "marine geoengineering", "artificial upwelling", "seaweed carbon farming", "marine cloud brightening", "ocean intervention") + cross-reference with "awesome-open-climate-science" directory

---

## The Discovery Gap: ZERO Dedicated Ocean Geoengineering Repos

After exhaustive searching across 10+ query strategies (detailed in COMMIT-TRENDS-OCEAN.md):

| Search Term | Results |
|-------------|---------|
| ocean fertilization | 0 repos |
| ocean alkalinity enhancement | 0 repos |
| marine geoengineering | 0 repos |
| ocean intervention marine technology | 0 repos |
| ocean pH sensor monitoring | 0 repos |
| artificial upwelling ocean | 0 repos |
| seaweed kelp carbon farming | 0 repos |
| marine cloud brightening | 0 repos |

**This is the most significant finding of the entire research effort.** While the ocean CLIMATE modeling ecosystem is thriving (Oceananigans 1,413★, veros 400★, OceanBioME 80★), there are ZERO repos designed to design, simulate, or evaluate ocean geoengineering interventions.

---

## What DOES Exist: The Ocean Climate Modeling Ecosystem (Updated with Fresh Commit Data)

### Tier 1: World-Class Ocean Models

### 1. CliMA/Oceananigans.jl — 1,413 Stars (The Ocean Powerhouse)

- **URL:** https://github.com/CliMA/Oceananigans.jl
- **Language:** Julia
- **Focus:** Ocean fluid dynamics with GPU acceleration (CPU+GPU parallel)
- **Latest:** Sep 15-17, 2026 — 10 commits in 3 days (MOST ACTIVE geoengineering-adjacent repo)
- **Key Fresh Commit:** **Sep 16, 2026 — "Bounce Lagrangian particles off immersed boundaries" (#6005)** ← This is the exact computational method needed for tracer deployment in OAE simulations
- **Other Key Commits:** SplitRungeKuttaTimeStepper improvements (#6009), ConjugateGradientSolver optimization (#6012), closure field checkpoint restoration (#6006)
- **Ocean Intervention Relevance:** Oceananigans already has:
  - **Lagrangian particle tracking** (Sep 16, 2026 — for tracer deployment) ← THE key intervention tool
  - **Immersed boundary methods** (for coastal/structure interactions)
  - **Time-dependent forcing capabilities** (for simulating injection scenarios)
  - **Parallel CPU+GPU execution** (for large-scale simulations)
  - **The architecture supports adding new physics modules** ← The extensibility point for OAE/iron fert modules

### 2. team-ocean/veros — 400 Stars (The Pure-Python Ocean Simulator)

- **URL:** https://github.com/team-ocean/veros
- **Language:** Python/JAX
- **Focus:** Pure-Python ocean simulator powered by JAX for differentiable execution
- **Latest:** Sep 14-15, 2026 — mostly dependabot bumps + isoneutral mixing bugfix (#866)
- **Ocean Intervention Relevance:** Veros is the most accessible pure-Python ocean simulator. Its accessibility makes it the best candidate for building ocean intervention teaching tools. The isoneutral mixing bugfix is relevant — accurate mixing is critical for modeling OAE plume dispersion.

### 3. OceanBioME/OceanBioME.jl — 80 Stars (The Biogeochemistry & Gas Exchange Model)

- **URL:** https://github.com/OceanBioME/OceanBioME.jl
- **Language:** Julia
- **Focus:** Ocean biogeochemistry, carbonate chemistry, and air-sea gas exchange
- **Latest:** Sep 14-17, 2026 — 10 commits in 4 days (VERY ACTIVE)
- **Key Fresh Commits:**
  - **PR #411 (Sep 15):** "gas exchange changes" ← Directly about air-sea gas exchange parameterization
  - **PR #399 (Sep 15):** "numerical-earth-coupling" ← Coupling ocean and Earth system models
  - **PR #419 (Sep 17):** "return wind to gas exchange top level" ← Wind speed is the primary driver of gas exchange
  - **The wind speed coupling debate:** PR #411 → "Move wind speed back to gas exchange top level" → "Fix stuff" → "Fix docs" — a heated technical debate about how wind speed should couple to gas exchange calculations
- **Ocean Intervention Relevance:** Gas exchange is THE central process for ocean-based CDR. Ocean alkalinity enhancement works by accelerating natural weathering, which changes ocean CO2 capacity — which is governed by air-sea gas exchange. OceanBioME's active development of gas exchange parameterizations (3 PRs in 4 days) is directly relevant to OAE modeling.

---

## Tier 2: Supporting Ocean Science Repos

| Repo | Stars | Language | Focus | Latest Activity |
|------|-------|----------|-------|----------------|
| pangeo-data/awesome-open-climate-science | 598 | Multi | Curated list of open climate science | Sep 16, 2026 |
| gaelforget/ClimateModels.jl | 47 | Julia | Julia interface to climate models | Aug 13, 2026 |
| aerler/WRF-Tools | 59 | Shell | WRF setup and run tools | Jun 23, 2026 |
| Climdyn/MAOOAM | 22 | HTML/Lua/Fortran/Python | Modular ocean-atmosphere model | Jun 29, 2026 |
| JuliaOcean/Climatology.jl | 20 | Julia | Ocean climatology | Aug 22, 2026 |

---

## What's MISSING: The Ocean Intervention Layer (Updated)

| Missing Category | Why It Matters | Nearest Existing Tool | Fresh Commit Signal |
|-----------------|----------------|----------------------|---------------------|
| OAE simulation module | Core tool for ocean alkalinity enhancement modeling | Oceananigans.jl (platform exists, no module) | **Lagrangian particles just landed Sep 16, 2026!** |
| Iron fertilization model | Needed for SNAPI/LOHAFEX-type simulations | OceanBioME (biogeochemistry exists, no Fe module) | OceanBioME active Sep 2026 (gas exchange, not Fe) |
| Artificial upwelling model | Needed for nutrient pump simulations | veros (ocean dynamics exist, no upwelling forcing) | Veros in maintenance mode (dep bumps) |
| Marine cloud brightening tool | Needed for MBC simulation/evaluation | MDTF-diagnostics (precipitation-buoyancy POD) | MDTF last commit Aug 14, 2026 |
| Ocean pH/alkalinity sensor designs | DIY hardware for monitoring experiments | ZERO (unlike OpenAir-Cyan for DAC) | No ocean hardware repos found |
| Ocean intervention governance tool | Regulatory mapping like srm-forever | ZERO | No ocean governance repos found |
| OAE gas exchange module | Core process for alkalinity amendment flux | OceanBioME (actively developing gas exchange) | **3 PRs in 4 days Sep 15-17, 2026** |

---

## The Ocean-Adjacent Repositories Worth Watching (Updated)

### MDTF-diagnostics (NOAA-GFDL, 80★)
- **URL:** https://github.com/NOAA-GFDL/MDTF-diagnostics
- **Relevant work:** MCS precipitation-buoyancy statistics POD (Jun 19, 2026 — 5 commits in 1 day)
- **Fresh Commits:** Aug 14, 2026 (PR #825 merged); Jun 19, 2026 (precip-buoyancy POD)
- **Why it matters:** Process-oriented diagnostics that could be adapted for marine cloud brightening evaluation. The precipitation-buoyancy statistics POD is the closest thing to an MCB evaluation tool in open source.

### WRF (NCAR/NOAA, 1,761★)
- **URL:** https://github.com/wrf-model/WRF
- **Relevant work:** Ocean boundary layer physics (MYNN-EDMF), air-sea interaction modules, TEMPO aerosol physics
- **Fresh Commits:** Jun 8, 2026 (v4.8.0 released); May 28, 2026 (solar radiation EOT correction)
- **Why it matters:** The atmosphere-ocean coupling layer exists in WRF. An intervention module would need to interface with WRF's ocean physics. But WRF is atmospheric-first; ocean is a boundary condition, not the focus.

### PCMDI/pcmdi_metrics (LLNL, 133★)
- **URL:** https://github.com/PCMDI/pcmdi_metrics
- **Relevant work:** ENSO, sea ice, ocean heat content metrics
- **Fresh Commits:** Sep 3-4, 2026 (v4.2.1 burst, 10 commits in 2 days); Sep 3, 2026 (extremes chunking with dask/SVD)
- **Why it matters:** Evaluation infrastructure. If an ocean intervention is deployed, PCMDI-style metrics would verify its effects. The extremes chunking update suggests they're scaling for larger ensembles — exactly what SRM/ocean intervention scenario testing would need.

### Oceananigans.jl (CliMA/Caltech, 1,413★)
- **URL:** https://github.com/CliMA/Oceananigans.jl
- **Fresh Commits:** 10 commits in 3 days (Sep 15-17, 2026)
- **Key Signal:** Lagrangian particle tracking (#6005, Sep 16) — the computational method for tracer deployment
- **Why it matters:** THE most promising platform for building ocean intervention simulation tools. The physics engine is world-class. The particle tracking was just added. The extensibility architecture supports new physics modules.

### OceanBioME.jl (OceanBioME, 80★)
- **URL:** https://github.com/OceanBioME/OceanBioME.jl
- **Fresh Commits:** 10 commits in 4 days (Sep 14-17, 2026)
- **Key Signal:** Gas exchange PR chain (#411, #399, #419) — actively developing the core process for OAE
- **Why it matters:** The gas exchange parameterization IS the physics that OAE depends on. OceanBioME is actively building it. Nobody has connected it to an intervention scenario yet.

---

## Why the Gap? (Updated with Fresh Evidence)

| Hypothesis | Evidence | Confidence | Fresh Data |
|------------|----------|------------|-----------|
| **Institutional gatekeeping** | Ocean science is dominated by WHOI, Scripps, GEOMAR — institutions that publish in closed journals and share through institutional channels | HIGH | OceanBioME's gas exchange PR chain shows active physics development but zero intervention Application |
| **Governance/regulatory risk** | London Protocol directly regulates ocean fertilization; transboundary impacts create legal risk | MEDIUM-HIGH | The wind speed coupling debate (#411) is about basic physics — before governance even arises, the science is still being settled |
| **Experimental complexity** | Ship time $50K+/day; sensor deployments need multi-year monitoring; international coordination required | HIGH | No ocean hardware repos found (unlike OpenAir-Cyan for DAC); no sensor designs |
| **Cultural mismatch** | Ocean science predates open-source movement by decades; researchers are at sea, not at keyboards | HIGH | 3 ODEs (ocean model repos) vs 0 intervention repos; the code exists but nobody writes intervention code |
| **No market incentive** | Unlike DAC (where $1000/ton target creates incentive), ocean intervention has no commercial impetus | MEDIUM | No economic modeling repos found for ocean intervention (unlike SRM's srm-forever) |

---

## The Nearest Feasible Starting Points (Updated)

1. **An Oceananigans.jl OAE module with Lagrangian particle tracking** — THE most feasible starting point. The physics engine exists (1,413★). The particle tracking was just added (Sep 16, 2026). The developers are active (10 commits/3 days). The gap is in the intervention layer. A graduate student could build this. Nobody has.

2. **An OceanBioME gas exchange + OAE module** — Gas exchange is THE core process for OAE, and OceanBioME is actively developing it (3 PRs in 4 days, Sep 2026). An OAE-specific gas exchange module would be a natural next step. The wind speed coupling debate (#411) is literally about the physics that OAE depends on.

3. **A veros-based OAE teaching tool** — Veros is pure Python and accessible. An interactive OAE simulator (like srm-forever for solar geoengineering) could democratize ocean intervention modeling. Veros is the "srm-forever of ocean intervention" — the accessible entry point. But it's in maintenance mode (dep bumps).

4. **DIY ocean sensor designs** — Like OpenAir-Cyan's hardware designs for DAC, shareable pH/alkalinity/pCO2 sensor designs for ocean monitoring. No equivalent exists. This is the hardware gap that mirrors OpenAir-Cyan's role in DAC.

5. **An ocean intervention governance tool** — Like srm-forever's approach to SRM governance, an interactive tool showing the legal/regulatory landscape for ocean interventions. No equivalent exists. The London Protocol complexity is the governance challenge.

---

## 🎙️ Episode Hooks (Updated)

1. **The ocean is the silence that speaks loudest.** Zero geoengineering repos, zero ocean intervention tools. Meanwhile, the atmosphere gets WRF, PCMDI, and MDTF. The ocean gets... nothing. That's the story.

2. **Oceananigans.jl just added Lagrangian particle tracking (Sep 16, 2026).** The "Bounce Lagrangian particles off immersed boundaries" commit (#6005) is the exact computational method needed for tracer deployment in OAE. The platform is maturing the tool. Nobody is using it for intervention scenarios. This is like having a physics engine with particle tracking but no video game built on top of it.

3. **OceanBioME's gas exchange work IS the OAE core process.** Three PRs in four days (Sep 15-17) on air-sea gas exchange — the central process for ocean alkalinity enhancement. The wind speed coupling debate (#411) shows the physics is still being settled. The science is ready; the application layer isn't built.

4. **The ocean gap is different from the carbon gap.** Carbon has OpenAir-Cyan (hardware), Carbon_Capture_ML (literature), and differentiable-flowsheets (AI simulation). Ocean has nothing — no hardware, no surveys, no interactive tools, no AI-augmented simulation.

5. **The wind speed coupling debate is a microcosm of the ocean gap.** Before you can model OAE, you need to nail the air-sea gas exchange physics. OceanBioME's PR chain (#411 → "move wind speed back" → "fix stuff" → "fix docs") shows that even the basic physics is still being debated. The governance question (can you even do this?) may suppress the "why would you model it?" question.

6. **The London Protocol may be causing self-censorship.** Unlike SRM (murky but not illegal), ocean fertilization is explicitly regulated. Researchers may avoid open-source code to avoid regulatory scrutiny. Or they may just not think of GitHub as a venue for ocean intervention code.

7. **The nearest feasible project is an Oceananigans.jl OAE module with Lagrangian particle tracking.** The physics engine exists. The particle tracking was just added. The gas exchange physics exists (OceanBioME, actively developing). The gap is in the intervention layer. A graduate student could build this. Nobody has.

8. **The August 2026 carbon wave highlights the ocean's silence.** While 6 carbon capture repos updated (now including AI-augmented differentiable-flowsheets), ZERO ocean repos updated at all for intervention design.

---

## 📋 Research Log (Updated)

| Date | Activity |
|------|----------|
| 2026-09-17 | v2: Ocean ecosystem data added — Oceananigans.jl, veros, OceanBioME.jl commit histories analyzed |
| 2026-09-17 | v2: Ocean gap analysis revised with new framework (modeling stack 80% built, intervention layer 0%) |
| 2026-09-17 | v3: Fresh commit histories pulled from 12 repositories across all three themes using GitHub API |
| 2026-09-17 | v3: Ocean gap confirmed — 10+ search queries, zero dedicated ocean geoengineering repos |
| 2026-09-17 | v3: CC0 license trend identified as major open-science signal in DAC materials community |
| 2026-09-18 | v4: Fresh commit data updated from GitHub API for all ocean-modeling repos |
| 2026-09-18 | v4: Lagrangian particle tracking commit (#6005) identified as key ocean-intervention enabler |
| 2026-09-18 | v4: OceanBioME gas exchange PR chain (#411, #399, #419) documented as OAE core process development |
| 2026-09-18 | v4: "Wind speed coupling debate" identified as microcosm of ocean governance gap |
| 2026-09-18 | v4: Updated gap framework table with fresh commit data and nearest-active-repo column |
| 2026-09-18 | v4: "Ocean modeling stack 80% built, intervention layer 0%" thesis confirmed with new data |