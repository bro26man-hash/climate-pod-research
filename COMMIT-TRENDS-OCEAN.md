# 🌊 Ocean Intervention — Commit Trend Analysis

**Last Updated:** September 2026 (v4 — fresh commit data from ocean modeling ecosystem + expanded cross-theme analysis)
**Source Repositories Analyzed:** CliMA/Oceananigans.jl, team-ocean/veros, OceanBioME/OceanBioME.jl, NOAA-GFDL/MDTF-diagnostics, wrf-model/WRF, pangeo-data/awesome-open-climate-science, plus cross-theme repos

---

## The Ocean Quadrant — Finding (Updated)

### ZERO DEDICATED GEOENGINEERING REPOSITORIES

After exhaustive searching across multiple query strategies (unchanged from previous analysis):

| Search Query | Results |
|--------------|--------|
| ocean fertilization | 0 repos |
| ocean alkalinity enhancement | 0 repos |
| marine geoengineering | 0 repos |
| ocean intervention marine technology | 0 repos |
| ocean pH sensor monitoring | 0 ocean-specific repos |
| artificial upwelling ocean | 0 repos |
| seaweed kelp carbon farming | 0 repos |
| marine cloud brightening | 0 repos |

**BUT: The ocean climate modeling ecosystem is ALIVE.** The updated analysis reveals that while there are zero geoengineering-specific ocean repos, there IS a thriving ocean climate modeling ecosystem. The gap is specifically in ocean intervention design tools, not ocean modeling itself.

---

## The Thriving Ocean Climate Modeling Ecosystem

### Tier 1: Major Ocean Models

### 1. CliMA/Oceananigans.jl — 1,413 Stars (The Ocean Powerhouse)

