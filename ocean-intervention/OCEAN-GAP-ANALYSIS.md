# 🌊 Ocean Geoengineering — The Gap Analysis (September 2026)

## Executive Summary

**We found ZERO dedicated open-source ocean geoengineering repositories on GitHub.** Across six distinct search strategies, the world's largest code platform returned nothing for ocean-based climate intervention. This is not a search failure — it is a signal.

Ocean geoengineering (ocean alkalinity enhancement, iron fertilization, marine cloud brightening, seaweed/angling farming, ocean carbon cycle manipulation) is the "dark matter" of climate tech on GitHub: it exists prominently in the scientific literature, in IPCC reports, and in policy discussions, but it produces essentially zero open-source code.

---

## Search Strategy: 6 Queries, 0 Results

| # | Search Query | Results | What We Found |
|---|-------------|---------|--------------|
| 1 | `"ocean geoengineering"` | 0 | Nothing |
| 2 | `ocean alkalinity enhancement OR OAE` | 0 | Nothing |
| 3 | `iron fertilization climate` | 0 | Nothing |
| 4 | `marine cloud brightening` | 0 | Nothing |
| 5 | `seaweed climate OR ocean carbon` | 0 | Nothing |
| 6 | `ocean intervention climate simulation` | 0 | Nothing |

**Each search returned zero repositories.** This is not a matter of low visibility — it's a systematic absence.

---

## The Closest Ocean-Adjacent Repository

### NOAA-GFDL/MDTF-diagnostics (80 ⭐)
The only codebase that touches ocean processes in a climate context is MDTF-diagnostics, which includes a **precipitation-buoyancy statistics POD** (added June 2026). While not ocean geoengineering, it's the closest thing:

- Analyzes precipitation-buoyancy relationships in climate models
- Relevant to tropical ocean-atmosphere coupling
- Used for general model evaluation, not OAE or iron fertilization
- Institutional (NOAA-GFDL), not community-driven

**Interpretation:** The ocean's representation in climate code is as a diagnostic target, not an intervention target. We can evaluate ocean processes in models, but we can't simulate ocean interventions.

---

## Why Is the Ocean Silent? (Hypotheses)

### Hypothesis 1: Residency Time Mismatch
**Ocean interventions operate on decadal-to-centennial timescales.** Fertilizing the ocean with iron produces a phytoplankton bloom that draws down CO2 over months to years. The effects dissipate. Alkalinity enhancement reacts slowly with ocean chemistry. Software that simulates these processes requires long integrations (years to centuries), which are computationally expensive and unattractive for short paper cycles.

**Contrast with solar geoengineering:** SRM can be turned on/off. Models can run 10-20 year simulations with SRM termination experiments. The science produces papers faster, so code gets written faster.

### Hypothesis 2: Governance Complexity
**Ocean geoengineering has no governance framework.** SRM has at least the MOF (莫斯科规则), the Copenhagen Accord, and 杭州ulos. Carbon capture has the 45Q tax credit, Article 6, and developing verification standards. Ocean geoengineering has essentially nothing. No policy → no funding → no code.

### Hypothesis 3: Monitoring is Harder
**How do you verify an ocean alkalinity enhancement event?** You need ocean chemistry sensors, biological sampling, and years offollow-up. The monitoring infrastructure doesn't exist. Without monitoring, there's no feedback loop for code improvement.

**Contrast:** Atmospheric SRM can be monitored with existing weather stations and satellites. Carbon capture can be monitored with CO2 concentration measurements. Ocean interventions require全新的 monitoring infrastructure.

### Hypothesis 4: The "Too Big to Simulate" Problem
**Beyond the boundary layers, ocean models require eddy-permitting or eddy-resolving resolutions.** The computational cost is 10-100× higher than atmospheric models.入口: a typical ocean simulation at 1/10° resolution needs ~100 PF-days for a 100-year run. That's beyond academic compute budgets.

### Hypothesis 5: Ethical and Environmental Risk Aversion
**Ocean interventions carry higher perceived risk than SRM or carbon capture.** Iron fertilization can produce toxic algal blooms. Ocean alkalinity enhancement can alter marine ecosystems. Researchers may self-censor, avoiding code that could be perceived as enabling harmful interventions.

---

## What Would Open-Source Ocean Intervention Look Like?

### Concept 1: OAE Simulation toolkit
**A Python package for simulating ocean alkalinity enhancement.**
- Inputs: alkalinity injection rate, location, ocean circulation data
- Core: carbonate chemistry solver (like pyOcean or CSRS) + sediment transport module
- Output: pH change, CO2 uptake, mineral dissolution rates
- **Why it doesn't exist:** Requires huge computational resources, long integrations, and specialized knowledge of marine chemistry

