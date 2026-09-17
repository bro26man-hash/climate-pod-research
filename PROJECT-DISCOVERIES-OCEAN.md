# 🌊 Ocean Intervention — Project Discovery Catalog

**Last Updated:** September 2026 (v3 update — fresh commit data + ocean-adjacent simulation infrastructure)
**Research Method:** GitHub repository search ("ocean fertilization", "ocean alkalinity enhancement", "marine geoengineering", "artificial upwelling", "seaweed carbon farming", "marine cloud brightening", "climate simulation operations", "ocean model diagnostics") + cross-reference with "awesome-open-climate-science" directory

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

## What DOES Exist: The Ocean Climate Modeling & Simulation Ecosystem

### Tier 1: World-Class Ocean Models

| Repo | Stars | Language | Focus | Fresh Activity |
|------|-------|----------|-------|----------------|
| **CliMA/Oceananigans.jl** | 1,413 | Julia | Ocean fluid dynamics (CPU+GPU) | 10 commits in 3 days (Sep 15-17, 2026) |
| **team-ocean/veros** | 400 | Python/JAX | Pure-Python ocean simulator | Dependabot bumps + Dion's isoneutral mixing bugfix (#866, Sep 14) |
| **OceanBioME/OceanBioME.jl** | 80 | Julia | Ocean biogeochemistry & carbonate chemistry | 10 commits in 4 days (Sep 14-17, 2026) — gas exchange focus |

### Tier 2: Climate Simulation Operations & Infrastructure (NEW for v3)

| Repo | Stars | Language | Focus | Fresh Activity |
|------|-------|----------|-------|----------------|
| **roocs/clisops** | 25 | Python | Climate Simulation Operations — utilities for processing, regridding, and analyzing climate model output | Active: 10 commits in Sep 2026 (dependabot bumps + version 0.18.1 release Jul 2026 + documentation fix Jul 15) |
| **wrf-model/WRF** | 1,761 | Fortran | Weather Research and Forecasting model — includes ocean boundary layer physics (MYNN-EDMF) | 10 commits in 18 days (May-Jun 2026) — v4.8.0, solar radiation EOT fix |
| **NOAA-GFDL/MDTF-diagnostics** | 80 | Jupyter Notebook | Process-oriented diagnostics for weather and climate simulations | Aug 14, 2026 PR merge — MCS precipitation-buoyancy POD (Jun 2026) |

### Tier 3: Supporting Infrastructure

| Repo | Stars | Language | Focus |
|------|-------|----------|-------|
| pangeo-data/awesome-open-climate-science | 598 | Multi | Curated list of open climate science tools |
| gaelforget/ClimateModels.jl | 47 | Julia | Julia interface to climate models |
| Climdyn/MAOOAM | 22 | HTML/Lua/Fortran/Python | Modular ocean-atmosphere model |
| JuliaOcean/Climatology.jl | 20 | Julia | Ocean climatology |
| JGCRI/xanthos | 38 | Python | Global hydrologic framework |

---

## The Ocean-Adjacent Repositories Worth Watching (v3 — Detailed)

### 1. roocs/clisops — Climate Simulation Operations

- **URL:** https://github.com/roocs/clisops
- **Language:** Python
- **Focus:** Utilities for processing, regridding, and analyzing climate model output — the "plumbing" of climate data pipelines
- **Latest:** Sep 8, 2026 (dependabot bumps), Jul 15, 2026 (documentation fix), Jul 7, 2026 (v0.18.1 release)

**Fresh Commit Evidence (v3):**

| Date | Commit | Author | Significance |
|------|--------|--------|-------------|
| Sep 8, 2026 | Bump httpx2 from 2.5.0 to 2.12.0 | github-actions[bot] | Dependency update |
| Sep 8, 2026 | Bump httpx2 (second PR) | dependabot[bot] | Dependency update |
| Sep 8, 2026 | Bump pip from 26.1.2 to 26.2 | github-actions[bot] | Python version update |
| Sep 8, 2026 | Bump pip (second PR) | dependabot[bot] | Python version update |
| Sep 1, 2026 | Bump pygments from 2.19.1 to 2.20.0 | github-actions[bot] | Dependency update |
| Sep 1, 2026 | Bump pygments (second PR) | dependabot[bot] | Dependency update |
| Jul 15, 2026 | Fix regrid documentation | Martin Schupfner | **Only substantive human commit — documentation fix on regrid functionality** |
| Jul 7, 2026 | Prepare version 0.18.1 | Trevor James Smith | Version release |
| Jul 7, 2026 | Bullet version: 0.18.0 → 0.18.1 | Trevor James Smith | Patch release |

**Key Insight:** 6 out of 10 recent commits are dependabot dependency bumps. The only substantive human contribution in the recent history is a documentation fix on the `regrid` functionality (Jul 15, 2026). The v0.18.1 release (Jul 7, 2026) suggests active maintenance.

