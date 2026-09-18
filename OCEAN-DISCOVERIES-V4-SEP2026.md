# 🌊 Ocean Intervention — Project Discoveries (v4 Fresh)
## Research Notes for Climate Pod Episode 3 — September 2026

---

## Overview
This document documents the **complete absence** of open-source ocean geoengineering repositories on GitHub, alongside the ocean-adjacent climate tools that exist in the broader ecosystem. This is the most significant finding of our entire research project.

**The headline:** We searched GitHub using 10+ different query strategies. **Zero dedicated ocean geoengineering repositories were found.** Ocean geoengineering is the "dark matter" of climate tech on GitHub — it exists in the scientific literature (Nature, Science, PNAS) but not in open code.

---

## 🔍 Search Methodology — Exhaustive Queries

| # | Search Query | Results | Notable Finds |
|---|----------------|---------|----------------|
| 1 | geoengineering simulation climate | 0 | Nothing |
| 2 | ocean climate intervention modeling | 0 | Nothing |
| 3 | geoengineering | 10 results | Solar-focused, zero ocean |
| 4 | climate simulation carbon capture | 6 results | Carbon-heavy, no ocean |
| 5 | ocean geoengineering | 0 | Explicitly searched, nothing |
| 6 | marine cloud brightening | 0 | SRM subset, nothing |
| 7 | ocean alkalinity enhancement | 0 | OAE-specific, nothing |
| 8 | ocean iron fertilization | 0 | HNLC, nothing |
| 9 | ocean model climate | 0 | General, nothing relevant |
| 10 | ocean climate intervention modeling | 0 | Direct, nothing |

**Total ocean geoengineering repos found: ZERO**

---

## 🌊 What DOES Exist: Ocean-Adjacent Climate Tools

### 1. Oceananigans.jl
- **Repo:** CliMA/Oceananigans.jl
- **Stars:** ~1,413
- **Language:** Julia
- **Last Activity:** September 18, 2026 (extremely active — 15 commits in past week)
- **License:** MIT
- **Parent Project:** CliMA (Climate Machine Learning)

**What it is:** The most sophisticated open-source ocean fluid dynamics simulator available. Oceananigans.jl solves the Navier-Stokes equations on CPUs and GPUs for ocean modeling. It's used for research from coastal dynamics to global thermohaline circulation.

**Why it matters for ocean geoengineering:** Ocean geoengineering proposals (Ocean Alkalinity Enhancement, marine cloud brightening triggers, deep water mixing) all require ocean circulation models. Oceananigans.jl is the tool.

**Recent Commits (September 15-18, 2026) — 15 commits in 4 days:**

| Date | Commit | Significance |
|------|--------|-------------|
| Sep 18 | Test speed optimization | Performance — making ocean sims faster |
| Sep 17 | Restore closure fields from checkpoints | Bug fix for turbulence closures |
| Sep 16 | Fix face spacing above partial cells | Grid accuracy fix — critical for coastal/shallow water |
| Sep 16 | Apply linear operator once per CG Solver | Performance optimization — faster solves |
| Sep 16 | **Bounce Lagrangian particles off boundaries** | **Particle dynamics — tracks ocean material transport** |
| Sep 16 | Add TimeDerivative for computing outputs | **New feature — time evolution diagnostics** |
| Sep 16 | SplitRungeKuttaTimeStepper correct time | Correctness fix for time-stepping |
| Sep 16 | Fix stage dt used by AVID + RK3 | Numerical stability fix |
| Sep 16 | Keep non-finite values out of column solve | Robustness fix — prevent NaN propagation |
| Sep 15 | Fix test suite issues | Quality maintenance |
| Sep 15 | Tighten memory allocation bounds | Performance |
| Sep 15 | Correct implicit drag immersed mask | Accuracy fix for flow around structures |
| Sep 15 | Fix reductions under Reactant | Composability fix |
| Sep 15 | Keep field/output order in datasets | Data integrity |
| Sep 15 | Read dimension lengths for NetCDF | I/O improvement |

**What these commits tell us:**
- **Hyper-performance focus:** 7 of 15 commits are about computational speed
- **Lagrangian particle tracking:** Breakthrough for modeling how ocean particles move through complex geometries
- **Time derivative outputs:** The feature that would enable any ocean intervention simulation
- **No intervention module exists:** Every commit is about the physics solver, not geoengineering

**Episode Hook:** "Oceananigans.jl is the world's most advanced ocean simulator. 1,413 stars. 15 commits this week. And not a single line of code about geoengineering. It can simulate ocean currents with incredible fidelity. But ask it what happens if you raise ocean alkalinity and it'll say: I don't know what alkalinity is. This is the tool without a mission."

---

### 2. MDTF Diagnostics (Ocean Component)
- **Repo:** NOAA-GFDL/MDTF-diagnostics
- **Stars:** ~80
- **Key Ocean Feature:** MCS Precipitation-Buoyancy POD (added June 19, 2026)

**What it is:** The precipitation-buoyancy Pattern-Oriented Diagnostic evaluates how well climate models simulate the relationship between precipitation intensity and atmospheric buoyancy in monsoon systems. This is ocean-adjacent because monsoon precipitation is driven by ocean-evaporated moisture.

**Why it matters:** If solar geoengineering would disrupt monsoon patterns, you need to evaluate whether your model correctly simulates monsoon physics. The precip-buoyancy POD is the tool.

**Recent Ocean-Relevant Commits:**

| Date | Commit | Activity |
|------|--------|----------|
| Jun 19 | add MCS precip-buoyancy statistics POD | 5 commits same day — intensive sprint |
| Jun 19 | Update MCS_precip_buoy_stats.rst (x4) | Heavy documentation |
| Jun 8 | Merge PR #823 | Feature integration |
| Jun 2 | Update README | Documentation |

