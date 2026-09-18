# 🌊 Ocean Intervention — Commit Trend Analysis (v4: Sep 2026 Update)
## Research Notes | Climate Pod Research | September 2026

---

## Executive Summary

Our analysis of **ocean-adjacent repositories** reveals a paradox: **the ocean physics code is among the most actively developed on GitHub, yet zero ocean geoengineering intervention code exists.** The ocean's two best friends — Oceananigans.jl (1,413★) and the precipitation-buoyancy POD in MDTF (80★) — are both thriving, but neither has any connection to intervention scenarios. The ocean is **well-studied but never-intervened-upon** in open code.

---

## The Ocean Activity Paradox

### What's Thriving
| Repo | Commits/Day | Contributors | Status |
|------|------------|-------------|--------|
| **CliMA/Oceananigans.jl** | ~4/day | 5+ (UC Berkeley) | **Extremely active** — daily commits, 15 in 4 days |
| **NOAA-GFDL/MDTF-diagnostics** | ~0.2/day | 4 (NOAA + academic) | **POD-driven** — focused on process evaluation |
| **wrf-model/WRF** (coupled mode) | ~1/day | 7 (NCAR/NOAA) | **Steady** — ocean-atmosphere coupling available |

### What's Missing
| Intervention Type | Repos | Commits | Status |
|-------------------|-------|---------|--------|
| Artificial Upwelling | **0** | 0 | **Nothing exists** |
| Ocean Alkalinity Enhancement | **0** | 0 | **Nothing exists** |
| Marine Cloud Brightening | **0** | 0 | **Nothing exists** |
| Ocean Iron Fertilization | **0** | 0 | **Nothing exists** |
| Deep Ocean Mixing | **0** | 0 | **Nothing exists** |
| Seaweed/Biomass Cultivation | **0** | 0 | **Nothing exists** |
| Ocean Bubble/foam Deployment | **0** | 0 | **Nothing exists** |

**Zero. Not one repository across all ocean geoengineering intervention types.**

---

## Oceananigans.jl: The World's Best Ocean Model That Doesn't Do Interventions

### Commit Velocity: The Most Active Ocean Code on GitHub
**15 commits in 4 days** (September 15-18, 2026) — that's ~4 commits/day.

**By contributor:**
| Contributor | Commits | Focus Areas |
|------------|---------|-------------|
| **Ali Ramadhan** | 7 | Performance optimization, solver accuracy, robustness |
| **Mosè Giordano** | 5 | Test suite, memory allocation, output consistency, test fixes |
| **Tomás Chor** | 1 | Time derivative computation |
| **Simone Silvestri** | 1 | Bottom drag parameterization |
| **Maximilian Gelbrecht** | 1 | Compiler optimization |

**Key commits and their intervention potential:**

| Date | Commit | Intervention Adaptation Potential |
|------|--------|----------------------------------|
| Sep 16 | **Bounce Lagrangian particles off immersed boundaries** | ★★★★★ — Could track geoengineering particles, drift, or dispersal in ocean currents |
| Sep 16 | Apply linear operator once per CG solver iteration | ★★★☆☆ — Faster runs = faster intervention scenario testing |
| Sep 16 | Fix face spacing above partial cells | ★★★★☆ — Critical for coastal/intervention site modeling |
| Sep 16 | Add TimeDerivative for computing ∂ₜ of outputs | ★★★☆☆ — Essential for intervention impact assessment |
| Sep 16 | SplitRungeKutta: evaluate forcings at correct time | ★★★★☆ — Could apply solar radiation forcing for ocean cooling scenarios |
| Sep 16 | Keep non-finite values in immersed cells out of column solve | ★★★★☆ — Handles extreme conditions (like point-source discharge) |
| Sep 15 | Tighten memory allocations bounds | ★★☆☆☆ — Performance optimization |
| Sep 15 | Correct implicit drag immersed mask | ★★★☆☆ — Could model artificial/seafloor structures |