**Why This Matters for Ocean Geoengineering:** clisops is the climate data pipeline tool that would process output from ocean geoengineering simulations. If someone built an OAE module in Oceananigans.jl, they'd need clisops-style tools to regrid the output, analyze the results, and compare against observations. The regrid documentation fix is specifically relevant — regridding is how you map simulation output onto observation grids for comparison.

### 2. NOAA-GFDL/MDTF-diagnostics — The Ocean-Adjacent Tool

- **URL:** https://github.com/NOAA-GFDL/MDTF-diagnostics
- **Fresh Activity:** Aug 14, 2026 — PR #825 merged (Aparna Radhakrishnan). Jun 19, 2026 — MCS precipitation-buoyancy POD (5 commits in 1 day by Wei-Ming Tsai).

**Why This Matters:** The precipitation-buoyancy POD is the closest thing to ocean process diagnostics in open source. It evaluates how convective dynamics respond to buoyancy perturbations — directly relevant to marine cloud brightening (MCB), where you'd want to verify that cloud brightening is actually changing precipitation patterns.

### 3. WRF — The Atmosphere-Ocean Coupled Model

- **URL:** https://github.com/wrf-model/WRF
- **Fresh Commit Evidence (v3):** 10 commits, May-Jun 2026

| Date | Commit | Significance for Ocean |
|------|--------|------------------------|
| May 27, 2026 | MYNN-EDMF update | **Ocean boundary layer physics** — air-sea coupling improves |
| May 28, 2026 | Solar radiation EOT correction | **Solar radiation forcing** — drives sea surface temperature |
| Jun 5, 2026 | TEMPO aerosol options off | **Aerosol deposition** — affects ocean nutrient cycling |

**Why This Matters:** WRF's ocean boundary layer physics (MYNN-EDMF) is the atmospheric model's interface with the ocean. Any ocean intervention would need to account for how the atmosphere responds — and WRF is where that coupling happens. The solar radiation correction affects sea surface temperature calculations, which drive ocean dynamics.

### 4. PCMDI/pcmdi_metrics — The Evaluation Infrastructure

- **URL:** https://github.com/PCMDI/pcmdi_metrics
- **Fresh Activity:** v4.2.1 (Sep 3-4, 2026) — 10 commits in 2 days by Jiwoo Lee at LLNL, PRs from James Goodnight and Jared Lewis.

**Why This Matters:** If an ocean intervention is deployed, we need tools to evaluate whether it worked. PCMDI's metrics framework (v4.2.1) provides the evaluation infrastructure. ENSO, sea ice, ocean heat content — the key variables that ocean interventions would affect.

---

## What's MISSING: The Ocean Intervention Layer

| Missing Category | Why It Matters | Nearest Existing Tool |
|-----------------|----------------|----------------------|
| OAE simulation module | Core tool for ocean alkalinity enhancement modeling | Oceananigans.jl (platform exists, no module) |
| Iron fertilization model | Needed for SNAPI/LOHAFEX-type simulations | OceanBioME (biogeochemistry exists, no Fe module) |
| Artificial upwelling model | Needed for nutrient pump simulations | veros (ocean dynamics exist, no upwelling forcing) |
| Marine cloud brightening tool | Needed for MBC simulation/evaluation | MDTF-diagnostics (precipitation-buoyancy POD) |
| Ocean pH/alkalinity sensor designs | DIY hardware for monitoring experiments | ZERO (unlike OpenAir-Cyan for DAC) |
| Ocean intervention governance tool | Regulatory mapping like srm-forever | ZERO |
| Climate data pipeline for ocean interventions | Processing and regridding of simulation output | clisops (v0.18.1, active but not ocean-specific) |

---

## The Ocean-Adjacent Simulation Stack — What Exists vs. What's Missing

| Layer | Tool | Status | Fresh Evidence |
|-------|------|--------|---------------|
| Ocean physics | Oceananigans.jl (1,413★) | World-class, VERY active | 10 commits/3 days (Sep 2026); Lagrangian particles; immersed boundaries |
| Ocean dynamics (Python) | veros (400★) | Maintained | Dependabot bumps; Dion's isoneutral mixing bugfix |
| Biogeochemistry | OceanBioME.jl (80★) | VERY active | 10 commits/4 days; gas exchange parameterization active |
| Climate data ops | clisops (25★) | Maintained | v0.18.1 release; regrid documentation fix |
| Atmospheric model | WRF (1,761★) | World-class | v4.8.0; ocean boundary layer physics; solar radiation fix |
| Model evaluation | PCMDI metrics (133★) | Active | v4.2.1 2-day burst release |
| Process diagnostics | MDTF-diagnostics (80★) | Active | MCS precipitation-buoyancy POD |
| **Ocean intervention design** | **None** | **Complete gap** | **No OAE/iron/fertilization/upwelling modules exist** |
| Ocean sensor design | **None** | **Complete gap** | **No DIY ocean sensor hardware exists** |
| Ocean governance | **None** | **Complete gap** |

