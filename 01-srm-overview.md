# 01 — Solar Geoengineering Episode: Research Overview

> **Episode Theme:** ☀️ Solar Radiation Management (SRM)
> **Research Date:** 2026-09

---

## Episode Premise

Can we safely simulate solar radiation management? Why is the open-source SRM codebase so sparse compared to other climate technologies? This episode explores the simulation tools, the institutional silos, and the governance questions that dominate the SRM conversation.

---

## 🔍 Open-Source SRM & Climate Simulation Projects Discovered

| Repo | Stars | Language | Last Update | Description |
|------|-------|----------|-------------|-------------|
| **wrf-model/WRF** | 1,761 | Fortran | Jun 2026 | Official Weather Research & Forecasting model; actively maintained, v4.8.0 just released |
| **ClimateMARGO/ClimateMARGO.jl** | 73 | Julia | Aug 2026 | Idealized climate-economic modelling framework for optimizing mitigation/adaptation trade-offs |
| **GeoVision (pixnum-hub/GeoVision)** | — | HTML | Dec 2025 | Geoengineering Simulator — brand new, single-author project |
| **PSLmodels/Geo-DICE** | 2 | MATLAB | Aug 2018 | Modified DICE model with geoengineering feedback |
| **FMS-ESM/AM3** | 4 | — | Mar 2015 | GFDL atmospheric model (legacy, but still referenced) |
| **pmip4/pmip_p2fvar_analyzer** | 4 | — | Sep 2025 | CMIP6 climate data analysis tool |
| **Fatema-Nur/LOD-Climate-Prediction-System** | — | — | Nov 2025 | Physics-based climate prediction system |
| **prashaant1926/open-earth-digital-twin-simulation** | — | — | Oct 2025 | Earth system digital twin simulation |
| **RhondaMueller/Codes-RFG-Arctic-Impacts** | 1 | — | Apr 2024 | Radiative forcing code focused on Arctic impacts |
| **jlehtomaa/OOCC_2021** | 2 | Python | — | Simple model for solar geoengineering governance |
| **KOSASIH/GCCS-Core** | 9 | Python | — | Global Climate Control System core algorithms |

---

## 📊 Commit Trend Analysis (SRM & Climate Simulation)

### WRF Model (wrf-model/WRF)
The most active climate simulation codebase on GitHub (1,761 stars). Recent commit history shows:
- **v4.8.0 release cycle (June 2026):** Multiple commits around release preparation, registry changes, and physics package updates
- **Physics & aerosol updates:** Commits like "Turn off tempo_aerosolaware and tempo_hailaware in Registry" and "Upating MYNN-EDMF pointer" show ongoing process-level model development
- **Multi-institutional collaboration:** Contributors from NCAR (weiwangncar), NSSL (Anthony Islas, Joseph Olson), and international developers (Lluís Fita)
- **Trend sign:** Heavy institutional backbone — this is where real SRM-adjacent atmospheric modeling happens, but it's closed-lab science with open code

### ClimateMARGO.jl (ClimateMARGO/ClimateMARGO.jl)
Julia-based interdisciplinary climate-economic model. Recent activity:
- **August 2026:** Two README updates by maintainer Fons van der Plas
- **2022–2023 era:** Dependency upgrades (JuMP/Ipopt), Pluto notebook integration, deprecation cleanup
- **Trend sign:** Small but sustained individual-academic maintenance. Julia is gaining traction in climate science for its speed + readability combo

### GeoVision (pixnum-hub/GeoVision)
A geoengineering simulator in HTML. Very new (Dec 2025, 4 commits in one day):
- **Initial commit → LICENSE → README in a single batch**
- **Trend sign:** Seed-stage project. Could become important for educational/visualization SRM tools if maintained

### Legacy & Niche
- **Geo-DICE (PSLmodels):** Dormant since 2018. The geoengineering-DICE synthesis was ahead of its time
- **AM3 (FMS-ESM):** Legacy GFDL model, still stars but no visible recent commits
- **OOCC_2021:** Governance-focused Python model with very low recent activity

---

## 🎙️ Episode Talking Points

1. **The Simulation Gap:** Most SRM simulation code lives in closed academic labs (GFDL, NCAR, ETH). Open-source exists (WRF, MARGO) but it's not purpose-built for SRM — it's repurposed weather/climate models
2. **Julia is Emerging:** ClimateMARGO.jl shows Julia's potential as the language for next-gen climate-economic models
3. **Visualization Needs:** GeoVision's emergence (however nascent) signals demand for accessible SRM visualization tools
4. **Governance Code is Scarce:** Only OOCC_2021 attempts to model SRM governance — and it's barely maintained
5. **Arctic Focus:** Codes-RFG-Arctic-Impacts is the only repo specifically modeling SRM effects on polar regions

---

## ⚠️ Key Risks & Uncertainties
- SRM code often overlaps with military/defense research — open-source access may be limited by export controls
- Radiative forcing estimates vary dramatically between models — which one is "right" isn't settled
- Governance tools lag far behind engineering tools
