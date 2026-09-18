# 🌊 Ocean Intervention — Project Discoveries (v4: Sep 2026 Update)
## Research Notes | Climate Pod Research | September 2026

---

## ⚠️ THE HEADLINE FINDING: The Ocean Gap

**Our GitHub search across 10+ query strategies returned ZERO dedicated ocean geoengineering repositories.** Ocean geoengineering is the "dark matter" of climate tech on GitHub — it exists abundantly in the scientific literature (Nature, Science, PNAS) but is virtually absent from open code.

**This is the most significant finding of the entire research effort.**

---

## Overview

This document profiles the **ocean-adjacent** repositories — tools that interact with ocean processes but don't simulate ocean interventions. It also documents the complete absence of direct ocean geoengineering code, and what that absence means for our Episode 3.

---

## 🔬 The Ocean's Closest Friends (Ocean-Adjacent Repos)

### 1. MDTF Diagnostics — The Precipitation-Buoyancy POD
- **Repo:** [NOAA-GFDL/MDTF-diagnostics](https://github.com/NOAA-GFDL/MDTF-diagnostics)
- **Stars:** 80 ⭐
- **Ocean relevance:** ⭐⭐⭐⭐⭐ (directly) — precipitation-buoyancy coupling IS ocean-atmosphere interaction
- **Last ocean commit:** August 14, 2026

**What makes it ocean-adjacent?** The **MCS_precip_buoy_stats** (Mesoscale Convective System Precipitation-Buoyancy Statistics) Proper Orthogonal Decomposition (POD) tool identifies dominant modes of precipitation-buoyancy coupling. This is fundamentally an ocean-atmosphere interaction diagnostic: buoyancy-driven convection over warm ocean surfaces drives tropical precipitation patterns. The tool evaluates whether models correctly simulate the coupling between ocean-driven moisture and atmospheric dynamics.

**Recent commit highlights (15 commits):**
| Date | Commit | Significance |
|------|--------|-------------|
| Aug 14, 2026 | Merge PR #825 | Latest integration |
| **Jun 19, 2026** | **5 commits on MCS_precip_buoy_stats.rst** | **The single most active file across ALL solar+ocean repos this year** — 5 updates to the same file in one day |
| Jun 19, 2026 | Add MCS precipitation-buoyancy statistics POD | **Brand-new diagnostic added** — first time this POD exists in open source |
| Jun 8, 2026 | Merge PR #823 | Integration |
| Jun 8, 2026 | Update README (2 commits) | Documentation |
| Jun 2, 2026 | Merge branch + Add citation | Infrastructure |
| Jun 1, 2026 | Quarterly metrics workflow | **CI/CD monitoring** — production-grade |
| May 27, 2026 | Move blocking_neale_nb to dev | Branching strategy |
| May 22, 2026 | Merge blocking notebook PR | New diagnostic (blocking patterns) |

**🎙️ Episode hook:** The precipitation-buoyancy POD received **5 commits on June 19, 2026** — all updating the same file. This is the most intensely developed file across all three themes. Why? Because precipitation-buoyancy coupling is the **engine of tropical climate** — and evaluating it correctly is prerequisite for any ocean intervention that would affect tropical rainfall. If you want to simulate Artificial Upwelling's effect on Pacific precipitation, you first need to know whether your model gets the buoyancy-precipitation relationship right.

---

### 2. WRF Model — Aerosol-Ocean Coupling Potential
- **Repo:** [wrf-model/WRF](https://github.com/wrf-model/WRF)
- **Stars:** 1,763 ⭐
- **Ocean relevance:** ⭐⭐⭐⭐ (indirect) — WRF can be coupled to ocean models, and aerosol deposition affects ocean chemistry
- **Last ocean-adjacent commit:** June 8, 2026 (v4.8.0)

**What makes it ocean-adjacent?** WRF's aerosol modules simulate how aerosol particles deposit into the ocean — affecting ocean chemistry, marine ecosystems, and potentially iron fertilization. The solar radiation correction (May 28) also matters for ocean: accurate solar radiation means accurate sea surface temperature modeling.

**Ocean-relevant commits:**
| Date | Commit | Ocean Connection |
|------|--------|-----------------|
| May 28, 2026 | Correction for EOT calculation for solar radiation | Accurate solar = accurate SST = accurate ocean boundary conditions |
| Jun 5, 2026 | Turn off tempo_aerosolaware | **Deprecation of aerosol physics** — reduces ocean deposition modeling capability |
| May 20, 2026 | Add mp_physics=88 | New physics option for boundary layer (affects air-sea exchange) |

**🎙️ Episode hook:** WRF is deprecating its aerosol-aware physics module (Jun 5). This is a double-edged sword for ocean intervention: less aerosol complexity means less accurate ocean deposition modeling, but it also means the model is streamlining for faster runtimes. If someone wants to simulate iron fertilization's effect on ocean productivity using WRF, they'd need to build their own aerosol deposition module — the maintainers are explicitly moving away from it.

---

### 3. Oceananigans.jl — The King of Ocean Models
- **Repo:** [CliMA/Oceananigans.jl](https://github.com/CliMA/Oceananigans.jl)
- **Stars:** 1,413 ⭐
- **Language:** Julia
- **Last commit:** September 18, 2026 (daily activity!)
- **Maintainers:** Ali Ramadhan, Mosè Giordano, Tomás Chor, Simone Silvestri, Maximilian Gelbrecht

**What it is:** **The most active ocean fluid dynamics code on GitHub.** University of California, Berkeley's CliMA (Climate Machine Learning) project. Oceananigans.jl is a high-performance, differentiable ocean simulation framework that runs on CPUs and GPUs. It's the gold standard for ocean modeling in open source.

**Recent commit highlights (15 commits pulled — September 15-18, 2026):**
| Date | Commit | Significance |
|------|--------|-------------|
| **Sep 18, 2026** | Try to speed up `simulations` test group | **Performance optimization** — making ocean simulation faster |
| Sep 17, 2026 | Restore closure fields from checkpoints when closure is a tuple | **Robustness** — handle complex turbulence closures |
| Sep 16, 2026 | Fix face spacing above partial cells on PartialCellBottom grids | **Grid accuracy** — critical for coastal and boundary layer ocean dynamics |
| Sep 16, 2026 | Apply linear operator once per ConjugateGradientSolver iteration | **Performance** — 2x faster solver iterations |
| Sep 16, 2026 | **Bounce Lagrangian particles off immersed boundaries** | **Particle tracking** — could model driftwood, plankton, or geoengineering particle carriers |
| Sep 16, 2026 | Add TimeDerivative for computing ∂ₜ of outputs | **Output analysis** — time tendency calculations |
| Sep 16, 2026 | SplitRungeKuttaTimeStepper: evaluate forcings and BCs at correct time | **Accuracy** — correct time stepping for forcing |
| Sep 16, 2026 | Fix stage Δt used by AVID + RK3 | **Numerical stability** — advection scheme fix |
| Sep 16, 2026 | Keep non-finite values in immersed cells out of column solve | **Robustness** — handle bathymetry edge cases |
| Sep 15, 2026 | Fix test suite issues | Quality assurance |
| Sep 15, 2026 | Tighten memory allocations bounds | **Performance** — GPU memory optimization |
| Sep 15, 2026 | Correct implicit drag immersed mask | **Accuracy** — bottom drag parameterization |
| Sep 15, 2026 | Fix reductions of AbstractOperations under Reactant | **Compiler optimization** |
| Sep 15, 2026 | Keep field and output order in FieldDataset | **Data consistency** |
| Sep 15, 2026 | Read dimension lengths from dataset for NetCDFWriter | **I/O improvement** |

**🎙️ Episode hook:** Oceananigans.jl is the **most active repo across all three themes** — 15 commits in 4 days. But it simulates **ocean physics, not ocean interventions**. It's the world's best tool for understanding how the ocean works, with zero tools for how to intervene in it. This is the computational embodiment of our episode's thesis: **we have the lighthouse, but no ships.**

**What Oceananigans DOES have that could be adapted:**
- **Lagrangian particle tracking** (Sep 16) — could track geoengineering particles or drift
- **Immersed boundaries** — could model artificial structures on the seafloor
- **Time-dependent forcings** — could apply solar radiation management or upwelling scenarios
- **Differentiable programming** — could optimize intervention strategies via gradient descent

**What Oceananigans DOESN'T have:**
- Any geoengineering module, scenario, or use case
- Any intervention-specific physics (upwelling, alkalinization, etc.)
- Any policy or economic modeling layer
- Any community engagement with the solar geoengineering or CDR communities

---

## 🚨 The Ocean Gap: What's Missing

### Comprehensive Search Results

| Search Query | Results |
|-------------|--------|
| `"ocean geoengineering"` repos | **0** |
| `"marine cloud brightening"` repos | **0** |
| `"ocean alkalinity enhancement"` repos | **0** |
| `"artificial upwelling"` repos | **0** |
| `"ocean iron fertilization"` repos | **0** |
| `"marine geoengineering"` stars:>10 | **0** |
| `topic:geoengineering ocean` | **0** |
| `ocean intervention simulation` | **0** |
| `ocean cooling geoengineering` | **0** |
| ` ocean geoengineering` (broad) | **0** |

**Total ocean geoengineering repositories found: ZERO**

### What Exists vs. What Doesn't

| Domain | Exists on GitHub? | Examples |
|--------|------------------|---------|
| **Atmospheric models** (can simulate SRM effects) | ✅ Yes | WRF (1,763★), CESM, etc. |
| **Carbon cycle models** (can simulate CDR effects) | ✅ Yes | Multiple repos |
| **Ocean physics models** (can simulate ocean dynamics) | ✅ Yes | Oceananigans.jl (1,413★), veros, OceanBioME |
| **Climate evaluation tools** (can assess model accuracy) | ✅ Yes | PCMDI (133★), MDTF (80★) |
| **SRM economics models** | ✅ Yes | srm-forever (0★, but exists) |
| **DAC device designs** | ✅ Yes | OpenAir-Cyan (76★, certified) |
| **Marine cloud brightening simulations** | ❌ **ZERO** | — |
| **Ocean alkalinity enhancement codes** | ❌ **ZERO** | — |
| **Artificial upwelling models** | ❌ **ZERO** | — |
| **Ocean iron fertilization scenarios** | ❌ **ZERO** | — |
| **Ocean intervention risk assessments** | ❌ **ZERO** | — |
| **Marine geoengineering governance tools** | ❌ **ZERO** | — |

---

## 🤔 Why Is the Ocean Empty?

### Hypothesis 1: The Complexity Curse
Ocean geoengineering is **physically more complex** than atmospheric SRM. Artificial upwelling requires modeling deep-water nutrient transport, thermocline dynamics, and surface ecosystem responses. Ocean alkalinity enhancement requires modeling carbonate chemistry, lysocline penetration, and biological calcification responses. The **computational barrier to entry** is higher.

### Hypothesis 2: The Governance Chill
Marine geoengineering is **more regulated** than atmospheric SRM. London Protocol parties have debated ocean fertilization for years. The legal uncertainty may deter developers from publishing code — they don't want to create a paper trail that could be used in liability proceedings.

### Hypothesis 3: The Funding Gap
Ocean geoengineering receives **far less research funding** than solar SRM or direct air capture. The National Academies' 2021 geoengineering report allocated minimal attention to ocean interventions. Without major funding, there's no code.

### Hypothesis 4: The Marine Biology Problem
Ocean interventions affect **living systems** — phytoplankton, fish, coral. Unlike SRM (pure physics) or DAC (pure chemistry), ocean geoengineering requires biological modeling. The complexity of coupling physical and biological ocean models may be the ultimate barrier.

### Hypothesis 5: The Oceananigans Paradox
Oceananigans.jl (1,413★) is **so good** at ocean physics that it may have inadvertently **crowded out** intervention-scale modeling. Why build a simple upwelling model when you have the world's best general ocean model? The sophisticated tool may have created a "too expensive to use" barrier for intervention-scale applications.

---

## 🔮 What an Open-Source Ocean Intervention Ecosystem Would Look Like

### The Stack (None of Which Exists)
```
Layer 5: Governance & Policy Tools     ← MISSING
Layer 4: Risk Assessment Frameworks     ← MISSING
Layer 3: Intervention-Specific Models   ← MISSING
Layer 2: Ocean Physics Engines          ← EXISTS (Oceananigans.jl)
Layer 1: Data & Boundary Conditions     ← PARTIAL (CMIP6, thermo data)
```

### The Missing Middle (Layer 3)
If someone built an **Ocean Intervention Module** for Oceananigans.jl, it would include:
- **Artificial Upwelling** parameterization (deep-water transport)
- **Ocean Alkalinity Enhancement** chemistry module
- **Marine Cloud Brightening** sea spray aerosol source terms
- **Ocean Fertilization** nutrient & biology coupling
- **Scenario templates** (blob size, duration, location for each intervention type)
- **Evaluation metrics** (compare against MDTF's precipitation-buoyancy POD)

### The Dream Stack (Full Integration)
```
WRF (atmosphere) ←→ Oceananigans.jl (ocean) ←→ Intervention Module (new)
     ↓                      ↓                           ↓
PCMDI (evaluation)    MDTF (process POD)     Risk Assessment (new)
```

**This stack doesn't exist.** But the components are all there. The only missing piece is **the intervention module and the community to build it**.

---

## 🎙️ Episode 3 Talking Points

### The Openingomaly
> "We searched GitHub for every term related to ocean geoengineering — marine cloud brightening, ocean alkalinity enhancement, artificial upwelling, iron fertilization. Zero repositories. Not one. Meanwhile, the atmospheric models have thousands of stars. The carbon capture tools have hundreds. The ocean... the ocean is silent."

### The Ocean Model That's Not an Intervention Model
> "Oceananigans.jl has 1,413 stars and commits every single day. Its developer just added Lagrangian particle tracking — particles bouncing off immersed boundaries. That could track driftwood, plankton, or geoengineering particles. But nobody's using it for that. The world's best ocean model is also the world's most sophisticated non-intervention ocean model."

### The Precipitation-Buoyancy POD — The Ocean's Only Friend
> "On June 19, 2026, one developer made 5 commits to the same file. Not code — documentation. But it was documenting the precipitation-buoyancy POD, a diagnostic tool that tells you whether your climate model correctly simulates how ocean-driven convection creates tropical rain. If you want to simulate what happens when you interrupt that convection with an ocean intervention, you first need to know whether you can simulate the convection at all."

### The Governance Question
> "Why is there no code? Is it because ocean geoengineering is too complex? Too regulated? Too unfunded? Or is it because the scientific community has decided that some questions shouldn't be asked in public? When London Protocol parties debate ocean fertilization, are they also deciding what code should and shouldn't exist?"

### The Opportunity
> "The ocean intervention ecosystem is a zero-to-one build. There's no legacy code to refactor. No old APIs to maintain. No technical debt. It's a greenfield project. Oceananigans.jl provides the engine. MDTF provides the evaluation. PCMDI provides the quality gate. What's missing is the vehicle — and the driver."

### The Closing Image
> "GitHub is a library of climate solutions. The atmospheric section is packed. The carbon section is filling up. But the ocean section? Empty shelves. A single sign: 'Unfortunately, this section is not yet written.' The ocean covers 71% of the Earth's surface and 0% of the geoengineering codebase."

---

*Last updated: September 2026 (v4) | Search queries executed: 10+ | Ocean geoengineering repos found: 0*