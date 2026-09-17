# 🌊 Ocean Intervention — Project Discoveries

**Research Date:** September 2026  
**Podcast Episode:** Ocean Intervention — Episode 3

---

## Overview

This document catalogs the open-source ocean intervention and marine geoengineering projects discovered through GitHub research, along with the critical finding of **the ocean geoengineering gap** — the near-total absence of dedicated ocean geoengineering repositories on GitHub.

---

## The Ocean Intervention Gap: Headline Finding

After exhaustive GitHub searches across multiple query strategies — "geoengineering ocean", "marine geoengineering", "ocean fertilization", "ocean climate model", "ocean alkalinity enhancement", "iron fertilization" — this research found:

> **Zero dedicated ocean geoengineering simulation or modeling repositories.**

The ocean intervention quadrant of climate tech is the "dark matter" of open-source climate research. It exists in the scientific literature (dozens of papers on ocean alkalinity enhancement, iron fertilization, seaweed farming, and ocean upwelling) but not in open code.

### What WAS Found (Ocean-Adjacent Projects)

| Repository | Stars | Focus | Relevance |
|------------|-------|-------|-----------|
| CrayLabs/NCAR_ML_EKE | 20 | ML for ocean climate modeling at scale | ★★★☆☆ — HPC ocean simulation |
| VikingVador/Master-Thesis-Ocean-SG-FNO | 2 | FNO for subgrid-scale ocean processes | ★★☆☆☆ — Deep ocean modeling |
| mlmac-seid/marine-cloud-brightening-simulation | 0 | Marine cloud brightening via RRTM | ★★★☆☆ — SRM-adjacent |
| AidanCraw/mcb-tc-model | 1 | MCB effects on tropical cyclone tracks | ★★☆☆☆ — SRM simulation |
| FMS-ESM/AM3 | 4 | Atmospheric component of GFDL CM3 | ★★☆☆☆ — Climate model component |
| FMS-ESM/HiRAM | 9 | High-resolution atmospheric model | ★☆☆☆☆ — Weather scale |

**Key Insight:** Almost all "ocean" projects are either (a) atmospheric models that happen to include ocean coupling, (b) ML for ocean climate simulation, or (c) marine cloud brightening (which is really SRM, not ocean intervention).

**True ocean intervention projects — ocean alkalinity enhancement, iron fertilization, seaweed/biochar, ocean upwelling — have NO open-source implementation on GitHub.**

---

## Ocean-Adjacent Project Analysis

### CrayLabs/NCAR_ML_EKE ⭐ 20
- **Language:** Jupyter Notebook
- **Focus:** Using Machine Learning at Scale in HPC Simulations with SmartSim — applied to ocean climate modeling
- **Last Updated:** Aug 10, 2026
- **Key Feature:** uses SmartSim to run ML models alongside ocean climate simulations at HPC scale
- **Podcast Angle:** This is the closest thing to a production-grade ocean climate simulation with ML. If ocean geoengineering ever gets modeling tools, this is the stack they'd be built on.
- **Commit Insight:** Active through 2022 (10 commits Mar 2022), then a fix-commit in 2022. No updates in 4 years.

### mlmac-seid/marine-cloud-brightening-simulation
- **Language:** R
- **Focus:** Using RRTM (Rapid Radiative Transfer Model) to simulate marine cloud brightening effects on solar radiation
- **Last Updated:** Jul 7, 2025
- **Key Feature:** Radiative transfer modeling for marine cloud brightening — the only marine-based geoengineering simulation found
- **Podcast Angle:** Marine cloud brightening is technically SRM, not ocean intervention, but it's ocean-adjacent. The RRTM approach is the same physics that would underpin any ocean-based climate intervention.

### AidanCraw/mcb-tc-model (1 star)
- **Language:** Jupyter Notebook
- **Focus:** Modeling system to assess tropical cyclone track changes due to Marine Cloud Brightening
- **Last Updated:** Apr 28, 2020
- **Key Feature:** Connects MCB to TC tracks — a specific, high-impact question
- **Commit Insight:** 10 commits over 4 weeks (Apr 2020). Then silence. Classic academic deposit pattern.

### VikingVador/Master-Thesis-Ocean-SG-FNO (2 stars)
- **Language:** Jupyter Notebook
- **Focus:** Fourier Neural Operators for subgrid-scale processes in ocean-climate simulations
- **Last Updated:** Mar 30, 2026
- **Key Feature:** Deep learning for ocean subgrid processes — the ML corner of ocean modeling

---

## What's Missing: The Ocean Intervention Map

The following ocean geoengineering approaches have **NO dedicated open-source repositories on GitHub:**

### Ocean Alkalinity Enhancement (OAE)
- **Concept:** Adding alkaline minerals (olivine, limewater) to the ocean to increase CO2 absorption
- **Research:** Dozens of papers (Kheshgi et al., 2022; Renforth et al., 2023)
- **Open Code:** None found
- **What a repo would look like:** Ocean chemistry model, dissolution kinetics, transport simulations

### Iron Fertilization
- **Concept:** Adding iron to iron-limited ocean regions to stimulate phytoplankton blooms and carbon sequestration
- **Research:** LOHAFEX experiment, SEEDS experiment, many modeling studies
- **Open Code:** None found
- **What a repo would look like:** Biogeochemistry model, plankton dynamics, carbon export calculations

### Seaweed/Biofilm Farming
- **Concept:** Growing seaweed for carbon sequestration or biofuel
- **Research:** Growing academic interest, but mostly empirical
- **Open Code:** None found
- **What a repo would look like:** Growth model, carbon accounting, lifecycle analysis

