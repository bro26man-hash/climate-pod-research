# ☀️ Solar Geoengineering — Research Notes

**Source:** GitHub API-based project discovery + commit-history analysis
**Branch:** `solar-geoengineering`
**Scope:** Solar Radiation Management (SRM) — albedo modification, radiative forcing, and the open-source simulation landscape

---

## ✦ Project Discoveries

| # | Project | Repo | Stars | Last Activity | SRM Relevance |
|---|---------|------|------|---------------|---------------|
| 1 | **CESM** (Community Earth System Model) | [ESCOMP/CESM](https://github.com/ESCOMP/CESM) | 490 ⭐ | Sep 2026 | Institutional backbone for SRM scenario runs (Python/C) |
| 2 | **ClimaAtmos.jl** (atmosphere / cloud microphysics / albedo) | [CliMA/ClimaAtmos.jl](https://github.com/CliMA/ClimaAtmos.jl) | 119 ⭐ | Sep 2026 | Best open substitute for aerosol–cloud forcing work |
| 3 | **ClimaLand.jl** (land surface & soil carbon) | [CliMA/ClimaLand.jl](https://github.com/CliMA/ClimaLand.jl) | 71 ⭐ | Sep 2026 | Land-surface boundary for coupled SRM simulations |
| 4 | **Oceananigans.jl** (GPU ocean sim) | [CliMA/Oceananigans.jl](https://github.com/CliMA/Oceananigans.jl) | 1,333 ⭐ | Sep 2026 | Ocean component / upwelling modelling infrastructure |
| 5 | **ClimateMARGO.jl** (climate-economic optimizer) | [ClimateMARGO/ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl) | 73 ⭐ | Jun 2026 | Cost-optimal SRM trajectory design (inactive) |
| 6 | **AM3** (GFDL atmospheric model, legacy) | [FMS-ESM/AM3](https://github.com/FMS-ESM/AM3) | 4 ⭐ | Mar 2015 | Fortran legacy; institutional SRM history |

**Other finds (small / experimental):**
- `prashaant1926/open-earth-digital-twin-simulation` — open Earth-system digital twin concept (Oct 2025)
- `Fatema-Nur/LOD-Climate-Prediction-System` — physics-based climate simulation (Nov 2025)
- `RhondaMueller/Codes-RFG-Arctic-Impacts` — radiative-forcing code focused on Arctic impacts (Apr 2024)
- `pmip4/pmip_p2fvar_analyzer` — CMIP6 palaeo-climate data analysis utilities (Sep 2025)

---

## 📈 Commit Trend Summary

- **ClimaAtmos.jl is the most active open atmosphere code.** Late-August→September 2026 saw a release cadence of roughly one patch/minor per month: `v0.42.8` (Aug 29), `v0.42.9` (Sep 4), plus physics work on TKE tendencies from updraft pressure drag, CloudMicrophysics `v0.39` upgrade, and a GCMDriven SCM column-forcing port. This steady, contributor-diversified rhythm (Teja Reddy, Nat Efrat-Henrici, Sajjad Azimi, Anna Jaruga) makes it the most credible open building block for aerosol–cloud albedo work.
- **CESM** remains a steady institutional maintenance target (NCAR), updated through Sep 2026 — the主力 vehicle for real SRM injection scenario experiments, but not "open community" in the Julia sense.
- **ClimaLand.jl** is active on the land side (bugfixes, `v1.12.0`/`v1.12.1` releases early Sep 2026) but narrow in scope.
- **Oceananigans.jl** (1,333 ⭐) is an order-of-magnitude more active than the atmosphere packages — near-daily commits, GPU acceleration, TripolarGrid for global basins, Zarr I/O — and is the ocean infrastructure any open SRM/upwelling tool would chain onto.
- **The open-source SRM-application gap is the story.** Almost no dedicated, well-maintained, open SRM simulator exists; what there is straddles (a) closed institutional Fortran models (GFDL/NCAR) and (b) emerging-but-narrow Julia components. Dedicated radiative-forcing/srms code lives in tiny, often archived repos (AM3 from 2015; ~4 stars).

---

## 💡 Talking Points

1. **Can we simulate SRM safely in the open?** The pieces exist (ClimaAtmos for atmosphere, Oceananigans for ocean), but they have not been coupled into a purpose-built SRM simulator. The gap is integration/governance, not physical parameterization.
2. **Cloud-albedo fidelity is the key unknown.** ClimaAtmos's cloud-microphysics work is the most relevant open lever — getting droplet nucleation under perturbed solvency right matters more than the dynamics.
3. **Institutional lock-in vs. the Julia stack.** Real SRM scenarios are run inside GFDL/NCAR (Fortran/closed). The CliMA Julia stack offers an open, developer-friendly alternative but lacks an SRM-specific use-case sponsor.
4. **The Arctic is a canary.** Open radiative-forcing code (`Codes-RFG-Arctic-Impacts`) highlights that regional impact verification — not global mean forcing — is what governance demands, and the tooling is almost absent.
5. **Verification, not simulation, is the blocker.** Once you can simulate SRM, you still need an observational/verification backbone (satellite retrieval, deployment monitoring) that is weakly represented in open source.

---

## 🔑 Key Terminology

- **Radiative forcing (RF)** — change in net irradiance at the tropopause (W/m²); SRM aims for negative RF.
- **Aerosol–cloud interaction (ACI)** — the least-quantified lever in SRM; seeding marine clouds or adding stratospheric aerosols.
- **Albedo modification** — increasing reflectivity (surface or atmospheric).
- **Offset targeting** - maintaining a fixed temperature target via continuous aerosols; termination risk.
- **Stratospheric aerosol injection (SAI)** - the most-studied SRM method; requires ~µm sulfate/diamond dust particles.
- **Simulating "safely"** — meaning robustly quantifying uncertainty and termination spikes, not weather prediction.

---

*Commit data pulled from GitHub API: ClimaAtmos.jl, ClimaLand.jl, Oceananigans.jl, CESM, ClimateMARGO.jl (Sept 2026 snapshots).*
