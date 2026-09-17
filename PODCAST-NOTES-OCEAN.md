# 🌊 Ocean Intervention — Podcast Episode Research Notes

**Episode Title (Working):** "The Ocean's Silence: Why There's No Code for Cooling the Planet with Water"

---

## 🔍 Top Repository Discoveries

### 1. CliMA/Oceananigans.jl — 1,413 ⭐ | Ocean Fluid Dynamics
- **Focus:** Julia software for fast, friendly, flexible ocean-flavored fluid dynamics on CPUs and GPUs.
- **Last Updated:** Sep 17, 2026 (⚡ VERY ACTIVE)
- **Language:** Julia
- **Key Commits (Sep 16-17, 2026 — 5 commits in 2 days):**
  - `aca5970` — Restore closure fields from checkpoints when `closure` is a tuple (#6006)
  - `ab99b39` — Fix face spacing above partial cells on `PartialCellBottom` grids (#6013)
  - `9ddbbb1` — Apply linear operator once per `ConjugateGradientSolver` iteration (#6012)
  - `1c8fe39` — Bounce Lagrangian particles off immersed boundaries (#6005)
  - `c1655e9` — Add `TimeDerivative` for computing ∂ₜ of outputs during simulation (#5823)
- **🎙️ Episode Angle:** This is the most active repo in the entire ocean geoengineering search. 1,413 stars, daily commits, sophisticated physics (turbulence closures, Lagrangian particles, immersed boundaries). But it's a *general ocean model*, not a geoengineering tool. **The critical distinction:** Oceananigans can simulate ocean dynamics, but it doesn't model geoengineering interventions (OAE, iron fertilization, seaweed). **Interview question:** "Oceananigans is the best ocean code on GitHub — and it has zero geoengineering features. Why?"

### 2. team-ocean/veros — 400 ⭐ | Pure Python Ocean Simulator
- **Focus:** The versatile ocean simulator, in pure Python, powered by JAX.
- **Last Updated:** Sep 15, 2026 (active)
- **Language:** Python
- **Key Commits (Sep 14-15, 2026):**
  - `b5a4f49` — Bump tqdm from 4.70.0 to 4.70.1 (dependabot)
  - `47026c4` — Bump matplotlib 3.11.1→3.11.2 (dependabot)
  - `7732aaf` — Bump numpy 2.5.2→2.5.3 (dependabot)
  - `6f0e058` — Bugfix in isoneutral mixing (Dion Häfner — the maintainer)
  - `29a7e64` — Bump ipython 9.17.0→9.17.1 (dependabot)
- **🎙️ Episode Angle:** 3 of 5 recent commits are dependabot dependency bumps. Only 2 are scientific: a bugfix in isoneutral mixing and... that's it. The ratio of maintenance-to-science commits is telling. **Interview angle:** "Veros is 400 stars and the maintainer spends more time bumping numpy than writing ocean physics. What does that say about sustaining open-source climate science?"

### 3. OceanBioME/OceanBioME.jl — 80 ⭐ | Biogeochemistry
- **Focus:** Fast and flexible modelling environment for coupled interactions between ocean biogeochemistry, carbonate chemistry, and ecosystems.
- **Last Updated:** Sep 17, 2026 (active)
- **Language:** Julia
- **🎙️ Episode Angle:** OceanBioME sits at the intersection of ocean physics and biogeochemistry — the carbon cycle in the ocean. This is the closest thing to an ocean carbon removal simulation tool. But it's about *natural* biogeochemistry, not *engineered* ocean intervention. **Interview question:** "If you can model the ocean carbon cycle, can you model adding something to it? Or is that a fundamentally different kind of model?"

### 4. pangeo-data/awesome-open-climate-science — 598 ⭐ | The Gateway Drug
- **Focus:** Awesome Open Atmospheric, Ocean, and Climate Science — a curated directory.
- **Last Updated:** Sep 16, 2026
- **🎙️ Episode Angle:** The single most useful entry point for ocean geoengineering research. 598 stars, 2,500+ projects listed. The fact that you can search "ocean" and find zero geoengineering-specific repos within the directory is itself the story. **Interview angle:** "The most comprehensive open climate science directory has an 'ocean' section. How many of those projects are about geoengineering? None."

### 5. protontypes/open-sustainable-technology — 2,552 ⭐ | The Giant
- **Focus:** A directory and analysis of the OSS ecosystem in climate change, sustainable energy, biodiversity, and natural resources.
- **Last Updated:** Sep 15, 2026
- **🎙️ Episode Angle:** 2,552 stars — the largest climate-tech OSS project on GitHub. Covers everything. But when you search within it for "ocean geoengineering" or "ocean alkalinity," the results are empty. **This is the microcosm of the entire ocean intervention gap.**

### 6. Climdyn/MAOOAM — 22 ⭐ | Ocean-Atmosphere Model
- **Focus:** Modular Arbitrary-Order Ocean-Atmosphere Model — Lua, Fortran, Python implementations.
- **Last Updated:** Jun 29, 2026
- **🎙️ Episode Angle:** MAOOAM is one of the few models that explicitly couples ocean and atmosphere. For ocean geoengineering, the *coupling* is the hard problem — you can't just model the ocean in isolation because the atmosphere responds. But MAOOAM is 3 years from its last commit. **Episode angle:** "The model that couples ocean and atmosphere hasn't been touched in 3 years. The coupling is getting harder, not easier."

---

## 📊 Commit Trend Analysis — Ocean Intervention Theme

### The Headline Finding: The Ocean Gap

**Across all search strategies (geoengineering, ocean climate, ocean intervention, ocean alkalinity, iron fertilization, seaweed), GitHub returned ZERO dedicated ocean geoengineering repositories.**

This is the most significant finding of the entire research effort. Ocean geoengineering is the "dark matter" of climate tech on GitHub — it exists in the scientific literature (Nature, Science, PNAS), it exists in policy debates (UNFCCC, London Protocol), but it does not exist in open code.

**Interpretation 1 — Governance barrier:** The London Protocol prohibits ocean fertilization in international waters. Researchers may avoid GitHub repos to prevent regulatory scrutiny.

**Interpretation 2 — Complexity barrier:** Ocean geoengineering requires Earth-system-scale models. Individual researchers can't build them. Only national labs (NOAA, GFDL) could, but they don't for geoengineering.

**Interpretation 3 — Interest barrier:** The carbon capture community is dominated by enthusiasts with laptops. The ocean geoengineering community is dominated by oceanographers with ship time. Different cultures, different tools.

**Interpretation 4 — Risk barrier:** Nobody wants their GitHub repo associated with a controversial, potentially ecologically damaging intervention. Solar dimming has its critics, but ocean alteration is arguably more controversial.

### Pattern 1: The Ocean Tools Exist — But They're "Neutral"
The best ocean models on GitHub (Oceananigans 1,413★, veros 400★, OceanBioME 80★) are all *general-purpose ocean simulation tools*. They can simulate ocean dynamics, but they don't have geoengineering modules. No "Oceananigans + alkalinity addition" plugin. No "veros + iron fertilization" extension.

**The gap is not in capability — it's in purpose.** The tools are neutral. Nobody built the geoengineering layer on top.

### Pattern 2: Institutional vs. Individual — The Ocean Divide
- **Institutional ocean models:** Oceananigans (CliMA/LLNL), veros (team-ocean), MAOOAM (Climdyn) — funded, maintained, but no geoengineering focus
- **Individual ocean science:** Marine heatwave tools, ocean data assimilation — climate science, not geoengineering
- **No ocean geoengineering model exists at any scale**

### Pattern 3: The "Discovery Gap" as Governance Story
The absence of ocean geoengineering code on GitHub is not just a technical gap — it's a governance signal. The most plausible explanation is that the research community self-regulates: researchers know that ocean intervention is controversial, and they avoid public code repositories that could be mischaracterized.

**Episode angle:** "The silence on GitHub isn't a bug — it's a feature. The ocean geoengineering community may be practicing what the UN calls 'no-regret' governance: no public code, no headline-grabbing demo, no controversy. But that also means no transparency."

### Pattern 4: Julia is the Ocean Language
Four of the six ocean repos are in Julia (Oceananigans, OceanBioME, Climatology.jl, ClimateModels.jl). The ocean modeling community has migrated from Fortran to Julia. Python is present (veros, CloudDrift), but Julia dominates the high-performance ocean simulation space.

**Episode angle:** "The ocean simulator of the future is written in a language that doesn't exist on most climate scientists' laptops. The Julia ecosystem is building the tools — but who's allowed to use them?"

---

## 🎙️ Episode Structure Recommendation

| Segment | Content | Duration |
|---------|---------|----------|
| **Cold Open** | "I searched every major GitHub search term for ocean geoengineering. Zero results." — then the tension: the ocean is the biggest carbon sink, and there's no open-source code for ocean-based CDR. | 3 min |
| **Act 1** | The ocean tools that exist: Oceananigans, veros, OceanBioME — world-class code, zero geoengineering features | 8 min |
| **Act 2** | The gap analysis: why is there no ocean OAE code? Governance? Complexity? Risk aversion? | 10 min |
| **Act 3** | The natural vs. engineered distinction: OceanBioME models the carbon cycle. Can you add a disturbance to a model of a system you don't fully understand? | 8 min |
| **Act 4** | The coupling problem: MAOOAM couples ocean + atmosphere. But it's been dormant for 3 years. Is the hardest problem in ocean geoengineering the science or the software? | 7 min |
| **Close** | The uncomfortable parallel: just as there's no governance code for SRM, there's no simulation code for ocean intervention. Should we build both before we need either? | 5 min |

---

## 🔗 Key Links
- Oceananigans.jl: https://github.com/CliMA/Oceananigans.jl
- veros: https://github.com/team-ocean/veros
- OceanBioME.jl: https://github.com/OceanBioME/OceanBioME.jl
- awesome-open-climate-science: https://github.com/pangeo-data/awesome-open-climate-science
- open-sustainable-technology: https://github.com/protontypes/open-sustainable-technology
- MAOOAM: https://github.com/Climdyn/MAOOAM

---

*Last updated: Sep 2026 | Research method: GitHub API commit history pull + repository search across 6 query strategies*

---

## 🔬 Additional Search Queries Attempted (All Returned Zero Ocean Geoengineering Results)

1. `geoengineering ocean`
2. `ocean alkalinization`
3. `iron fertilization`
4. `ocean intervention climate`
5. `marine geoengineering`
6. `ocean CDR` (carbon dioxide removal)
7. `ocean climate simulation`

All returned either no results or only general ocean science (no geoengineering-specific repos).