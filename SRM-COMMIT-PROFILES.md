# ☀️ Solar Geoengineering — Repository Profiles (Updated Sep 2026)

**Branch:** solar-geoengineering
**Last Updated:** September 17, 2026
**New commits sourced:** September 2026

---

## Tier 1 — Active & Most Important

### WRF Model (wrf-model/WRF)
- **Stars:** 1,761 | **Forks:** 408 | **Language:** Fortran | **License:** Apache 2.0
- **Last commit:** June 8, 2026 (v4.8.0 release)
- **Frequency:** ~3-5 commits/month sustained
- **SRM Relevance:** Primary model for simulating atmospheric conditions including aerosol interactions. Version 4.8.0 includes updated aerosol-aware physics parameterizations directly applicable to stratospheric aerosol injection modeling.
- **Key contributors:** Anthony Islas (NCAR), weiwangncar (NCAR), Joseph Olson (NCAR), Kelly Werner (NCAR)
- **Why it matters:** This is the only major climate simulation code on GitHub that is actively developed, open-source, and capable of modeling SRM-relevant atmospheric physics. But it requires HPC infrastructure and deep expertise — not accessible to non-specialists.

### PCMDI Metrics Package (PCMDI/pcmdi_metrics)
- **Stars:** 133 | **Forks:** 49 | **Language:** Python | **License:** BSD-3-Clause
- **Last commit:** September 4, 2026 (v4.2.1)
- **Frequency:** Bursty — 10 commits in 2 days for releases
- **SRM Relevance:** The evaluation toolkit. If SRM is deployed, we need to verify it's working. PCMDI provides the metrics for ENSO, MJO, monsoon, cloud feedback, and more.
- **Key contributors:** Jiwoo Lee (LLNL), James Goodnight (LLNL), Jared Lewis (LLNL)
- **Why it matters:** This is the verification infrastructure for any climate intervention. Without it, we can't distinguish SRM-induced cooling from natural variability.

### ClimateMARGO.jl (ClimateMARGO/ClimateMARGO.jl)
- **Stars:** 73 | **Forks:** 15 | **Language:** Julia | **License:** MIT
- **Last commit:** August 17, 2026 (README update after 2-year dormancy)
- **Frequency:** Dormant 2022-2023, showing signs of revival
- **SRM Relevance:** Idealized climate-economic modeling — optimizes trade-offs between mitigation, adaptation, and geoengineering. Makes SRM policy questions computationally tractable.
- **Key contributors:** Fons van der Plas (lead), Henri Drake
- **Why it matters:** This is the "Killer App" for SRM policy analysis — not simulating the physics, but simulating the decisions. The Julia renaissance suggests a new wave of researchers entering this space.

## Tier 2 — Legacy & Niche

### FMS-ESM/AM3
- **Stars:** 4 | **Language:** Fortran | **Last commit:** March 2015
- **SRM Relevance:** GFDL's AM3 atmospheric model — historically used for SAI (Solar Radiation Management) experiments. Legacy but foundational.

### pmip4/pmip_p2fvar_analyzer
- **Stars:** 4 | **Last commit:** September 2025
- **SRM Relevance:** CMIP6 data analysis for paleoclimate modeling — useful for understanding past climate responses that inform SRM research.

### Hausfath/srm-forever
- **Stars:** 0 | **Language:** HTML | **Last commit:** August 26, 2026
- **SRM Relevance:** Interactive single-page economic model comparing SRM vs. rapid mitigation. Uses Weitzman certainty-equivalent discounting. Transparent, published in a single HTML file.

---

## 🎙️ Updated Episode Angle

**The SRM simulation stack has a split personality:**

- **The physics layer** (WRF) is alive, well-funded, and institutional — but impenetrable to non-specialists
- **The evaluation layer** (PCMDI) is the gold standard — but designed for CMIP6 model comparison, not intervention verification
- **The policy layer** (ClimateMARGO) is dormant but showing signs of revival — idealized models could democratize SRM discourse
- **The missing layer:** An open-source SRM-specific simulator that bridges all three

**Episode title idea:** "The SRM Simulation Gap: Why the Most Important Climate Tool Doesn't Exist"
