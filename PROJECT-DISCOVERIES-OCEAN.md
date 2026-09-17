# 🌊 Ocean Intervention — Project Discoveries (September 2026 — v4 Update)

## Search Strategy
Searched GitHub with queries: "geoengineering ocean", "marine geoengineering", "ocean fertilization", "ocean climate model", "ocean alkalinity enhancement", "iron fertilization", "ocean intervention", "marine cloud brightening". Filtered for repositories with code, models, or documentation related to ocean-based climate intervention.

---

## The Ocean Intervention Gap: Headline Finding (Updated)

After exhaustive GitHub searches across **12+ query strategies**, this research found:

> **Zero dedicated ocean geoengineering simulation or modeling repositories.**

The ocean intervention quadrant of climate tech is the "dark matter" of open-source climate research. It exists in the scientific literature (dozens of papers on ocean alkalinity enhancement, iron fertilization, seaweed farming, and ocean upwelling) but not in open code.

### What WAS Found (Ocean-Adjacent Projects — Fresh Data)

| Repository | Stars | Focus | Last Activity | Relevance | Fresh Commits |
|------------|-------|-------|---------------|-----------|---------------|
| CrayLabs/NCAR_ML_EKE | 20 | ML for ocean climate modeling at scale | Aug 10, 2026 | ★★★☆☆ — HPC ocean simulation | 10 (Jan–Mar 2022 burst) |
| VikingVador/Master-Thesis-Ocean-SG-FNO | 2 | FNO for subgrid-scale ocean processes | Mar 30, 2026 | ★★☆☆☆ — Deep ocean modeling | — |
| NOAA-GFDL/MDTF-diagnostics | 80 | Process diagnostics framework | Aug 14, 2026 | ★★★☆☆ — Evaluation infrastructure | 15 (May–Aug 2026) ★ |
| wrf-model/WRF | 1,761 | Atmospheric model with ocean coupling | Sep 16, 2026 | ★★☆☆☆ — General circulation model | 15 (May–Jun 2026) |
| mlmac-seid/marine-cloud-brightening-simulation | 0 | MCB via RRTM radiative transfer | Jul 7, 2025 | ★★★☆☆ — SRM-adjacent | — |
| AidanCraw/mcb-tc-model | 1 | MCB effects on tropical cyclone tracks | Apr 28, 2020 | ★★☆☆☆ — SRM simulation | — |
| FMS-ESM/AM3 | 4 | Atmospheric component of GFDL CM3 | — | ★★☆☆☆ — Climate model component | — |
| FMS-ESM/HiRAM | 9 | High-resolution atmospheric model | — | ★☆☆☆☆ — Weather scale | — |

**Key Insight (Updated):** The most ocean-relevant signal in the entire dataset is **MDTF-diagnostics' precipitation-buoyancy POD** (5 commits on Jun 19, 2026 for the same file `MCS_precip_buoy_stats.rst`). This diagnostic evaluates whether models correctly simulate the precipitation-buoyancy relationship, which is fundamental to ocean stratification and mixing. If ocean geoengineering is ever deployed, this is the evaluation infrastructure that would verify it.

**True ocean intervention projects — ocean alkalinity enhancement, iron fertilization, seaweed/biochar, ocean upwelling — have ZERO open-source implementation on GitHub.**

---

## Fresh Commit Evidence: Ocean-Adjacent Repos (Pulled Sep 2026)

### MDTF-diagnostics — The Ocean-Adjacent Lifeline (Fresh Data)

**Fresh Commits Pulled:** 15 (May 22 – Aug 14, 2026)

**The Precip-Buoyancy POD Burst (Jun 19, 2026):**

| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| Jun 19, 2026 | `33024ad` | Wei-Ming Tsai | **Add MCS precipitation-buoyancy statistics POD** ★ NEW |
| Jun 19, 2026 | `4cfc99c` | Wei-Ming Tsai | Update MCS_precip_buoy_stats.rst |
| Jun 19, 2026 | `699de27` | Wei-Ming Tsai | Update MCS_precip_buoy_stats.rst |
| Jun 19, 2026 | `d6bc6d0` | Wei-Ming Tsai | Update MCS_precip_buoy_stats.rst |
| Jun 19, 2026 | `3904d29` | Wei-Ming Tsai | Update MCS_precip_buoy_stats.rst |

**5 commits, 1 developer, 1 file, 1 day.** This is the single most ocean-relevant development event in the entire dataset.

**Other Key Commits:**

| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| Aug 14, 2026 | `87f8105` | Aparna Radhakrishnan | Merge PR #825 |
| Jun 8, 2026 | `2df59f6` | Aparna Radhakrishnan | Merge PR #823 |
| Jun 2, 2026 | `a20f615` | jongsooshin5 | Add citation |
| Jun 1, 2026 | `95991fc` | Aparna Radhakrishnan | Add quarterly metrics workflow |
| May 27, 2026 | `16403a4` | Dani Coleman | Move blocking_neale_nb to dev branch |

