# ☀️ Episode 1: Solar Geoengineering — Research Notes

## Theme Overview
Solar geoengineering (Solar Radiation Management, SRM) aims to reflect a small fraction of sunlight back to space to cool the planet. This episode explores the open-source simulation landscape, key modeling projects, and the governance questions surrounding SRM.

---

## 🔍 Discovered Projects

### 1. ClimateMARGO/ClimateMARGO.jl
- **Stars:** 73 | **Language:** Julia | **Last Updated:** Aug 17, 2026
- **Focus:** Idealized climate-economic modelling framework for optimizing trade-offs between emissions mitigation, adaptation, and geoengineering
- **Why it matters:** The most active and starred Julia-based climate-econ integration model. Bridges the gap between physics-based climate models and economic optimization — essential for SRM cost-benefit analysis.
- **Key commit pattern:** Bursty development — 2 commits on Aug 17, 2026 (README updates), then long gaps from 2022-2023. This is typical of research software: intensive development pushes followed by long dormancy.

### 2. PSLmodels/Geo-DICE
- **Stars:** 2 | **Language:** MATLAB | **Last Updated:** Sep 27, 2018
- **Focus:** Modified DICE (Dynamic Integrated Climate-Economy) model that includes geoengineering as a policy lever
- **Why it matters:** The DICE model is the foundational economic framework for climate policy. This version explicitly model geoengineering — the first major IAM to do so. Now dormant (last commit 2018).
- **Key commit pattern:** Only 4 commits total, all from 2016-2018. This is a "push-and-abandon" research project — common for academic codebases.

### 3. brandonhimpfen/awesome-geoengineering
- **Stars:** 4 | **Language:** Python | **Last Updated:** Sep 6, 2026
- **Focus:** Curated list of geoengineering projects, research, organizations, tools, and resources
- **Why it matters:** The best single point of entry for the field. Actively maintained with 7 commits across 2025-2026, including a v2.0.0 release in May 2026.
- **Key commit pattern:** Steady, regular updates — Jan 2026, Mar 2026, May 2026 (v2.0.0), Sep 2026. This is the most consistently maintained geoengineering resource on GitHub.

### 4. KOSASIH/GCCS-Core
- **Stars:** 9 | **Language:** Python | **Last Updated:** Oct 29, 2024
- **Focus:** Global Climate Control System — foundational framework with core algorithms, data pipelines, and simulation tools
- **Why it matters:** Ambitious attempt to build an end-to-end open-source climate control simulation stack. The "Global Climate Control System" name alone raises governance questions worth discussing on the podcast.
- **Key commit pattern:** 10 commits all on a single day (Oct 29, 2024) — a massive initial push, then silence. Classic "launch event" pattern with no sustained development.

### 5. jlehtomaa/OOCC_2021
- **Stars:** 2 | **Language:** Python | **Last Updated:** Unknown
- **Focus:** A simple model for solar geoengineering governance
- **Why it matters:** Governance-focused SRM model — rare in the open-source landscape. Most SRM code focuses on physics; this tackles the political/social dimension.

### 6. cjcarlson/geomalaria
- **Stars:** 3 | **Language:** R
- **Focus:** Malaria risk modeling in a world with solar geoengineering
- **Why it matters:** Highlights the second-order ecological concerns of SRM.geoengineering could alter precipitation patterns, affecting disease vectors. This is the kind of unintended-consequence modeling the podcast should spotlight.

---

## 📊 Commit Trend Analysis — Solar Geoengineering Theme

| Pattern | Observation | Podcast Angle |
|---------|-------------|---------------|
| **Bursty institutional development** | ClimateMARGO had 2 commits in one day (Aug 17, 2026), then 2-year gaps | "Research software is event-driven, not sustained"\|
| **Academic abandonware** | Geo-DICE: 4 commits over 2 years, then 8 years of silence | "Professors build tools for papers, not communities"\|
| **Community curation survives** | awesome-geoengineering is the only consistently maintained repo | "Lists outlive models — the open-source geoengineering ecosystem is curated, not built"\|
| **Single-day launches** | GCCS-Core: 10 commits on Oct 29, 2024, then dead | "The GitHub launch event is a mirage — momentum rarely persists"\|
| **Dormancy is the default** | 4 of 6 SRM repos have no commits in 12+ months | "Solar geoengineering code is mostly frozen in time"\|

### Key Insight
The SRM open-source ecosystem is characterized by **intermittent bursts of activity followed by long dormancy**. No single project has sustained continuous development. This raises a critical question for the episode: *Can open-source models ever be credible for a technology that requires continuous, real-time simulation to inform policy?*

---

## 🎙️ Episode Talking Points

1. **The DICE model legacy** — How an economics model from the 1990s still shapes SRM policy debates, and why the geoengineering variant is dormant
2. **Julia vs. MATLAB vs. Python** — The language divide in climate simulation. Julia's ClimateMARGO is powerful but small; Python dominates but lacks dedicated SRM tools
3. **Governance is the missing code** — The only SRM governance model (OOCC) has 2 stars. We're not building the tools to govern what we can't yet simulate
4. **The awesome-geoengineering paradox** — The best-maintained resource is a list, not a simulation. Curation is easier than computation
5. **Second-order effects** — geomalaria shows that SRM's precipitation impacts could be as dangerous as the warming it aims to fix

---

## 📋 Key Questions for Guests

- Why is there no open-source SRM model with the fidelity of, say, an NWP weather model?
- What would it take to build a living, continuously-updated SRM simulation?
- Should geoengineering models be governed differently because of their dual-use nature?
- How do we validate models that can't be run experimentally on the real climate?

---

## 🔗 Links
- [ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- [Geo-DICE](https://github.com/PSLmodels/Geo-DICE)
- [awesome-geoengineering](https://github.com/brandonhimpfen/awesome-geoengineering)
- [GCCS-Core](https://github.com/KOSASIH/GCCS-Core)
- [OOCC_2021](https://github.com/jlehtomaa/OOCC_2021)
- [geomalaria](https://github.com/cjcarlson/geomalaria)
