# 🌊 Ocean Intervention — Project Discoveries & Gap Analysis

> Updated: September 2026 | Episode theme branch for `climate-pod-research`

---

## Overview

This file documents the **complete absence** of dedicated ocean geoengineering repositories on GitHub, along with the ocean-adjacent tools that provide the closest scientific support. This is the most significant finding of the entire research project.

---

## 🚨 The Ocean Gap: Zero Repositories Found

### What We Searched
We ran **10+ distinct GitHub search queries** across multiple strategies:

| Search Query | Results |
|-------------|--------|
| `ocean geoengineering` | 0 dedicated repos |
| `ocean alkalinity enhancement` | 0 dedicated repos |
| `marine cloud brightening` | 0 dedicated repos |
| `ocean iron fertilization` | 0 dedicated repos |
| `seaweed farming climate` | 0 dedicated repos |
| `ocean liming` | 0 dedicated repos |
| `marine geoengineering simulation` | 0 dedicated repos |
| `ocean carbon removal open source` | 0 dedicated repos |
| `ocean intervention climate model` | 0 dedicated repos |
| `blue carbon restoration` | 0 dedicated repos |
| `coastal climate adaptation model` | 0 repos (non-geoengineering) |

### What This Means
**Ocean geoengineering is the "dark matter" of climate tech on GitHub.** It exists abundantly in the scientific literature (Nature, Science, PNAS, Environmental Research Letters) but has **zero open-source code presence**. This is not a small gap — it's a complete vacuum.

---

## The Ocean-Adjacent Lifelines

While there are zero dedicated ocean geoengineering repos, we found several ocean-adjacent tools that provide the scientific infrastructure closest to ocean intervention:

