# ☀️ Solar Geoengineering — Open-Source Project Discoveries

## Branch: `solar-geoengineering`
*Last updated by podcast research, Sept 2026*

---

## 1. Overview

Solar Radiation Management (SRM) is arguably the most contentious and least understood area of geoengineering. On GitHub, the open-source footprint is surprisingly thin — most high-fidelity SRM simulation happens inside closed academic labs (GFDL, NCAR, ETH Zurich). What follows is a catalog of the publicly visible projects, their activity levels, and what the codebase tells us about where solar geoengineering research is heading.

---

## 2. Project Catalog

### 🔬 PCMDI/pcmdi_metrics — **133 ⭐** — `Python`
**URL:** https://github.com/PCMDI/pcmdi_metrics
**Last updated:** Sept 4, 2026
**Focus:** Collective & Systematic Evaluation of Climate and Earth System Models

The most actively maintained climate-model evaluation tool on GitHub. While not SRM-specific, it is the workhorse for validating whether models can even reliably simulate the effects of intentional radiative forcing.

**Recent commits (Sept 3–4, 2026):**
- v4.2.1 release — maintenance & bugfix sprint
- Fix roundoff in mean_climate figures (`90cbc50`)
- Extreme-values chunking improvements (`1424_jsgoodni_extremes_chunking`)
- Variability-modes Dask SVD memory fix (`1423/lewisjared`)

**Podcast angle:** Before you can simulate SRM, you need models that pass peer review. PCMDI is the gatekeeper.

---

### 🌍 Fatema-Nur/LOD-Climate-Prediction-System — **unlisted stars** — `Python`
**URL:** https://github.com/Fatema-Nur/LOD-Climate-Prediction-System
**Last updated:** Nov 2025
**Focus:** Physics-based regional climate prediction (includes ocean & atmosphere coupling)

A smaller but scientifically grounded effort — looks at regional prediction, which is the natural complement to global SRM interventions.

---

### 🪐 prashaant1926/open-earth-digital-twin-simulation — **0 ⭐**
**URL:** https://github.com/prashaant1926/open-earth-digital-twin-simulation
**Last updated:** Oct 10, 2025
**Focus:** Distributed Earth system simulation via agent-based modeling (Co-Sci platform)

**Commit history:** Single initial commit (`d94e155`, Oct 2025) — project structure only, no code yet.

**Podcast angle:** Represents the "digital twin" vision — a living simulation of Earth's systems. Very aspirational; may be somewhere between concept paper and prototype.

---

### 🧊 FMS-ESM/AM3 — **4 ⭐** — `Fortran`
**URL:** https://github.com/FMS-ESM/AM3
**Last updated:** Mar 2015
**Focus:** NOAA GFDL Atmospheric Model (AM3), legacy version

A decade-old but historically significant open-source Earth system model. Still the basis for many SRM sensitivity studies.

---

### 📊 pmip4/pmip_p2fvar_analyzer — **4 ⭐** — `Python`
**URL:** https://github.com/pmip4/pmip_p2fvar_analyzer
**Last updated:** Sep 2025
**Focus:** CMIP6 paleoclimate and sensitivity variabilities

Useful for understanding how Earth system models respond to forcing perturbations — directly relevant to SRM scenario testing.

---

### 🧊 RhondaMueller/Codes-RFG-Arctic-Impacts — **1 ⭐**
**URL:** https://github.com/RhondaMueller/Codes-RFG-Arctic-Impacts
**Last updated:** Apr 2024
**Focus:** Radiative forcing + Greenland ice sheet impacts

One of the few repos explicitly linking SRM-style forcing to Arctic consequences — highly relevant to the geoengineering ethics conversation.

---

### 📓 stvdio-luisgui/Climate-earth-system-modeling-notes — **unlisted stars** — `Jupyter Notebook`
**URL:** https://github.com/stvdio-luisgui/Climate-earth-system-modeling-notes
**Last updated:** Aug 14, 2026
**Focus:** Reproducible ESM exercises: energy-balance models, sensitivity analysis

**Recent commits (Aug 13–14, 2026):**
- Initial commit (`4772a9a`)
- Added zero-dimensional Earth energy-balance model (`cc2c0ef`)
- README clarity revisions (`acd59ea`, `355ba5e`)

**Podcast angle:** The "Jupyter notebook as ecologist's field guide" — low-barrier entry into climate simulation, ideal for educational podcast segments.

---

## 3. The Solar Geoengineering "Code Gap"

| Metric | Finding |
|--------|---------|
| Dedicated SRM repos | **< 5** with meaningful code (search returned zero hits for "solar radiation management") |
| Active committers | 1 (PCMDI/Jiwoo Lee, 5 commits in 48 hrs on Sept 3–4, 2026) |
| Language dominance | Fortran (legacy models) + Python (newer tools) — no newer languages (Rust, Go, etc.) yet |
| Governance code | **None found** on GitHub — regulatory/ethical frameworks are not open-sourced anywhere |

**Key takeaway for the episode:** The SRM simulation world is dominated by legacy institutional models (GFDL, NCAR) guarded behind closed doors or academic gatekeeping. The open-source gap is not just about code — it's about who gets to decide whether we inject sulfur into the stratosphere.
