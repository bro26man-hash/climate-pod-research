# ☀️ Solar Geoengineering — Technical Deep Dive

## Model Architectures

### ClimateMARGO.jl (Julia)
- **Type:** Idealized climate-economic integrated assessment model (IAM)
- **Core approach:** Optimizes trade-offs between mitigation, adaptation, and geoengineering using Julia's JuMP optimization interface
- **Key features:**
  - Climate module simplified energy balance model
  - Economic module with damage functions
  - Geoengineering module with stratospheric aerosol injection (SAI) parameterized
  - Pluto.jl notebooks for interactive exploration
- **Limitations:** Idealized — not a full GCM. No interactive radiation scheme, no ocean coupling

### Geo-DICE (MATLAB)
- **Type:** Modified DICE model with explicit geoengineering module
- **Core approach:** Adds SRM as a control variable in the DICE optimal growth framework
- **Key features:**
  - Carbon cycle + climate module from original DICE
  -SRM effectiveness parameterized as a function of emission reductions
  - Welfare function includes SRM benefits and costs
- **Limitations:** DICE is highly simplified (1-box ocean, no spatial dimensions). MATLAB license barrier.

### GCCS-Core (Python)
- **Type:** End-to-end climate control system simulation framework
- **Core approach:** Modular pipeline — data collection → processing → simulation → output
- **Key features:**
  - Data collection scripts (shell + Python)
  - Setup and training pipelines
  - README-driven architecture (documentation as design)
- **Limitations:** No actual climate simulation code visible in commits. The 10-commit burst created infrastructure, not models.

---

## What's Missing in Open-Source SRM

1. **No interactive atmospheric models** — No open-source equivalent of CESM, E3SM, or GISS ModelE with SRM modules
2. **No coupled ocean-atmosphere SRM models** — SAI affects ocean chemistry; no open-source model captures this
3. **No regional precipitation models** — SRM's most dangerous side effect (boundary droughts) has no dedicated simulation tool
4. **No ensemble frameworks** — ClimateMARGO is a single model; no probabilistic SRM assessment exists in open source
5. **No data assimilation** — No open-source system to constrain SRM models with observations

---

## Emerging Trends

- **Julia is gaining ground** in climate-econ integration (ClimateMARGO, ClimateBMI, others) — Julia's multiple dispatch and GPU support make it ideal for parameterized physics
- **Governance modeling** is the next frontier — OOCC and similar projects represent a shift from "can we model SRM?" to "should we model SRM?"
- **Curated lists beat built tools** — awesome-geoengineering's sustained maintenance vs. model dormancy suggests the community values orientation over computation
- **Second-order effects** are getting attention — geomalaria opens the question of whether SRM models need to include ecological and health impacts

---

## References & Further Reading
- DICE model origin: Nordhaus, 1992, *Science*
- SAI simulation approaches: National Academies, 2015, *Climate Intervention: Reflecting Sunlight to Cool Earth*
- Julia for climate: ClimateUART, ClimateBMI projects
- Governance frameworks: The Oxford Geoengineering Program, Large-scale Complex Infrastructure Systems (LSCIS)
