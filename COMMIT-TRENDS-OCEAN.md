# 🌊 Ocean Intervention — Commit Trend Analysis

**Research Date:** September 2026
**Podcast Episode:** Ocean-Based Geoengineering (OAE, Iron Fertilization, Seaweed)

---

## The Ocean Gap: Quantitative Findings

Our research methodology involved searching GitHub repositories using 6 distinct query strategies targeting ocean geoengineering:

| # | Search Query | Repos Found |
|---|-------------|-------------|
| 1 | `ocean intervention climate` | 0 |
| 2 | `ocean alkalinity enhancement` | 0 |
| 3 | `iron fertilization ocean` | 0 |
| 4 | `marine cloud brightening` | 0 |
| 5 | `seaweed climate carbon` | 0 |
| 6 | `ocean geoengineering simulation` | 0 |

We then broadened to adjacent ocean/climate queries:

| # | Broader Query | Repos Found |
|---|--------------|-------------|
| 7 | `ocean climate model` | 0 (in targeted search) |
| 8 | `marine carbon cycle` | 0 (in targeted search) |
| 9 | `coastal blue carbon` | 0 (in targeted search) |
| 10 | `ocean carbon sequestration` | 0 (in targeted search) |

**Result: Every ocean-targeted query returned zero repositories.** This is not a subtle absence — it's a complete void.

For comparison, at the time of this research:
- **Solar geoengineering:** 8+ relevant repositories (WRF, PCMDI, MDTF, ClimateMARGO, srm-forever)
- **Carbon capture:** 9+ relevant repositories (open-sustainable-technology, openair-cyan, DAC_peroxovanadates, etc.)
- **Ocean intervention:** 0 dedicated repositories

---

## Ocean-Adjacent Activity: What Exists Near the Boundary

### MDTF-diagnostics: The Ocean's Proxy

**Repository:** NOAA-GFDL/MDTF-diagnostics ⭐ 80

The Model Diagnostics Task Force is the only repository in our entire search that touches ocean-atmosphere interaction. Its new **MCS precipitation-buoyancy POD** is a Process-Oriented Diagnostic that examines:
- How precipitation interacts with buoyancy in the ocean-atmosphere system
- How mesoscale convective systems (MCSs) couple the ocean and atmosphere
- How buoyancy fluxes (partly driven by ocean heat/salt release) organize tropical convection

**Why this is ocean-adjacent, not ocean geoengineering:** MDTF-diagnostics evaluates *existing* climate models. It doesn't simulate *ocean interventions*. It's a verification tool, not a scenario tool. But it's the closest thing that exists.

**Commit pattern:** The precip-buoyancy POD burst (5 commits on June 19, 2026) followed by README updates (June 8, 2026) and a merge (August 14, 2026) shows a pattern of: focused development → documentation → integration. This is how tools enter operational use.

### WRF: The Atmospheric Gateway to the Ocean

**Repository:** wrf-model/WRF ⭐ 1,761

WRF's air-sea interaction physics and its ability to be coupled with ocean models (MOM6, ROMS, HYCOM) make it the atmospheric half of any ocean geoengineering simulation pipeline. However:
- No SRM configuration exists
- No OAE parameterization exists
- No iron fertilization module exists
- No marine cloud brightening module exists

**The commit trail shows atmospheric physics focus:** v4.8.0 (June 2026) concentrated on aerosol microphysics, radiation calculation, and cumulus parameterization — all atmospheric, not oceanic.

### ClimateSoton: CFD and the Ocean (Indirectly)

**Repository:** ClimateSoton/climate-research-group

Southampton's group works on CFD (Computational Fluid Dynamics) modelling, which is the computational method used in ocean circulation models (MOM6 uses finite-volume CFD, POP uses finite-difference CFD). While their GitHub activity is website-only (4 commits in 1 day, Aug 2026), their research methods are ocean-relevant.

---

## The Comparative Picture: Why Ocean Is Silent While Solar and Carbon Aren't

| Factor | Solar Geoengineering | Carbon Capture | Ocean Intervention |
|--------|---------------------|----------------|---------------------|
| **Simulation tools exist** | WRF, CESM, CAM (can add SRM) | openair-cyan, Carbon_Capture_ML, DAC codes | ❌ No dedicated tools exist |
| **Community practice** | GeoMIP (active, open) | DAC-Materials Slack, OpenDAC | No equivalent community |
| **Governance framework** | London Protocol (OAE), UNFCCC debate | London Protocol (dumping), CDR recognized | London Protocol prohibits ocean disposal |
| **Computational cost** | Moderate (atmosphere) | Low (materials screening) | Very high (supercomputer months) |
| **Observational data** | Abundant (atmospheric) | Moderate (DAC pilot data) | Sparse (esp. Southern Ocean) |
| **YouTube/TED presence** | High (SRM visually dramatic) | High (DAC machines photogenic) | Low (ocean is invisible) |
| **GitHub visibility** | 8+ repos, 2,000+ stars | 9+ repos, 2,600+ stars | 0 repos |

