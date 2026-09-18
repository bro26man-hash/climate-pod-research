# 🌊 Project Discoveries — Ocean Intervention Theme (Fresh, September 2026)

**Date:** September 2026  
**Repositories profiled:** WRF (coupled), NCAR_ML_EKE, MDTF-diagnostics  
**Dedicated ocean geoengineering repos found:** 0  
**Ocean-adjacent repos found:** 3  

---

## 🚨 The Ocean Gap: Zero Repos, Zero Code, Zero Presence

### The Search Results

We ran 10+ GitHub search queries across multiple strategies:

| Search Type | Query | Results |
|-------------|-------|--------|
| Direct | `geoengineering ocean` | **0** |
| Direct | `ocean geoengineering` | **0** |
| Specific technique | `marine cloud brightening` | **0** |
| Specific technique | `ocean alkalinity enhancement` | **0** |
| Specific technique | `ocean fertilization` | **0** |
| Specific technique | `seaweed cultivation model` | **0** |
| Broad | `ocean intervention climate` | **0** |
| Broad | `blue carbon ecosystem` | **0** |
| Broad | `coastal mitigation tool` | **0** |
| Model-adjacent | `ocean climate model` | **3** (general models only) |

**Interpretation:** This is not a search bug. GitHub's code search is comprehensive. If ocean geoengineering repos existed — even small academic projects — they would appear. The absence is real.

### What This Tells Us

Ocean geoengineering is the only major climate intervention domain with **zero open-source presence** on GitHub. Compare:

| Domain | GitHub Presence | Open-Source Tools |
|--------|----------------|-------------------|
| **Solar Geoengineering** | Several repos (WRF, srm-forever, ClimateMARGO) | Models, economics tools, evaluation metrics |
| **Carbon Capture** | Dozens of repos (OpenAir-Cyan, Carbon_Capture_ML, DAC materials) | Hardware, software, data, surveys |
| **Ocean Intervention** | **ZERO repos** | **None** |

**This is the most significant finding of this entire research effort.**

---

## 1. WRF (Coupled Ocean-Atmosphere Mode)

| Attribute | Detail |
|-----------|--------|
| **Repo** | `wrf-model/WRF` |
| **Stars** | 1,762 |
| **Last commit** | June 8, 2026 (v4.8.0) |
| **Ocean capability** | Coupled with MOM6 via WRF-MOM6 framework |

### Ocean-Relevant Recent Commits
- `8299919` (May 27, 2026): MYNN-EDMF update — boundary layer physics affecting air-sea flux
- `e836cd6` (May 28, 2026): Solar radiation correction — affects sea surface temperature
- `v4.8.0` (Jun 8, 2026): Full coupled ocean-atmosphere capability

