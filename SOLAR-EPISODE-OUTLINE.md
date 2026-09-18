# ☀️ Episode 1 Outline: "Why Is There So Little Code for Blocking the Sun?"
## Solar Geoengineering GitHub Research | Climate Pod Research

---

## Episode Metadata
- **Title:** "Why Is There So Little Code for Blocking the Sun?"
- **Theme:** Solar Geoengineering (SRM)
- **Duration target:** 45-60 minutes
- **Research basis:** 6 GitHub repositories, 60+ commits analyzed
- **Key GitHub repos:** WRF, PCMDI/pcmdi_metrics, NOAA-GFDL/MDTF-diagnostics, ClimateMARGO/ClimateMARGO.jl, hausfath/srm-forever, yanpefnsc/orbital-climate-simulator

---

## Act 1: The Establishment (15 min)

### Opening Image
> "On September 4th, 2026, the climate model evaluation community did something remarkable. In a single day, they pushed 10 commits to a Python repository. They fixed a rounding bug that could mask a 0.004°C warming signal. They optimized memory handling for datasets the size of continents. But not a single commit was about simulating solar geoengineering."

### The Big Three
1. **WRF (1,763★)** — The atmospheric workhorse
   - v4.8.0 released June 2026 with a direct solar radiation correction
   - Aerosol-aware physics module being *deprecated* (not enhanced)
   - 7 active developers across NCAR, NOAA, and universities
   - **Quote for show:** "The most sophisticated atmospheric model on Earth is getting better at simulating sunlight — and simultaneously moving away from aerosol schemes."

2. **PCMDI Metrics (133★)** — The quality gatekeepers
   - v4.2.1 released September 2026 with 10 commits in 1 day
   - Roundoff fix: prevents "1.00" masking of climate signals
   - Dask-based SVD: enables analysis of massive CMIP6 datasets
   - **Quote for show:** "If you can't measure it precisely, you can't evaluate whether SRM makes things worse."

3. **MDTF Diagnostics (80★)** — The process detectives
   - Precipitation-buoyancy POD: 5 commits on a single file in one day
   - The closest thing to an SRM evaluation tool in open source
   - Quarterly metrics workflow: production-grade monitoring
   - **Quote for show:** "We can evaluate Earth System Models down to the level of individual rain clouds — but we have no tool to evaluate what happens when you add a layer of sulfate to the stratosphere."

### Act 1 Key Insight
> "The infrastructure for evaluating climate models is thriving. The infrastructure for simulating geoengineering is almost nonexistent. We have better tools to measure global temperature than to model what happens if we try to cool the planet."

---

## Act 2: The Rebels (15 min)

### srm-forever (0★)
- **Theory:** Weitzman certainty-equivalent discounting applied to SRM cost dynamics
- **Question answered:** "What does it cost to keep SRM going forever?"
- **Commit pattern:** 4 commits in a single day — perfectly ordered architecture
- **The catch:** Zero stars, zero forks, zero community
- **Quote for show:** "This is the most theoretically ambitious SRM project on GitHub — and nobody has starred it. It's like a paper published in an empty journal."

### Orbital-Climate-Simulator (2★)
- **What it is:** A 48-hour prototype simulating an SRM drone fleet
- **Tech stack:** Python + SQLite + matplotlib + Streamlit
- **Commit pattern:** 12 commits in 2 days — feature-first sprint
- **The catch:** It's a concept, not a validated model
- **Quote for show:** "In two days, one developer built a mission-control dashboard for a solar geoengineering drone fleet. SQLite for telemetry, matplotlib for visualization, Streamlit for the UI. It's the closest thing to SRM mission control in open source — and it was built in a weekend."

### ClimateMARGO (73★, dormant)
- **What it is:** The only open-source optimization framework for mitigation-vs-SRM trade-offs
- **Commit pattern:** 12 commits in January 2022, then 2.5 years of silence, then 2 README updates
- **The ghost pattern:** Papers cite it, nobody maintains it
- **Quote for show:** "ClimateMARGO is a ghost. Two README updates after 2.5 years of silence — but zero code commits. It's the academic haunting: cited but never run, referenced but never maintained."

