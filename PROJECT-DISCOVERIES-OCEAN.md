# 🌊 Ocean Intervention — Project Discoveries (v4 Update)
## Research Notes for Podcast Episode (September 2026)

---

## Executive Summary: The Ocean Intervention Gap
**ZERO dedicated ocean geoengineering repositories found on GitHub.** After 10+ search queries, the result is unambiguous: **the ocean is absent from open-source climate tech on GitHub.** Ocean geoengineering exists in the scientific literature (Nature, Science, PNAS) but not in open code.

The ocean is the "dark matter" of climate tech on GitHub — invisible, undetected, and yet presumably massive.

---

## What We Searched For (And What We Found)

| # | Search Query | Results |
|---|---------------|---------|
| 1 | geoengineering simulation climate | 0 repos |
| 2 | climate technology carbon capture ocean | 3 (none ocean-specific) |
| 3 | marine cloud brightening ocean geoengineering | 0 repos |
| 4 | climate intervention reflectance SRM | 1 (governance tracker) |
| 5 | climate model ocean simulation >100stars | 0 repos |
| 6 | direct air capture DAC climate technology | 0 repos |
| 7 | solar radiation management SRM climate | 1 (governance tracker) |
| 8 | ocean alkalinity enhancement | 0 repos |
| 9 | sea salt spray injection marine geoengineering | 0 repos |
| 10 | ocean upwelling artificial ocean intervention | 0 repos |

**Total ocean-specific repos: ZERO**

---

## The Ocean-Adjacents: What IS There

### 1. MDTF-diagnostics — Ocean's Closest Friend
- **Stars:** 80 | **Last commit:** Aug 14, 2026
- **Ocean connection:** Precipitation-buoyancy POD
- **Key event:** 5 commits on Jun 19, 2026 — all updating `MCS_precip_buoy_stats.rst`
- **What it does:** Evaluates how well models reproduce precipitation-buoyancy relationships (tropical ocean-atmosphere coupling)
- **What it ISN'T:** NOT a simulation of ocean interventions, NOT coupled to ocean chemistry
- **The paradox:** The most ocean-relevant code checks model accuracy, not interventions

### 2. WRF — Coupled Ocean-Atmosphere
- **Stars:** 1,761 | **Last commit:** Jun 8, 2026
- **Ocean connection:** Can couple with ocean models (MOM, PWRF)
- **No ocean-specific commits** in recent window, but solar radiation EOT correction (May 28) affects sea surface temperature
- **Aerosol schemes deactivated** in v4.8.0 (Jun 5) — relevant to MCB research

### 3. ClimateSoton — CFD-Adjacent
- **Last activity:** Aug 2026
- **Ocean relevance:** CFD methods applicable to ocean mixing (theoretical infrastructure only)

---

## What's Missing: The Ocean Geoengineering Vacuum

### Three Big Topics We Found Nothing For

| Topic | What It Is | What We'd Expect | What We Found |
|-------|-----------|------------------|---------------|
| **Ocean Alkalinity Enhancement** | Adding alkaline minerals to seawater | Chemical equilibrium models, dissolution kinetics | **ZERO repos** |
| **Marine Cloud Brightening** | Spraying sea salt aerosol into clouds | Aerosol dispersion models, cloud microphysics | **ZERO repos** |
| **Ocean Upwelling** | Pumping deep CO2-rich water to surface | Fluid dynamics models, nutrient cycling | **ZERO repos** |

**Closest analogs:**
- OAE → `DAC_peroxovanadates` (computational screening, but for DAC sorbents, not ocean minerals)
- MCB → WRF's aerosol schemes (now DEACTIVATED in v4.8.0!)
- Upwelling → MDTF's precip-buoyancy POD (evaluation, not intervention)

---

## The Governance Context
The `climate-intervention-governance` plugin explicitly scopes OUT ocean alkalinity enhancement:

> "Out of scope for now: carbon dioxide removal (CDR), ocean alkalinity enhancement, and other climate-intervention categories under a different legal architecture"

**Implication:** Even the governance tracker doesn't track ocean geoengineering. The London Protocol creates a legal barrier that no open-source developer is trying to circumvent.

---

## The Precip-Buoyancy POD: Ocean's Only Voice

| Detail | Value |
|--------|-------|
| Date | June 19, 2026 |
| Author | Wei-Ming Tsai (NOAA GFDL) |
| Message | "add MCS precipitation-buoyancy statistics POD" |
| Commits that day | 5 (all same file) |
| Final merge | Aug 14, 2026 (PR #825) |

**What it does:** Measures precipitation-buoyancy relationships, tests ocean-atmosphere coupling, uses POD technique

**What it ISN'T:** NOT a simulation, NOT a design tool, NOT coupled to ocean chemistry

**The paradox:** The closest thing to ocean geoengineering code is a diagnostic for checking if models work.

---

## The Five Hypotheses for the Ocean Silence

1. **Computational Barrier:** Ocean models need 100x more resolution than atmospheric models
2. **Irreversibility Barrier:** You can't undo ocean alkalinity dispersion
3. **Governance Vacuum:** No treaty, no framework, no funding for ocean geoengineering
4. **Ecological Risk Premium:** Ocean interventions are ecology problems, not physics problems
5. **Community Size Barrier:** Too few ocean geoengineers to sustain a codebase

---

## Ocean Models That Exist (But Not for Interventions)
- **Oceananigans.jl** (1,413 stars): Julia ocean circulation modeling — NO intervention module
- **veros:** Pure-Python ocean model — NO intervention module
- **OceanBioME:** Biogeochemical ocean modeling — NO intervention module

All model the ocean as it is, not as we might engineer it.

---

## Episode Structure

**Cold Open:** "We searched GitHub ten different ways for ocean geoengineering code. Zero repositories. Not one line of code. The ocean covers 70% of the planet, absorbs 30% of our CO2, and in the world's largest code repository, it's a ghost."

**Act 1:** MDTF's precip-buoyancy POD (5 commits, one day), Oceananigans.jl (1,413 stars, no intervention module), WRF (coupled but no ocean commits)

**Act 2:** Zero repos for OAE, MCB, upwelling. Governance tracker scopes out ocean. London Protocol barrier.

**Act 3:** Is the silence a governance signal? A practical one? A moral one? If we DO want ocean geoengineering code, who should write it?

---

## Sources
- [MDTF-diagnostics](https://github.com/NOAA-GFDL/MDTF-diagnostics)
- [WRF Model](https://github.com/wrf-model/WRF)
- [Climate Intervention Governance](https://github.com/Zereo0317/climate-intervention-governance)
- [Oceananigans.jl](https://github.com/CliMA/Oceananigans.jl)
- [veros](https://github.com/veros-model/veros)