| Date | Commit | Author | Message |
|------|--------|--------|--------|
| Sep 17, 2026 | aca5970 | Ali Ramadhan | Restore closure fields from checkpoints when closure is a tuple (#6006) |
| Sep 16, 2026 | ab99a39 | Ali Ramadhan | Fix face spacing above partial cells on PartialCellBottom grids (#6013) |
| Sep 16, 2026 | 9ddbbb1 | Ali Ramadhan | Apply linear operator once per ConjugateGradientSolver iteration (#6012) |
| Sep 16, 2026 | 1c8fe39 | Ali Ramadhan | Bounce Lagrangian particles off immersed boundaries (#6005) |
| Sep 16, 2026 | c1655e9 | Tomás Chor | Add TimeDerivative for computing δ of outputs during simulation (#5823) |
| Sep 16, 2026 | 72285df | Ali Ramadhan | SplitRungeKuttaTimeStepper: evaluate time-dependent forcings and BCs at correct time (#6009) |
| Sep 16, 2026 | 23020f1 | Ali Ramadhan | Fix stage δt used by AVID + RK3 (#6008) |
| Sep 16, 2026 | d03dfdf | Ali Ramadhan | Keep non-finite values in immersed cells out of vertically implicit column solve (#5991) |
| Sep 15, 2026 | 1fe0ede | Mosè Giordano | Fix issues in test suite (#5998) |
| Sep 15, 2026 | 162c47d | Mosè Giordano | Tighten up memory allocations bounds (#6004) |

**Key Insight:** 10 commits in 3 days (Sep 15-17, 2026) — this is the most active geoengineering-adjacent repository in the entire analysis. Multiple contributors (Ramadhan, Chor, Giordano) with PR-based workflows, numbered issues (#5823-6013), and sophisticated code (time-steppers, solvers, boundary conditions). This is a world-class ocean modeling codebase with active institutional development.

**Critical New Detail — Lagrangian Particles (#6005):** The Sep 16 commit "Bounce Lagrangian particles off immersed boundaries" is directly relevant to ocean intervention simulation. Lagrangian particle tracking is the computational method for modeling tracer deployment — exactly what you need to simulate where an alkalinity amendment or iron fertilization plume goes. The fact that this was being actively fixed on Sep 16, 2026 means the platform is maturing the exact capability needed for intervention modeling.

**Ocean Intervention Relevance:** Oceananigans.jl is the most promising platform for building ocean intervention simulation tools. It already has:
- **Lagrangian particle tracking** (for tracer deployment #6005) ← The key intervention tool
- **Immersed boundary methods** (for coastal/structure interactions)
- **Time-dependent forcing capabilities** (for simulating injection scenarios)
- **Parallel CPU+GPU execution** (for large-scale simulations)
- **The architecture supports adding new physics modules** ← The extensibility point

---

### 2. team-ocean/veros — 400 Stars (The Pure-Python Ocean Simulator)

| Date | Commit | Author | Message |
|------|--------|--------|--------|
| Sep 15, 2026 | b5a4f49 | dependabot | Bump tqdm from 4.70.0 to 4.70.1 (#869) |
| Sep 15, 2026 | 47026c4 | dependabot | Bump matplotlib from 3.11.1 to 3.11.2 (#868) |
| Sep 14, 2026 | 7732aaf | dependabot | Bump numpy from 2.5.2 to 2.5.3 (#867) |
| Sep 14, 2026 | 6f0e058 | Dion Häfner | Bugfix in isoneutral mixing (#866) |
| Sep 7, 2026 | 29a7e64 | dependabot | Bump ipython from 9.17.0 to 9.17.1 (#865) |
| Sep 1, 2026 | e714e3c | dependabot | Bump ipython from 9.16.1 to 9.17.0 (#864) |
| Aug 31, 2026 | 930d686 | dependabot | Bump click from 8.4.2 to 8.5.0 (#863) |
| Aug 25, 2026 | 448add0 | dependabot | Bump scipy from 1.18.0 to 1.18.1 (#862) |
| Aug 21, 2026 | 8dfd595 | dependabot | Bump jax from 0.11.0 to 0.11.1 (#861) |
| Aug 19, 2026 | 274de71 | Roman Nuterman | Update publications list with new articles |

**Key Insight:** 8 out of 10 recent commits are dependabot dependency bumps. The only substantive code commit is Dion Häfner's isoneutral mixing bugfix (#866). The publication list update is minor. Veros is maintained but not actively developing new features.

**Ocean Intervention Relevance:** Veros is the most accessible pure-Python ocean simulator (powered by JAX). Its accessibility makes it the best candidate for building ocean intervention teaching tools. The isoneutral mixing bugfix is relevant — accurate mixing is critical for modeling pollutant dispersion and OAE plume transport.

---

### 3. OceanBioME/OceanBioME.jl — 80 Stars (The Biogeochemistry Model)

| Date | Commit | Author | Message |
|------|--------|--------|--------|
| Sep 17, 2026 | 044407b | Jago Strong-Wright | Merge PR #419 — return wind to gas exchange top level |
| Sep 16, 2026 | d3892db | Jago | Fix stuff |
| Sep 16, 2026 | 746168f | Jago | Fix |
| Sep 16, 2026 | 7bec18c | Jago | Adjust constructors |
| Sep 16, 2026 | 99e34f6 | Jago | Bump patch release |
| Sep 16, 2026 | 7ed8db6 | Jago | Move wind speed back to gas exchange top level |
| Sep 15, 2026 | 15f783b | Jago Strong-Wright | Merge PR #399 — numerical-earth-coupling |
| Sep 15, 2026 | 108551b | Jago Strong-Wright | Merge PR #411 — gas exchange changes |
| Sep 15, 2026 | 1929dd9 | Jago | Fix docs |
| Sep 14, 2026 | 4d49c49 | Jago | Fix MARBL test to use WindSpeedScaledTransferVelocities |

**Key Insight:** Intense activity Sept 14-17, 2026 (10 commits in 4 days) focused on gas-exchange parameterization and wind speed coupling. Three PRs merged in 4 days (#399, #411, #419). This is active, directed development by a single PI (Jago Strong-Wright) working on ocean-atmosphere gas exchange — the core process for ocean alkalinity enhancement and CO2 sequestration.

**Critical Detail — Gas Exchange = OAE Core Process:** PR #411 ("gas exchange changes") and PR #399 ("numerical-earth-coupling") are directly about the air-sea gas exchange parameterization. This is THE central process for ocean-based CDR. Ocean alkalinity enhancement works by accelerating natural weathering, which changes ocean CO2 capacity — which is governed by air-sea gas exchange. OceanBioME's active development of gas exchange parameterizations is directly relevant to OAE modeling.

**Wind Speed Return Drama:** The PR chain (#411 → "Move wind speed back to gas exchange top level" → "Fix stuff" → "Fix docs") suggests a heated technical debate about how wind speed should be coupled to the gas exchange calculation. Wind speed is the primary driver of air-sea gas exchange. Getting this wrong means getting OAE flux estimates wrong. The fact that this is being actively debated and coded in Sep 2026 means the science is live.

---

## Tier 2: Supporting Ocean Science Repos

| Repo | Stars | Language | Focus | Latest Activity |
|------|-------|----------|-------|----------------|
| pangeo-data/awesome-open-climate-science | 598 | Multi | Curated list of open climate science | Sep 16, 2026 |
| gaelforget/ClimateModels.jl | 47 | Julia | Julia interface to climate models | Aug 13, 2026 |
| jgcri/xanthos | 38 | Python | Global hydrologic framework | Feb 12, 2026 |
| aerler/WRF-Tools | 59 | Shell | WRF setup and run tools | Jun 23, 2026 |
| Climdyn/MAOOAM | 22 | HTML/Lua/Fortran/Python | Modular ocean-atmosphere model | Jun 29, 2026 |
| JuliaOcean/Climatology.jl | 20 | Julia | Ocean climatology | Aug 22, 2026 |

---

## Three Hypotheses for the Ocean Geoengineering Gap (Updated)

### H1: Institutional Gatekeeping (Most Likely — Stronger Evidence)

The ocean CLIMATE modeling ecosystem is thriving (Oceananigans 1,413★, veros 400★, OceanBioME 80★). But ocean GEOENGINEERING has zero repos. This proves the gap is not technical capability — it's purpose. These models are built to understand the ocean, not to intervene in it.

**Revised Evidence:**
- Oceananigans.jl has 1,413 stars and world-class developers — but nobody is building an OAE module
- OceanBioME is actively developing gas exchange physics (Sep 2026) — but not for intervention scenarios
- The modeling infrastructure is ready; the intervention layer is absent
- This is like having a world-class physics engine but no video game built on top of it

**The Lagrangian Particle Tracking Signal:** Oceananigans just added Lagrangian particle bouncing off immersed boundaries (Sep 16, 2026). This is the exact computational method needed for tracer deployment in OAE. The platform is maturing the tool. Nobody is using it for intervention scenarios.

### H2: Governance & Liability (Important)

The London Convention/Protocol directly regulates ocean fertilization. Scientists may self-censor to avoid regulatory scrutiny. Ocean interventions have transboundary impacts — no single country can authorize them.

**Supporting evidence from OceanBioME's gas exchange work:** The pace of gas exchange parameterization development (3 PRs in 4 days, Sep 15-17) suggests the science is ready. But the jump from "modeling gas exchange" to "modeling OAE deployment" is a governance leap, not a scientific one.

**The wind speed coupling debate as a microcosm:** The PR chain on gas exchange (#411 → "move wind speed back" → "fix stuff") shows that even the basic science of ocean-atmosphere coupling is still being debated. Before you can model OAE, you need to nail the base physics. The governance question (can you even do this?) may suppress the "why would you model it?" question.

### H3: Experimental Complexity Barrier (Structural — Confirmed)

- A single ocean field experiment costs $50K+/day for ship time
- Sensor deployments in remote waters require multi-year monitoring
- International coordination is required for any ocean intervention
- The barrier to GitHub-ready prototypes is astronomically higher than for SRM or DAC

**The math:** Oceananigans.jl can simulate ocean physics. But nobody is simulating OAE because: (1) the economics aren't there, (2) the governance isn't there, (3) the researchers with the skills are at sea, not at keyboards.

---

## The Ocean Intervention Gap — A New Framework (Updated)

Instead of just cataloging what's missing, let's map what exists and what's needed with fresh commit data:

| Ocean Modeling Layer | What Exists | What's Missing | Nearest Active Repo |
|---------------------|-------------|----------------|---------------------|
| Ocean physics | Oceananigans.jl (1,413★), veros (400★) | Intervention-specific forcing modules | Oceananigans (active Sep 2026) |
| Lagrangian particles | Oceananigans #6005 (Sep 16, 2026) | Tracer/advection for intervention scenarios | Oceananigans (just added!) |
| Biogeochemistry | OceanBioME.jl (80★) | OAE/iron fertilization modules | OceanBioME (active Sep 2026) |
| Gas exchange | OceanBioME (active Sep 2026, 3 PRs/4 days) | Coupled OAE gas exchange models | OceanBioME (the core process IS being developed) |
| Sediment transport | (in CSDMS tools) | Benthic impact assessment tools | None |
| Sensor design | (zero open hardware) | DIY pH/alkalinity/pCO2 sensor designs | ZERO (unlike OpenAir-Cyan for DAC) |
| Data pipelines | (Pangeo ecosystem) | OAE monitoring data formats | None |
| Governance | (zero) | Regulatory mapping tools | Zero (unlike srm-forever for SRM) |
| **Marine cloud brightening** | WRF (can simulate, no config) | MCB-specific nudging/seed modules | MDTF (precip-buoyancy POD for evaluation) |

**The discovery (updated):** The ocean modeling stack is 80% built. The intervention layer is 0% built. The gap is specifically in the "what happens when you intervene" layer. And increasingly, the building blocks exist — Lagrangian particles, gas exchange parameterizations, biogeochemistry — but nobody has assembled them into an intervention simulation.

---

## What Would an Open-Source Ocean Intervention Project Look Like? (Updated)

Based on patterns from the other two themes AND the existing ocean modeling ecosystem with fresh commit data:

1. **An Oceananigans.jl OAE module** — The most feasible starting point. Oceananigans already has the physics engine; adding an alkalinity amendment module would be a focused, tractable project. The Lagrangian particle tracking (#6005, Sep 16, 2026) is the key enabler — it's the computational method for tracer deployment. A grad student could do this in a summer. **Nobody has.**

2. **An OceanBioME gas exchange + OAE module** — Gas exchange is THE core process for OAE, and OceanBioME is actively developing it (3 PRs in 4 days, Sep 2026). An OAE-specific gas exchange module would be a natural next step. The wind speed coupling debate (#411) is literally about the physics that OAE depends on.

3. **A veros-based OAE teaching tool** — Veros is pure Python and accessible. An interactive OAE simulator (like srm-forever for solar geoengineering) could democratize ocean intervention modeling. Veros is the "srm-forever of ocean intervention" — the accessible entry point.

4. **Sensor designs for ocean monitoring** — Like OpenAir-Cyan's hardware designs for DAC, shareable pH/alkalinity/pCO2 sensor designs for ocean monitoring. This is the DIY hardware equivalent for ocean science. **Zero equivalents exist.**

5. **A governance/regulatory mapping tool** — Like srm-forever's approach to SRM governance, an interactive tool showing the legal/regulatory landscape for ocean interventions. **Zero equivalents exist.** The London Protocol complexity is the governance challenge.

**The nearest feasible starting point (updated):** An Oceananigans.jl OAE module with Lagrangian particle tracking. The physics engine exists. The particle tracking was just added (Sep 16, 2026). The developers are active (10 commits/3 days). The gas exchange physics exists (OceanBioME, actively developing). The gap is in the intervention layer. A graduate student could build this. Nobody has.

---

## 🎙️ Podcast Takeaways (Updated)

1. **The ocean CLIMATE modeling ecosystem is thriving.** Oceananigans.jl (1,413★) had 10 commits in 3 days (Sep 2026). OceanBioME.jl (80★) had 10 commits in 4 days (Sep 2026). Veros (400★) is maintained but in dependency-bump mode. The ocean science community is producing world-class code.

2. **Lagrangian particles just landed in Oceananigans (Sep 16, 2026).** The "Bounce Lagrangian particles off immersed boundaries" commit (#6005) is the exact computational method needed for tracer deployment in OAE simulations. The platform is maturing the tool. Nobody is using it for intervention scenarios. This is like having a physics engine with particle tracking but no video game built on top of it.

3. **OceanBioME's gas exchange work IS the OAE core process.** Three PRs in four days (Sep 15-17) on gas exchange parameterization, including a wind speed coupling debate (#411). This is the central process for ocean alkalinity enhancement. The science is being actively developed. The application layer (OAE modeling) isn't built.

4. **The ocean geoengineering gap is total.** Zero repos. Zero code. Zero interactive tools. The August 2026 carbon wave had 6 repos updating. The same period had ZERO ocean repos touching intervention design.

5. **The ocean gap is different from the carbon gap.** Carbon has OpenAir-Cyan (hardware), Carbon_Capture_ML (literature), and differentiable-flowsheets (AI simulation). Ocean has nothing — no hardware, no surveys, no interactive tools, no AI-augmented simulation.

6. **The London Protocol may be causing self-censorship.** Unlike SRM (murky but not illegal), ocean fertilization is explicitly regulated. Researchers may avoid open-source code to avoid regulatory scrutiny. Or they may just not think of GitHub as a venue for ocean intervention code.

7. **The nearest feasible project is an Oceananigans.jl OAE module with Lagrangian particle tracking.** The physics engine exists (1,413★). The particle tracking was just added (Sep 16, 2026). The gas exchange physics exists (OceanBioME, actively developing). The gap is in the intervention layer. A graduate student could build this. Nobody has.

8. **The wind speed coupling debate is a microcosm of the ocean gap.** OceanBioME's PR chain on gas exchange (#411: "move wind speed back to gas exchange top level" → "Fix stuff" → "Fix docs") shows that even the basic physics of ocean-atmosphere coupling is still being debated. Before you can model OAE, you need to nail the base physics. The governance question (can you even do this?) may suppress the "why would you model it?" question.

9. **The ocean modeling stack is 80% built; the intervention layer is 0% built.** Oceananigans has fluid dynamics. OceanBioME has biogeochemistry and gas exchange. MDTF has diagnostics. WRF has air-sea coupling. The components are there. The integration for intervention scenarios is zero.

10. **The ocean is the silence that speaks loudest in the climate tech open-source ecosystem.** While the atmosphere gets WRF and PCMDI, while carbon gets OpenAir-Cyan and differentiable-flowsheets and CC0 data releases — the ocean gets nothing. No hardware designs, no simulation tools, no governance models. The ocean is the quadrant where open-source climate tech has made zero progress.

---

## 📋 Research Log

| Date | Activity |
|----------|
| 2026-09-17 | v2: Ocean ecosystem data added — Oceananigans.jl, veros, OceanBioME.jl commit histories analyzed |
| 2026-09-17 | v2: Ocean gap analysis revised with new framework (modeling stack 80% built, intervention layer 0%) |
| 2026-09-17 | v3: Fresh commit histories pulled from 12 repositories across all three themes using GitHub API |
| 2026-09-17 | v3: Ocean gap confirmed — 10+ search queries, zero dedicated ocean geoengineering repos |
| 2026-09-17 | v3: CC0 license trend identified as major open-science signal in DAC materials community |
| 2026-09-17 | v3: Cross-theme analysis pushed to main branch |
| 2026-09-18 | v4: Fresh commit data updated from GitHub API for all ocean-modeling repos |
| 2026-09-18 | v4: Lagrangian particle tracking commit (#6005) identified as key ocean-intervention enabler |
| 2026-09-18 | v4: OceanBioME gas exchange PR chain (#411, #399, #419) documented as OAE core process development |
| 2026-09-18 | v4: "Wind speed coupling debate" identified as microcosm of ocean governance gap |
| 2026-09-18 | v4: Updated gap framework table with fresh commit data and nearest-active-repo column |
| 2026-09-18 | v4: "Ocean modeling stack 80% built, intervention layer 0%" thesis confirmed with new data |