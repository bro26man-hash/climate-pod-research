# ☀️ Solar Geoengineering — Research Notes

**Podcast theme:** Solar Radiation Management (SRM)
**Repository branch:** `solar-geoengineering`
**Source:** GitHub API research — open-source project discovery + commit-history analysis

## Episode Angle
Can we simulate solar geoengineering — and its risks — in the open? The short answer: the *full-physics* SRM models live mostly behind closed doors at NCAR and GFDL, while the open-source side is dominated by governance models, radiative-transfer snippets, and legacy atmospheric code. That gap between ambition and open availability is itself the story.

## Project Discoveries

| Project | ⭐ | Last updated | Notes |
|---|---|---|---|
| [ClimateMARGO/ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl) | 73 | 2026-08-17 | Idealized climate-economic framework for balancing mitigation, adaptation and geoengineering trade-offs — the closest thing to an open SRM optimizer |
| [CliMA/Insolation.jl](https://github.com/CliMA/Insolation.jl) | 23 | 2026-08-10 | Fast, accurate solar geometry and top-of-atmosphere insolation — supporting tooling for radiative-forcing work |
| [jlehtomaa/OOCC_2021](https://github.com/jlehtomaa/OOCC_2021) | 2 | — | Simple Python model for solar geoengineering *governance* (not physics) |
| [mlmac-seid/marine-cloud-brightening-simulation](https://github.com/mlmac-seid/marine-cloud-brightening-simulation) | — | 2025-11-06 | Uses the Rapid Radiative Transfer Model (RRTM) to simulate marine cloud brightening effects on net solar radiation |
| [FMS-ESM/AM3](https://github.com/FMS-ESM/AM3) | 4 | 2015-03 | GFDL atmospheric model (legacy Fortran) — representative of the "closed lab" generation that still props up SRM simulation |
| [pmip4/pmip_p2fvar_analyzer](https://github.com/pmip4/pmip_p2fvar_analyzer) | 4 | 2025-09-05 | CMIP6 climate-data analysis tooling, useful for forcing/response studies |
| [Fatema-Nur/LOD-Climate-Prediction-System](https://github.com/Fatema-Nur/LOD-Climate-Prediction-System) | — | 2025-11 | Physics-based climate simulation (notebook / Python) |
| [prashaant1926/open-earth-digital-twin-simulation](https://github.com/prashaant1926/open-earth-digital-twin-simulation) | — | 2025-10 | "Earth system digital twin" experiment |
| [RhondaMueller/Codes-RFG-Arctic-Impacts](https://github.com/RhondaMueller/Codes-RFG-Arctic-Impacts) | 1 | 2024-04 | Radiative-forcing code focused on Arctic impacts of geoengineering |

## Commit-Trend Summary (from recent commit histories)
- **CESM (ESCOMP/CESM)** is the most active general Earth-system repo, but its 2026 commits are about **CESM3** alpha/beta polishing (`alpha09f`, `alpha09g`, `beta09`), **GPU/pelayout** performance work, and CO2 compset naming — i.e. next-gen model performance and modernization, *not* SRM scenario injection.
- **Marine biogeochemistry (MARBL)** is a visible sub-theme in CESM commits — the ocean carbon cycle is getting more open attention than solar forcing.
- **No active, open SRM injection / radiative-forcing model** appears in recent commit histories. The handful of solar-themed repos (ClimateMARGO, OOCC, the MCB RRTM model) are small governance or single-purpose experiments with low commit cadence.
- **Insolation.jl** is the one genuinely maintained, purpose-built solar/radiative tool in the CliMA ecosystem.
- Legacy atmospheric code (GFDL AM3, 2015) still anchors SRM simulation where it exists, alongside a new wave of Jupyter/notebook experiments and digital-twin attempts.

## The Big Takeaway
SRM simulation ambition greatly outpaces open-source availability. Full-physics SRM models remain locked in national labs; the open field is governance models, radiative-transfer utilities, and legacy atmospheric code. Arctic-focused risk code and digital-twin experiments hint at where the next open wave might form — if it does.

## Key Terminology
SRM, solar radiation management, marine cloud brightening (MCB), radiative forcing, insolation, albedo, geoengineering governance, climate models (CESM, GFDL AM3), CMIP6, radiative transfer (RRTM), digital twin.
