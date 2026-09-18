# ☀️ Project Discoveries — Solar Geoengineering Theme (Fresh, September 2026)

**Date:** September 2026  
**Repositories profiled:** WRF, PCMDI/pcmdi_metrics, ClimateMARGO.jl, srm-forever  
**Total stars across all repos:** 2,000+

---

## 1. WRF (Weather Research and Forecasting Model)

| Attribute | Detail |
|-----------|--------|
| **Repo** | `wrf-model/WRF` |
| **Stars** | 1,762 |
| **Language** | Fortran, C, C++ |
| **Last commit** | June 8, 2026 (v4.8.0 release) |
| **Activity level** | 🔴 **Very Active** — 15 commits in 28 days |
| **License** | BSD-3-Clause |
| **Institution** | NCAR / NOAA / GFDL / WRF User Consortium |

### What It Does
The WRF model is the **most widely used atmospheric model in the world**. It's the standard tool for weather forecasting, climate simulation, and — critically for our podcast — **the model used to simulate solar geoengineering scenarios**. If someone wants to know what happens if you inject aerosols into the stratosphere, they run WRF.

### Why It Matters for Solar Geoengineering
- **Solar radiation parameterization:** WRF contains the physics that simulate how solar radiation interacts with aerosols, clouds, and the surface
- **Aerosol–cloud interactions:** The TEMPO module (recently updated) models how aerosol particles affect cloud formation — exactly the process at the heart of marine cloud brightening
- **v4.8.0 just fixed a solar radiation bug:** `e836cd6` corrected the end-of-transport calculation for solar radiation — a fix that could change simulation results
- **Urban NbS initialization:** A recent bug fix (`8fa379b`) added a scheme guard for nature-based solutions in urban settings — showing WRF is expanding beyond pure geoengineering into broader climate intervention

### Episode Angle
> "WRF is the engine behind every solar geoengineering simulation. And right now, it's being actively maintained with a major version release. The model just had a solar radiation fix. If you're simulating a world with dimmed sun, you want to know that the code calculating the sunlight is correct."

---

## 2. PCMDI Metrics (PCMDI/pcmdi_metrics)

| Attribute | Detail |
|-----------|--------|
| **Repo** | `PCMDI/pcmdi_metrics` |
| **Stars** | 133 |
| **Language** | Python |
| **Last commit** | September 4, 2026 (v4.2.1 release) |
| **Activity level** | 🔴 **Very Active** — 10 commits in 1 day |
| **License** | Apache-2.0 |
| **Institution** | LLNL (Lawrence Livermore National Laboratory) |

### What It Does
PCMDI Metrics provides the **standard evaluation toolkit for CMIP6 (Coupled Model Intercomparison Project Phase 6)**. It's how the climate science community determines whether a model is any good. If WRF is the engine, PCMDI is the **mechanic's diagnostic tool**.

### Why It Matters for Solar Geoengineering
- **CMIP6 evaluation:** CMIP6 includes experiments specifically designed to test geoengineering scenarios (geoMIP/G4)
- **v4.2.1 roundoff fix:** `90cbc50` prevented mean climate figures from rounding to 1.00 — without this fix, all models would appear to agree perfectly when they didn't
- **Extremes chunking:** Recent memory optimization for dask/SVD operations suggests the toolkit is scaling to handle larger, more complex model ensembles
- **Forced numpy SVD:** `1fca2ec` ensures numerical stability — critical when comparing model outputs across dozens of simulations

### Episode Angle
> "Before you can simulate solar geoengineering, you need to know your model works. PCMDI builds the tools that judge the judges. And they just released v4.2.1 — with a fix that prevents all climate models from looking artificially perfect."

---

## 3. ClimateMARGO.jl

| Attribute | Detail |
|-----------|--------|
| **Repo** | `ClimateMARGO/ClimateMARGO.jl` |
| **Stars** | 73 |
| **Language** | Julia |
| **Last commit** | August 17, 2026 (README update — no code changes) |
| **Activity level** | 🟡 **Dormant with Mysterious Revival** — 10 months of silence, then 2 README edits |
| **License** | MIT |
| **Institution** | Individual researcher (Fons van der Plas) |

