# 🌊 Ocean Intervention — Detailed Commit Histories

**Last Updated:** September 2026

---

## CliMA/Oceananigans.jl — Recent 10 Commits (MOST ACTIVE)

| SHA | Date | Author | Message |
|-----|------|--------|--------|
| aca5970 | Sep 17, 2026 | Ali Ramadhan | Restore closure fields from checkpoints when closure is a tuple (#6006) |
| ab99a39 | Sep 16, 2026 | Ali Ramadhan | Fix face spacing above partial cells on PartialCellBottom grids (#6013) |
| 9ddbbb1 | Sep 16, 2026 | Ali Ramadhan | Apply the linear operator once per ConjugateGradientSolver iteration (#6012) |
| 1c8fe39 | Sep 16, 2026 | Ali Ramadhan | Bounce Lagrangian particles off immersed boundaries (#6005) |
| c1655e9 | Sep 16, 2026 | Tomás Chor | Add TimeDerivative for computing δt of outputs during simulation (#5823) |
| 72285df | Sep 16, 2026 | Ali Ramadhan | SplitRungeKuttaTimeStepper: evaluate time-dependent forcings and BCs at correct time (#6009) |
| 23020f1 | Sep 16, 2026 | Ali Ramadhan | Fix stage δt used by AVID + RK3 (#6008) |
| d03dfdf | Sep 16, 2026 | Ali Ramadhan | Keep non-finite values in immersed cells out of vertically implicit column solve (#5991) |
| 1fe0ede | Sep 15, 2026 | Mosè Giordano | Fix issues in test suite (#5998) |
| 162c47d | Sep 15, 2026 | Mosè Giordano | Tighten up memory allocations bounds (#6004) |

**Pattern:** Intense institutional development. 10 commits in 3 days by 3 contributors (Ramadhan, Chor, Giordano) with PR-based workflows and numbered issues (#5823-6013). Lagrangian particle bouncing (#6005) is directly relevant to tracer deployment simulations for ocean intervention. Time-dependent forcing capabilities (#6009) are essential for simulating injection scenarios.

## team-ocean/veros — Recent 10 Commits

| SHA | Date | Author | Message |
|-----|------|--------|--------|
| b5a4f49 | Sep 15, 2026 | dependabot | Bump tqdm from 4.70.0 to 4.70.1 (#869) |
| 47026c4 | Sep 15, 2026 | dependabot | Bump matplotlib from 3.11.1 to 3.11.2 (#868) |
| 7732aaf | Sep 14, 2026 | dependabot | Bump numpy from 2.5.2 to 2.5.3 (#867) |
| 6f0e058 | Sep 14, 2026 | Dion Häfner | Bugfix in isoneutral mixing (#866) |
| 29a7e64 | Sep 7, 2026 | dependabot | Bump ipython from 9.17.0 to 9.17.1 (#865) |
| e714e3c | Sep 1, 2026 | dependabot | Bump ipython from 9.16.1 to 9.17.0 (#864) |
| 930d686 | Aug 31, 2026 | dependabot | Bump click from 8.4.2 to 8.5.0 (#863) |
| 448add0 | Aug 25, 2026 | dependabot | Bump scipy from 1.18.0 to 1.18.1 (#862) |
| 8dfd595 | Aug 21, 2026 | dependabot | Bump jax from 0.11.0 to 0.11.1 (#861) |
| 274de71 | Aug 19, 2026 | Roman Nuterman | Update publications list with new articles |

**Pattern:** Maintenance mode. 8/10 commits are dependabot dependency bumps. Only 2 substantive commits: isoneutral mixing bugfix (relevant for accurate pollutant dispersion modeling) and publications update. The project is maintained but not actively developing new features.

## OceanBioME/OceanBioME.jl — Recent 10 Commits (MOST ACTIVE FOR OCEAN BIOGEOCHEMISTRY)

| SHA | Date | Author | Message |
|------|--------|--------|--------|
| 044407b | Sep 17, 2026 | Jago Strong-Wright | Merge PR #419 — return wind to gas exchange top level |
| d3892db | Sep 16, 2026 | Jago | Fix stuff |
| 746168f | Sep 16, 2026 | Jago | Fix |
| 7bec18c | Sep 16, 2026 | Jago | Adjust constructors |
| 99e34f6 | Sep 16, 2026 | Jago | Bump patch release |
| 7ed8db6 | Sep 16, 2026 | Jago | Move wind speed back to gas exchange top level |
| 15f783b | Sep 15, 2026 | Jago Strong-Wright | Merge PR #399 — numerical-earth-coupling |
| 108551b | Sep 15, 2026 | Jago Strong-Wright | Merge PR #411 — gas exchange changes |
| 1929dd9 | Sep 15, 2026 | Jago | Fix docs |
| 4d49c49 | Sep 14, 2026 | Jago | Fix MARBL test to use WindSpeedScaledTransferVelocities |

**Pattern:** Directed, intensive development by a single PI (Jago Strong-Wright). 10 commits in 4 days focused on gas exchange parameterization and wind speed coupling. 3 PRs merged (#399, #411, #419). The gas exchange work is THE central process for ocean-based CDR and OAE.

**Key relevance:** OceanBioME's active gas exchange development is the most directly applicable existing code for ocean intervention modeling. OAE works by changing ocean carbonate chemistry, which is governed by air-sea CO2 flux. OceanBioME is building the physics engine for that flux.

## Cross-Reference: The Ocean-Adjacent Tools

| Tool | Repo | What It Offers for Ocean Intervention |
|------|------|---------------------------------------|
| Atmospheric model | WRF (1,761★) | Ocean boundary layer physics, air-sea coupling |
| Model evaluation | PCMDI (133★) | ENSO, sea ice, ocean heat content metrics |
| Process diagnostics | MDTF (80★) | Precipitation-buoyancy POD (MCB-relevant) |
| Ocean physics | Oceananigans (1,413★) | Fluid dynamics, Lagrangian particles, immersed boundaries |
| Ocean biogeochemistry | OceanBioME (80★) | Carbonate chemistry, gas exchange, MARBL ecosystem |
| Ocean simulator (Python) | veros (400★) | Pure-Python, JAX-powered, accessible |
| Climate models interface | ClimateModels.jl (47★) | Julia interface to multiple climate models |
| Ocean-atmosphere model | MAOOAM (22★) | Modular coupled ocean-atmosphere model |
| Curated list | awesome-open-climate-science (598★) | Gateway to all open climate science tools |

**The analysis:** We have 8 tools for understanding the ocean. We have 0 tools for intervening in it.