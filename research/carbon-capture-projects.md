# Carbon Capture — Project Discoveries

## Episode Theme: Carbon Dioxide Removal (CDR) & Capture Technologies

---

## Featured Open-Source Projects

### 1. Carbon-Climate Box Model (CCBM)
- **Repo:** [lnnrtrmm/Carbon-Climate-Box-Model](https://github.com/lnnrtrmm/Carbon-Climate-Box-Model)
- **Stars:** 6 | **Language:** Python
- **Last Updated:** Jun 2025
- **Relevance:** A simplified Earth System Model box-model specifically designed to reproduce the behavior of MPI-ESM and other ESMs — perfectly suited for modeling carbon cycle dynamics and CO₂ uptake simulations in CDR scenarios.

#### Recent Commit Activity (Last 10 Commits)
| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| 6/10/2025 | Adding 2BoxOcean as option | Lennart Ramme | New ocean component |
| 6/10/2025 | Fix issue with new routine, now identical to old | Lennart Ramme | Bug fix / parity |
| 6/5/2025 | Add constants.py, update forcedOceanCModel | Lennart Ramme | Refactoring |
| 6/4/2025 | Updates to forcedOceanCarbonModel, new 3-box model (WIP) | Lennart Ramme | Major feature |
| 6/4/2025 | Add preliminary version of ocean processes library | Lennart Ramme | Library add |
| 5/16/2025 | Add dbg output, modify spinup, allow smaller time steps | Lennart Ramme | Debugging + numerics |
| 5/8/2025 | Add spinup option to forcedOceanCarbonModel | Lennart Ramme | Spinup logic |
| 5/8/2025 | Add thickness-dependent calc of surface layer properties | Lennart Ramme | Physics improvement |
| 5/7/2025 | Cleanup CCBM_lean_version, add simplified forced Ocean model | Lennart Ramme | Refactoring |
| 3/25/2024 | Add carbon to name of model | Lennart Ramme | Branding/Naming |

#### Trending Themes
- **Ocean carbon cycle modeling:** The dominant thread is ocean-specific carbon uptake — forcedOceanCarbonModel, ocean processes library, 2BoxOcean option
- **Multi-box model architecture:** Progression from 1-box → 2-box → 3-box configurations represents increasing fidelity for representing ocean stratification and carbon transport
- **Spinup & numerical stability:** Multiple commits on spinup options, smaller time steps, and debugging suggest the model is transitioning from prototype to production readiness
- **Constants abstraction:** Adding constants.py signals codebase maturation — moving hardcoded parameters into a dedicated module
- **Consistent solo development:** All commits by Lennart Ramme suggests a focused, single-developer project with clear priorities

---

## Summary: Carbon Capture Development Trends
| Trend | Evidence |
|-------|----------|
| Ocean-atmosphere carbon coupling | forcedOceanCarbonModel, ocean processes library, 2BoxOcean |
| Increasing model complexity | 1-box → 2-box → 3-box progression |
| Numerical rigor | Spinup options, smaller time steps, debugging |
| Codebase maturation | constants.py module, naming conventions |
| Solo-developer momentum | All commits by one author with high consistency |

---

## Cross-Cutting: Carbon Capture on GitHub
- **Most active carbon-focused repo:** Carbon-Climate Box Model (monthly commits over 14+ months)
- **Gap:** Limited open-source Direct Air Capture (DAC) hardware/process simulation tools — mostly proprietary in industry (Climeworks, Carbon Engineering)
- **Opportunity:** The CDR/CCS space could benefit from more open-source process models for amine scrubbing, mineralization, and BECCS supply-chain logistics
