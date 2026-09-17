# ☀️ Solar Geoengineering — Project Discoveries

## Discovery Methodology
Searched GitHub using queries: `geoengineering simulation climate`, `geoengineering`, `solar geoengineering`, `climate simulation modeling`. Filtered for repos with solar/radiation management focus.

## Top Findings

| # | Repo | Stars | Language | Status | Focus Area |
|---|------|-------|----------|--------|------------|
| 1 | **ClimateMARGO/ClimateMARGO.jl** | 73 | Julia | ✅ Active (Aug 2026) | Climate-economic optimization with SRM |
| 2 | **openair-collective/openair-cyan** | 76 | — | ⚠️ Dormant (Feb 2024) | DIY DAC device (cross-listed) |
| 3 | **brandonhimpfen/awesome-geoengineering** | 4 | Python | ✅ Active (Sep 2026) | Curated geoengineering resource list |
| 4 | **jlehtomaa/OOCC_2021** | 2 | Python | ⚠️ Dormant (Nov 2021) | SRM governance modeling |
| 5 | **PSLmodels/Geo-DICE** | 2 | MATLAB | ⚠️ Dormant (Sep 2028) | DICE + geoengineering |
| 6 | **cjcarlson/geomalaria** | 3 | R | ⚠️ Dormant (Feb 2022) | SRM health impact assessment |
| 7 | **JdeJong96/sai-git** | — | Jupyter | ✅ Active (Aug 2025) | CESM SAI data analysis |
| 8 | **jnickla1/CESM2geoeng_documentation** | — | Doc | ⚠️ Empty | CESM2 geoengineering paper docs |

## Key Insight: The 73-Star Ceiling
The most-starred solar geoengineering-specific repository has **73 stars** — ClimateMARGO.jl. Compare this to:
- WRF climate model: **1,761 stars**
- OpenAir-Cyan (DAC): **76 stars**
- awesome-geoengineering (directory): **4 stars**

The SRM simulation community on GitHub is **tiny and fragile**. The entire ecosystem could be sustained by a single funded researcher leaving the field.

## The Active Repos (as of search date)

### ClimateMARGO.jl — The Flagship
- **Maintainer:** Fons van der Plas
- **Contributors:** Henri Drake (earlier)
- **Recent commits:** 2 on Aug 17, 2026 (README), long gaps before
- **Technical notes:** Julia-based, uses JuMP and Ipopt for optimization. Has Pluto notebook integration.
- **What's missing:** No web interface, no documented API, no community contributions.

### sai-git — The Recent Learner
- **Maintainer:** Jasper de Jong
- **Recent commits:** 15 between Feb-Aug 2025
- **Technical notes:** Jupyter notebooks for CESM SAI analysis. Uses xarray/open_mfdataset.
- **Notable:** Creating FLUT (Fully Logged Utility Tool?) and TMQ notebooks. Working on precipitation (PRECT) and temperature (TREFHT) maps.
- **What's missing:** Not a simulation tool — purely analysis/visualization of existing CESM output.

## The Dormant Repos — Tombstones

| Repo | Peak Activity | Last Commit | Number of Commits | Elegy |
|------|--------------|-------------|-------------------|-------|
| Geo-DICE | 2016-2018 | Sep 2018 | 4 | The canonical climate-economics model with SRM, abandoned after its creators moved on. |
| OOCC_2021 | Jul-Sep 2021 | Nov 2021 | 15+ | The only SRM governance model. Dense initial work, then silence. |
| geomalaria | Jan-Feb 2022 | Feb 2022 | 15+ | The only SRM health-impact tool. Intense burst, then permanent quiet. |
| CESM2geoeng | — | — | 0 | Empty repo. Paper exists; code does not. The reproducibility gap made visible. |

---

## Cross-Reference: awesome-geoengineering
- **Repo:** brandonhimpfen/awesome-geoengineering
- **Stars:** 4 | **Last Updated:** Sep 6, 2026
- **Why include it:** It's the only actively maintained *directory* of geoengineering resources. Updated as recently as Sep 2026.
- **Notable:** The curator is clearly tracking the field. Versioned to 2.0.0 in May 2026.
- **Episode use:** A starting point for listeners who want to explore further. The README is the syllabus.