### Ocean Upwelling / Artificial Upwelling
- **Concept:** Pumping deep, nutrient-rich water to the surface to stimulate productivity
- **Research:** Small-scale experiments, modeling studies
- **Open Code:** None found
- **What a repo would look like:** Ocean circulation model, nutrient transport, productivity estimation

---

## MDTF-diagnostics: The Ocean-Adjacent Lifeline

The closest thing to ocean process diagnostics in open source is **NOAA-GFDL/MDTF-diagnostics** (80★), which had a precipitation-buoyancy POD (Process-Oriented Diagnostic) in June 2026. This is the evaluation infrastructure that would be needed to verify any ocean intervention.

**Podcast Angle:** If ocean geoengineering is deployed, how do you verify it worked? MDTF-diagnostics is the evaluation toolkit that would need to be extended for ocean-specific diagnostics. The current precipitation-buoyancy POD is a building block, not a complete solution.

---

## Commit Trend Analysis: Ocean-Adjacent Repos

| Repository | Stars | Last Activity | Commits | Activity Level |
|------------|-------|---------------|---------|----------------|
| NCAR_ML_EKE | 20 | Mar 30, 2022 | 10 | ★★☆☆☆ (dormant) |
| marine-cloud-brightening | 0 | Jul 7, 2025 | 10 | ★★☆☆☆ (maintenance) |
| mcb-tc-model | 1 | Apr 28, 2020 | 10 | ★☆☆☆☆ (dormant) |
| Ocean-SG-FNO | 2 | Mar 30, 2026 | ? | ★★☆☆☆ (thesis) |

**Overall Assessment:** Ocean-adjacent repos are all dormant, thesis-sized, or maintenance-only. There is no active, community-driven ocean intervention modeling ecosystem on GitHub.

---

## 🌊 The Ocean Gap: A Governance Story

The absence of ocean geoengineering code on GitHub is not a bug — it's a governance signal.

### Why Is the Ocean Intervention Space So Empty?

1. **Regulatory uncertainty** — Ocean fertilization and OAE are governed by the London Protocol and London Convention, which restrict ocean disposal. Researchers may avoid building tools that could be seen as facilitating prohibited activities.

2. **No pilot projects** — Unlike DAC (which has multiple operational plants) and SRM (which has small-scale experiments), ocean intervention has almost no operational pilot projects. Without real-world deployments to model, the code doesn't get built.

3. **Complexity gap** — Ocean models are computationally expensive and require HPC infrastructure. The barrier to entry is much higher than, say, a Python-based carbon cost model.

4. **Discipline silos** — Oceanographers and climate modelers don't share code. Ocean models (MOM6, NEMO) are Fortran behemoths maintained by massive consortia. The "open-source geingerning" community doesn't touch them.

5. **Ethical concerns** — Ocean intervention raises unique ethical questions (who owns the ocean? what are the side effects?). Some researchers may deliberately avoid building tools that could lower the barrier to deployment.

### What Would Open-Source Ocean Intervention Look Like?

If someone built the "OpenAir-Cyan of ocean intervention", what would it be?

- **OAE Calculator:** A simple tool that estimates how much olivine would need to be dissolved to offset X tons of CO2, with uncertainty quantification
- **Ocean Transport Model:** A simplified 2D model of alkalinity transport in the ocean, runnable on a laptop
- **Impact Assessment Framework:** A tool that estimates ecological side effects of ocean intervention
- **Governance Dashboard:** A tool that monitors and verifies ocean intervention deployments

### The Opportunity

The ocean intervention gap is the biggest opportunity in open-source climate tech. The field is so empty that the first person to build a serious, maintenance-quality ocean intervention model could own the space.

---

## 🎙️ Podcast Episode Notes: Ocean Intervention

### Key Questions for the Episode
1. Why is ocean geoengineering the empty quadrant of climate tech on GitHub? What does the silence mean?
2. Is the absence a governance signal — are researchers self-censoring because of regulatory concerns?
3. What would the "OpenAir-Cyan of ocean intervention" look like? What's the simplest possible tool that would be useful?
4. Can MDTF-diagnostics be extended for ocean-specific diagnostics? What building blocks exist?
5. The London Protocol and London Convention — how do international regulations affect open-source ocean geoengineering?
6. Ocean alkalinity enhancement: is it the most viable ocean intervention, or is it still too speculative for code?

### Thesis Statements for the Episode
- Ocean geoengineering is the "dark matter" of open-source climate tech — invisible, undetected, but potentially massive
- The silence on GitHub is itself a governance signal: regulatory uncertainty, discipline silos, and ethical concerns are keeping researchers from building tools
- The first person to build a maintenance-quality ocean intervention model could own the entire space
- MDTF-diagnostics' precipitation-buoyancy POD is the building block we should watch for ocean-adjacent evaluation

### Sources
- https://github.com/CrayLabs/NCAR_ML_EKE
- https://github.com/VikVador/Master-Thesis-Ocean-SG-FNO
- https://github.com/mlmac-seid/marine-cloud-brightening-simulation
- https://github.com/AidanCraw/mcb-tc-model
- https://github.com/NOAA-GFDL/MDTF-diagnostics
- https://github.com/FMS-ESM/AM3
- https://github.com/FMS-ESM/HiRAM
- Related literature: Kheshgi et al. (2022), Renforth et al. (2023) on ocean alkalinity enhancement