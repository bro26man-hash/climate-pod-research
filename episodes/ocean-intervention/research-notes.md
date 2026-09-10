# 🌊 Ocean-Based Geoengineering — Research Notes

**Podcast theme:** Ocean Intervention (ocean alkalinity enhancement, iron fertilization, seaweed, upwelling)
**Repository branch:** `ocean-intervention`
**Source:** GitHub API research — open-source project discovery + commit-history analysis

## Episode Angle
Ocean geoengineering is the **empty quadrant** of open-source climate tech on GitHub. A dedicated search for repositories on ocean alkalinity enhancement, iron fertilization, seaweed, and offshore upwelling returned **essentially zero dedicated projects** — and that absence is the story worth telling.

## Project Discoveries

| Project | ⭐ | Last updated | Relevance |
|---|---|---|---|
| [OSU-CEOAS-Schmittner/UVic2.9](https://github.com/OSU-CEOAS-Schmittner/UVic2.9) | 13 | 2026-07-23 | Closest open match: UVic Earth System Model *with the Model of Ocean Biogeochemistry and Isotopes (MOBI)* — a real, maintained ocean biogeochemistry model (Fortran) |
| [ESCOMP/CESM](https://github.com/ESCOMP/CESM) | 490 | 2026-09-10 | Community Earth System Model; recent commits foreground the **MT+MARBL** marine biogeochemistry component and CO2-focused compset work — the main open venue for ocean carbon-cycle simulation |
| [lnnrtrmm/Carbon-Climate-Box-Model](https://github.com/lnnrtrmm/Carbon-Climate-Box-Model) | 6 | — | Simple climate-carbon box model reproducing MPI-ESM behavior — adjacent to ocean carbon cycling (Python) |
| [Team50-Labs/NebuGrid-OpenSource](https://github.com/Team50-Labs/NebuGrid-OpenSource) | 0 | 2026-08 | Fog-harvesting & drip-irrigation water-scarcity tooling — tangential (water harvesting), not ocean geoengineering proper |

> ⚠️ **Discovery note:** A targeted GitHub search for ocean geoengineering repositories (alkalinity enhancement, iron fertilization, seaweed, upwelling) returned **no dedicated repositories**. Ocean geoengineering is the thinnest open-source slice of the three episode themes.

## Commit-Trend Summary (from recent commit histories)
- **CESM (ESCOMP/CESM)** — the most active Earth System Model in the sample — shows its *ocean-relevant* open work concentrated in **MT+MARBL** (marine biogeochemistry) performance optimization and CO2 compset naming in 2026. This is mainstream *ocean carbon-cycle* modeling, not deliberate intervention (fertilization / alkalinity) — but it's the open codebase closest to ocean intervention.
- **UVic2.9 + MOBI** is the only identified open model explicitly coupling an *ocean biogeochemistry* component (MOBI) into an Earth System Model — and it's still maintained (July 2026).
- Beyond CESM/MARBL and UVic2.9/MOBI, **no open-source repository was found** that simulates ocean alkalinity enhancement, iron fertilization, macroalgae/seaweed, or ocean upwelling as an intervention.
- The active CliMA component stack (ClimaAtmos, ClimaLand, Thermodynamics) is atmosphere/land-focused and does not reach into ocean-intervention physics.

## The Big Takeaway
Want open-source ocean geoengineering? It doesn't meaningfully exist yet on GitHub — not for fertilization, not for alkalinity, not for seaweed. The handful of ocean *biogeochemistry* models (CESM/MARBL, UVic2.9/MOBI) simulate the global carbon cycle, not deliberate ocean manipulation. The experimental complexity, governance sensitivity, and institutional siloing of ocean research create the largest open-source gap in climate tech — a rich, honest angle for the episode.

## Key Terminology
Ocean alkalinity enhancement (OAE), artificial ocean alkalinization, iron fertilization (OIF), macroalgae / seaweed culturing, ocean upwelling / downwelling, marine biogeochemistry, MOBI (Model of Ocean Biogeochemistry and Isotopes), air-sea CO2 flux, carbonate chemistry, ocean carbon cycle, DAC, SRM, ocean governance.
