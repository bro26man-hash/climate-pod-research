# ☀️ Solar Geoengineering — Episode Research Notes

## Overview
Solar Radiation Management (SRM) aims to reflect sunlight back to space to offset warming. This branch covers open-source simulation models, codebases, and tools relevant to solar geoengineering research.

---

## 🔍 Project Discoveries

### 1. [Codes-RFG-Arctic-Impacts](https://github.com/RhondaMueller/Codes-RFG-Arctic-Impacts)
- **Stars:** 1 | **Language:** Jupyter Notebook
- **Description:** Radiative forcing geoengineering code analyzing Arctic temperature extremes and permafrost thawing under SRM scenarios.
- **Key files:** `analysis/` directory with permafrost area analysis, climate model (CLM) analysis scripts (`Min_clm_2.py`, `Mean_clm_2.py`, `Max_clm_2.py`)
- **Relevance:** Directly models geoengineering radiative forcing impacts on sensitive Arctic regions — perfect for discussing unintended consequences of SRM.

### 2. [open-earth-digital-twin-simulation](https://github.com/prashaant1926/open-earth-digital-twin-simulation)
- **Language:** TeX | **Last updated:** 2025-10-10
- **Description:** Open-source distributed simulation platform modeling Earth's major environmental systems using real-time public data.
- **Relevance:** A "digital twin" of Earth's systems is exactly the kind of infrastructure needed to simulate SRM deployment scenarios — temperature feedbacks, atmospheric chemistry changes, etc.

### 3. [FMS-ESM/AM3](https://github.com/FMS-ESM/AM3)
- **Stars:** 4 | **Language:** FORTRAN
- **Description:** The atmospheric component of the GFDL coupled model CM3 — a full Earth System Model used for climate projections including SRM simulations.
- **Relevance:** GFDL's models are the backbone of most published SRM research (e.g., GeoMIP experiments). AM3 simulates atmospheric dynamics, radiation, and aerosols — all critical for modeling stratospheric aerosol injection.
- **Note:** Last commit was 2015; the codebase is older but still scientifically relevant as the basis for many SRM simulation studies.

### 4. [LOD-Climate-Prediction-System](https://github.com/Fatema-Nur/LOD-Climate-Prediction-System)
- **Last updated:** 2025-11-20
- **Description:** Physics-based simulation of the Sun–Earth–Moon system visualizing Earth's Length of Day changes and climate indicators.
- **Relevance:** While focused on LOD/moon dynamics, the framework for physics-based climate prediction is adaptable to SRM scenario modeling.

---

## 📊 Commit Trends & Development Activity

| Repo | Last Activity | Commit Frequency | Status |
|------|--------------|-----------------|--------|
| Codes-RFG-Arctic-Impacts | Apr 2024 | Low — mostly README cleanup; last adds Sep 2024 | ⚠️ Semi-dormant |
| open-earth-digital-twin-simulation | Oct 2025 | Single init commit | 🆕 Early stage |
| FMS-ESM/AM3 | Mar 2015 | No recent commits since 2015 | 🔒 Archived/Stable |
| LOD-Climate-Prediction-System | Nov 2025 | Active — Nov 2025 | 🟢 Recently updated |

**Trend:** Solar geoengineering code on GitHub is sparse. Most SRM simulation work happens in academic laboratories (GFDL, NCAR, ETH Zurich) using proprietary or internal tools. The few open-source repos tend to be either (a) heavily stabilized/archived like AM3, or (b) very recent and experimental.

---

## 🎙️ Podcast Talking Points
1. **The simulation gap:** Why is there so little open-source SRM code? (Risk of unilateral deployment, computational cost, model complexity)
2. **Arctic as a canary:** The RFG-Arctic-Impacts repo highlights how SRM could worsen polar amplification if not globally coordinated
3. **From Fortran to Jupyter:** The evolution of climate modeling tools from institutional legacy code to accessible notebooks
4. **Digital twins as SRM testbeds:** How open-earth-digital-twin-simulation could become a platform for SRM scenario exploration

---

## 📚 Further Reading
- GeoMIP (Geoengineering Model Intercomparison Project): https://g6.ipsl.sorbonne-universite.fr/gemip/
- GFDL AM3 paper: Donner et al., 2011, JAdvModelEarthSyst
- Arctic permafrost feedback: Rhonda Mueller's research (UVA)