# 🌊 Ocean Intervention — Project Discovery Catalog

**Last Updated:** September 2026
**Research Method:** GitHub repository search ("ocean fertilization", "ocean alkalinity enhancement", "marine geoengineering", "artificial upwelling", "seaweed carbon farming", "marine cloud brightening") + cross-reference with "awesome-open-climate-science" directory

---

## The Discovery Gap: ZERO Dedicated Ocean Geoengineering Repos

After exhaustive searching across 8+ query strategies (detailed in COMMIT-TRENDS-OCEAN.md):

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

## What DOES Exist: The Ocean Climate Modeling Ecosystem

### Tier 1: World-Class Ocean Models

| Repo | Stars | Language | Focus | Activity Level |
|------|-------|----------|-------|----------------|
| **CliMA/Oceananigans.jl** | 1,413 | Julia | Ocean fluid dynamics (CPU+GPU) | VERY HIGH (10 commits/3 days, Sep 2026) |
| **team-ocean/veros** | 400 | Python/JAX | Pure-Python ocean simulator | Moderate (dep bumps + occasional fixes) |
| **OceanBioME/OceanBioME.jl** | 80 | Julia | Ocean biogeochemistry & carbonate chemistry | VERY HIGH (10 commits/4 days, Sep 2026) |

### Tier 2: Supporting Infrastructure

| Repo | Stars | Focus |
|------|-------|-------|
| pangeo-data/awesome-open-climate-science | 598 | Curated list of open climate science tools |
| gaelforget/ClimateModels.jl | 47 | Julia interface to climate models |
| Climdyn/MAOOAM | 22 | Modular ocean-atmosphere model |
| JuliaOcean/Climatology.jl | 20 | Ocean climatology |

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

---

## The Ocean-Adjacent Repositories Worth Watching

### MDTF-diagnostics (NOAA-GFDL, 80★)
- **URL:** https://github.com/NOAA-GFDL/MDTF-diagnostics
- **Relevant work:** MCS precipitation-buoyancy statistics POD (Jun 2026)
- **Why it matters:** Process-oriented diagnostics that could be adapted for marine cloud brightening evaluation

### WRF (NCAR/NOAA, 1,761★)
- **URL:** https://github.com/wrf-model/WRF
- **Relevant work:** Ocean boundary layer physics (MYNN-EDMF), air-sea interaction modules
- **Why it matters:** The atmosphere-ocean coupling layer exists in WRF. An intervention module would need to interface with WRF's ocean physics.

### PCMDI/pcmdi_metrics (LLNL, 133★)
- **URL:** https://github.com/PCMDI/pcmdi_metrics
- **Relevant work:** ENSO, sea ice, ocean heat content metrics
- **Why it matters:** Evaluation infrastructure. If an ocean intervention is deployed, PCMDI-style metrics would verify its effects.

---

## Why the Gap?

| Hypothesis | Evidence | Confidence |
|------------|----------|------------|
| **Institutional gatekeeping** | Ocean science is dominated by WHOI, Scripps, GEOMAR — institutions that publish in closed journals and share through institutional channels | HIGH |
| **Governance/regulatory risk** | London Protocol directly regulates ocean fertilization; transboundary impacts create legal risk | MEDIUM-HIGH |
| **Experimental complexity** | Ship time $50K+/day; sensor deployments need multi-year monitoring; international coordination required | HIGH |
| **Cultural mismatch** | Ocean science predates open-source movement by decades; researchers are at sea, not at keyboards | HIGH |
| **No market incentive** | Unlike DAC (where $1000/ton target creates incentive), ocean intervention has no commercial impetus | MEDIUM |

---

## The Nearest Feasible Starting Points

1. **Oceananigans.jl OAE module** — The platform exists with 1,413 stars and active development. Adding an alkalinity amendment module is tractable for a focused research project.

2. **Veros-based OAE teaching tool** — Veros is pure Python and accessible. An interactive OAE simulator could democratize ocean intervention modeling.

3. **OceanBioME gas exchange for OAE** — OceanBioME is actively developing gas exchange parameterization (Sep 2026). An OAE-specific module would be a natural next step.

4. **DIY ocean sensor designs** — Like OpenAir-Cyan for DAC, shareable pH/alkalinity/pCO2 sensor designs for ocean monitoring. No equivalent exists.

5. **Ocean intervention governance tool** — Like srm-forever for SRM, an interactive regulatory mapping tool. No equivalent exists.

---

## 🎙️ Episode Hooks

1. **The ocean is the silence that speaks loudest.** Zero geoengineering repos, zero ocean intervention tools. Meanwhile, the atmosphere gets WRF, PCMDI, and MDTF. The ocean gets... nothing. That's the story.

2. **Oceananigans.jl is the platform the ocean needs.** 1,413 stars, 10 commits in 3 days, world-class Julia code. But it models ocean physics — not ocean intervention. The gap is specifically in the "what happens when you intervene" layer.

3. **OceanBioME's gas exchange work is the most relevant code in the ocean quadrant.** Three PRs in four days on air-sea gas exchange — the core process for ocean alkalinity enhancement. The science is ready; the intervention layer isn't built.

4. **The ocean gap is different from the carbon gap.** Carbon has OpenAir-Cyan (hardware) and literature surveys. Ocean has nothing — no hardware, no surveys, no interactive tools.

5. **The London Protocol may be causing self-censorship.** Unlike SRM (murky but not illegal), ocean fertilization is explicitly regulated. Researchers may avoid open-source code to avoid regulatory scrutiny.
