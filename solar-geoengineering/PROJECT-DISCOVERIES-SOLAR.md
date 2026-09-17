# ☀️ Solar Geoengineering — Project Discoveries (September 2026)

## Search Strategy
Searched GitHub with queries: "geoengineering simulation climate", "geoengineering", "climate simulation", "solar geoengineering". Filtered for repositories with code, documentation, or models related to solar radiation management (SRM).

---

## Ranked Discoveries

### Tier 1: Essential (Active or High-Impact)

| # | Repository | Stars | Language | Last Activity | Why It Matters |
|---|-----------|-------|----------|---------------|---------------|
| 1 | **wrf-model/WRF** | 1,761 | Fortran | Sep 16, 2026 | The atmospheric model that underpins all SRM simulation. v4.8.0 just released with solar radiation fixes. |
| 2 | **NOAA-GFDL/MDTF-diagnostics** | 80 | Jupyter | Aug 14, 2026 | Process diagnostics framework. New precip-buoyancy POD. Ocean-adjacent tool. |
| 3 | **ClimateMARGO/ClimateMARGO.jl** | 73 | Julia | Aug 17, 2026 | Climate-economicmodel. Revival signal after 2.5yr dormancy. Could integrate SRM scenarios. |
| 4 | **brandonhimpfen/awesome-geoengineering** | 4 | Python | Sep 6, 2026 | The curated gateway list. Most sustainably maintained project. v2.0.0 released May 2026. |

### Tier 2: Relevant (Dormant but Influential)

| # | Repository | Stars | Language | Last Activity | Why It Matters |
|---|-----------|-------|----------|---------------|---------------|
| 5 | **pixnum-hub/GeoVision** | — | HTML | Dec 6, 2025 | Web-based geoengineering simulator. All 4 commits on one day. Functional? |
| 6 | **KOSASIH/GCCS-Core** | 9 | Python | Aug 2026 | Global Climate Control System core framework. Ambitious scope. |
| 7 | **jlehtomaa/OOCC_2021** | 2 | Python | Nov 15, 2021 | Governance model for SRM. Frozen since paper publication. |
| 8 | **antara-banerjee/GeoengineeringLE_WinterWarming** | 2 | Python | Apr 24, 2021 | Ensemble analysis for winter warming SRM experiments. Peer-review quality code. |
| 9 | **PSLmodels/Geo-DICE** | 2 | Matlab | Sep 27, 2018 | Modified DICE model with geoengineering. 8 years frozen. |
| 10 | **cjcarlson/geomalaria** | 3 | R | — | Malaria risk modeling with SRM. Ecological side-effect analysis. |

### Tier 3: Edge Cases

| # | Repository | Stars | Language | Last Activity | Notes |
|---|-----------|-------|----------|---------------|-------|
| 11 | **nicmenegoni/ROKA** | 33 | Matlab | Aug 15, 2026 | Rock slope analysis — false positive (geological, not climate) |
| 12 | **nicmenegoni/DICE** | 21 | Matlab | Sep 1, 2026 | Rock discontinuity analysis — false positive |

---

## The Governance Gap (Solar Theme)

**Three governance-related repos found, all dormant:**

1. **OOCC_2021** — Simple SRM governance model, paper-driven, frozen 2021
2. **Geo-DICE** — Modified DICE with geoeconomic scenarios, frozen 2018
3. **SRM economics models** (srm-forever, orbital-climate-simulator) — Interactive tools, tiny repos, emerging

**Pattern:** Governance code is created for papers, not maintained. The physics community has no equivalent of "Astropy" for SRM governance — a成熟, community-maintained tool.

---

## The Simulation Stack (What's Actually Used)

Based on commit analysis, the SRM simulation stack in 2026 is:

1. **WRF** (atmospheric physics, radiation, aerosol transport)
2. **MDTF-diagnostics** (model evaluation, process verification)
3. **ClimateMARGO** (economic scenario framing, mitigation/adaptation trade-offs)
4. **awesome-geoengineering** (discovery gateway)

Everything else is either dormant or a one-off paper artifact.

---

## What's Missing for Solar Episode

- **No interactive SRM simulators exist that are actively maintained.** GeoVision was one attempt, frozen after 4 commits.
- **No open-source radiative transfer code specific to SRM.** WRF handles it but it's a general circulation model, not a targeted SRM tool.
- **No SRM-specific CWM (climate working memory) or data assimilation tools.**
- **The governance gap is the story.** Everything from OOCC_2021 onward has been frozen.

---

*Last updated: September 2026.*