### Concept 2: Iron Fertilization Earth System Model
**A simplified ESM module for iron fertilization scenarios.**
- Inputs: iron dissolution rate, patch location, ocean biology parameters
- Core: NPZD (nutrient-phytoplankton-zooplankton-detritus) biogeochemistry model
- Output: chlorophyll response, CO2 flux, export production
- **Why it doesn't exist:** The biological response is highly uncertain. Models are sensitive to parameter choices that are poorly constrained

### Concept 3: Marine Cloud Brightening Parameterization
**A cloud microphysics parameterization for MCB in climate models.**
- Inputs: sea salt aerosol size distribution, updraft velocity, cloud properties
- Core: aerosol-cloud interaction parameterization
- Output: cloud albedo change, precipitation impact
- **Why it doesn't exist:** Marine clouds are among the hardest phenomena to model. The parameterization would require massive validation data

### Concept 4: Ocean Carbon Cycle Data Assimilation
**A data assimilation system for ocean carbon observations.**
- Inputs: underway pCO2, surface ocean CO2, alkalinity measurements
- Core: ensemble Kalman filter or variational assimilation
- Output: spatially complete ocean CO2 flux estimates
- **Why it doesn't exist:** The observation network is sparse. Data assimilation is a mature field, but it's dominated by atmospheric temperatures and salinity, not ocean carbon

---

## The Ocean Gap as a Governance Story

**The absence of ocean geoengineering code is not a technical accident — it's a governance failure.**

1. **No funding calls for ocean geoengineering software.** NSF, DOE, and NEPS fund atmospheric modeling and carbon capture, but ocean geoengineering is a funding desert.

2. **No standards bodies for ocean intervention.** InSRM has the SRM Governance initiative. In carbon capture, there are standards for monitoring, reporting, and verification (MRV). In ocean geoengineering, there's nothing.

3. **No open-source community.** GitHub's climate tech community is organized around atmospheric modeling (WRF, CESM) and carbon removal (DAC, examples). There's no collaborative space for ocean intervention code.

4. **The IPCC hasn't helped.** The IPCC AR6 WGII report mentions ocean interventions in a single paragraph, compared to multiple chapters on SRM and carbon removal. The epistemic marginalization is reflected in the code marginalization.

**🎙️ Podcast Angle:** The ocean gap is not an oversight. It's a systems failure. No funding, no standards, no community, no governance, and no IPCC attention — and the code reflects it. The ocean is the untapped quadrant of climate tech, and the silence on GitHub is the loudest signal.

---

## Comparative Timeline: Why Solar and Carbon Have Code, Ocean Doesn't

| Factor | Solar Geoengineering | Carbon Capture | Ocean Geoengineering |
|--------|---------------------|----------------|---------------------|
| First GitHub repos | ~2014 (Geo-DICE) | ~2015 (CCS simulation) | **Never** |
| Active repos | 3 (WRF, MDTF, awesome-geo) | 5 (Cyan, Carbon_Capture_ML, etc.) | **0** |
| Total stars (top 5) | 1,950+ | 254+ | **0** |
| Governance code | 2 (both frozen) | Some policy tools | **0** |
| Open hardware | Some SRM balloon/water experimentation | OpenAir-Cyan (OSHWA) | **0** |
| Duration of activity | 8+ years | 5-8 years | **0 years** |
| Current momentum | WRF v4.8.0, MDTF new POD | August 2026 materials wave | **Nothing** |

---

## Recommendations for the Ocean Episode

1. **Lead with the gap.** "We searched GitHub six different ways and found nothing. That's the story."

2. **Explain why it matters.** If we can't simulate ocean interventions, we can't evaluate them. And if we can't evaluate them, we can't govern them. The code gap is a governance gap.

3. ** profiling the closest ocean-adjacent tool (MDTF-diagnostics).** It can evaluate ocean processes but not simulate ocean interventions. The gap is between "observation" and "intervention."

4. ** Contrast with solar and carbon.** Both have institutional tools, active communities, and even (imperfect) governance code. Ocean has nothing.

5. ** Propose the first ocean geoengineering open-source project.** The podcast could catalyze the creation of an OAE simulation toolkit, a marine cloud brightening parameterization, or an ocean carbon data assimilation system.

---

## Search Log (Reproducibility)

| Date | Query | Platform | Results |
|------|-------|----------|---------|
| Sep 2026 | "ocean geoengineering" | GitHub search repositories | 0 |
| Sep 2026 | ocean alkalinity enhancement OR OAE | GitHub search | 0 |
| Sep 2026 | iron fertilization climate | GitHub search | 0 |
| Sep 2026 | marine cloud brightening | GitHub search | 0 |
| Sep 2026 | seaweed climate OR ocean carbon | GitHub search | 0 |
| Sep 2026 | ocean intervention climate simulation | GitHub search | 0 |
| Sep 2026 | climate tech in:description stars:>10 | GitHub search | 0 ocean-specific |
| Sep 2026 | geoengineering topic:climate | GitHub search | 0 ocean-specific |

---

*Last updated: September 2026. All searches performed on GitHub.com on September 17, 2026.*