# 🌊 Ocean Intervention — Project Discoveries
## Research Notes for Climate Technology Podcast Series
### Updated: September 2026 (v4 — fresh commit data + expanded gap analysis)

---

## Overview

Ocean intervention geoengineering — marine cloud brightening, ocean fertilization, artificial upwelling, ocean alkalinity enhancement, and ocean thermal energy conversion — represents the **largest complete absence** in the open-source climate tech GitHub ecosystem. After searching across 10+ query strategies, we found **zero dedicated repositories** for ocean geoengineering.

This is not a GitHub problem — it's a **field problem**. Ocean geoengineering is underfunded, under-researched, and ethically contested. The scientific literature exists (Nature, Science, PNAS), but the code does not.

---

## The Ocean Gap: What's Missing

### Zero Repositories Found Across All Searches

| Search Query | Results |
|-------------|--------|
| `ocean climate intervention` | 0 repos |
| `ocean cloud brightening marine geoengineering` | 0 repos |
| `ocean alkalinization` | 0 repos |
| `marine geoengineering simulation` | 0 repos |
| `ocean fertilization climate` | 0 repos |
| `artificial upwelling ocean climate` | 0 repos |
| `ocean thermal energy conversion geoengineering` | 0 repos |
| `marine cloud brightening simulation` | 0 repos |
| `ocean alkalinity enhancement` | 0 repos |
| `climate ocean intervention` | 0 repos |

**Total ocean geoengineering repos found: 0. Across 10+ queries. On GitHub — the world's largest code hosting platform.**

### Contrast with Other Themes

| Theme | Total Repos Found | Most Active Repo | Stars |
|-------|------------------|------------------|-------|
| ☀️ Solar Geoengineering | 8+ | ClimateMARGO.jl | 73 |
| 🌍 Carbon Capture | 9+ | open-sustainable-technology | 2,552 |
| 🌊 Ocean Intervention | **0** | N/A | N/A |

---

## Ocean-Adjacent Tools (What Does Exist)

