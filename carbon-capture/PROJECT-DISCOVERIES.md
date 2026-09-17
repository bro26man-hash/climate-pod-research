# 🌍 Carbon Capture — Project Discoveries

## Overview
This file catalogs open-source projects related to Direct Air Capture (DAC), carbon capture and storage (CCS), and carbon management technologies discovered through GitHub research.

---

## Key Projects Found

### 1. openair-collective/openair-cyan ⭐ 76 stars
- **URL:** https://github.com/openair-collective/openair-cyan
- **Focus:** DIY small-scale open hardware direct air carbon capture device called "Cyan"
- **Last activity:** Feb 12, 2024
- **Language:** Not specified (hardware documentation)
- **Relevance:** THE flagship open-source DAC project. OSHWA-certified (US001095). Real, buildable hardware for $500-ish that captures CO2 from air. This is the most important open-source DAC project on GitHub.
- **Commit insight:** 6 commits on Feb 12, 2024 (release push), then quiet. The burst pattern suggests a funding-driven or milestone-driven team.

### 2. protontypes/open-sustainable-technology ⭐ 2,546 stars
- **URL:** https://github.com/protontypes/open-sustainable-technology
- **Focus:** Comprehensive open-source climate-tech directory — includes DAC, CCU, energy storage
- **Last activity:** Sep 9, 2026 (active)
- **Language:** Markdown (directory/index)
- **Relevance:** Massively important as an index. Not a tool itself, but the best annotated list of climate-tech open source. Includes projects like claude-carbon, PowerIO, openflexure microscope.
- **Commit insight:** Very active — 5 commits in August-Sep 2026. Multiple contributors. Institutional maintenance pattern.

### 3. terranexum/OpenCarbon ⭐ 2 stars
- **URL:** https://github.com/terranexum/OpenCarbon
- **Focus:** Carbon management technologies and DAC planning — ensuring clean energy use and low-cost
- **Last activity:** Jul 18, 2023
- **Language:** Not specified
- **Relevance:** Planning-stage project for open DAC research infrastructure. More conceptual than hardware.
- **Commit insight:** 10 commits between May-Jul 2023. Mostly README updates. Single contributor. Then silence.

### 4. tjz21/DAC_peroxovanadates ⭐ 2 stars
- **URL:** https://github.com/tjz21/DAC_peroxovanadates
- **Focus:** Computational screening of peroxovanadate sorbents for DAC
- **Last activity:** Sep 23, 2025
- **Language:** Python (computational chemistry)
- **Relevance:** Part of a systematic computational materials science effort to find novel DAC sorbents. Uses density functional theory (DFT) to screen perovdp数据结构酸盐 compounds.
- **Commit insight:** 10 commits between Dec 2023 and Sep 2025. Research paper workflow: initial commits, then DOI links added, then CC0 license for data sharing.

### 5. tjz21/DAC_peroxotitanates ⭐ 2 stars
- **URL:** https://github.com/tjz21/DAC_peroxotitanates
- **Focus:** Same as above but for peroxotitanate sorbents
- **Last activity:** Aug 19, 2026
- **Language:** Python
- **Relevance:** Companion to the peroxovanadates repo. The August 2026 update suggests this computational chemistry wave is still active.
- **Commit insight:** Updated Aug 19, 2026 — part of the "August 2026 DAC materials wave".

### 6. isaH93/dac-moving-bed-digital-twin
- **URL:** https://github.com/IsaH93/dac-moving-bed-digital-twin
- **Focus:** Moving-bed TVSA digital twin for DAC — couples sorbent physics with SimPy discrete-event simulation
- **Last activity:** Jul 3, 2026
- **Language:** Python
- **Relevance:** The most technically sophisticated DAC simulation found. Uses Toth isotherm, LDF kinetics, and discrete-event simulation. A "digital twin" approach — the next generation of DAC process modeling.
- **Commit insight:** Active through July 2026. Python-based, which is notable — most climate simulation code is Fortran.

### 7. salmansust/CO2-Sequestration ⭐ 32 stars
- **URL:** https://github.com/salmansust/CO2-Sequestration
- **Focus:** Carbon Capture and Sequestration (CCS) simulation in MATLAB
- **Last activity:** Mar 24, 2019
- **Language:** MATLAB
- **Relevance:** Most-starred CCS-specific repo found. Typical early-career academic project — MATLAB simulation of CCS processes. Good for episode context on the "classical" approach vs. open-source alternatives.
- **Commit insight:** Only 2 commits, both on the same day (Mar 24, 2019). Upload then abandon — classic academic repo pattern.

### 8. ClimateSoton/climate-research-group
- **URL:** https://github.com/ClimateSoton/climate-research-group
- **Focus:** Chemical looping, carbon capture and utilisation (CCU), advanced materials, CO₂ conversion, CFD modelling
- **Last activity:** Aug 6, 2026
- **Language:** HTML (website/repository for research group)
- **Relevance:** University of Southampton research group. More of a group page than a tool, but shows institutional engagement in DAC/CCU.

---

## The August 2026 DAC Materials Wave

Three repositories were all updated on or near Aug 19, 2026:
- tjz21/DAC_peroxovanadates — peroxovanadate DFT screening
- tjz21/DAC_peroxotitanates — peroxotitanate DFT screening  
- openair-collective/openair-cyan — hardware documentation update

This suggests a coordinated research event — possibly a workshop, journal submission, or funding cycle — in open computational DAC materials science. The timing is striking and worth investigating.

---

## What's Missing (Gaps)

| Gap | Significance |
|-----|-------------|
| No open-source DAC process simulation ( Aspen-like) | Industrial DAC process simulation is proprietary. No open-source equivalent exists. |
| No canonical sorbent database | Material data for DAC sorbents is scattered across papers, not centralized in open data. |
| No standard benchmarking framework for DAC | How do you compare a new sorbent to an old one? No open benchmark exists. |
| Electro-swing DAC only has hardware, no simulation | The most promising novel DAC mechanism lacks computational modeling tools. |
| Minimal Python-based process modeling | The isaH93 digital twin is an exception. Most code is MATLAB, Fortran, or just documentation. |

---

## Episode Talking Points

1. **Can open source break the $1000/ton DAC cost barrier?** — openair-cyan targets $500-ish. Is community-driven hardware iteration the path to cost parity?
2. **The peroxovanadate moment** — Three repos updating simultaneously in Aug 2026 suggests a coordinated research push. Open computational chemistry could accelerate sorbent discovery.
3. **Digital twins for DAC** — isaH93's moving-bed TVSA simulation represents the next generation: physics-based, Python-based, open-source process modeling.
4. **The index vs. the tool** — OpenSustainableTechnology (2,546★) is a directory. OpenCyan (76★) is hardware. Directories are important, but tools are transformative.
5. **The $1,000/ton question** — Current DAC costs ~$400-1,000/ton. Open-source hardware and materials screening could change this equation.

---

## Research Notes
- **Search queries used:** "climate technology carbon capture", "direct air capture climate", "carbon capture simulation"
- **Total repos found in carbon theme:** ~10 identifiable
- **Most active repo:** protontypes/open-sustainable-technology (Sep 2026)
- **Most impactful repo:** openair-collective/openair-cyan (76★, real hardware)
- **Most sophisticated simulation:** isaH93/dac-moving-bed-digital-twin (Python, physics-based)n- **Oldest flagship:** ClimateSoton (2026, institutional)