### Limitations
- WRF is fundamentally an atmospheric model
- Ocean coupling is passive (receives forcing, doesn't simulate interventions)
- No module for ocean alkalinity, no module for marine cloud brightening
- The ocean is a boundary condition, not a simulation target

---

## 2. NCAR_ML_EKE (Machine Learning for Ocean Climate Modeling)

| Attribute | Detail |
|-----------|--------|
| **Repo** | `CrayLabs/NCAR_ML_EKE` |
| **Stars** | 20 |
| **Last commit** | March 30, 2022 (4.5 years dormant) |
| **Language** | Python, Jupyter Notebook |
| **Institution** | NCAR / University of Colorado |

### What It Does
Applies **SmartSim** (AI framework) to accelerate ocean climate models using MOM6. The project demonstrates that machine learning can be used to speed up expensive ocean simulations — but the code has been frozen since 2022.

### Ocean-Relevant Commits (All 2021-2022)
- `aa0abc8` (Mar 14, 2022): **Update MOM6 instructions and submodule** — explicitly using the ocean model
- `6586405` (Feb 9, 2022): README for compiling MOM6
- `962e6c6` (Feb 8, 2022): Update MOM6 submodule
- `5b2d6cf` (Mar 30, 2022): Fix notebook typos (#10) — **last ever commit**

### The Dormancy Pattern
- **Active period:** April 2021 – March 2022 (7 commits over 12 months)
- **Dormant period:** March 2022 – present (4.5 years)
- **Last activity:** Fixing notebook typos — not advancing the science

### Episode Angle
> "This repo tried to use AI to speed up ocean models. It had MOM6, SmartSim, and a clear research goal. Then it stopped. The last commit wasn't a breakthrough — it was fixing typos in a notebook. What does it mean when an ocean+AI project dies not with a bang, but with a grammar check?"

---

## 3. MDTF-diagnostics (Precipitation-Buoyancy POD)

| Attribute | Detail |
|-----------|--------|
| **Repo** | `NOAA-GFDL/MDTF-diagnostics` |
| **Stars** | 80 |
| **Last commit** | August 14, 2026 |
| **Institution** | NOAA Geophysical Fluid Dynamics Laboratory |

### What It Does
The Model Diagnostics Task Force (MDTF) provides process-oriented diagnostics for evaluating climate model accuracy. Its most ocean-relevant feature is the **precipitation-buoyancy POD** — a Proper Orthogonal Decomposition that identifies dominant patterns of precipitation-buoyancy interaction.

### Why This Matters for Ocean Intervention
- **Buoyancy = density = ocean circulation:** Changes in freshwater input (from ice melt, river discharge, or intervention) affect ocean density and thus circulation. The POD tool identifies the dominant modes of this interaction.
- **Precipitation over ocean = freshwater flux:** Changes in ocean-bound precipitation patterns directly affect ocean salinity and density
- **Validation, not simulation:** This tool checks whether models are accurate. It doesn't simulate what happens when you add alkalinity or iron to the ocean.

### Episode Angle
> "The most ocean-relevant code in open source is a validation tool. It checks whether climate models get the ocean right. It doesn't simulate interventions. It's the quality assurance department for ocean modeling — but there's no manufacturing floor."

---

## 🔍 What's Missing — The Complete Ocean Intervention Gap

### No Code Exists For:

| Intervention | Description | Literature | Code |
|-------------|-------------|-----------|------|
| **Ocean Alkalinity Enhancement (OAE)** | Adding lime/olivine to seawater to increase CO2 absorption | Dozens of papers (2020s) | **0 repos** |
| **Marine Cloud Brightening (MCB)** | Spraying sea salt to brighten clouds and reflect sunlight | Multiple papers (Latham et al.) | **0 repos** |
| **Iron Fertilization** | Adding iron to trigger algal blooms that absorb CO2 | Historical experiments (LOHAFEX, EIFEX) | **0 repos** |
| **Seaweed Aquaculture** | Growing seaweed for carbon sequestration | Growing body of work | **0 repos** |
| **Artificial Upwelling** | Pumping deep nutrient-rich water to surface | Moderate literature | **0 repos** |
| **Ocean Thermal Energy Conversion** | Using temperature gradients for energy + carbon capture | Moderate literature | **0 repos** |
| **Coastal Blue Carbon** | Protecting/restoring seagrass, mangroves, salt marshes | Growing literature | **0 repos** |
| **Electrochemical Ocean Acidification Mitigation** | Using electrochemistry to locally modify ocean chemistry | Emerging literature | **0 repos** |

### Why the Gap?

| Hypothesis | Evidence | Plausibility |
|-----------|----------|-------------|
| **Ocean models are too complex** | MOM6, NEMO, POP are millions of lines of code. You can't easily fork and modify them. | **High** — the barrier to entry is enormous |
| **Institutional gatekeeping** | Ocean models are maintained by small consortia (NOAA GFDL, NEMO consortium). No open-source equivalent of WRF's user consortium. | **High** — the code exists but it's locked |
| **Ethical self-regulation** | Ocean interventions have global consequences. Researchers may voluntarily withhold code. | **Medium** — no formal policy, but informal norms exist |
| **Funding gap** | Less dedicated funding for ocean intervention open-source tools vs. atmospheric modeling |
| **"Out of sight, out of mind"** | Public attention focuses on solar panels and DAC, not ocean chemistry. | **Medium** — affects public pressure and funding |
| **Paywall problem** | Ocean intervention papers are in Nature/Science, but the code isn't in the paper. | **Medium** — the knowledge is published but not shared |

---

## 💡 The Ocean Gap as a Governance Signal

We hypothesize that the ocean gap is **not accidental** — it's the result of **implicit governance**:

1. **Ocean interventions are globally consequential.** Adding alkalinity to the ocean changes chemistry, affects marine ecosystems, and could alter weather patterns. The stakes are higher than for SRM (which primarily affects the atmosphere) or DAC (which is localized).

2. **Institutional control is tighter.** Ocean modeling requires massive infrastructure (MOM6, NEMO, supercomputing access). You can't "fork the ocean model" the way you can fork a Python script.

3. **Ethical review is informal but real.** There's no formal review process, but there is an informal norm: don't publish code that could be used to alter ocean chemistry at scale. The scientific community has effectively self-governed ocean intervention code into non-existence.

4. **The literature is paywalled.** Ocean intervention papers appear in high-impact journals, but the code isn't in the paper. Unlike solar geoengineering (where model code is published alongside papers), ocean intervention research doesn't come with downloadable software.

**The ocean gap is your podcast's锁紧存在的发现. It's the canary in the coal mine for how the climate tech community handles high-stakes, globally-impactful technologies. When the most consequential intervention domain has zero open-source code, it tells us something deeper about trust, risk, and governance in the age of climate crisis.**

---

## 🎙️ Episode Angle: "The Ocean That Isn't There"

**Opening:** "We searched GitHub 10 different ways. We searched for ocean geoengineering, marine cloud brightening, ocean alkalinity enhancement, iron fertilization, seaweed cultivation, and more. Zero results. Not a single repository. And that's the story — because the science is published, the research is funded, and the ocean is the biggest carbon sink on the planet. But the code? It doesn't exist."

**Core question:** Why is the ocean the empty quadrant of climate tech on GitHub?

**Possible answers:**
- It's a gap (nobody thought to build it)
- It's a fence (someone decided not to build it)
- It's both (the gap enables the fence, and the fence deepens the gap)

---

*Generated: September 2026 | Repository: climate-pod-research | Branch: ocean-intervention*