### Act 2 Key Insight
> "The SRM software ecosystem has three rebels building in isolation, one ghost that everyone cites but nobody maintains, and zero community. The theory exists. The prototypes exist. What doesn't exist is a conversation."

---

## Act 3: The Gap (15 min)

### The Five Missing Things
1. **No SRM scenario module for WRF** — the world's most popular atmospheric model has no geoengineering plugin
2. **No CMIP6 SRM experiments in PCMDI** — the evaluation toolkit doesn't include geoengineering metrics
3. **No Marine Cloud Brightening code** — not a single repo simulates ship tracks or cloud seeding
4. **No real-time SRM monitoring** — orbital-climate-simulator is a weekend project, not an operational system
5. **No SRM risk assessment frameworks** — srm-forever handles costs but not climate catastrophic risks

### The Structural Problem
- The **evaluation community** (PCMDI, MDTF) doesn't think about SRM
- The **modeling community** (WRF) doesn't have resources for SRM scenarios
- The **theory community** (srm-forever, ClimateMARGO) works in isolation
- The **prototyping community** (orbital-climate-simulator) hasn't connected to either

### The Opportunity
> "What if someone built an SRM plugin for WRF? What if PCMDI added geoengineering metrics to its evaluation toolkit? What if ClimateMARGO's optimization framework was connected to a real-time monitoring system? The pieces exist. They just haven't been assembled."

### Act 3 Key Insight
> "The gap in solar geoengineering code isn't a technology gap. It's a coordination gap. The evaluation infrastructure is mature. The atmospheric models are sophisticated. The economic theory is elegant. What's missing is a community that connects these worlds."

---

## Closing Segment (5 min)

### The Railway Track Metaphor
> "Imagine a railway system with world-class tracks (WRF), precision signaling (PCMDI), and train diagnostics (MDTF). But there are no trains. No one has built the vehicle that runs on this infrastructure. That's solar geoengineering on GitHub. We have the rails. We just don't have the train."

### Call to Action for Listeners
- **Developers:** The WRF model needs an SRM module. The contribution window is open.
- **Scientists:** PCMDI is looking for new metrics. Why not propose SRM-specific ones?
- **Economists:** srm-forever needs collaborators. The Weitzman framework is ready for real data.
- **Everyone:** The ocean geoengineering gap is even bigger. (Tune in next episode.)

### Final Quote
> "On September 4th, they fixed a rounding bug. On August 26th, someone coded the economics of forever. On September 15th, a weekend warrior built a drone fleet. The pieces are there. The question is whether we assemble them."

---

## Production Notes

### Sound Design Suggestions
- **Act 1:** Keyboard clacking (typing), server hum — the sound of institutional infrastructure
- **Act 2:** Pitched-downElectronic heartbeat — the isolation of individual builders
- **Act 3:** Silence, then a single音符 — the gap, then the possibility
- **Closing:** Railway sounds transitioning to smooth travel — from tracks to train

### Visual Aids (if video/podcast video)
- Commit velocity chart comparing all 6 repos
- Timeline of commits overlaid with release dates
- Solar radiation fix commit diff screenshot
- PCMDI v4.2.1 release commit list
- srm-forever repo screenshot (zero stars is powerful)
- Orbital-climate-simulator dashboard preview

### Pre-Show Research Refresh
- [ ] Check PCMDI/pcmdi_metrics for v4.2.2 or newer
- [ ] Check WRF for v4.8.1 or post-release commits
- [ ] Check ClimateMARGO for any new code commits (unlikely but worth verifying)
- [ ] Check orbital-climate-simulator for v2 development
- [ ] Re-read srm-forever's Weitzman discounting essay

---

*Last updated: September 2026 | Research basis: 6 GitHub repositories, 60+ commits, 3 development patterns identified*