**The podcast thesis (Updated v3):** The ocean climate modeling stack is 80% built. Climate simulation operations tools like clisops (v0.18.1) provide the data pipeline. Oceananigans.jl provides the physics engine. PCMDI provides the evaluation framework. But the intervention layer — the "what happens when you add alkalinity to the ocean" layer — is 0% built. The ocean gap is specifically in the application layer, not the infrastructure layer.

---

## Why the Gap? (Updated v3)

| Hypothesis | Evidence | Confidence |
|------------|----------|------------|
| **Institutional gatekeeping** | Ocean science is dominated by WHOI, Scripps, GEOMAR — institutions that publish in closed journals and share through institutional channels; clisops (25★) is Python but maintained by a small community, not a major institution | HIGH |
| **Governance/regulatory risk** | London Protocol directly regulates ocean fertilization; transboundary impacts create legal risk; no ocean intervention governance tool exists on GitHub | MEDIUM-HIGH |
| **Experimental complexity** | Ship time $50K+/day; sensor deployments need multi-year monitoring; international coordination required; zero DIY ocean sensor projects (vs. OpenAir-Cyan for DAC) | HIGH |
| **Cultural mismatch** | Ocean science predates open-source movement by decades; researchers are at sea, not at keyboards; clisops regrid fix by a single contributor (Martin Schupfner) suggests small community | HIGH |
| **No market incentive** | Unlike DAC (where $1000/ton target creates incentive), ocean intervention has no commercial impetus; no ocean intervention repos in the August 2026 wave either |
| **The "stack is built but nobody built the app" problem** | Oceananigans.jl is a world-class physics engine (1,413★, 10 commits/3 days). OceanBioME is actively developing gas exchange. clisops provides data pipelines. But nobody wrote the OAE module. It's like having a physics engine but no video game. | HIGH |

---

## The Nearest Feasible Starting Points (Updated v3)

1. **An Oceananigans.jl OAE module** — The platform exists with 1,413 stars and active development. Adding an alkalinity amendment module is tractable for a focused research project. A grad student could do this in a summer.

2. **OceanBioME gas exchange for OAE** — OceanBioME is actively developing gas exchange parameterization (Sep 2026: 10 commits in 4 days, PRs #399, #411, #419). An OAE-specific gas exchange module would be a natural next step.

3. **A clisops-based ocean intervention data pipeline** — clisops provides regrid, regridding, and analysis tools (v0.18.1, Jul 2026). An ocean-intervention-specific regridding module could plug into this infrastructure.

4. **DIY ocean sensor designs** — Like OpenAir-Cyan for DAC, shareable pH/alkalinity/pCO2 sensor designs for ocean monitoring. No equivalent exists. The ocean needs its own OpenAir-Cyan.

5. **Ocean intervention governance tool** — Like srm-forever for SRM, an interactive regulatory mapping tool. No equivalent exists.

**The nearest feasible starting point (Updated v3):** An Oceananigans.jl OAE module. The physics engine exists. The developers are active (10 commits in 3 days). The gap is in the intervention layer. And clisops (v0.18.1) provides the data pipeline you'd need to process the output.

---

## 🎙️ Episode Hooks (Updated v3)

1. **The ocean is the silence that speaks loudest.** Zero geoengineering repos, zero ocean intervention tools. Meanwhile, the atmosphere gets WRF, PCMDI, and MDTF. The ocean gets... climate simulation operations tools (clisops) and world-class physics engines (Oceananigans). But no intervention layer at all.

2. **Oceananigans.jl is the platform the ocean needs.** 1,413 stars, 10 commits in 3 days, world-class Julia code. But it models ocean physics — not ocean intervention. The gap is specifically in the "what happens when you intervene" layer.

3. **OceanBioME's gas exchange work is the most relevant code in the ocean quadrant.** Three PRs in four days (Sep 15-17) on air-sea gas exchange — the core process for ocean alkalinity enhancement. The science is ready; the intervention layer isn't built.

4. **clisops is the hidden infrastructure story.** Climate simulation operations — regridding, data processing, analysis — at v0.18.1 (Jul 2026). Small repo (25★), but the regrid documentation fix (Jul 15) is the kind of tool you'd need to compare ocean intervention output against observations. The plumbing exists; the fixtures haven't been installed.

5. **WRF just fixed its ocean boundary layer physics.** The MYNN-EDMF update (May 27, 2026) improves air-sea coupling in the atmosphere model. The solar radiation EOT fix (May 28) affects sea surface temperature calculations. These are ocean-relevant improvements to an atmospheric model — the coupling layer that ocean interventions would interact with.

6. **The August 2026 carbon wave highlights the ocean's silence.** While 6 carbon capture repos updated in 5 days, ZERO ocean repos updated at all — not even the ocean-adjacent ones. Oceananigans was quiet in August 2026. OceanBioME was quiet. The ocean quadrant is completely silent.

7. **The ocean needs its own OpenAir-Cyan.** hardware designs for ocean sensors — pH, alkalinity, pCO2 — shared openly for monitoring experiments. No equivalent to the DIY DAC hardware movement exists for ocean science.
