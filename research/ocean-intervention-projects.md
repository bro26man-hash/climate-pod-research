# Ocean Intervention — Project Discoveries

## Episode Theme: Ocean-Based Climate Interventions (Iron Fertilization, Albedo, Deep Ocean Storage)

---

## Featured Open-Source Projects

### 1. ACCESS-ESM1.6 — Australia's Coupled Earth System Model
- **Repo:** [ACCESS-NRI/ACCESS-ESM1.6](https://github.com/ACCESS-NRI/ACCESS-ESM1.6)
- **Stars:** 3 | **Language:** Shell / Fortran / C
- **Last Updated:** Aug 2026
- **Relevance:** Fully-coupled global climate model with atmosphere, ocean, land, sea ice, and ocean biogeochemistry components — directly applicable to ocean iron fertilization simulations and ocean-atmosphere interaction studies.

#### Recent Commit Activity (Last 10 Commits)
| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| 8/27/2026 | spack.yaml: access-spack-packages with oasis3-mct fixes (#223) | Harshula Jayasuriya | Build infra |
| 8/18/2026 | Merge PR #218 (next-release) | Dougie Squire | Release merge |
| 8/18/2026 | Update ACCESS-ESM1.6 version to 2026.04.002 | Dougie Squire | Versioning |
| 8/18/2026 | Update access_spack_packages to 2026.08.009 | Dougie Squire | Dependency mgmt |
| 8/18/2026 | Update UM | Dougie Squire | Model components |
| 8/14/2026 | Update FMS and MOM5 | Dougie Squire | Ocean/ice components |
| 8/7/2026 | Infra Update v9: Consolidate Config Into Manifest (#209) | Tommy Gatti | Build system |
| 8/6/2026 | 2026.04.001 new build (#213) | Anton Steketee | Release |
| 8/6/2026 | spack.yaml: use tag-based real versions (#212) | Harshula Jayasuriya | Build hw/deps |
| 7/28/2026 | Change configs tests to supported branches (#211) | Anton Steketee | CI/CD |

#### Trending Themes
- **Heavy infrastructure work:** The overwhelming majority of recent commits are build-system and dependency updates (spack, FMS, MOM5, UM) — not science code
- **Rapid release cadence:** Version 2026.04.001 → 2026.04.002 in under a month suggests a fast-moving development cycle
- **Reproducibility focus:** spack-based dependency management and tag-based versioning prioritize reproducible science builds
- **Build-system maturation:** Consolidating configs into manifests, updating test branches — signs of a team-scale software engineering effort
- ⚠️ **Implication for ocean intervention research:** The code has ocean biogeochemistry components, but current development emphasis is on infrastructure rather than new ocean intervention parameterizations

---

### 2. CMEW — Climate Model Evaluation Workflow
- **Repo:** [MetOffice/CMEW](https://github.com/MetOffice/CMEW)
- **Stars:** 5 | **Language:** Python
- **Last Updated:** Sep 2026
- **Relevance:** A Cylc 8 workflow for evaluating all Earth System Model components — essential for validating ocean intervention models before and after deployment simulations.

#### Recent Commit Activity (Last 10 Commits)
| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| 9/2/2026 | Refactor update_recipe_file.py to remove KGO files | Emma Hogan | Legacy cleanup |
| 8/28/2026 | Remove environment variables from create_request_file.py | Naomi Parsons | CI/CD improvement |
| 8/28/2026 | Remove fetch_recipe.py | Emma Hogan | Legacy removal |
| 8/24/2026 | Create generic install_package script | Emma Hogan | Infrastructure |
| 8/18/2026 | Update testing documentation | Paul Earnshaw | Docs |
| 8/18/2026 | Add documentation for all AutoAssess apps | Paul Earnshaw | Feature docs |
| 8/17/2026 | Top-level AutoAssess page is missing | Paul Earnshaw | Bug fix |
| 8/17/2026 | Remove environment variables from create_variables_file.py | Naomi Parsons | CI/CD |
| 8/17/2026 | Remove environment variables from fetch_recipe.py | Naomi Parsons | CI/CD |
| 8/17/2026 | Add monsoon test file | Naomi Parsons | Testing |

#### Trending Themes
- **Legacy code removal:** Active deletion of old recipe files (fetch_recipe.py, KGO files) — streamlining toward a cleaner evaluation pipeline
- **Environment variable elimination:** Multiple PRs removing hardcoded env vars from recipe generation — improves usability and reproducibility for ocean intervention case studies
- **AutoAssess app expansion:** New documentation and pages for automated assessment apps — enabling systematic comparison of ocean intervention model outputs against observational benchmarks
- **Monsoon testing:** New monsoon test file expands the evaluation framework beyond standard climate modes to region-specific phenomena relevant to ocean intervention impact assessment
- **Rapid, distributed team activity:** 8 contributors making commits across Aug 17–Sep 2, 2026 signals a well-organized development team

---

## Summary: Ocean Intervention Development Trends
| Trend | Evidence |
|-------|----------|
| Infrastructure over science | Most commits are build system, not new parameterizations |
| Release velocity | ACCESS-ESM1.6 shipping monthly versions |
| Reproducibility emphasis | spack, tag-based versions, env var removal |
| Evaluation framework maturation | CMEW's AutoAssess expansion, monsoon test coverage |
| Gap in intervention-specific code | Limited open-source ocean fertilization/albedo modification parameterizations |

---

## Cross-Cutting: Ocean Intervention on GitHub
- **Most relevant model:** ACCESS-ESM1.6 with its ocean biogeochemistry components
- **Best evaluation framework:** CMEW with AutoAssess for validating intervention outcomes
- **Gap:** Very few open-source repositories specifically implementing ocean iron fertilization,marine cloud brightening, or ocean albedo modification parameterizations — most are in central climate modeling centers locked behind collaboration agreements
- **Opportunity:** An open-source ocean intervention parameterization module would fill a significant gap in the available toolchain for geoengineering research
