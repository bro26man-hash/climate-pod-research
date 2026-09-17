# 🌊 Ocean Intervention — Cross-Reference: Solar & Carbon Repositories

**Date:** September 2026
**Purpose:** Compare how solar and carbon communities handle governance, and what the ocean community could learn

---

## Governance Comparison

| Aspect | Solar Geoengineering | Carbon Capture | Ocean Intervention |
|--------|---------------------|----------------|-------------------|
| **Modeling tools** | WRF (atmospheric), ClimateMARGO (economic) | None (climate-capture-and-storage is dead) | None |
| **Evaluation metrics** | PCMDI metrics (v4.2.1, actively maintained) | None | None |
| **Curated lists** | awesome-geoengineering (v2.0.0, monthly updates) | None | None |
| **Economics models** | srm-forever (interactive, Aug 2026) | None | None |
| **DIY/community** | None | OpenAir-Cyan (OSHWA-certified, frozen) | None |
| **Interactive tools** | orbital-climate-simulator, srm-forever | None | None |
| **Regulatory tools** | None (London Protocol mentioned in literature only) | None (no regulatory repos) | None (London Protocol mentioned in literature only) |

**Key insight:** Even the weakest quadrant (carbon capture) has something the ocean doesn't: a DIY hardware community and an ML survey. The ocean has zero of everything.

---

## What Solar Has That Ocean Needs

### 1. PCMDI Metrics — Governance Infrastructure
PCMDI's carbon-copy of governance: active development, institutional backing, regular releases. The ocean has no equivalent. An "OceanCAMI" (Ocean Carbon Assessment Metrics) would be the first governance infrastructure for ocean geoengineering.

### 2. ClimateMARGO — Economic Optimization with Geoengineering
ClimateMARGO explicitly includes geoengineering as a policy variable. No economic model exists for ocean intervention costs, feasibility, or optimization. A "OceanMARGO" module for alkalinity enhancement costs would be a starting point.

### 3. Awesome-Geoengineering — Curation Layer
The curated list exists for solar geoengineering. There's no equivalent for ocean. An "awesome-ocean-geoengineering" list would be the lowest-barrier entry point — just a Markdown file with links.

---

## What Carbon Has That Ocean Needs

### 1. OpenAir-Cyan — DIY Hardware (Frozen but Existed)
The fact that a DIY community existed for carbon capture, even briefly, shows that the hardware barrier is lower than expected. An open-source OAE monitoring kit (pH sensors, alkalinity titration protocols) could be the ocean equivalent.

### 2. Carbon_Capture_ML — Survey/Mapping Layer
A comprehensive survey of ML for carbon capture. A "Ocean_GeoeniML" survey of machine learning for ocean intervention would serve the same mapping function.

---

## The Missing Bridge: From Ocean Science to Ocean Geoengineering

The gap isn't just missing geoengineering code. It's missing *bridges* between ocean science and geoengineering:

```
Ocean Science (、海洋科学)          Ocean Geoengineering (海洋地球工程)
                                   \
  Oceananigans.jl ——→???——→    Alkalinity tracer module
  OceanBioME.jl ——→???——→    Ecological impact module
  MDTF-diagnostics ——→???——→  Geoengineering evaluation metrics
  veros ——→???——→            OAE simulation module
                                   /
Ocean Science  ←——— bridge ——→  Ocean Geoeniengineering
```

The bridges (modules, plugins, extensions) don't exist. The ocean science community builds general-purpose tools. The geoengineering community doesn't exist on GitHub. Nobody is building the bridges.

---

## Recommendations for the Episode

1. **"Start with curation"** — Before any code, create `awesome-ocean-geoengineering`. It's a Markdown file. Anyone can do it. It's the first building block.

2. **"The Oceananigans plugin angle"** — A single PR adding an alkalinity tracer to Oceananigans would be the first geoengineering module in any ocean model. It's achievable by one person, one summer.

3. **"Build the governance layer first"** — Solar geoengineering has PCMDI metrics. Ocean geoengineering needs "OceanCAMI" — an evaluation framework before a simulation framework.

4. **"The ocean gap is the canary in the coal mine"** — If ocean geoengineering is ever considered, the absence of code means there's no publicly accessible model to evaluate the proposal. The science would be trust-based, not code-based. That's a reproducibility crisis for geoengineering.

---

*Cross-reference analysis conducted September 2026 for the Climate Technology & Geoengineering podcast series.*