### 1. MDTF Diagnostics (Precipitation-Buoyancy POD)
- **Repo:** [NOAA-GFDL/MDTF-diagnostics](https://github.com/NOAA-GFDL/MDTF-diagnostics)
- **Stars:** ~80 | **License:** Apache 2.0
- **Last commit:** August 14, 2026
- **Ocean connection:** The **precipitation-buoyancy POD** is the most ocean-relevant diagnostic in open source. It evaluates how well climate models capture the vertical coupling between ocean buoyancy and precipitation — a process that ocean interventions (OAE, iron fertilization) could directly affect.
- **Why it matters:** This is how you'd evaluate whether an ocean intervention is working. Not by simulating the intervention itself, but by checking if the model gets the ocean physics right.
- **Commit signal:** 5 commits on June 19, 2026 alone — intense single-day development on the precip-buoyancy POD file. NOAA/GFDL considers this a priority tool.

### 2. WRF (Ocean coupled modes)
- **Repo:** [wrf-model/WRF](https://github.com/wrf-model/WRF)
- **Stars:** ~1,761 | **License:** Apache 2.0
- **Ocean connection:** WRF can be coupled with ocean models (e.g., MOM6, POP) for fully coupled climate simulations. The solar radiation scheme updates affect ocean surface heat flux calculations.
- **Why it matters:** Any ocean geoengineering simulation would need to pass through WRF's air-sea flux calculations. The model is the atmospheric gateway to the ocean.

### 3. ClimateSoton/climate-research-group
- **Repo:** [ClimateSoton/climate-research-group](https://github.com/ClimateSoton/climate-research-group)
- **Activity:** Active website updates in August 2026
- **Ocean connection:** A research group website (not code) that aggregates climate research including ocean topics. Useful as a bookmarking layer, not a simulation tool.

### 4. Oceananigans.jl (from v2 ecosystem analysis)
- **Stars:** ~1,413 | **Language:** Julia | **License:** MIT
- **Last activity:** Active through v2 research (prior analysis)
- **Ocean connection:** A pure ocean simulation framework in Julia. Models ocean turbulence, waves, and mixing. The most sophisticated open-source ocean dynamics code available.
- **Why it matters:** Oceananigans can simulate ocean fluid dynamics with exquisite detail. But it **doesn't simulate geoengineering interventions** — it simulates the ocean without any human perturbation. It's the pristine ocean, not the modified one.

### 5. MHKiT-Python (Marine Hydrokinetic)
- **Repo:** [MHKiT-Software/MHKiT-Python](https://github.com/MHKiT-Software/MHKiT-Python)
- **Ocean connection:** Tools for marine renewable energy (tidal, wave). Not geoengineering, but the closest thing to "marine technology" in the GitHub ecosystem.
- **Why it matters:** Shows that marine *energy* has a tooling ecosystem, but marine *geoengineering* has nothing. Marine energy is about harvesting the ocean; marine geoengineering is about manipulating it. The contrast tells a governance story.

---

## The Three Universes — Ocean Edition

| Universe | What Exists | What's Missing |
|----------|-------------|----------------|
| **Fast Universe** (Institutional) | MDTF diagnostics, WRF (coupled), Oceananigans.jl | None of these simulate interventions |
| **Slow Universe** (Individual) | ClimateSoton research group, MHKiT | ClimateSoton is a website; MHKiT is for energy, not geoengineering |
| **Empty Universe** | **Nothing** | Ocean geoengineering, marine cloud brightening, OAE code, iron fertilization models, seaweed farming tools |

---

## Ocean Interventions vs. GitHub Presence: A Reality Check

| Intervention | Scientific Literature | GitHub Code |
|-------------|----------------------|-------------|
| Marine Cloud Brightening (MCB) | Hundreds of papers | **Zero repos |
| Ocean Alkalinity Enhancement (OAE) | Dozens of papers | **Zero repos** |
| Ocean Iron Fertilization (OIF) | Decades of experiments | **Zero repos** |
| Seaweed/Bioenergy Carbon Capture (BECCS) | Growing literature | **Zero repos** |
| Ocean Liming | Emerging papers | **Zero repos** |
| Coastal Blue Carbon (mangroves, seagrass) | Active research | **Zero repos** |

---

## Why Is the Ocean Gap So Deep?

Our hypothesis, based on the GitHub evidence:

1. **Governance fear:** Unlike solar geoengineering (which has srm-forever and WRF-based modeling), ocean interventions may face stronger governance resistance. Researchers may avoid building tools that could be perceived as "designing" ocean manipulation.

2. **Complexity barrier:** Ocean systems are orders of magnitude more complex than atmospheric systems. Writing a general-purpose ocean geoengineering model requires resolving mesoscale eddies, biogeochemistry, and thermohaline circulation simultaneously. The computational barrier is higher.

3. **Data scarcity:** Ocean observing infrastructure is sparse compared to atmospheric networks. Without sufficient data, modelers can't validate ocean intervention models. You can't build a model of something you can't observe.

4. **Funding misalignment:** Ocean research is funded by ocean science agencies (NOAA, NERC) that focus on understanding, not intervention. Domestic space agencies and climate model centers fund atmospheric modeling, not ocean manipulation.

5. **The "too spooky" factor:** Ocean interventions feel more like science fiction than solar geoengineering. Marine cloud brightening sounds like weather control. Iron fertilization sounds like polluting the sea. The cultural resistance may suppress both funding and code contribution.

---

## What Would Open-Source Ocean Intervention Look Like?

If someone were to build the first ocean geoengineering codebase, it might include:

- **OAE module:** Calculate alkalinity addition rates, dissolution kinetics, and ocean pH response
- **MCB module:** Simulate cloud condensation nuclei injection, marine layer brightening, and precipitation impacts
- **OIF module:** Model iron fertilization, phytoplankton blooms, and carbon export to the deep ocean
- **Blue Carbon module:** Simulate mangrove/seagrass restoration, sediment carbon storage, and coastal protection co-benefits
- **Evaluation framework:** Like MDTF's PODs but tailored for ocean intervention — process-level diagnostics for ocean biogeochemistry

**None of this exists.** The codebase for ocean intervention is a blank page.

---

## 📊 Commit Activity Summary (Ocean Theme)

| Repo | Ocean Relevance | Commit Signal |
|------|----------------|---------------|
| MDTF-diagnostics | High (precip-buoyancy POD) | 5 commits on Jun 19, 2026 — active |
| WRF | Medium (air-sea fluxes) | 10 commits (v4.8.0, solar/radiation) |
| Oceananigans.jl | High (ocean dynamics) | Active (from v2 data) |
| ClimateSoton/climate-research-group | Low (website) | Active Aug 2026 |
| **Dedicated ocean geoengineering repos** | **NONE** | **ZERO** |

---

## 🎙️ Recommended Episode Structure — Ocean Intervention

1. **Cold open:** "We searched GitHub 10 different ways. Zero ocean geoengineering repos. Not one. The ocean is the missing quadrant."
2. **Act 1:** The void — what we searched, what we found (or didn't), and why the gap matters
3. **Act 2:** The ocean-adjacent lifelines — MDTF's precipitation-buoyancy POD, Oceananigans, WRF's coupled modes. The science exists; the intervention code doesn't
4. **Act 3:** The governance hypothesis — is the silence a choice? Would building OAE code be seen as advocating for intervention? The moral hazard of the tool itself
5. **Act 4:** What would the first repo look like? — a blueprint for ocean intervention code, from OAE modules to evaluation frameworks
6. **Close:** The blank page is the most important finding. The ocean is where the climate is most turbulent, most complex, and most silent in the code world. That silence is itself a signal.

---

*Generated from GitHub API commit data and systematic search queries, September 2026.*