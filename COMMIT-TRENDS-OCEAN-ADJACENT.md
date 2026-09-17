# 🌊 Ocean Intervention — Commit Trend & Adjacent Analysis

**Date:** September 2026
**Core Finding:** Zero ocean geoengineering repositories exist on GitHub across 7 search strategies
**Adjacent Analysis:** 6 nearest ocean science repos examined for comparison

---

## The Ocean Gap — Updated

This analysis confirms and extends the original OCEAN-GAP-ANALYSIS.md finding. Across 7 search strategies, **zero dedicated ocean geoengineering repositories** were found on GitHub.

### Search Strategy Results (Expanded)

| # | Query | Results | Ocean Geoengineering Repos |
|---|-------|---------|---------------------------|
| 1 | `geoengineering ocean` | 0 ocean-specific | 0 |
| 2 | `ocean alkalinization` | 0 | 0 |
| 3 | `iron fertilization` | 0 | 0 |
| 4 | `ocean intervention climate` | 0 | 0 |
| 5 | `marine geoengineering` | 0 | 0 |
| 6 | `ocean CDR` | 0 | 0 |
| 7 | `ocean climate simulation` | General climate only | 0 |

**Total ocean geoengineering repos found: ZERO**

---

## Adjacent Ocean Science Repos — Commit Analysis

These are the closest open-source tools to ocean geoengineering. None have geoengineering modules, but their commit patterns provide context.

| Repo | Stars | Language | Recent Commits | Activity Pattern | Geoengineering Modules? |
|------|-------|----------|---------------|-----------------|------------------------|
| **Oceananigans.jl** | 1,413 | Julia | Frequent (institutional) | Active, institutional | ❌ No alkalinity, no engineered tracers |
| **veros** | 400 | Python/JAX | Infrequent | Low activity | ❌ No nutrient cycling, no geoengineering |
| **OceanBioME.jl** | 80 | Julia | Infrequent | Low activity | ❌ Natural carbon cycle only, no engineered additions |
| **MDTF-diagnostics** | 80 | Jupyter/Python | 15 commits (May–Aug 2026) | Institutional bursts | ⚠️ Precip-buoyancy POD — closest ocean-adjacent diagnostic |
| **MAOOAM** | 22 | Python | ~2 years dormant | Dormant | ❌ No geoengineering extensions |
| **Climatology.jl** | 20 | Julia | Infrequent | Reference data, not simulation | ❌ Not a simulation tool |

**Key observation:** Even the most active ocean science repos (Oceananigans, MDTF) have zero geoengineering modules. The gap is not just missing code — it's missing *awareness* that geoengineering modules should exist.

---

## MDTF-Diagnostics: The Ocean-Adjacent Lifeline

**NOAA-GFDL/MDTF-diagnostics** is the closest thing to an ocean geoengineering diagnostic tool that exists on GitHub. Its recent commits reveal interesting patterns:

### Recent Commit Pattern (May–Aug 2026)

| Date | Commit | Significance |
|------|--------|-------------|
| Aug 14, 2026 | `87f8105`: Merge PR #825 | Institutional maintenance |
| Jun 19, 2026 | `33024ad`: **Add MCS precip-buoyancy statistics POD** | **New process-oriented diagnostic** |
| Jun 19, 2026 | `4cfc99c`, `699de27`, `d6bc6d0`, `3904d29`: 4× README updates | Documentation push for new POD |
| Jun 8, 2026 | `2df59f6`: Merge PR #823 | Institutional merge |
| Jun 2, 2026 | `a20f615`: Add citation | Academic rigor |
| Jun 1, 2026 | `95991fc`: Add quarterly metrics workflow | Traffic logging / usage tracking |
| May 27, 2026 | `16403a4`: Move diagnostics to dev branch | Refactoring |

### What the Precip-Buoyancy POD Means for Ocean Geoengineering

The **precip-buoyancy POD** (Process-Oriented Diagnostic) is the closest ocean-adjacent tool to ocean geoengineering simulation. Here's why it matters:

1. **Buoyancy dynamics** are fundamental to ocean mixing — which is the core mechanism of Ocean Alkalinity Enhancement (OAE)
2. **Precipitation patterns** are directly affected by ocean interventions
3. **Process-oriented diagnostics** are the first step toward process-oriented geoengineering model evaluation
4. **But it doesn't model engineered interventions** — it only observes natural processes

