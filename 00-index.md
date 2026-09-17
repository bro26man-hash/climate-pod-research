# 🌊 Ocean Intervention — Episode Research Notes

> **Branch:** `ocean-intervention`  
> **Theme:** Ocean-Based Geoengineering (OAE, Iron Fertilization, Seaweed, etc.)  
> **Last Updated:** 2026-09-16

---

## 🎙️ Episode Overview

Ocean-based geoengineering is the **most under-represented domain on GitHub in the entire climate-tech landscape**. Despite the ocean covering 71% of Earth's surface and its central role in every major climate intervention scenario, dedicated open-source ocean geoengineering repositories are virtually nonexistent. Our discovery: **the ocean is the empty quadrant of climate-tech GitHub** — and understanding *why* reveals the structural barriers that separate open-source climate code from ocean science.

---

## 🔍 Project Discoveries

### Direct Ocean Geoengineering Repositories

| Repo | Stars | Language | Last Updated | Focus | Relevance |
|------|-------|----------|-------------|-------|-----------|
| **Team50-Labs/NebuGrid-OpenSource** | 0 | — | Aug 2026 | Fog-harvesting & drip irrigation (water security) | Water capture, not ocean geo |
| **terranexum/OpenCarbon** | 2 | — | Jul 2023 | Carbon management planning | CDR, not ocean-specific |
| **Fatema-Nur/LOD-Climate-Prediction-System** | — | Python | Nov 2025 | Climate simulation (general) | Can model ocean impacts but not ocean-specific |
| **prashaant1926/open-earth-digital-twin-simulation** | — | Python | Oct 2025 | Earth system digital twin | System-level, ocean included |

### Adjacent/Related Repositories

| Repo | Stars | Language | Last Updated | Focus | Role |
|------|-------|----------|-------------|-------|------|
| **wrf-model/WRF** | 1,761 | Fortran | Sep 2026 | Weather Research & Forecasting | Closest open climate model with ocean coupling (module closed) |
| **NOAA-GFDL/MDTF-diagnostics** | 80 | Jupyter | Aug 2026 | Climate simulation diagnostics | CMIP6 analysis incl. ocean |
| **JGCRI/xanthos** | 38 | Python | Aug 2023 | Global hydrologic framework | Ocean precipitation impacts |
| **roocs/clisops** | 25 | Python | Sep 2026 | Climate Simulation Operations | Data ops for ocean datasets |
| **pmip4/pmip_p2fvar_analyzer** | 4 | Python | Sep 2025 | CMIP6 climate data analysis | Paleoclimate/ocean data |

### The Ocean Discovery Gap — What We Found (and Didn't Find)

**Dedicated ocean geoengineering repositories: ~0**

No repositories found that are specifically dedicated to:
- Ocean Alkalinity Enhancement (OAE) simulation
- Iron fertilization modeling
- Seaweed/kelp farming for carbon export
- Ocean upwelling manipulation
- Marine cloud brightening over ocean

Adjacent repos touch the ocean as a *component* of Earth system models, but none treat the ocean as a *target* for intervention.

---

## 📊 Commit Trend Analysis

### Why the Ocean Quadrant Is Empty — Structural Barriers

| Barrier | Description | GitHub Manifestation |
|---------|-------------|---------------------|
| **1. Institutional Siloing** | Ocean research concentrated in ≈10 institutions (Woods Hole, Scripps, GEOMAR, CSIRO, JAMSTEC) with proprietary data ecosystems | Repos are internal; nothing public |
| **2. Data Sensitivity** | Ocean carbon measurements involve regulated research vessels and proprietary sensor data | Open data pipelines don't exist |
| **3. Experimental Complexity** | Ocean interventions require ship deployments, not just code runs | Software is a tiny fraction of total effort |
| **4. Governance Vacuum** | No international framework for ocean geoengineering = no incentive to open-source | No governance repo exists to reference |
| **5. Funding Misalignment** | Climate-tech VC money flows to energy, DAC, and SRM — not ocean | No startup ecosystem to generate OSS |

### Nearby Commit Activity (for context)

- **WRF** (1,761★): Last commits Jun 2026 — version bumps & physics fixes. Most active ocean-capable climate model, but ocean module is institutional/closed.
- **clisops** (25★): Last commits Sep 2026 — entirely CI bot dependency updates. Stable but no science development.
- **Xanthos** (38★): Last commits Aug 2023, then silence. Hydrologic framework including ocean precipitation; development stalled.
- **PMIP4/CMIP6 tools**: Active Sept 2026 but only for ocean *diagnostics*, not intervention simulation.

---

## 🎙️ Episode Narrative Arc

1. **The Empty Quadrant** — Open GitHub has climate models, climate econ, DAC materials, and SRM — but virtually nothing for ocean intervention. Why?
2. **The Institutional Wall** — Ocean research is siloed in a handful of institutions that guard their data and code.
3. **The Ocean Is Harder Than Land** — SRM has clean conceptual models (reflect light). Ocean alkalinity enhancement involves carbonate chemistry, biological pumps, and decades-long timescales. The modeling problem is orders of magnitude more complex.
4. **Governance as a Prerequisite** — Without an international governance framework, there's no social license to even *simulate* ocean intervention openly.
5. **The Path Forward** — What would an open ocean geoengineering codebase look like? Shared ocean chemistry modules? Coupled climate-ocean models with intervention scenarios? Collaborative observatories?

---

## 🔗 Key Links
- [WRF Model](https://github.com/wrf-model/WRF)
- [ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- [Xanthos](https://github.com/JGCRI/xanthos)
- [NOAA-GFDL](https://github.com/NOAA-GFDL)
- [geomalaria](https://github.com/cjcarlson/geomalaria)
- [CMIP6/Paleo](https://github.com/pmip4)