### 1. NOAA-GFDL MDTF-diagnostics (Closest Ocean Tool)
- **Repo:** [NOAA-GFDL/MDTF-diagnostics](https://github.com/NOAA-GFDL/MDTF-diagnostics)
- **Stars:** 80 | **Language:** Jupyter Notebook | **License:** Not specified
- **Last commit:** August 14, 2026 (active)
- **Focus:** Analysis framework and collection of process-oriented diagnostics for weather and climate simulations. The **precip-buoyancy POD** (Proof-of-Concept) is the most ocean-relevant diagnostic tool in open source.

**Recent Commit Signals (8 commits pulled):**
| Date | Commit | Significance |
|------|--------|-------------|
| Aug 14, 2026 | Merge pull request #825 | Institutional maintenance continues |
| Jun 19, 2026 | Update MCS_precip_buoy_stats.rst (×4) | **5 commits for same file — intense development** |
| Jun 19, 2026 | Add MCS precipitation-buoyancy statistics POD | **New ocean-adjacent diagnostic feature** |
| Jun 8, 2026 | Merge pull request #823 | Institutional maintenance |
| Jun 8, 2026 | Update README | Documentation update |

**Key insight:** The **June 19, 2026 precip-buoyancy POD burst** (5 commits for the same file in one day) is the closest thing to an ocean intervention research tool on GitHub. But it's a **diagnostic for evaluating model accuracy**, not a simulation of ocean interventions. It evaluates how well models reproduce precipitation-buoyancy relationships — relevant for understanding ocean-atmosphere coupling, but not for simulating ocean fertilization or cloud brightening.

**Podcast Angle:** The best ocean tool on GitHub is for *evaluating models*, not *simulating interventions*. That gap — between diagnostic and intervention — is the core of the ocean geoengineering void.

---

### 2. WRF Model (Coupled Ocean-Atmosphere)
- **Repo:** [wrf-model/WRF](https://github.com/wrf-model/WRF)
- **Stars:** 1,761 | **Language:** Fortran | **License:** Apache-2.0
- **Focus:** The WRF model can be coupled with ocean models (ROMS, MOM) for coupled ocean-atmosphere simulations. But the ocean component is typically external — WRF itself is atmospheric.

**Relevant WRF commits (from our analysis):**
- v4.8.0 release (Jun 2026): aerosol physics changes with ocean-atmosphere coupling implications
- Solar radiation EOT fix (May 2026): affects ocean surface energy balance

**Key insight:** WRF-with-ocean-coupling is the closest thing to an ocean simulation tool, but it's designed for weather forecasting, not ocean intervention research. The ocean component is typically external (ROMS, MOM), and none of those are in this repo.

---

### 3. Oceananigans.jl (Foundational, but not Intervention-Focused)
- **Stars:** 1,413 (from v2 analysis)
- **Language:** Julia
- **Focus:** Turbulence-resolving ocean simulation. Used for physical oceanography, not geoengineering. No intervention modules.

**Key insight:** Oceananigans is the best ocean simulation code on GitHub, but it simulates ocean physics — not ocean interventions. It's a climate model component, not a geoengineering tool.

---

### 4. veros & OceanBioME (From v2 analysis)
- **veros:** Ocean general circulation model (Python), used for theoretical ocean dynamics
- **OceanBioME:** Biogeochemistry model coupling, used for marine ecosystem simulations
- Neither has geoengineering intervention modules

---

## The Interpretive Gap: Why Does the Ocean Empty Quadrant Exist?

### Hypothesis 1: Funding and Institutional Invisibility
Ocean geoengineering receives **far less funding** than solar or carbon approaches. The US National Oceanic and Atmospheric Administration (NOAA) has no dedicated geoengineering program. The UK's Radcliffe Institute's geoengineering program focuses on solar. Ocean algoengineering is a fringe topic at oceanographic institutions.

### Hypothesis 2: Governance and Ethical Taboo
Ocean interventions are **globally consequential** — you can't modify the ocean without affecting everyone. The London Protocol explicitly prohibits ocean fertilization. The carbon capture community at least has 45Q tax credits. Ocean geoengineering has nothing.

### Hypothesis 3: Technical Difficulty
Ocean geoengineering requires **large-scale deployment** that can't be tested in a lab. You can't simulate marine cloud brightening on GitHub. You need ships, monitors, and ocean-going campaigns. The cost of entry is millions, not thousands.

### Hypothesis 4: The "Market Failure" Pattern
Ocean geoengineering is a **global public good problem** — nobody has incentive to fund it because the benefits are diffuse and the costs are concentrated. Compare: carbon capture has private sector incentives (45Q, ESG). Solar geoengineering has military/intelligence interest. Ocean geoengineering has nobody.

---

## What an Open-Source Ocean Intervention Ecosystem Would Look Like

### Theoretical Framework
1. **Marine Cloud Brightening Simulator** — A repo that simulates ship-track cloud brightening effects using large-eddy simulation (LES). Similar to how OpenAir-Cyan is a DIY DAC, this could be a "DIY MCB" tool.
2. **Ocean Fertilization Decision Tool** — Like CarbonLens, an LCA tool for ocean fertilization vs. alternative marine interventions.
3. **Artificial Upwelling Design Repository** — Open hardware designs for ocean upwelling pumps, similar to OpenAir-Cyan's hardware approach.
4. **Ocean Alkalinity Enhancement Tracker** — A data repository for ocean alkalinity experiments, with CC0 data licensing (following tjz21's model).

### What's Missing vs. What Exists

| Ocean Intervention Concept | Equivalent in Solar | Equivalent in Carbon | Open-Source Ocean Equivalent? |
|---------------------------|---------------------|---------------------|-------------------------------|
| Climate simulation model | WRF (1,761★) | CESM, HadGEM (not on GH) | Oceananigans.jl (physics only) |
| Diagnostic/evaluation tool | PCMDI_metrics (133★) | MDTF-diagnostics (80★) | MDTF precip-buoyancy POD only |
| Economic/policy model | ClimateMARGO (73★) | DICE variants | **None** |
| Curated resource list | awesome-geoengineering (4★) | open-sustainable-technology (2,552★) | **None** |
| DIY/hardware project | GeoVision (0★, dead) | OpenAir-Cyan (76★, frozen) | **None** |
| Data/screening repo | Geo-DICE (2★) | tjz21 DAC repos (CC0, 2★) | **None** |

**Every single ocean geoengineering category is empty.** The gap is total.

---

## Episode Notes — Ocean Intervention Branch

### Key Narrative Arcs
1. **"The Empty Quadrant"** — After 10+ search queries, zero ocean geoengineering repos exist on GitHub. Compare: 8+ solar repos, 9+ carbon repos. The ocean is the missing theme.
2. **"The Diagnostic That Came Close"** — MDTF-diagnostics' precip-buoyancy POD (5 commits in one day, Jun 2026) is the closest thing to an ocean tool. But it evaluates models, not interventions.
3. **"Why Did Nobody Build It?"** — Four hypotheses: funding invisibility, governance taboo, technical difficulty, and the global public good problem.
4. **"What Would Open-Source Ocean Geoengineering Look Like?"** — We sketch the theoretical ecosystem: MCB simulators, fertilization decision tools, upwelling hardware, alkalinity trackers.

### Open Questions for Guests
- Why is there zero open-source code for ocean geoengineering when the scientific literature is growing?
- Would a "DIY marine cloud brightening" project face regulatory barriers that OpenAir-Cyan didn't?
- Is the absence of ocean geoengineering code a governance signal — implicit prohibition through lack of infrastructure?
- Should the climate-tech open-source community create an ocean intervention theme, or is the absence correct?
- What would happen if someone released ocean alkalinity enhancement data under CC0 (like tjz21's DAC materials)?

### The "Silence as Signal" Argument
The absence of ocean geoengineering code might itself be the most important finding. Just as the WRF aerosol scheme changes (solar episode) tell a story about institutional avoidance, the zero-repository result for ocean geoengineering tells a story about **which climate interventions the tech community finds permissible**. Solar gets models (even flawed ones). Carbon gets hardware (even frozen ones). Ocean gets nothing.
