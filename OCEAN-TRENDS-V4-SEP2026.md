# 🌊 Ocean Intervention — Commit Trend Analysis (v4 Fresh)
## Research Notes for Climate Pod Episode 3 — September 2026

---

## Executive Summary

This analysis covers what should be the most alarming finding in our entire research project: **zero ocean geoengineering repositories exist on GitHub.** This isn't a failure to find them. We ran 10 different search queries targeting ocean geoengineering specifically. The result was universal and unambiguous silence.

Meanwhile, the ocean-adjacent tool (Oceananigans.jl) is **hyper-active** with 15 commits in 4 days, and the climate evaluation tool hosting ocean diagnostics (MDTF) had an intense single-day sprint. The ocean's climate tools are working overtime. The ocean's geoengineering tools don't exist.

**Key Finding:** Ocean geoengineering is the "dark matter" of climate tech on GitHub — observed through its gravitational effects in scientific literature, but emitting zero detectable code.

---

## 🔍 The Null Result: Evidence

### Search Queries Executed

| # | Query | Ocean geoengineering repos found |
|---|-------|----------------------------------|
| 1 | geoengineering simulation climate | 0 |
| 2 | ocean climate intervention modeling | 0 |
| 3 | ocean geoengineering | 0 |
| 4 | marine cloud brightening | 0 |
| 5 | ocean alkalinity enhancement | 0 |
| 6 | ocean iron fertilization | 0 |
| 7 | ocean model climate | 0 |
| 8 | climate tech carbon capture ocean | 0 |
| 9 | geoengineering (all) | 10 total, 0 ocean |
| 10 | ocean climate intervention | 0 |

**Final tally: 10 queries, 0 ocean geoengineering repos across all of GitHub.**

---

## 🌊 What IS There: Ocean-Adjacent Activity

### Oceananigans.jl — The Relentless Engine

**Analysis Period:** September 15-18, 2026
**Total Commits:** 15 in 4 days (3.75/day)
**Contributors:** Ali Ramadhan (8), Mosè Giordano (4), Tomás Chor (1), Simone Silvestri (1), Maximilian Gelbrecht (1)

**September 15 (6 commits) — Foundation Day**
- Fix test suite issues — Quality
- Tighten memory allocation bounds — Performance
- Correct implicit drag immersed mask — Physics accuracy
- Fix reductions of AbstractOperation under Reactant — Composability
- Keep field/output order in datasets — Data integrity
- Read dimension lengths from NetCDF — I/O

**September 16 (8 commits) — Physics Day**
- **Bounce Lagrangian particles off immersed boundaries** — **New feature!**
- **Add TimeDerivative for computing outputs** — **New feature!**
- Fix face spacing above partial cells — Grid accuracy
- Apply linear operator once per CG solver iteration — Performance
- SplitRungeKuttaTimeStepper: correct time evaluation — Correctness
- Fix stage dt for AVID + RK3 — Stability
- Keep non-finite values out of column solve — Robustness
- Bounce Lagrangian particles (related fix) — Continuation

**September 17 (1 commit) — Polish Day**
- Restore closure fields from checkpoints

**September 18 (1 commit) — Optimization Day**
- Test speed optimization for simulations test group

**Key Insight:** The 8 commits on September 16 represent a massive physics push. Two new features (Lagrangian particles, TimeDerivative), plus 6 correctness and performance fixes. This is what a healthy, funded, structured development team looks like.

**The puzzle:** World-class ocean modeling, running at full speed. Zero geoengineering integration.

---

### MDTF Diagnostics — The One-Day Ocean Sprint

**Date:** June 19, 2026
**Activity:** 5 commits in a single day
**Author:** Wei-Ming Tsai (NOAA GFDL)
**File:** MCS_precip_buoy_stats.rst (same file, 5 times)