**The gap within the gap:** Even the closest ocean tool only diagnoses *natural* processes. There's no bridge from "observing ocean dynamics" to "simulating engineered ocean interventions."

---

## The Governance Simulation Gap

If ocean geoengineering were a policy option tomorrow, the open-source ecosystem has **nothing** to offer:

| What Would Be Needed | What Exists |
|---------------------|-------------|
| Ocean circulation model with alkalinity tracer | Oceananigans has tracers, but no alkalinity module |
| Dissolution kinetics for olivine/limestone | Zero repos |
| Ecological impact model (phytoplankton response) | OceanBioME models natural cycles, not engineered additions |
| Counter-ion balance (Na+, Mg2+) for OAE | Zero repos |
| Economic model (mining, grinding, shipping) | Zero repos |
| Governance/compliance checker (London Protocol) | Zero repos |

**Every single module in a hypothetical open-source OAE model would need to be written from scratch.**

---

## Comparison: Ocean Gap vs. Solar Gap vs. Carbon Gap

| Dimension | Solar Geoengineering | Carbon Capture | Ocean Intervention |
|-----------|---------------------|----------------|-------------------|
| Active repos | 3 (WRF, PCMDI, awesome-geoening) | 0 (all frozen/ghost) | 0 |
| Simulation code | Yes (WRF atmospheric model) | No | No |
| Governance tools | 3 (PCMDI metrics, SRM economics, awesome-geoengineering list) | 0 | 0 |
| DIY community | None | Yes (OpenAir-Cyan, OSHWA-certified) | None |
| Interactive tools | 2 (orbital-climate-simulator, srm-forever) | 0 | 0 |
| Recent activity | Institutional bursts (PCMDI v4.2.1) | Single-day blitz then freeze | Zero |
| Governance signal | Active (PCMDI metrics updates) | Absent | Absent |

**The ocean is the empty quadrant.** Not just empty of code — empty of community, empty of tools, empty of governance. 

---

## What Would Break the Ocean Gap?

### Scenario 1: The "Wikipedia Effect"
A single comprehensive textbook or review paper on ocean geoengineering could trigger community-driven code development. The solar geoengineering space has `awesome-geoengineering` — the ocean space has nothing equivalent.

### Scenario 2: The "Oceananigans Plugin"
A graduate student adds an alkalinity tracer to Oceananigans.jl.One PR. One module. The first brick in the ocean geoengineering code layer. The infrastructure already exists (Oceananigans has tracer frameworks) — someone just needs to build the specific geoengineering module.

### Scenario 3: The "Regulation Trigger"
If the London Protocol relaxes ocean fertilization restrictions, research funding would flow, and code would follow. But regulation is currently tightening, not loosening.

### Scenario 4: The "Climate Emergency Pivot"
If SRM proves insufficient and carbon capture falls short, ocean intervention becomes the only remaining lever. The desperation would drive the code. But that's a terrible reason to start.

---

## Episode Talking Points

1. **"The ocean is the empty quadrant"** — Zero repos. Zero tools. Zero governance. While solar has WRF and PCMDI, and carbon has DIY devices and ML surveys, the ocean has nothing.

2. **"MDTF is the ocean-adjacent lifeline, but it's a diagnostic, not a simulation"** — The closest ocean tool can observe buoyancy dynamics but can't model engineered interventions.

3. **"Every module in a hypothetical OAE model would need to be written from scratch"** — No alkalinity tracers, no dissolution kinetics, no ecological models, no economic models. The entire stack is missing.

4. **"The silence is a governance signal"** — Researchers aren't publishing ocean geoengineering code because the regulatory environment makes it politically risky. The code gap mirrors the governance gap.

5. **"If ocean geoengineering becomes a policy option, we'd be starting from zero"** — No simulation tools, no governance frameworks, no open-source community. Just papers and policy briefs.

---

*Analysis conducted September 2026 for the Climate Technology & Geoengineering podcast series. Extends the original OCEAN-GAP-ANALYSIS.md with commit trend data from adjacent ocean science repositories.*