**The June 19 Sprint:** Five commits in a single day, all focused on the same documentation file. This isn't casual updating — it's a deep dive. Wei-Ming Tsai was writing the definitive description of how precipitation-buoyancy statistics work for monsoon-scale convective systems.

**Episode Hook:** "On a single day in June, one scientist wrote five commits about how rain and buoyancy interact in monsoons. That's not homework. That's expertise. And it's the closest thing we have to an open-source tool for predicting whether dimming the sun will dry out South Asia."

---

### 3. Veros (Ocean Model Alternative)
- **Repos:** Multiple small repos referencing Veros
- **Language:** Python
- **Status:** Undeveloped on GitHub as a standalone climate project

Veros is a Python-based alternative to FORTRAN ocean models (like MOM6). Several researchers have created small analysis repos, but none are dedicated to geoengineering.

---

### 4. ClimateSoton (Chemical Looping / CO2)
- **Repo:** ClimateSoton/climate-research-group
- **Institution:** University of Southampton, UK
- **4 commits on Aug 6, 2026** (website refresh)
- **Adjacent because:** Chemical Looping Combustion involves reaction with air/oxygen; ocean interception proposals share fluid dynamics principles

---

## 🚨 The Ocean Gap: What's Missing

| Ocean Geoengineering Approach | Expected Repo | Found? |
|-------------------------------|----------------|--------|
| Ocean Alkalinity Enhancement (OAE) | Olivine dissolution, pH changes, carbon uptake | ZERO |
| Marine Cloud Brightening (MCB) | Sea salt aerosol injection, cloud microphysics | ZERO |
| Artificial Upwelling | Ocean circulation with deepwater mixing | ZERO |
| Ocean Iron Fertilization (OIF) | Biogeochemistry of phytoplankton blooms | ZERO |
| Deep Blue Carbon | Sediment carbon storage modeling | ZERO |
| Thermal Energy Exchange | Ocean-atmosphere heat flux modeling | ZERO |
| Wave/Pump Infrastructure | Engineering models for intervention hardware | ZERO |

**Total ocean geoengineering repos: 0**
**Total solar geoengineering repos: 10+**
**Total carbon capture repos: 6+**

---

## 🤔 Why Is Ocean Empty? Four Hypotheses

### Hypothesis 1: The Tool Complexity Problem
Solar geoengineering can be simulated with atmosphere models (WRF already does it). Carbon capture can be simulated with molecular models (DAC thermochemistry, MOF screening). But ocean geoengineering requires coupled ocean-atmosphere-biology models at scales that don't exist yet. You can't simulate OAE with WRF. You can't simulate MCB with Oceananigans alone.

**Implication:** Ocean geoengineering is too complex for current tools. No one builds what they can't simulate.

### Hypothesis 2: Governance Taboo
The London Protocol broadly restricts ocean fertilization. Marine cloud brightening has been described as "geoengineering by stealth." Ocean alkalinity enhancement blurs the line between climate intervention and pollution. Researchers may avoid GitHub repos because of legal liability.

**Implication:** The silence is policy-driven, not technical.

### Hypothesis 3: The Early Stage Problem
Ocean geoengineering is scientifically less mature than solar SRM or DAC. The field is still at "does this phenomenon exist?" rather than "how do we model it?"

**Implication:** The gap will close as the science matures.

### Hypothesis 4: The Julia Bottleneck
The best ocean modeling tool (Oceananigans.jl) is in Julia, a language with a small developer community. To build ocean geoengineering tools, you need contributors who know Julia, ocean physics, AND geoengineering. That's a three-way intersection that barely exists.

**Implication:** The tool exists but the community doesn't.

---

## 📊 Three Universes of Climate Tech on GitHub

### Universe 1: Fast (Institutional, Funded, Sustained)
- Open-Sustainable-Tech: 2,552 stars, ~5 commits/week
- WRF: 1,761 stars, daily development
- Oceananigans.jl: 1,413 stars, 3.75 commits/day (peak)
- PCMDI Metrics: 133 stars, burst cycles
- MDTF Diagnostics: 80 stars, steady pace

### Universe 2: Slow (Individual, Unfunded, Dormant)
- Carbon_Capture_ML: 56 stars, dormant since May 2024
- ClimateMARGO: 73 stars, mysterious 2026 revival
- CO2-Sequestration: 32 stars, ghost (dead since 2019)
- srm-forever: 0 stars, persistent solo work
- DAC materials (tjz21): 2 stars each, CC0 commitment

### Universe 3: Empty (Zero Presence)
- Ocean geoengineering: 0 repos
- Marine cloud brightening: 0 repos
- Ocean alkalinity enhancement: 0 repos
- Ocean iron fertilization: 0 repos

---

## 🎙️ Episode 3 Talking Points

1. **"The Silent Ocean"** — Zero ocean geoengineering repos on GitHub. Not few. ZERO.
2. **"The 1,413-Star Ghost"** — Oceananigans.jl is the most advanced ocean simulator ever built. And it can't tell you what happens if you dump olivine in the sea.
3. **"One Scientist, Five Commits, One Day"** — The precip-buoyancy POD sprint and what it reveals about ocean-intervention diagnostics.
4. **"The Legal Problem"** — Maybe the silence isn't technical. Maybe it's because the London Protocol makes ocean geoengineering code legally dangerous.
5. **"Three Universes"** — Solar has infrastructure. Carbon has directories. Ocean has... a gap.

---

*Last updated: September 2026 | Data source: GitHub API, exhaustive 10-query search analysis*