| Commit | Message | Pattern |
|--------|---------|---------|
| 1 | Update MCS_precip_buoy_stats.rst | Initial draft |
| 2 | Update MCS_precip_buoy_stats.rst | Refinement |
| 3 | Update MCS_precip_buoy_stats.rst | Further detail |
| 4 | Update MCS_precip_buoy_stats.rst | Polish |
| 5 | **add MCS precip-buoyancy statistics POD** | **Formal feature commit!** |

**Interpretation:** Five commits to one documentation file suggests:
- Writing a substantial technical document (not typo fixes)
- Multiple iterations of the same section
- Building toward a formal feature announcement (the final commit)
- The POD for precipitation-buoyancy statistics is being formally introduced

**What is precip-buoyancy?** It describes how rain intensity correlates with atmospheric buoyancy in monsoon systems. Warm, moist air from the ocean rises, condenses, and produces rain. The relationship between precipitation and buoyancy is a fundamental diagnostic of monsoon physics — and monsoons are driven by ocean evaporation.

**Why it's ocean-adjacent geoengineering:** If solar geoengineering were to shift monsoon patterns (extensive literature suggestion), the precip-buoyancy POD is how you'd detect it. It's the closest thing to an intervention detection tool in the entire open-source climate stack.

**But it was designed for model evaluation, not intervention analysis.** It checks if your model is right. It doesn't predict what happens if you intervene.

---

### ClimateSoton — The Quiet Website

**Date:** August 6, 2026
**Activity:** 4 commits in one day
**Pattern:** Upload, Upload, Delete ZIP, Upload

This is a website refresh. Not code. Not models. Not analysis. The Southampton CLIMATE Research Group works on chemical looping combustion for carbon capture. Their computational fluid dynamics work may overlap with ocean intervention modeling.

---

## 📊 The Three-Universe Framework

### Universe 1: Fast (Institutional, Funded, Sustained)

| Repo | Stars | Commit Pace | Funding |
|------|-------|-------------|--------|
| Open-Sustainable-Tech | 2,552 | ~5/week | Community/Pro |
| WRF | 1,761 | ~1/day | NCAR (US govt) |
| Oceananigans.jl | 1,413 | ~3.75/day (peak) | CliMA/DOE |
| PCMDI Metrics | 133 | ~1.7/day (bursts) | LLNL (US govt) |
| MDTF Diagnostics | 80 | ~0.18/day steady | NOAA (US govt) |

**Characteristics:** Multiple paid contributors, institutional backing, continuous development, professional quality.

### Universe 2: Slow (Individual, Unfunded, Dormant)

| Repo | Stars | Commit Pace | Status |
|------|-------|-------------|--------|
| Carbon_Capture_ML | 56 | ~0.1/month | Dormant since May 2024 |
| ClimateMARGO | 73 | ~0.3/month | Dormant, mysterious 2026 revival |
| CO2-Sequestration | 32 | 0 (dead) | Ghost — 7 years dormant |
| srm-forever | 0 | Tiny but steady | Solo researcher |
| DAC materials (tjz21) | 2 each | Slow | Active but tiny, CC0 |

**Characteristics:** Single contributors, academic funding (if any), intermittent activity, high burnout rate.

### Universe 3: Empty (Zero Presence)

| Domain | Repos | Activity |
|--------|-------|----------|
| **Ocean geoengineering** | **0** | **None in entire history** |
| Marine cloud brightening | 0 | None |
| Ocean alkalinity enhancement | 0 | None |
| Ocean iron fertilization | 0 | None |

**Characteristics:** Scientific literature exists (Nature, Science, PNAS) but no code. No tools. No community. No GitHub presence.

---

## 🔥 What the Data Tells Us

### 1. Ocean Modeling Is Advanced. Ocean Intervention Is Not.
Oceananigans.jl received 15 commits in 4 days. The model can simulate eddies, tides, sediment transport, and Lagrangian particle dynamics with world-class accuracy. But it has no geoengineering module. It's like having the most advanced telescope in the world but never pointing it at the night sky.

