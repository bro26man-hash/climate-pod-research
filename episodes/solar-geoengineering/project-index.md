# ☀️ Solar Geoengineering — Project Index

Quick-reference companion to `episodes/solar-geoengineering/research-notes.md` for the solar-geoengineering episode.

| # | Project | Repo | ⭐ | Last Active | SRM Relevance |
|---|---------|------|----|-------------|---------------|
| 1 | CESM (Community Earth System Model) | [ESCOMP/CESM](https://github.com/ESCOMP/CESM) | 490 | Sep 2026 | Institutional backbone for SRM scenario runs (Python/C) |
| 2 | ClimaAtmos.jl (atmosphere / cloud microphysics / albedo) | [CliMA/ClimaAtmos.jl](https://github.com/CliMA/ClimaAtmos.jl) | 119 | Sep 2026 | Best open substitute for aerosol–cloud forcing work |
| 3 | ClimaLand.jl (land surface & soil carbon) | [CliMA/ClimaLand.jl](https://github.com/CliMA/ClimaLand.jl) | 71 | Sep 2026 | Land-surface boundary for coupled SRM simulations |
| 4 | Oceananigans.jl (GPU ocean sim) | [CliMA/Oceananigans.jl](https://github.com/CliMA/Oceananigans.jl) | 1,333 | Sep 2026 | Ocean component / upwelling modelling infrastructure |
| 5 | ClimateMARGO.jl (climate-economic optimizer) | [ClimateMARGO/ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl) | 73 | Jun 2026 | Cost-optimal SRM trajectory design (inactive) |
| 6 | AM3 (GFDL atmospheric model, legacy) | [FMS-ESM/AM3](https://github.com/FMS-ESM/AM3) | 4 | Mar 2015 | Fortran legacy; institutional SRM history |

**Other finds (small / experimental):**

- [`prashaant1926/open-earth-digital-twin-simulation`](https://github.com/prashaant1926/open-earth-digital-twin-simulation) — open Earth-system digital twin concept (Oct 2025)
- [`Fatema-Nur/LOD-Climate-Prediction-System`](https://github.com/Fatema-Nur/LOD-Climate-Prediction-System) — physics-based climate simulation (Nov 2025)
- [`RhondaMueller/Codes-RFG-Arctic-Impacts`](https://github.com/RhondaMueller/Codes-RFG-Arctic-Impacts) — radiative-forcing code focused on Arctic impacts (Apr 2024)
- [`pmip4/pmip_p2fvar_analyzer`](https://github.com/pmip4/pmip_p2fvar_analyzer) — CMIP6 palaeo-climate data analysis utilities (Sep 2025)

## 📈 Thematic Trend Takeaway

> **The open-source SRM-application gap is the story.** There is no single, well-maintained, open SRM simulator. What exists splits between (a) closed institutional Fortran models (GFDL/NCAR, e.g. CESM, AM3) and (b) emerging-but-narrow Julia components (ClimaAtmos, ClimaLand, Oceananigans) that have not yet been coupled into a purpose-built SRM tool. The most live open physics for SRM — aerosol–cloud albedo — is being built inside **ClimaAtmos.jl** (roughly monthly patch releases through Sep 2026: `v0.42.8`, `v0.42.9`, TKE/updraft-drag work, CloudMicrophysics `v0.39`). **Oceananigans.jl** (1,333 ⭐, near-daily commits, GPU, TripolarGrid, Zarr I/O) is the ocean infrastructure any open SRM/upwelling tool would chain onto, but it is not SRM-specific. **Verification infrastructure** (satellite retrieval, deployment monitoring) is the weakest open link — everything hangs on getting simulation right, but governance demands regional impact verification that is almost absent in open source.
