# ☀️ Solar Geoengineering — Project Discoveries

## Overview
This file catalogs open-source projects related to solar radiation management (SRM) and solar geoengineering simulation discovered through GitHub research.

---

## Key Projects Found

### 1. PCMDI/pcmdi_metrics ⭐ 133 stars
- **URL:** https://github.com/PCMDI/pcmdi_metrics
- **Focus:** ESM (Earth System Model) evaluation toolkit, CMIP6 metrics
- **Last activity:** Sep 4, 2026 (v4.2.1 release)
- **Relevance:** Critical for evaluating climate model outputs used in SRM research. CMIP6 experiments include solar geoengineering scenarios (GEOMIP). This toolkit is how researchers quantify whether SRM simulations actually work.
- **Language:** Python
- **Commit insight:** 10 commits in 2 days for v4.2.1 release — institutional burst pattern typical of funded climate modeling groups.

### 2. FMS-ESM/AM3
- **URL:** https://github.com/FMS-ESM/AM3
- **Focus:** GFDL Atmospheric Model (AM3) — legacy Fortran code used in SRM modeling
- **Last activity:** Mar 2015
- **Relevance:** One of the classic models used to simulate stratospheric aerosol injection. Used in major SRM experiments including the Geoengineering Model Intercomparison Project (GeoMIP).
- **Language:** Fortran
- **Commit insight:** Dormant since 2015. Legacy codebase — the modern Python/data-science shift hasn't reached this domain.

### 3. pmip4/pmip_p2fvar_analyzer ⭐ 4 stars
- **URL:** https://github.com/pmip4/pmip_p2fvar_analyzer
- **Focus:** CMIP6 paleoclimate andPMIP data analysis
- **Last activity:** Sep 2025
- **Relevance:** Analyzes paleoclimate data relevant to volcanic analogue experiments for SRM. Understanding past natural experiments (e.g., Pinatubo) informs modern SRM modeling.
- **Language:** Python

### 4. RhondaMueller/Codes-RFG-Arctic-Impacts ⭐ 1 star
- **URL:** https://github.com/RhondaMueller/Codes-RFG-Arctic-Impacts
- **Focus:** SRM radiative forcing impacts on Arctic climate
- **Last activity:** Apr 2024
- **Relevance:** Directly addresses one of the most sensitive and politically charged SRM topics — Arctic impacts. Relevant to episode discussion of regional side effects.
- **Language:** Not specified

### 5. QuantaEnergy/.Symbol
- **URL:** https://github.com/QuantaEnergy/.Symbol
- **Focus:** Earth solar irradiance data and SRM resource links
- **Relevance:** Provides reference data on solar irradiance — the fundamental input parameter for any SRM scenario. Also links to geoengineering.global SRM resources.

---

## What's Missing (Gaps)

| Gap | Significance |
|-----|-------------|
| No interactive SRM simulation tools | Most code is evaluation (PCMDI) or legacy (AM3). No accessible, runnable SRM simulator exists in open source. |
| No Python-based radiative transfer models | The domain is dominated by Fortran and commercially licensed tools. |
| No open-source Coupled Model Intercomparison Project (CMIP) experiment frameworks | CMIP is centralized and closed; no community-driven alternatives. |
| GeoMIP experiment data tools absent | The intercomparison project itself has no open-source data analysis framework on GitHub. |

---

## Episode Talking Points

1. **Why is SRM code so scarce?** — The largest climate modeling centers (GFDL, NCAR, UK Met Office) use SRM internally but don't open-source their tools. This creates a democratic deficit in the SRM discourse.
2. **Can interactive models democratize the discourse?** — If anyone could run an SRM simulation in their browser, how would that change the political conversation?
3. **Arctic risks** — The RhondaMueller code highlights that SRM's effects on the Arctic are a first-order concern. What does open-source code reveal about regional inequality in SRM impacts?

---

## Research Notes
- **Search queries used:** "geoengineering simulation climate", "geoengineering solar radiation management"
- **Total repos found in solar theme:** ~5 identifiable, plus referenced in CMIP/paleoclimate contexts
- **Most active repo:** PCMDI/pcmdi_metrics (Sep 2026)
- **Oldest active repo:** FMS-ESM/AM3 (2015, dormant)