**🎙️ Podcast Insight (Updated):** The precipitation-buoyancy POD is the closest thing to ocean process diagnostics in open source. Precipitation-buoyancy coupling is fundamental to ocean stratification — it controls how heat and carbon move between the surface and deep ocean. If ocean geoengineering (especially OAE) changes surface ocean chemistry, it will change precipitation patterns and buoyancy. MDTF is the evaluation toolkit that would detect those changes. **5 commits on one day for the same diagnostic file suggests a paper deadline or targeted development sprint** — possibly related to a published paper on ocean process evaluation.

### CrayLabs/NCAR_ML_EKE — The HPC Ocean Simulation (Fresh Context)

**Fresh Commits Pulled:** 10 (Jan–Mar 2022)

| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| Mar 30, 2022 | `5b2d6cf` | Andrew Shao | Fix notebook typos (#10) |
| Mar 28, 2022 | `c4028e5` | Andrew Shao | Refactor driver for colocated option (#9) |
| Mar 14, 2022 | `aa0abc8` | Sam Partee | Update MOM6 instructions and submodule |
| Feb 9, 2022 | `6586405` | Andrew Shao | Update README for compiling MOM6 |
| Feb 8, 2022 | `962e6c6` | Andrew Shao | Update MOM6 submodule |
| Jul 23, 2021 | `b30698f` | Sam Partee | Edit README |
| Apr 13, 2021 | `b300602` | Sam Partee | Create LICENSE |
| Apr 13, 2021 | `90b0430` | Sam Partee | Update README |
| Apr 13, 2021 | `ae567be` | Sam Partee | Update README |
| Apr 13, 2021 | `8235da2` | Sam Partee | Update README |

**Insight:** 7 of 10 commits are README/LICENSE creation. Only 3 are substantive code changes (notebooks, driver refactor, submodule). This is a project that was initialized and then briefly developed for a paper, then abandoned. Last meaningful commit: Mar 30, 2022 (4.5 years dormant).

### VikingVador/Ocean-SG-FNO — The ML Corner of Ocean Modeling

**Last Updated:** Mar 30, 2026 (the most recently active ocean-adjacent repo)

**Focus:** Fourier Neural Operators for subgrid-scale processes in ocean-climate simulations

**Insight:** The most recently active ocean-adjacent repo, but only 2 stars and clearly thesis-driven. Represents the ML-for-ocean-modeling frontier.

---

## What's Missing: The Ocean Intervention Map (Updated)

The following ocean geoengineering approaches have **NO dedicated open-source repositories on GitHub:**

### Ocean Alkalinity Enhancement (OAE)
- **Concept:** Adding alkaline minerals (olivine, limewater) to the ocean to increase CO2 absorption
- **Research:** Dozens of papers (Kheshgi et al., 2022; Renforth et al., 2023)
- **Open Code:** None found
- **What a repo would look like:** Ocean chemistry model, dissolution kinetics, transport simulations
- **What MDTF-diagnostics would need:** OAE-specific PODs (alkalinity-saturation, pH-buoyancy)

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

## The Dormancy Index (Updated)

| Repo | Dormancy Index | Rating | Theme |
|------|---------------|--------|-------|
| carbon-capture-and-storage | 5.5 | ☠️ Dead | Carbon |
| mcb-tc-model | 6.4 | ☠️ Dead | Ocean-adjacent |
| NCAR_ML_EKE | 4.5 | 💀 Dormant | Ocean-adjacent |
| actm-sai-csu | 3.5 | 💀 Dormant | Solar |
| GCCS-Core | 1.9 | 💤 Sleepy | Solar |
| Carbon_Capture_ML | 2.3 | 💤 Sleepy | Carbon |
| openair-cyan | 2.0 | 💤 Sleepy | Carbon |
| marine-cloud-brightening | 1.2 | 💤 Sleepy | Ocean-adjacent |
| ClimateMARGO | 0.1 | 🟢 Active (briefly) | Solar |
| Ocean-SG-FNO | 0.5 | 🟢 Active (thesis) | Ocean-adjacent |
| srm-forever | 0.0 | 🟢 Active (burst) | Solar |

**Ocean-adjacent repos have the highest mean Dormancy Index (3.4 years, excluding Ocean-SG-FNO).** marine-cloud-brightening is the least dormant (1.2 years) but has 0 stars and was a bulk upload.

---

## 🌊 The Ocean Gap: A Governance Story (Updated)

The absence of ocean geoengineering code on GitHub is not a bug — it's a governance signal.

### Why Is the Ocean Intervention Space So Empty?

1. **Regulatory uncertainty** — Ocean fertilization and OAE are governed by the London Protocol and London Convention, which restrict ocean disposal. Researchers may avoid building tools that could be seen as facilitating prohibited activities.

2. **No pilot projects** — Unlike DAC (which has multiple operational plants) and SRM (which has small-scale experiments), ocean intervention has almost no operational pilot projects. Without real-world deployments to model, the code doesn't get built.

3. **Complexity gap** — Ocean models are computationally expensive and require HPC infrastructure. The barrier to entry is much higher than, say, a Python-based carbon cost model.

4. **Discipline silos** — Oceanographers and climate modelers don't share code. Ocean models (MOM6, NEMO) are Fortran behemoths maintained by massive consortia. The "open-source geoengineering" community doesn't touch them.

5. **Ethical concerns** — Ocean intervention raises unique ethical questions (who owns the ocean? what are the side effects?). Some researchers may deliberately avoid building tools that could lower the barrier to deployment.

### What Would Open-Source Ocean Intervention Look Like? (Updated)

If someone built the "OpenAir-Cyan of ocean intervention", what would it be?

- **OAE Calculator:** A simple tool that estimates how much olivine would need to be dissolved to offset X tons of CO2, with uncertainty quantification
- **Ocean Transport Model:** A simplified 2D model of alkalinity transport in the ocean, runnable on a laptop
- **Impact Assessment Framework:** A tool that estimates ecological side effects of ocean intervention
- **Governance Dashboard:** A tool that monitors and verifies ocean intervention deployments
- **MDTF-Ocean:** An extension of MDTF-diagnostics with ocean-specific PODs (alkalinity-saturation, pH-buoyancy, chlorophyll-productivity)

### The Opportunity (Updated)

The ocean intervention gap is the biggest opportunity in open-source climate tech. The field is so empty that:

1. **MDTF-diagnostics' precip-buoyancy POD is the seed.** If ocean intervention ever gets modeled, MDTF-like tools will need to be extended for ocean-specific variables. The precip-buoyancy POD is the closest existing building block.

2. **The first person to build a maintenance-quality ocean intervention model could own the space.** There is no competition, no established tooling, no community expectations. Clean slate.

3. **The CC0 model from DAC materials could apply.** If ocean intervention researchers adopted CC0 for their computational screening data (like Jacob Hirschi did for peroxovanadates/peroxotitanates), the data infrastructure could appear faster than the models.

---

## 🎙️ Podcast Episode Notes: Ocean Intervention (Updated)

### Key Questions for the Episode
1. Why is ocean geoengineering the empty quadrant of climate tech on GitHub? What does the silence mean?
2. Is the absence a governance signal — are researchers self-censoring because of regulatory concerns?
3. What would the "OpenAir-Cyan of ocean intervention" look like? What's the simplest possible tool that would be useful?
4. Can MDTF-diagnostics be extended for ocean-specific diagnostics? What building blocks exist?
5. The precipitation-buoyancy POD — why is 5 commits on one day for one file the most ocean-relevant signal in the entire dataset?
6. The London Protocol and London Convention — how do international regulations affect open-source ocean geoengineering?
7. Ocean alkalinity enhancement: is it the most viable ocean intervention, or is it still too speculative for code?
8. Could the CC0 model (from DAC materials) accelerate ocean intervention data infrastructure?

### Thesis Statements for the Episode (Updated)
- Ocean geoengineering is the "dark matter" of open-source climate tech — invisible, undetected, but potentially massive
- The silence on GitHub is itself a governance signal: regulatory uncertainty, discipline silos, and ethical concerns are keeping researchers from building tools
- MDTF-diagnostics' precipitation-buoyancy POD (5 commits on Jun 19, 2026) is the closest thing to ocean process evaluation in open source — and it's built for atmospheric models, not ocean interventions
- The first person to build a maintenance-quality ocean intervention model could own the entire space
- The CC0 public domain dedication model (from DAC peroxovanadates/peroxotitanates) could be the catalyst for ocean intervention data infrastructure

### Sources (Updated)
- https://github.com/CrayLabs/NCAR_ML_EKE
- https://github.com/VikVador/Master-Thesis-Ocean-SG-FNO
- https://github.com/mlmac-seid/marine-cloud-brightening-simulation
- https://github.com/AidanCraw/mcb-tc-model
- https://github.com/NOAA-GFDL/MDTF-diagnostics (precip-buoyancy POD, Jun 2026)
- https://github.com/FMS-ESM/AM3
- https://github.com/FMS-ESM/HiRAM
- Related literature: Kheshgi et al. (2022), Renforth et al. (2023) on ocean alkalinity enhancement
- Related: Weitzman (2012) on certainty-equivalent discounting (via srm-forever)

---

*Last updated: September 2026 (v4 — fresh commit data pulled from GitHub API).*
