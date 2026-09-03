# Solar Geoengineering — Project Discoveries

## Episode Theme: Solar Radiation Management (SRM)

---

## Featured Open-Source Projects

### 1. NorESM — Norwegian Earth System Model
- **Repo:** [NorESMhub/NorESM](https://github.com/NorESMhub/NorESM)
- **Stars:** 51 | **Language:** Python | **License:** GPL
- **Last Updated:** Aug 2026
- **Relevance:** Full Earth System Model with atmosphere, ocean, land, and sea ice components — essential for simulating solar radiation management scenarios (e.g., stratospheric aerosol injection, marine cloud brightening).

#### Recent Commit Activity (Last 10 Commits)
| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| 2/11/2026 | Merge PR #771 (TomasTorsvik-patch-1) | Tomas Torsvik | Latest merge |
| 2/10/2026 | Update README.md | Tomas Torsvik | Docs refresh |
| 3/7/2025 | Merge PR #653 (code of conduct) | Tomas Torsvik | Governance improvement |
| 3/7/2025 | Update CODE_OF_CONDUCT.md | Michael Schulz | Ethics/addition |
| 3/6/2025 | Minor adjustments, less US-specific | Tomas Torsvik | Inclusivity edits |
| 3/5/2025 | Include CODE_OF_CONDUCT.md | Tomas Torsvik | Docs |
| 4/30/2024 | Remove docs submodule (#516) | Tomas Torsvik | Infra cleanup |
| 3/22/2024 | Update README.md on master (#510) | Tomas Torsvik | Docs |
| 3/22/2024 | Add noresm2_1_develop branch to README (#507) | Tomas Torsvik | Branch management |
| 12/10/2023 | Remove fixed assignees | Steve Goldhaber | Infra |

#### Trending Themes
- **Governance & community building:** CODE_OF_CONDUCT additions, US-centric language removal
- **Documentation infrastructure:** Submodule removal, README consolidation
- **Release preparation:** The noresm2_1_develop branch reference suggests active version management

---

### 2. C-ESM-EP — CliMAF Earth System Model Evaluation Platform
- **Repo:** [jservonnat/C-ESM-EP](https://github.com/jservonnat/C-ESM-EP)
- **Stars:** 7 | **Language:** Jupyter Notebook / Python
- **Last Updated:** Jul 2026
- **Relevance:** Evaluation platform for IPSL and CNRM climate models — directly applicable to post-SRM simulation analysis and model validation.

#### Recent Commit Activity (Last 10 Commits)
| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| 7/21/2026 | Merge PR #72 (move_fixes_to_ORCHIDEE_mapper) | jservonnat | Feature consolidation |
| 7/9/2026 | Merge remote-tracking branch | Stéphane Sénési | Sync |
| 7/9/2026 | Improve ORCHIDEE_mapper: shorten titles, add alb_mean, Ctrl-click | Stéphane Sénési | Visualization |
| 7/1/2026 | Correction for save_mode (Jerome) | Josefine Ghattas | Bug fix |
| 6/30/2026 | Fix lat/lon names in routing files | Josefine Ghattas | Data correction |
| 6/4/2026 | Corrected path to script folder | Josefine Ghattas | Path fixes |
| 5/28/2026 | Corrected path to script | Josefine Ghattas | Path fixes |
| 5/27/2026 | Add ORCHIDEE essentials & mapper to run_comparison | Josefine Ghattas | Feature addition |
| 5/27/2026 | Renamed ORCHIDEE into ORCHIDEE_v0 | Josefine Ghattas | Versioning |
| 5/27/2026 | Old version not working, first mapper version | Josefine Ghattas | Debugging |

#### Trending Themes
- **ORCHIDEE land-surface mapper overhaul:** Major refactoring of ORCHIDEE (ORchid Canopy–Hydrology–Evapotranspiration model), adding alb_mean (albedo mean) which is critical for SRM albedo inversion studies
- **Visualization improvements:** Ctrl-click navigation, shortened figure titles — better UX for comparing SRM scenarios
- **Data file corrections:** Lat/lon naming fixes for river discharge and routing — ensures accurate ocean-atmosphere coupling analysis
- **Rapid iteration:** Multiple commits from multiple contributors in a compressed timeframe (May–Jul 2026) signals active development

---

## Summary: Solar Geoengineering Development Trends
| Trend | Evidence |
|-------|----------|
| Community governance maturing | CODE_OF_CONDUCT adds, language inclusivity edits |
| Visualization & UX focus | ORCHIDEE_mapper UX improvements, Ctrl-click navigation |
| Albedo analysis capability | alb_mean feature in mapper — directly relevant to SRM reflectivity studies |
| Active multi-contributor collaboration | Multiple contributors across NorESM and C-ESM-EP in 2025-2026 |
| Docs-first approach | Submodule cleanup, README consolidation in both repos |