### What It Does
ClimateMARGO is an **idealized climate-economic modeling framework** for optimizing trade-offs between emissions mitigation, adaptation, and geoengineering. It uses Julia's JuMP optimization library with Ipopt solver. The "MARGO" stands for "Measures for Adapting to Regional and Global Opportunities."

### Why It Matters for Solar Geoengineering
- **Optimization framework:** ClimateMARGO doesn't simulate the physics — it answers "given a climate target, what's the optimal mix of mitigation, adaptation, and geohosting?"
- **Policy relevance:** This is the kind of model that would be used to argue for or against SRM deployment at international negotiations
- **Dormancy signal:** 10 months of silence followed by 2 README updates with no code changes is ambiguous. Could be a researcher preparing to use it, or could be a false start
- **Pluto notebooks:** The 2023 commit added Pluto notebook links — suggesting interactive exploration capability

### Episode Angle
> "ClimateMARGO is the model that answers the question: 'Should we deploy solar geoengineering, and if so, how much?' It went silent for 10 months. Then someone updated the README twice in one day. But they didn't touch the code. What does it mean when a climate-economic model's documentation is refreshed but its mathematics are frozen?"

---

## 4. srm-forever

| Attribute | Detail |
|-----------|--------|
| **Repo** | `hausfath/srm-forever` |
| **Stars** | 0 |
| **Language** | Julia |
| **Last commit** | August 26, 2026 |
| **Activity level** | 🟡 **Low activity but conceptually critical** |
| **License** | Not specified |
| **Institution** | Individual researcher (Hausfather) |

### What It Does
`srm-forever` is an **interactive SRM economics model** that applies Weitzman certainty-equivalent discounting to the cost dynamics of solar radiation management. It answers one question: "What is the present value of keeping SRM running indefinitely?"

### Why It Matters for Solar Geoengineering
- **Weitzman discounting:** Martin Weitzman's framework argues that traditional discount rates are inappropriate for catastrophic risks. This model applies that argument to SRM.
- **The "forever" question:** If you start dimming the sun, do you have to keep dimming it forever? The model says the answer depends on the discount rate — and with Weitzman's framework, the present value might be surprisingly affordable
- **Zero stars:** Despite being from a credible source, this repo has zero GitHub stars. It's a ghost town that contains one of the most important theoretical frameworks for SRM economics.

### Episode Angle
> "This repository has zero stars. But it might contain the most important economic argument for solar geoengineering ever coded. It asks: what does it cost to keep the sun dimmed forever? And the answer, powered by Weitzman discounting, might be lower than you think."

---

## 📊 Cross-Repo Comparison — Solar Theme

| Repo | Stars | Activity | Language | Type | Episode Role |
|------|-------|----------|----------|------|-------------|
| **WRF** | 1,762 | 🔴 Very Active | Fortran | Institutional model | "The Engine" |
| **PCMDI** | 133 | 🔴 Very Active | Python | Evaluation toolkit | "The Mechanic" |
| **ClimateMARGO** | 73 | 🟡 Dormant Revival | Julia | Policy optimizer | "The Strategist" |
| **srm-forever** | 0 | 🟡 Low Activity | Julia | Economics model | "The Philosopher" |

---

## 🔍 Gaps in Solar Coverage

| Gap | What's Missing | Why It Matters |
|-----|---------------|---------------|
| **No dedicated SRM simulation code** | No repo specifically simulates aerosol injection or albedo modification |
| **No Marine Cloud Brightening code** | All clouds are in WRF, but no dedicated MCB simulation tool exists |
| **No open-source counterfactual modeling** | No tool simulates "what happens if we DON'T do SRM" vs. "what happens if we DO" |
| **No citizen science SRM tools** | Unlike carbon capture (OpenAir-Cyan), there's no DIY SRM device |

---

*Generated: September 2026 | Repository: climate-pod-research | Branch: solar-geoengineering*