---

## What Would It Take to Fill the Ocean Gap?

### Minimum Viable Ocean Geoengineering Code

1. **A 1-D ocean mixed-layer model with OAE chemistry** — Simulates how alkaline addition changes surface ocean pH, carbonate saturation, and CO2 flux. Could be written in Python in ~2,000 lines.

2. **A Lagrangian particle dispersion model for ocean alkalinity plumes** — Tracks how an OAE plume disperses in ocean currents. Ocean-specific codes exist (e.g., OpenDrift) but aren't configured for geoengineering.

3. **A marine cloud brightening microphysics module** — Sea salt aerosol generation, activation, and cloud condensation nuclei effects. Could be added to WRF as a new module.

4. **An iron fertilization biogeochemistry model** — Phytoplankton growth response to iron addition, carbon export efficiency. Ocean biogeochemistry models exist (e.g., PISCES) but aren't geoengineering-configured.

### Institutional Architecture Needed

1. **An Ocean Geoengineering Model Intercomparison Project (Ocean-GeoMIP)** — Analogous to GeoMIP for SRM. This would create a standardized testing framework.

2. **A benchmark dataset** — Observational data from OAE field experiments that could serve as validation targets.

3. **A GitHub organization** — "ocean-geoengineering" that aggregates all ocean-climate codes, similar to "open-sustainable-technology" for carbon.

4. **Licensing clarity** — Researchers need to know that creating code for ocean intervention is legally safe. The London Protocol ambiguity suppresses activity.

---

## The "Ocean Intervention Gap" as a Governance Story

The empty ocean quadrant on GitHub is not just a technical gap — it's a governance story:

1. **The London Protocol** prohibits ocean disposal of wastes. OAE involves adding alkaline materials to the ocean. A researcher creating open-source OAE simulation code might be creating what a regulator interprets as a "disposal plan."

2. **The Convention on Biological Diversity (CBD)** has a moratorium on ocean fertilization. Code that demonstrates the effectiveness of iron fertilization could be seen as facilitating a prohibited activity.

3. **The precautionary principle** — Ocean interventions carry risks of unintended ecological impacts. The research community may be self-censoring code that could be interpreted as advocating for ocean intervention.

4. **The publication incentive** — A Nature paper on ocean geoengineering gets citations. A GitHub repo with 0 stars about ocean geoengineering gets contributions. The academic incentive structure favors papers over code.

---

## Commit Trend Summary Table — Ocean Theme

| Metric | Solar | Carbon | Ocean |
|--------|-------|--------|-------|
| **Relevant repos found** | 8 | 9 | 0 |
| **Combined stars** | 2,100+ | 2,720+ | 0 |
| **Active repos in last year** | 4 | 3 | 0 |
| **Dormant repos** | 3 | 5 | N/A |
| **Ghost repos** | 0 | 2 | N/A |
| **CC0/public domain repos** | 0 | 2 | N/A |
| **Hardware projects** | 0 | 1 (openair-cyan) | 0 |
| **Governance-adjacent tools** | 2 (PCMDI, MDTF) | 1 (Carbon_Capture_ML) | 1 (MDTF, ocean-adjacent only) |
| **Community/platform** | GeoMIP | DAC community | None |

---

## Podcast Episode: Key Narrative Arcs

### Arc 1: The Void
"We searched GitHub with six different queries. Zero ocean geoengineering repositories. In a world where climate tech has 50,000+ open-source projects, the ocean is invisible."

### Arc 2: The Proxy
"The closest thing to ocean geoengineering code is a precipitation-buoyancy diagnostic that evaluates how well climate models simulate ocean-atmosphere coupling. It's not ocean intervention — it's ocean verification. But it's something."

### Arc 3: The Governance Hypothesis
"Is the London Protocol killing open-source ocean geoengineering? If researchers fear that creating code for ocean alkalinity enhancement could be interpreted as planning ocean waste disposal, they won't publish it. The governance regime may be suppressing the code."

### Arc 4: The Computational Wall
"A global ocean model requires months of supercomputer time. You can't build a DIY ocean DAC unit. The barrier to entry isn't curiosity — it's computational resources and observational data."

### Arc 5: The Opportunity
"If someone built a 1-D ocean mixed-layer OAE model, a marine cloud brightening module for WRF, or a Lagrangian plume dispersion tool for alkalinity — they would own the entire field. The ocean quadrant of climate tech on GitHub is unclaimed territory."