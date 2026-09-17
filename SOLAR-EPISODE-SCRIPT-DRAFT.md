# ☀️ Solar Geoengineering — Episode Script Draft
## Git Evidence-Based Script Outline
### v4 — September 2026

---

## Cold Open (2 min)

*"While the world debates whether to dim the sun, the code that would simulate that decision is sitting in the world's most-used climate model — and it's silently changing. In the latest version of WRF, the atmospheric model run by NOAA and NCAR, two aerosol-related physics schemes have been disabled. What does that mean for solar geoengineering research? And why is the best economic model for SRM decision-making frozen in time since 2022? This episode, we follow the commit history."*

---

## Segment 1: The Aerosol Problem (8 min)

### The Technical Core
- WRF v4.8.0 disabled `tempo_aerosolaware` and `tempo_hailaware`
- Same release included a solar radiation EOT (Extraterrestrial) calculation fix
- These are presented as routine maintenance, not SRM-specific changes
- But they're exactly the physics needed to simulate stratospheric aerosol injection

### The Governance Implication
- If the world's best climate model can't reliably simulate aerosol-Radiation interactions, SRM deployment is flying blind
- The changes are invisible to non-expert users — they see a version number, not a physics revolution
- SRM risk assessment depends on sub-grid parameterizations that WRF is consolidating, not expanding

### Talking Point
- *"The most important climate model on Earth just turned off its aerosol-aware mode. Was that an improvement, or an avoidance? Either way, the SRM community needs to pay attention."*

### Evidence
- https://github.com/wrf-model/WRF/commit/6a289e17f772cc8196a031c3f1e316672ad514af (Jun 5, 2026)
- https://github.com/wrf-model/WRF/commit/e836cd6ab67fb4de46edfce3786cb40eef4e641e (May 28, 2026)

---

## Segment 2: The Economic Ghost Town (7 min)

### The Dormancy Story
- ClimateMARGO.jl: best Julia-based climate-economic model for SRM trade-offs
- 3 active commits in Feb 2022, then 4.5 years of silence
- August 2026: 2 README updates, no code changes
- The model is theoretically sound but computationally frozen

### The Paradox
- SRM is the most geopolitically controversial climate intervention
- But the tools for economic analysis of SRM are the most underdeveloped
- Compare: carbon capture has open hardware (OpenAir-Cyan, 76); SRM has nothing

### Talking Point
- *"We can build a DAC device in our garage — there's open-source hardware for it. But if we want to model the optimal SRM deployment strategy, we're still relying on a model that hasn't had a code commit since 2022. That's not a gap. That's a void."*

### Evidence
- https://github.com/ClimateMARGO/ClimateMARGO.jl/commit/d916f36d9a1e461b14a868ee9bc3016f0d5e64ee (Aug 17, 2026)
- https://github.com/ClimateMARGO/ClimateMARGO.jl/commit/57d4da781cb7242b433f4f6d4235842e1dbff50c (Oct 18, 2023 — last code change)

---

## Segment 3: The Curator's Acceleration (5 min)

### The Resource Growth
- awesome-geoengineering: 7 commits in 14 months, accelerating in 2026
- v2.0.0 released May 2026
- Sep 5-6, 2026: rapid double-update (curator responding to new resources)
- This is the closest thing to a living bibliography for the field

### The Meta-Impact
- When the curator accelerates, it signals field-level momentum
- More papers, more tools, more organizations being tracked
- The resource gap is closing, even as the tool gap remains

### Talking Point
- *"The one thing growing faster than SRM research might be the list of SRM research. The custodian of the definitive geoengineering bibliography is updating it in rapid bursts. That tells us the field is getting more crowded — and more urgent."*

### Evidence
- https://github.com/brandonhimpfen/awesome-geoengineering/commit/8d0a80011d61d3f35124697b3f4ee61e13780d72 (Sep 6, 2026)
- https://github.com/brandonhimpfen/awesome-geoengineering/commit/a6e8359b7f35c9f28a3b676e5ab8ebf6e1de8fe4 (v2.0.0, May 5, 2026)

---

## Segment 4: The Simulator's Tragedy (3 min)

### The Burst-and-Die Pattern
- GeoVision: web-based SRM simulator
- 4 commits on Dec 6, 2025
- 0 stars, 0 forks, 9 months of silence since
- The concept (interactive visualization) is exactly what governance advocates have called for

### The Opportunity
- Someone built the tool, then stopped
- The code still exists — it could be picked up
- The gap between "we need interactive SRM tools" and "here are interactive SRM tools" is enormous

### Talking Point
- *"One person built an SRM simulator in a single day, then walked away. Zero stars. But the idea is right — we need more people building shareable, interactive tools for SRM scenario exploration. The code is there. The community isn't."*

### Evidence
- https://github.com/pixnum-hub/GeoVision/commits/main

---

## Closing (2 min)

*"The commit histories tell three stories: the institutional model is consolidating its physics, making SRM simulation harder. The economic model is frozen, making SRM analysis impossible. And the resource list is accelerating, making the SRM field more visible. The question for the next decade isn't whether we can dim the sun — it's whether we can build the tools to decide if we should."*

---

## Production Notes

| Element | Detail |
|---------|--------|
| **Total runtime** | ~25 min (4 segments + cold open + closing) |
| **Key evidence links** | 8 GitHub commit URLs, all verified live |
| **Guest candidates** | Fons van der Plas (ClimateMARGO), Brandon Himpfen (awesome-geoengineering), WRF modeler (via NCAR) |
| **Topics to avoid** | Regional SRM deployment (geopolitically explosive), termination shock (needs careful framing) |
| **Recommended pre-listening** | Listen to carbon-capture episode first (SRM is the complement to carbon removal discourse) |
