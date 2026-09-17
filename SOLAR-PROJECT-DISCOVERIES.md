# ☀️ Solar Geoengineering — Project Discoveries

## Research Date: September 2026

---

## 1. WRF Model (wrf-model/WRF)
- **Stars:** 1,761 | **Language:** Fortran | **Last Updated:** Sep 16, 2026
- **Focus:** Foundational atmospheric model — the backbone of SRM simulation pipelines
- **Why it matters for the podcast:** WRF's aerosol physics modules are the de facto simulation infrastructure for solar geoengineering research. Any discussion of SRM realism must confront WRF.
- **Key recent commits (May–Jun 2026):**
  - v4.8.0 release (Jun 8, 2026) — major version with TEMPO physics updates
  - TEMPORAL aerosol-aware and hail-aware options toggled off in Registry
  - MYNN-EDMF pointer update and icloud_bl package removal
  - ShinHong PBL namelist additions and revised MMM surface layer
  - Fix for solar radiation eot calculation
- **Episode angle:** "The Simulation Stack" — how atmospheric models that were never designed for SRM are being co-opted for solar geoengineering research, and what that means for governance.

---

## 2. PCMDI Metrics (PCMDI/pcmdi_metrics)
- **Stars:** 133 | **Language:** Python | **Last Updated:** Sep 4, 2026
- **Focus:** ESM evaluation toolkit — CMIP6 metrics, process-oriented diagnostics
- **Why it matters:** PCMDI's toolkit is how we evaluate whether climate models (including those used for SRM simulations) are trustworthy. v4.2.1 released Sep 4, 2026.
- **Key recent commits (Sep 2-4, 2026):**
  - 10+ commits in 3 days — version bump to 4.2.1
  - Roundoff fix preventing mean_climate figures from showing 1.00
  - Extremes chunking improvements (memory optimization for dask)
  - New AIMIP page added
  - Variability modes dask SVD memory fix
- **Episode angle:** "How Do We Know the Model Works?" — the evaluation infrastructure that should govern SRM research, and whether it's keeping pace.

---

## 3. ClimateMARGO (ClimateMARGO/ClimateMARGO.jl)
- **Stars:** 73 | **Language:** Julia | **Last Updated:** Aug 17, 2026
- **Focus:** Idealized climate-economic modeling framework for optimizing mitigation-adaptation-geoengineering trade-offs
- **Why it matters:** MARGO is one of the few open-source tools specifically designed to model geoengineering decision-making, not just the physics.
- **Key recent commits:**
  - **Two README updates on Aug 17, 2026** — first activity after 2+ years of dormancy (Oct 2023 → Aug 2026)
  - Prior: unit_conversions.jl update (Oct 2023), Pluto integration link (Jul 2023)
- **Episode angle:** "The Revival Signal" — is MARGO's awakening a real sign of growing policy-modeling interest, or just another false start? The dormancy-revival pattern is a metaphor for the field itself.

---

## 4. Awesome Geoengineering (brandonhimpfen/awesome-geoengineering)
- **Stars:** 4 | **Language:** Python (curated list)
- **Focus:** Curated directory of geoengineering projects, research, organizations, tools, and resources
- **Key recent commits:**
  - README updates Sep 5-6, 2026 (active curation)
  - v2.0.0 released May 5, 2026
  - Regular updates: Jan 2026, Mar 2026, May 2026, Sep 2026
- **Episode angle:** "The Map" — what's in the curated list, what's missing, and who's maintaining it.

---

## 5. SRM Governance Model (jlehtomaa/OOCC_2021)
- **Stars:** 2 | **Language:** Python
- **Focus:** Simple model for solar geoengineering governance
- **Episode angle:** "Governance by Simulation" — can we model the governance of SRM before we need it?

---

## 6. Geo-DICE (PSLmodels/Geo-DICE)
- **Stars:** 2 | **Language:** MATLAB
- **Focus:** Modified DICE economic model with geoengineering components
- **Episode angle:** The DICE model is the most influential climate-economic tool ever built. Geo-DICE adds SRM to the mix — but it's barely maintained.

---

## 7. Interactive SRM Dashboard (yanpefnsc/orbital-climate-simulator)
- **Stars:** 2 | **Language:** Python
- **Focus:** Interactive mission-control dashboard for a conceptual Solar Radiation Management drone fleet
- **Last Updated:** Sep 17, 2026 (very recent!)
- **Episode angle:** "From Model to Mission Control" — the democratization angle. Are interactive tools making SRM more accessible, or more dangerous?

---

## 8. SRM Economics Model (hausfath/srm-forever)
- **Stars:** 0 | **Language:** Not specified
- **Focus:** Interactive single-page SRM economics model
- **Last Updated:** Aug 26, 2026
- **Episode angle:** The "manifesto to MVP" pipeline — how an idea becomes a deployable tool.

---

## 9. Earth System Digital Twin (prashaant1926/open-earth-digital-twin-simulation)
- **Stars:** 0 | **Language:** Not specified
- **Focus:** Distributed Earth system simulation
- **Last Updated:** Oct 10, 2025
- **Episode angle:** "The Digital Twin Dream" — building a virtual Earth that can test SRM scenarios before real-world deployment.

---

## Solar Geoengineering Commit Trend Summary

| Pattern | Evidence | Implication |
|---------|----------|-------------|
| **Institutional bursts dominate** | PCMDI: 10+ commits in 3 days for v4.2.1; WRF: v4.8.0 release with 15 commits in 3 weeks | Climate software moves in institutional sprints, not continuous community development |
| **Dormancy is the default** | ClimateMARGO: 2.5 years dormant, then 2 README updates; Geo-DICE: minimal maintenance | Individual researchers build tools, then move on; no steward culture |
| **Active curation exists** | awesome-geoengineering: updated 5 times in 2026 | The directory is alive even when the code isn't |
| **Governance tools are nascent** | OOCC_2021 (2★), Geo-DICE (2★), SRM economics (0★) | Governance modeling is far behind physics modeling |
| **New interactive tools emerging** | orbital-climate-simulator (Sep 2026), srm-forever (Aug 2026) | The "democratization" wave is real but small |
| **No dedicated SRM simulation codebase** | WRF is used but not built for SRM; no repo purpose-built for SRM radiative forcing | The simulation stack is borrowed, not purpose-built — a governance risk |

---

## Key Takeaways for Episode 1 (Solar Geoengineering)

1. **The simulation infrastructure is institutional, not community.** WRF and PCMDI are funded, staffed, and maintained by major institutions. This is both a strength (reliability) and a weakness (accessibility).

2. **The governance gap is stark.** There are maybe 3 open-source tools for SRM governance modeling, all with minimal maintenance. The physics has outpaced the policy infrastructure by a decade.

3. **Dormancy is the norm, not the exception.** ClimateMARGO's revival is noteworthy precisely because it's unusual. Most tools are built and abandoned.

4. **The interactive tools are the new story.** orbital-climate-simulator and srm-forever represent a shift toward accessible, visual SRM exploration — but they're tiny projects.

5. **The absence of purpose-built SRM code is itself a story.** No one has built an open-source SRM simulation framework from scratch. We're all adapting atmospheric models that were designed for something else.