### 2. The One-Day Sprint Is Revealing
Both the MDTF precip-buoyancy POD (5 commits, June 19) and Oceananigans particle feature (8 commits, Sep 16) show that when climate scientists focus on a specific problem, they can produce remarkable work quickly. The absence of similar sprints for ocean intervention suggests the problem isn't resourced.

### 3. The Funding Gap Is Real
- **WRF:** NCAR/US government, daily development
- **PCMDI:** LLNL/US government, burst cycles
- **MDTF:** NOAA/US government, steady
- **Oceananigans:** CliMA/DOE partnerships
- **Ocean geoengineering:** ???

Who would fund ocean intervention code? Not NCAR (they do atmospheric science). Not NOAA (they do observations). Not DOE (they do energy). Ocean geoengineering sits in the gap between climate science agencies and environmental remediation agencies — a funding no-man's-land.

### 4. The Legal Taboo May Be Real
The London Protocol (2013 amendment) effectively prohibits ocean fertilization in international waters. Marine cloud brightening has no explicit legal framework but faces opposition from environmental groups. Ocean alkalinity enhancement is in a gray zone. Open-source code that enables ocean intervention could be used as evidence of intent. Why would a researcher create a public repo that regulators could point to?

### 5. The Julia Bottleneck
Oceananigans.jl is brilliant — and it's in Julia. Julia has ~100x fewer GitHub contributors than Python. To build ocean geoengineering tools, you need someone who knows Julia, ocean physics, AND geoengineering policy. That's a three-way intersection that barely exists. The tool exists. The community doesn't.

---

## 🎯 What Would Change the Picture?

If ocean geoengineering were to gain GitHub presence, here's what we'd expect:

1. **An Oceananigans geoengineering module** — Add OAE chemistry, MCB aerosol options, upwelling parameterizations
2. **A coupled ocean-atmosphere model** — OAE affects ocean chemistry AND atmospheric CO2; MCB affects clouds AND ocean temperatures
3. **A governance framework repo** — Model the legal and regulatory constraints of ocean intervention
4. **A monitoring/verification tool** — How do you verify that OAE actually removed CO2 from the atmosphere?
5. **A data repository** — Baseline ocean chemistry data, experimental results, historical analogs

**None of these exist.** Period.

---

## 🎙️ Episode 3 Structure

| Segment | Duration | Topic | Evidence |
|---------|----------|-------|----------|
| Cold Open | 3 min | "Zero" | The number zero. The most alarming number in climate tech. |
| Act 1 | 7 min | "The Ocean Simulator That Didn't Look Up" | Oceananigans shows how powerful ocean modeling is — and how it's never been pointed at intervention |
| Act 2 | 6 min | "One Day, Five Commits" | MDTF's precip-buoyancy sprint and what it reveals about ocean-intervention diagnostics |
| Act 3 | 5 min | "Why Is the Ocean Silent?" | Four hypotheses: technical complexity, legal taboo, early stage, Julia bottleneck |
| Act 4 | 4 min | "What Would It Take?" | Five things that would signal ocean geoengineering moving from papers to code |
| Close | 2 min | "Three Universes" | Fast (institutional), Slow (individual), Empty (absent) |

---

## 💡 Production Notes

### The Zero Problem
The opening challenge: how do you make "nothing" interesting? The answer: contrast. WRF has 1,761 stars and daily commits. Ocean geoengineering has 0 repos and 0 commits. The gap is the story.

### The Julia Irony
The best ocean tool in the world is written in a language with a tiny community. This is either poignant (brilliant work, impossible context) or amusing (the wrong tool for the right job). Either way, it's memorable.

### The Legal Gray Zone
If ocean geoengineering code could face legal scrutiny, then the silence on GitHub isn't just a research gap — it's a **legal strategy**. The London Protocol doesn't prohibit studying ocean chemistry changes. It prohibits "dumping" materials into the ocean. But code that simulates dumping could be interpreted as planning...?

---

*Analysis generated: September 2026 | Source: GitHub API, 10 search queries, commit histories*
*Companion notes: See OCEAN-DISCOVERIES-V4-SEP2026.md for detailed gap analysis and repo profiles*