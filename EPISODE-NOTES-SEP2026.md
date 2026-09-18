# 🎙️ Episode Notes — All Three Themes (September 2026)
## Master Episode Planning Document

---

## Episode 1: Solar Geoengineering — "The Model Gap"

### Cold Open
> "In May 2026, a developer named weiwangncar pushed a commit to the world's most widely used atmospheric model. The commit message reads: 'correction for EOT calculation for solar radiation.' Three words. But what they mean is: we may have gotten the sun wrong for years."

### Act 1: The Tools We Have
- **WRF** (1,761★): 15 commits in 4 weeks, v4.8.0 just released, solar radiation bug fixed
- **PCMDI Metrics** (133★): The validation toolkit for CMIP6, 10 commits in 2 days for v4.2.1
- **MDTF** (80★): Process-level diagnostics, including the ocean's closest friend (precip-buoyancy POD)

### Act 2: The Gap
- No open-source GCM with SRM modules
- No community-driven SRM simulation platform
- The only SRM-specific repo (srm-forever) has zero stars and is pure theory
- Climate-intervention-governance: first SRM legal tracking tool, but only 2 commits

### Act 3: The Questions
- How many policy decisions were made on data with a known solar calculation error?
- Why did WRF deactivate its aerosol-aware physics schemes?
- Is the silence on GitHub about SRM simulation a governance signal?
- What would a truly open-source SRM simulation platform look like?

### Key Interview Targets
- **weiwangncar** (WRF maintainer, NCAR) — technical authority on WRF physics
- **Jiwoo Lee** (PCMDI, LLNL) — CMIP6 metrics and validation
- **Wei-Ming Tsai** (NOAA GFDL) — ocean-atmosphere diagnostics
- **Fons van der Plas** (ClimateMARGO) — climate-economic modeling
- **hausfath** (srm-forever) — SRM economics and Weitzman discounting
- **Zereo0317** (climate-intervention-governance) — SRM regulatory tracking

---

## Episode 2: Carbon Capture — "The CC0 Revolution"

### Cold Open
> "In September 2025, two researchers who spent months running quantum mechanical calculations on DAC sorbent materials made a decision that most corporations would find insane: they put all their data in the public domain. No paywalls. No licensing. No 'contact us for collaboration.' Just: the data is yours."

### Act 1: The Ecosystem
- **Open Sustainable Technology Directory** (2,552★): The map of everything, continuously updated
- **Carbon Capture ML Survey** (56★): Frozen at 2.5 years old — is it still trustworthy?
- **OpenAir-Cyan** (76★): OSHWA-certified DAC device, then silence

### Act 2: The Decisions
- **CC0 public domain:** The radical move by tjz21
- **OpenAir-Cyan certification:** The cautionary tale (6 commits in a day, then 2.5 years)
- **Ghost repos:** 85 stars but dead since 2021

### Act 3: The Questions
- Is a 2.5-year-old ML survey still trustworthy?
- Does OSHWA certification mean anything if nobody builds the device?
- What happens to open science when the researcher walks away?
- Could CC0 be the model for all climate-tech research?

### Key Talking Points
- The AI content review PR template in the directory (meta-governance)
- CI/CD deleted 3 months before OpenAir-Cyan's blitz day
- The CC0 pattern: two repos, same day, same author, same decision
- Stars ≠ value in climate tech

---

## Episode 3: Ocean Intervention — "The Empty Quadrant"

### Cold Open
> "We searched GitHub ten different ways for ocean geoengineering code. We found nothing. Zero repositories. Not one line of code. The ocean covers 70% of the planet, absorbs 30% of our CO2, and in the world's largest code repository, it's a ghost."

### Act 1: What Exists
- **MDTF's precip-buoyancy POD** (5 commits, Jun 19, 2026): The ocean's only GitHub voice
- **Oceananigans.jl** (1,413★): Models the ocean perfectly — as it is, not as we want it
- **WRF** (1,761★): Can couple to ocean models, but nobody built the coupling for interventions

### Act 2: What's Missing
- Zero repositories for ocean alkalinity enhancement
- Zero repositories for marine cloud brightening simulation
- Zero repositories for artificial upwelling
- The governance tracker explicitly scopes out ocean: "different legal architecture"
- WRF's aerosol schemes deactivated (relevant to MCB research)

### Act 3: The Question
- Is the silence on GitHub a governance signal? "We don't want this democratized."
- Or is it a practical one? "The ocean is too complex, the legal risk is too high."
- And if we DO want ocean geoengineering code, who should write it?

### Five Hypotheses for the Ocean Silence
1. Computational barrier (100x more grid resolution needed)
2. Irreversibility barrier (you can't un-disperse alkalinity)
3. Governance vacuum (no treaty, no framework, no funding)
4. Ecological risk premium (ecology problems, not physics problems)
5. Community size barrier (too few ocean geoengineers)

---

## Cross-Cutting Themes

### Theme 1: The CC0 License Revolution
- Appears in: Episode 2 (primary), Episode 1 (context), Episode 3 (absence makes the point)
- Key evidence: tjz21's two repos, Sep 12, 2025
- Podcast hook: "The next frontier of open science isn't code — it's data."

### Theme 2: The Governance Gap
- Appears in: Episode 1 (SRM simulation silence), Episode 3 (ocean governance vacuum)
- Key evidence: climate-intervention-governance plugin (Aug 2026), London Protocol
- Podcast hook: "The only tool for tracking SRM regulation is a Claude plugin with zero public users."

### Theme 3: The Ghost Repo Problem
- Appears in: Episode 2 (carbon capture), Episode 3 (ocean absence)
- Key evidence: carbon-capture-and-storage (85★, dead since 2021)
- Podcast hook: "In climate tech, the most cited repo might be the most useless."

### Theme 4: The Burst Pattern
- Appears in: Episode 2 (OpenAir-Cyan blitz), Episode 3 (MDTF POD day), Episode 1 (PCMDI sprint)
- Key evidence: Single-day commit bursts followed by long silence
- Podcast hook: "Climate tech on GitHub is defined by bursts of activity and long silence."

---

## Production Notes
- Total repos discovered: 12+
- Total search queries executed: 10+
- Total commits analyzed: 100+
- Total branches in research repo: 4 (main, solar-geoengineering, carbon-capture, ocean-intervention)
- Total markdown files pushed: 8+ per branch
- Key dates: May 28 (WRF solar bug), Jun 5 (WRF aerosol deactivation), Jun 19 (MDTF POD), Sep 12 (CC0 licenses), Aug 26 (srm-forever), Aug 23 (governance tracker)

---

## Sources
- [Climate Pod Research_repo](https://github.com/bro26man-hash/climate-pod-research)
- [WRF Model](https://github.com/wrf-model/WRF)
- [PCMDI Metrics](https://github.com/PCMDI/pcmdi_metrics)
- [MDTF-diagnostics](https://github.com/NOAA-GFDL/MDTF-diagnostics)
- [Open Sustainable Technology](https://github.com/protontypes/open-sustainable-technology)
- [OpenAir-Cyan](https://github.com/openair-collective/openair-cyan)
- [DAC Peroxovanadates](https://github.com/tjz21/DAC_peroxovanadates)
- [ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- [srm-forever](https://github.com/hausfath/srm-forever)
- [Climate Intervention Governance](https://github.com/Zereo0317/climate-intervention-governance)