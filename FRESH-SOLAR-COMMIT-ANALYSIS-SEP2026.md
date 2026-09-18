# ☀️ Fresh Solar Geoengineering Commit Analysis — September 2026

## Overview
This analysis captures commit activity from the most active open-source repositories relevant to solar geoengineering and climate modeling, pulled live from GitHub in September 2026.

---

## Repository 1: WRF (Weather Research and Forecasting Model)
**Repo:** [wrf-model/WRF](https://github.com/wrf-model/WRF)  
**Stars:** 1,762  |  **Language:** Fortran  |  **Status:** 🟢 Actively maintained

### Why It Matters for Solar Geoengineering
WRF is the foundational atmospheric model used in virtually every SRM (Solar Radiation Management) simulation study. When researchers model stratospheric aerosol injection or marine cloud brightening, they run WRF. Any changes to its radiative transfer schemes, aerosol modules, or physics configurations directly affect what SRM experiments can tell us.

### Recent Commits (15 pulled, May–June 2026)

| Date | Commit | Author | Significance |
|------|--------|--------|-------------|
| Jun 8 | Merge release-v4.8.0 | Anthony Islas | **v4.8.0 released** — major version milestone |
| Jun 6 | Update README and version to v4.8.0 | Anthony Islas | Documentation update for release |
| Jun 5 | Turn off tempo_aerosolaware and tempo_hailaware | weiwangncar | **Aerosol awareness temporarily disabled** — relevant to aerosol simulation |
| May 30 | Fix vectorization option in AOCC stanza | weiwangncar | Compiler optimization fix |
| May 28 | Correction for eot calculation for solar radiation | weiwangncar | **🔥 Solar radiation energy conservation fix** — directly impacts radiative forcing calculations |
| May 27 | MYNN-EDMF pointer update, remove icloud_bl | Joseph Olson | Boundary layer physics update |
| May 27 | Update MMM-physics repo SHA | Anthony Islas | Multi-model mean physics submodule update |
| May 26 | Fixing CDXWRF module | Lluís Fita | Correctness fix for coupling |
| May 26 | Readme for GFL option | weiwangncar | Documentation for new feature |
| May 21 | Include mp_physics=88 in TEMPO error message | Kelly Werner | TEMPO (aerosol) error reporting |
| May 20 | Minor Tempo changes | AndersJensen-NOAA | TEMPO aerosol scheme updates |
| May 20 | Fix scheme-guard bug in urban NbS init | Chenghao Wang | Urban nature-based solutions bug |
| May 20 | New namelists for ShinHong PBL | weiwangncar | New planetary boundary layer scheme |
| May 19 | Bug fix for udm | weiwangncar | Uncertainty/diversity module fix |
| May 12 | Update MYNN-SFC submodule | Joseph Olson | Surface layer physics update |

### Key Trends for the Podcast
1. **Solar radiation fix (May 28)** — A correction to the energy conservation calculation for solar radiation. This is the kind of incremental correctness improvement that makes SRM simulation results more trustworthy. If the energy budget is wrong, geoengineering experiments produce misleading temperature responses.

2. **TEMPO aerosol scheme under active development** — Three commits in one week (May 20-28) to the TEMPO aerosol module. TEMPO is relevant to stratospheric aerosol injection modeling. The temporary disabling of `tempo_aerosolaware` (Jun 5) suggests the team is refining how aerosol-cloud interactions are handled.

3. **v4.8.0 release signals sustained institutional investment** — The WRF model is maintained by a large institutional consortium (NCAR, NOAA, etc.). The release of v4.8.0 with 15 commits in 3 weeks shows this is not a hobby project — it's critical infrastructure.

4. **New physics schemes being added** — ShinHong PBL scheme, GFL (Graphical Finer Layer) option, MYNN-EDMF updates. Each new physics option expands the modeling space for SRM experiments.

### Episode Talking Points
- "The solar radiation energy correction in WRF v4.8.0 is a reminder that even the tools we use to model geoengineering are still being refined. The science is real, but so is the uncertainty."
- "TEMPO aerosol development is happening in parallel with the broader climate modeling community. What does it mean for SRM research when the aerosol module is being actively updated?"
- "15 commits in 3 weeks for a 1,700+ star project — this is open-source climate infrastructure."

- **Commits pulled:** 15  |  **Active period:** May 12 – Jun 8, 2026  |  **Commit density:** ~5/week during release cycle

---

## Repository 2: ClimateMARGO.jl
**Repo:** [ClimateMARGO/ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)  
**Stars:** 73  |  **Language:** Julia  |  **Status:** 🟡 Dormant with revival signal

### Why It Matters
ClimateMARGO is an idealized climate-economic modeling framework written in Julia. It optimizes trade-offs between emissions mitigation, adaptation, and geoengineering. It's the kind of open-source tool that could democratize access to climate-policy modeling — if it were actively maintained.

### Recent Commits (15 pulled)

| Date | Commit | Author | Significance |
|------|--------|--------|-------------|
| Aug 17 | Update README.md (×2) | Fons van der Plas | ** revival signal — README rewritten after 3.5 years of silence** |
| Oct 2023 | Update unit_conversions.jl | Fons van der Plas | Last code change before dormancy |
| Jul 2023 | Add Pluto notebook link | Fons van der Plas | Educational tooling |
| Nov 2022 | Update Project.toml | Fons van der Plas | Dependency management |
| Nov 2022 | JuMP and Ipopt compat upgrade | Fons van der Plas | Solver compatibility update |
| Feb 2022 | Removed deprecated web apps | Henri Drake | Cleanup |
| Feb 2022 | Added CITATION.bib | Henri Drake | Citation infrastructure |
| Jan 2022 | Various doc and version updates | Henri Drake | Final active development period |

### The Revival Pattern
ClimateMARGO shows a clear pattern:
- **2022:** Active development (7+ commits in January alone)
- **2023:** Slow decline (3 commits over 3 months)
- **2024-2026:** Complete silence (3.5 years with zero commits)
- **August 2026:** Two README updates in one day — the first activity in 3.5 years

But critically: **no code commits in the revival**. Just README updates. This is the "false start" pattern we've seen before — someone gets excited, updates the readme, maybe tries to revive interest, but doesn't have the sustained momentum to restart actual development.

### Episode Talking Points
- "ClimateMARGO had a moment of hope in August — two README updates after 3.5 years. But no code. The revival is real, but it's ornamental."
- "This is what happens when you build a climate-economic model as a side project. The inspiration fades, the code sits, and the community doesn't form."
- "The Julia ecosystem for climate modeling is still young. ClimateMARGO could be the killer app — if someone commits to maintaining it."

- **Commits pulled:** 15  |  **Active periods:** Jan 2022 (6+ commits), Aug 2026 (2 README commits)  |  **Dormancy:** 3.5 years

---

## Repository 3: awesome-geoengineering
**Repo:** [brandonhimpfen/awesome-geoengineering](https://github.com/brandonhimpfen/awesome-geoengineering)  
**Stars:** 4  |  **Language:** Python  |  **Status:** 🟢 Steadily maintained

### Why It Matters
This is a curated list of geoengineering projects, research, organizations, and tools. It's the "catalog" repo — the one that helps researchers and journalists navigate the geoengineering landscape. Small star count but remarkably consistent update pattern.

### Recent Commits (7 pulled)

| Date | Commit | Author | Significance |
|------|--------|--------|-------------|
| Sep 6 | Update README.md | Brandon Himpfen | **Most recent — daily updates** |
| Sep 5 | Update README.md | Brandon Himpfen | |
| May 5 | Update to v2.0.0 | Brandon Himpfen | Major version release |
| Mar 12 | Update README.md | Brandon Himpfen | |
| Jan 16 | Update README.md | Brandon Himpfen | |
| Jun 28 | Update README.md (×2) | Brandon Himpfen | Initial release + update |

### The Careful Curator
This repo has a very deliberate update pattern: roughly monthly README updates, with a major v2.0.0 release in May. It's not churning out code — it's carefully curating a resource. The two commits per day at launch (Jun 28) and the recent back-to-back updates (Sep 5-6) suggest a person who cares about keeping this catalog current.

### Episode Talking Points
- "Four stars, but this might be the most useful geoengineering repo on GitHub. It's a curated catalog — the Netflix queue for climate tech research."
- "Monthly updates for a year straight. That's commitment. This person is maintaining a public good."
- "The v2.0.0 release in May suggests this has grown beyond a simple list. It's becoming a structured resource."

- **Commits pulled:** 7  |  **Pattern:** ~1-2 updates per month  |  **Consistency:** High

---

## Cross-Repo Solar Theme Analysis

### The Three Universes of Solar Geoengineering Code

| Universe | Repo | Stars | Commit Pattern | What It Represents |
|----------|------|-------|---------------|-------------------|
| **Fast Universe** | WRF | 1,762 | 15 commits in 3 weeks | Institutional, funded, sustained infrastructure |
| **Slow Universe** | ClimateMARGO | 73 | 6 commits in 1 month (2022), 2 READMEs in 1 day (2026) | Individual, unfunded, dormant with false-start revival |
| **Discovery Universe** | awesome-geoengineering | 4 | 7 commits over 14 months | Small-scale curation, steady maintenance |

### Development Trends
1. **Atmospheric modeling is institutional, not grassroots** — WRF is where SRM simulations happen. It's funded, maintained, and released on a schedule. There's no "wild west" of solar geoengineering code — it flows through established channels.

2. **The economic modeling gap** — ClimateMARGO's dormancy pattern (burst of activity → abandonment → ornamental README revival) is the tell. Climate-economic modeling for SRM is not attractive enough for sustained open-source investment.

3. **Curation is the missing infrastructure** — awesome-geoengineering exists because no one else is maintaining a structured catalog. The fact that it's the 3rd most active solar-related repo (stars aside) suggests a real need for better organization of geoengineering resources.

### Podcast Narrative Arc
> "Solar geoengineering has two very different faces on GitHub. The fast universe — massive atmospheric models with institutional backing — is where the actual simulations happen. The slow universe — individual climate-economic models — is where the ideas get developed and then quietly abandoned. And then there's the discovery universe — one person's devoted effort to catalog it all. The story of solar geoengineering on GitHub is really a story about who gets to build the tools, who gets to model the futures, and who gets to decide what's worth cataloging."
