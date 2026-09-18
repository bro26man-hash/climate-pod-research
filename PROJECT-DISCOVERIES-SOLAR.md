# ☀️ Solar Geoengineering — Project Discoveries

> Updated: September 2026 | Episode theme branch for `climate-pod-research`

---

## Overview

This file profiles the most significant open-source repositories relevant to **solar geoengineering (SRM)** and **climate-atmosphere modeling**. These repos were discovered through targeted GitHub searches and analyzed for commit activity, licensing, and research relevance.

---

## Tier 1 — High-Activity, Institutionally Funded

### 1. WRF (Weather Research and Forecasting Model)
- **Repo:** [wrf-model/WRF](https://github.com/wrf-model/WRF)
- **Stars:** ~1,761 | **Language:** C | **License:** Apache 2.0
- **Last commit:** September 16, 2026 (v4.8.0)
- **Focus:** The foundational mesoscale atmospheric model used worldwide for weather prediction and climate simulation. Recent commits include solar radiation scheme fixes and physics improvements critical for SRM modeling.
- **Why it matters for SRM:** Any solar geoengineering simulation — whether scattering sunlight via stratospheric aerosols or marine cloud brightening — must pass through WRF's radiation scheme. The v4.8.0 update signals active maintenance and increasing sophistication in how models handle solar flux perturbation.
- **Commit signal:** 10 recent commits including version bump and solar radiation fixes. **This is the most active and important repo in the solar theme.**
- **🎙️ Episode hook:** *"If you want to simulate what happens when you block sunlight, you have to talk to WRF. It's the 800-pound gorilla of atmospheric modeling."

### 2. PCMDI Metrics (PCMDI Metrics Package)
- **Repo:** [PCMDI/pcmdi_metrics](https://github.com/PCMDI/pcmdi_metrics)
- **Stars:** ~133 | **Language:** Python | **License:** Apache 2.0
- **Last commit:** September 4, 2026 (v4.2.1)
- **Focus:** Evaluation toolkit for Earth System Models (ESMs), built around CMIP6 data. Provides standardized metrics for comparing model output against observations.
- **Why it matters for SRM:** Before you can assess whether an SRM intervention works, you need to know if your model is any good. PCMDI provides the yardsticks. Without rigorous evaluation, SRM modeling is just storytelling with code.
- **Commit signal:** 10 commits in a single 2-day burst (rapid v4.2.1 release). Shows institutional velocity — PCMDI is a Program for Climate Model Diagnosis and Intercomparison at Lawrence Livermore.
- **🎙️ Episode hook:** *"You can't fix what you can't measure. PCMDI is the quality-control Lab for every climate model that claims to simulate solar geoengineering."

### 3. MDTF Diagnostics (Model Diagnostic Task Force)
- **Repo:** [NOAA-GFDL/MDTF-diagnostics](https://github.com/NOAA-GFDL/MDTF-diagnostics)
- **Stars:** ~80 | **Language:** Python | **License:** Apache 2.0
- **Last commit:** August 14, 2026
- **Focus:** Process-oriented diagnostics for climate models, including the famous **precipitation-buoyancy POD** (Priority of Learning). A tool for evaluating model accuracy at the process level.
- **Why it matters for SRM:** The precipitation-buoyancy POD is the closest thing to an ocean-adjacent diagnostic in open source. It evaluates how well models capture the physics of precipitation-buoyancy coupling — a process that SRM interventions could disturb (e.g., reducing evaporation via solar dimming).
- **Commit signal:** Active development with the precip-buoyancy POD receiving 5 commits on June 19, 2026 alone. This is the most ocean-relevant diagnostic tool and it's actively maintained.
- **🎙️ Episode hook:** *"The precipitation-buoyancy POD is the ocean's closest friend in the code world. Five commits in one day tells you NOAA thinks this is important."

---

## Tier 2 — Individual Researchers, Revival Signals

### 4. ClimateMARGO (Climate-Macro-Growth-Oscillation)
- **Repo:** [ClimateMARGO/ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- **Stars:** ~73 | **Language:** Julia | **License:** MIT
- **Last commit:** August 17, 2026 (README updates after 2+ year dormancy)
- **Focus:** Climate-economic modeling framework that couples climate dynamics with macroeconomic growth. Designed for integrated assessment of climate policies including geoengineering.
- **Why it matters for SRM:** ClimateMARGO could be the bridge between physical SRM modeling and economic impact assessment. If you want to answer "what does solar geoengineering do to GDP?" this is the tool.
- **Commit signal:** Two README updates after 2+ years of dormancy. **No code commits.** This is a revival signal — but ambiguous. Could indicate policy-modeling interest, or could be another false start.
- **🎙️ Episode hook:** *"ClimateMARGO woke up from a two-year nap with just README updates. Is someone about to run the numbers on SRM economics, or is it ghost-writing?"

### 5. srm-forever (SRM Cost Dynamics Model)
- **Repo:** [hausfath/srm-forever](https://github.com/hausfath/srm-forever)
- **Stars:** 0 | **Language:** Julia | **License:** MIT
- **Last commit:** August 26, 2026
- **Focus:** Interactive cost dynamics model for solar radiation management. Applies **Weitzman certainty-equivalent discounting** to SRM cost trajectories.
- **Why it matters for SRM:** This addresses the deepest theoretical question in SRM: *What does it cost to keep blocking sunlight forever?* The Weitzman framework accounts for uncertainty and catastrophic risk — the kind of thinking that should underpin any serious SRM deployment analysis.
- **Commit signal:** 4 recent commits. Small but focused development.
- **🎙️ Episode hook:** *"Zero stars, but conceptually this is the most important repo you've never heard of. It asks: what's the price of never turning off the dimmer switch?"

---

## Tier 3 — Adjacent Tools (Not SRM-Specific but Essential)

| Repo | Stars | Relevance |
|------|-------|----------|
| [NREL/SolTrace](https://github.com/NREL/SolTrace) | — | Concentrating solar power optical modeling — not SRM, but shows how solar radiation is modeled in engineering contexts |
| [sunpy/sunpy](https://github.com/sunpy/sunpy) | — | Solar physics (the actual star, not geoengineering) — useful for understanding solar irradiance variability |
| [PCMDI/pcmdi_mmips](https://github.com/PCMDI/pcmdi_mmips) | — | Anomaly diagnostics complement — part of the PCMDI ecosystem |

---

## 🔍 What's Missing in Solar SRM on GitHub

Despite thorough searching, we found **no dedicated marine cloud brightening (MCB) repositories**, **no open-source stratospheric aerosol injection (SAI) simulation tools**, and **no circle molecule Chem model repositories** specifically for SRM. The solar geoengineering software ecosystem is remarkably thin — dominated by atmospheric models that *could* be used for SRM but weren't built for it.

**This is the story:** SRM exists in the physics models, not in dedicated tools. The gap between "we can simulate climate" and "we can simulate geoengineering" is where the podcast should live.

---

## 📊 Commit Activity Summary (Solar Theme)

| Repo | Recent Commits | Velocity | Pattern |
|------|---------------|----------|---------|
| WRF | 10 (v4.8.0) | High | Institutional, steady, solar radiation fixes |
| PCMDI | 10 in 2 days | Burst | Rapid release cycle, institutional |
| MDTF | 5 (precip-buoyancy POD) | Moderate | Process-focused, targeted |
| ClimateMARGO | 2 (README only) | Dormant revival | Ambiguous signal |
| srm-forever | 4 | Low but steady | Theoretical, focused |

---

## 🎙️ Recommended Episode Structure — Solar Geoengineering

1. **Cold open:** What does WRF have to do with solar geoengineering?
2. **Act 1:** The physics — how climate models handle solar radiation (WRF, PCMDI)
3. **Act 2:** The evaluation problem — how do we know if SRM modeling is any good? (PCMDI metrics, MDTF)
4. **Act 3:** The economics — what does it cost to keep blocking sun forever? (srm-forever, Weitzman)
5. **Act 4:** The gap — why is there no dedicated SRM software?
6. **Close:** The marine cloud brightening vacuum and what it means for governance

---

*Generated from GitHub API commit data pulled September 2026.*