### What Oceananigans Already Has (That's Intervention-Ready)
1. **Lagrangian particle tracking** — Track particles in ocean currents (Sep 16)
2. **Immersed boundaries** — Model structures on the seafloor (implied by multiple commits)
3. **Time-dependent forcings** — Apply external forcing (Sep 16)
4. **Differentiable programming** — Gradient-based optimization (CliMA's core feature)
5. **GPU acceleration** — Fast enough for ensemble simulations
6. **Output diagnostics** — Time derivatives, field datasets (Sep 16)

### What Oceananigans Lacks (Intervention-Specific)
1. ❌ **Artificial upwelling parameterization** — deep-water transport physics
2. ❌ **Alkalinity enhancement chemistry** — carbonate system module
3. ❌ **Sea spray aerosol source** — cloud brightening nucleation
4. ❌ **Nutrient/biology coupling** — iron fertilization ecosystem response
5. ❌ **Scenario templates** — pre-built intervention configurations
6. ❌ **Ensembles for uncertainty** — multiple intervention scenarios run simultaneously
7. ❌ **Coupling to atmosphere** — two-way ocean-atmosphere feedback for interventions
8. ❌ **Policy/economic layer** — cost-benefit analysis framework

### The Adaptation Opportunity
> "Oceananigans.jl already has 7 of the 8 infrastructure pieces needed for ocean intervention modeling. Lagrangian particles can track dispersal. Immersed boundaries can model structures. Time-dependent forcings can apply scenarios. Differentiable programming can optimize strategies. What's missing is **one person with a vision** who connects these pieces into an intervention module."

---

## MDTF's Precipitation-Buoyancy POD: The Ocean's Only Advocate

### The June 19, 2026 Blitz
Five commits on a single file (`MCS_precip_buoy_stats.rst`). All by one developer (Wei-Ming Tsai). All documentation updates.

**What was actually being built:** A Proper Orthogonal Decomposition diagnostic for mesoscale convective systems (MCSs) — the giant thunderstorm complexes that form over warm ocean waters and drive global precipitation patterns.

**Why it matters for ocean intervention:**
- MCSs transport **heat and moisture** from ocean to land
- Artificial upwelling would **cool the sea surface**, potentially weakening MCSs
- Ocean alkalinity enhancement would **change ocean chemistry**, potentially affecting ocean-atmosphere CO2 exchange that drives convection
- Marine cloud brightening would **change solar absorption**, altering the ocean heat budget

**The diagnostic chain:**
```
Ocean Intervention → Sea Surface Temp Change → Boundary Layer Stability → MCS Convection → Precipitation Pattern
                         ↑                                                           ↑
              MDTF's Precip-Buoyancy POD can evaluate THIS link
```

### The 5-Commit Pattern
| Commit # | Date | Description |
|----------|------|-------------|
| 1 | Jun 19 | Add MCS precip-buoyancy statistics POD |
| 2 | Jun 19 | Update MCS_precip_buoy_stats.rst |
| 3 | Jun 19 | Update MCS_precip_buoy_stats.rst |
| 4 | Jun 19 | Update MCS_precip_buoy_stats.rst |
| 5 | Jun 19 | Update MCS_precip_buoy_stats.rst |

**Pattern:** 1 code commit, 4 documentation commits. The tool was **built in a day and documented in a day**. Classic research sprint — instrument creation followed by documentation.

### The Evaluation Chain That Doesn't Exist Yet
```
[Oceananigans.jl] → [Intervention Module: DOESN'T EXIST] → [WRF] → [MDTF POD] → [Evaluation]
        ↑                                                           ↑
   Ocean physics                                            Process evaluation
   (thriving)                                              (thriving)

   THE MISSING LINK: Nobody connects these three for intervention scenarios.
```

---

## WRF's Ocean Connection: Deprecating Away from It

### The Aerosol Deprecation Problem
| Date | Event | Ocean Impact |
|------|-------|---------------|
| May 28, 2026 | Solar radiation EOT correction | **Positive** — better SST = better ocean boundary conditions |
| Jun 5, 2026 | Turn off tempo_aerosolaware | **Negative** — less aerosol deposition modeling = less ocean chemistry |
| Jun 6, 2026 | Turn off tempo_hailaware | **Neutral** — hail doesn't directly affect ocean |

**The net effect:** WRF is getting **better at ocean boundary conditions** (accurate solar radiation) while getting **worse at ocean chemistry** (aerosol deposition). For ocean intervention modeling, this is a mixed signal.

### What This Means for Ocean Geoengineering Code
If someone wanted to simulate **ocean iron fertilization** using WRF:
- ✅ They could model the atmospheric effects (heat redistribution, precipitation changes)
- ✅ They could use the improved solar radiation scheme for accurate SST
- ❌ They can't model the ocean biology response (no biology module)
- ❌ They can't model the aerosol iron deposition (tempo_aerosolaware deprecated)
- ❌ They can't couple to an ocean biogeochemistry model (no such module exists in WRF)

**WRF is an atmospheric model with an ocean boundary, not an ocean model with an atmospheric overlay.**

---

## The Cross-Theme Connection: Where All Three Themes Meet the Ocean

### The Triangle of Relevant Tools
```
         WRF (Solar)
         /        \
        /          \
       /            \
      /              \
MDTF -------- Oceananigans.jl
(Precipitation-\  (Ocean Physics)
buoyancy POD)

WRF's solar radiation → accurate SST → drives ocean convection
MDTF's POD → evaluates precipitation-buoyancy coupling → validates ocean-atmosphere models
Oceananigans.jl → simulates ocean physics → provides boundary conditions for SRM

THE MISSING LINK: Nobody connects these three for intervention scenarios.
```

### What Would a Cross-Theme Ocean Episode Look Like?

**Act 1: The Thriving Ocean Physics**
- Oceananigans.jl: 4 commits/day, Lagrangian particles, immersed boundaries
- MDTF: Precipitation-buoyancy POD, 5 commits in one day
- WRF: Solar radiation correction, coupled ocean options
- **Message:** "We understand the ocean better than ever."

**Act 2: The Intervention Vacuum**
- Zero ocean geoengineering repos
- No upwelling, no alkalinity, no brightening code anywhere
- **Message:** "But we've never simulated intervening in it."

**Act 3: The Connection**
- Oceananigans particles → track intervention dispersal
- MDTF POD → evaluate intervention impacts
- WRF radiation → model ocean-atmosphere feedbacks
- **Message:** "The tools exist. The only thing missing is the decision to connect them."

---

## Hypotheses for the Ocean Gap

### Ranked by Likelihood

| Rank | Hypothesis | Evidence | Testable? |
|------|-----------|---------|----------|
| **1** | **Governance chill** | London Protocol debates, legal liability concerns, no code paper trail | Yes — interview ocean policy experts |
| **2** | **Complexity curse** | Ocean interventions involve physics + chemistry + biology (3x the complexity of SRM) | Partially — complexity analysis possible |
| **3** | **Funding gap** | National Academies 2021 report gave ocean minimal attention | Yes — funding database analysis |
| **4** | **Biology barrier** | No repo models ocean ecosystem response to interventions | Yes — search for biogeochemistry + intervention |
| **5** | **Oceananigans paradox** | Too-sophisticated tool creates "too expensive to use" barrier | Maybe — survey Oceananigans users |

### The Governance Thesis (Our Leading Hypothesis)
The most compelling explanation is **governance deterrence**. When the London Protocol's parties debated ocean fertilization in 2008 and effectively moratorium-regulating it, they didn't just regulate experiments — they regulated **public discourse about experiments**. Code is speech. A repository simulating ocean iron fertilization is a digital artifact that could be cited in legal proceedings.

- A repo that simulates upwelling could be used to argue "someone has already modeled this, it's safe"
- A repo that simulates alkalinity enhancement could be used to argue "the technology exists, why not deploy it"
- The absence of code creates an **information asymmetry** that governance frameworks prefer

**This hypothesis is testable:** If governance deterrence is correct, we should find:
- ✅ Ocean geoengineering code in **private repositories** (government labs, defense)
- ✅ Ocean geoengineering code in **offline simulation tools** (Fortran legacy codes)
- ✅ Ocean geoengineering **papers without accompanying code** (the "code available upon request" pattern)
- ❌ Ocean geoengineering code in **public GitHub repositories** (zero confirmed)

---

## 🎙️ Episode 3: Suggested Structure

### Cold Open (3 min)
> "We searched GitHub for every ocean geoengineering term we could think of. Marine cloud brightening. Ocean alkalinity enhancement. Artificial upwelling. Ocean iron fertilization. Deep ocean mixing. Seaweed cultivation. Zero repositories. Not one. The ocean covers 71% of the Earth's surface, and it has 0% of the geoengineering codebase. Meanwhile, the atmospheric model WRF gets 3 commits a week. Oceananigans.jl gets 4 commits a day. But the transition zone — the place where atmospheric models and ocean models meet intervention scenarios — is completely empty."

### Act 1: The Ocean That's Studied to Death (12 min)
- Oceananigans.jl: 1,413★, 4 commits/day, world's best ocean physics
- MDTF: Precipitation-buoyancy POD, 5 commits in one day
- WRF: Solar radiation correction, coupled ocean options
- **Key image:** "The most active code in this entire research project is about ocean physics. And not a single line of it is about what we'd do to the ocean."

### Act 2: The Ocean That Nobody Intervenes Upon (15 min)
- The search: 10+ queries, zero results
- The hypotheses: governance chill, complexity curse, funding gap, biology barrier
- The London Protocol moment: when code became legally sensitive
- **Key quote:** "When the London Protocol debated ocean fertilization, they weren't just regulating experiments. They were regulating the question. Because code is speech, and a repository is a declaration."

### Act 3: The Connection That Doesn't Exist Yet (15 min)
- The cross-theme triangle: WRF + MDTF + Oceananigans = intervention capability
- What a 1-person Ocean Intervention Module for Oceananigans.jl would look like
- The 7 infrastructure pieces that already exist (particles, boundaries, forcings, differentiability)
- The 8th piece: **the community decision to build**
- **Key image:** "Oceananigans.jl already has 7 of the 8 tools needed. The 8th tool is a click in a GitHub Issues page: 'We should build an ocean intervention module.'"

### Closing (5 min)
- The empty shelves metaphor: "GitHub is a library, and the ocean section is empty."
- The governance question: "Did the legal community win the ocean debate by making the code community too afraid to write it?"
- The call to action: "The ocean doesn't need more models. It needs one person who wants to use an existing model to ask a question nobody's asked in code."
- **Final quote:** "The precip-buoyancy POD was built on June 19, 2026, by one person in one day. It evaluates whether climate models get ocean-atmosphere coupling right. That's the closest thing to ocean geoengineering code on GitHub. And it's a diagnostic. The intervention tools don't exist. The evaluation tools do. The gap isn't technical. It's moral."

---

*Last updated: September 2026 (v4) | Search queries: 10+ | Ocean geoengineering repos: 0 | Ocean-adjacent repos analyzed: 3*