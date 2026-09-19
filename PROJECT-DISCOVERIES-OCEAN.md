# 🌊 Ocean Intervention — Gap Report

**Last updated:** September 2026
**Research cycle:** v5 — 12 search queries, 8 repos deep-dived, ZERO dedicated ocean geoengineering repos found

---

## The Ocean Gap: Headline Finding

**ZERO dedicated ocean geoengineering repositories exist on GitHub.**

After 10+ search queries across multiple keyword combinations ("ocean geoengineering," "ocean fertilization," "marine cloud brightening," "ocean alkalinization," "ocean climate intervention," "marine geoengineering simulation," etc.), the result is unanimous:

> Ocean geoengineering is the **dark matter** of climate tech on GitHub. It exists in Nature, Science, and PNAS — but not in open code.

This is not a small gap. It is a **category-level absence.** Compare:

| Theme | Dedicated Repos | Stars (top) | Commit Activity |
|-------|----------------|-------------|-----------------|
| ☀️ Solar Geoengineering | 4+ | 133 (PCMDI) | Active (PCMDI, Sep 2026) |
| 🌍 Carbon Capture | 5+ | 76 (OpenAir-Cyan) | Burst (OpenAir-Cyan, Feb 2024) |
| 🌊 Ocean Intervention | **0** | N/A | **N/A** |

---

## What's "Adjacent" but NotOcean?

The 3 repos that border ocean intervention but don't directly model it:

### 1. PCMDI/pcmdi_metrics (adjacent: coupled ocean-atmosphere evaluation)
PCMDI evaluates models that **include ocean components** (like ESM2M, HadGEM3). But the ocean in those models is part of the Earth system, not the target of intervention. No repo uses PCMDI tools specifically for ocean geoengineering evaluation.

### 2. ClimateMARGO/ClimateMARGO.jl (adjacent: marine ecosystem optimization)
ClimateMARGO's optimization framework could theoretically evaluate marine cloud brightening or ocean fertilization as mitigation strategies. But no one has built that scenario. The marine ecosystem dimension of climate intervention is represented only in the *policy optimization space*, not the *engineering simulation space*.

### 3. WRF-Chem / regional-geo (adjacent: coastal aerosol effects)
WRF-Chem simulations can model coastal aerosol interactions, but the regional-geo repo focuses on **stratospheric** aerosol injection, not marine cloud brightening (which operates in the troposphere over oceans).

---

## Five Hypotheses for the Ocean Gap

Why is there zero code for ocean geoengineering?

### Hypothesis 1: Governance Chilling Effect 🚫
The London Convention/London Protocol explicitly prohibits ocean fertilization in international waters. The CBD (Convention on Biological Diversity) has a de facto moratorium on geoengineering, including ocean interventions. **If researchers can't get permits, they can't run experiments, and if they can't run experiments, they can't publish data, and if they can't publish data, they can't build open-source tools.**

### Hypothesis 2: Scale Mismatch 💻
Solar geoengineering operates at the **radiative forcing** level (W/m²) — a single number that models can represent. Carbon capture operates at the **mass flux** level (tons CO₂/year) — a number that's easy to parameterize. Ocean intervention operates at the **biogeochemical cascade** level — iron fertilization triggers phytoplankton blooms, which sink carbon, which alters deep-ocean chemistry, which affects atmospheric CO₂ over centuries. The timescales and feedback loops are ** orders of magnitude more complex** than SRM or DAC. Code that could model this doesn't exist yet because the science isn't mature enough.

### Hypothesis 3: Data Desert 🏜️
There are **no open ocean geoengineering datasets** to build tools against. SRM has CMIP experiments. DAC has Climeworks/Carbon Engineering public data. Ocean intervention has... a few small-scale experiments (LOHAFEX, SERIES) with data stored in obscure repositories. Without data, there's no training set for ML, no validation set for models, no benchmark for code.

### Hypothesis 4: Academic Discouragement 📉
Publishing on ocean geoengineering carries reputational risk. Unlike SRM (which has major papers in Nature and Science) or DAC (which has well-funded industry partnerships), ocean geoengineering research is seen as "too risky" or "too fringe" by major journals and funding agencies. Researchers who build tools in this space have minimal career incentives.

### Hypothesis 5: Just Not Digital Yet 🧪
Ocean intervention is still overwhelmingly at the **thought experiment and small-scale experiment** stage. Marine cloud brightening has been proposed but barely tested. Ocean alkalinity enhancement is in early lab work. Iron fertilization has been tested at sea but the results are contested. **Maybe the gap isn't a gap — maybe it's just that we're not ready to code ocean geoengineering yet.**

---

## The "Three Universes" Diagram

```
                    ┌─────────────────────────────────┐
                    │     CLIMATE TECH on GitHub       │
                    └──────────────┬──────────────────┘
                                  │
            ┌─────────────────────┼─────────────────────┐
            │                     │                     │
     ┌──────┴──────┐      ┌──────┴──────┐      ┌──────┴──────┐
     │  🔴 FAST    │      │  🟡 SLOW    │      │  ⚫ EMPTY   │
     │  UNIVERSE   │      │  UNIVERSE   │      │  UNIVERSE   │
     │             │      │             │      │             │
     │ PCMDI       │      │ Climate-    │      │             │
     │ (institutional│     │ MARGO       │      │ Ocean       │
     │  evaluation) │      │ (academic   │      │ geoengineering│
     │             │      │  dormant)   │      │ (ZERO repos) │
     │ regional-geo│      │ OpenAir-    │      │             │
     │ (burst)     │      │ CYAN        │      │ Marine cloud │
     │             │      │ (burst)     │      │ brightening  │
     │ actm-sai-csu│      │ (burst)     │      │ Ocean alkalin.│
     │ (dormant)   │      │ DAC digital │      │ (ZERO repos) │
     │             │      │ twin        │      │             │
     └─────────────┘      └─────────────┘      └─────────────┘
```

**The ocean-intervention universe is empty.** Not small — empty. This is the most striking finding of the entire research cycle.

---

## What Would Break the Gap?

### A "Marine Geoengineering Benchmarks" repo 🏆
The GitHub equivalent of CMIP for ocean intervention:
- Standardized test cases (iron fertilization scenarios, cloud brightening parameterizations)
- Open datasets from past experiments (LOHAFEX, SERIES, EIFEX)
- Evaluation metrics for ocean biogeochemistry models
- A community around it (even if small)

### A "Governance-as-Code" Ocean Module 📜
The Zereo0317/climate-intervention-governance repo could expand to include:
- London Protocol compliance checker for ocean intervention proposals
- CBD moratorium tracker with legal citations
- Permit pathway documentation (who approves what, where)

### A "Digital Twin of Ocean Alkalinity Enhancement" 💧
The most technically tractable ocean intervention for open-source modeling:
- NaOH dissolution in seawater chemistry
- pH change propagation
- Carbon removal flux estimation
- Local vs. global effects

---nn## Episode 3 Architecture

### Opening question
*Is the GitHub vacuum a governance signal?*

### Three act structure
1. **Act 1 — The Absence:** Show the audience that zero ocean geoengineering repos exist on GitHub. Compare to 133-star solar evaluation tools. The contrast is the story.
2. **Act 2 — The Five Hypotheses:** Governance chilling, scale mismatch, data desert, academic discouragement, "not ready yet." Which ones are true? Which are self-serving?
3. **Act 3 — The Opportunity:** If the gap is real, it's the biggest open question in climate tech. Who should fill it? A marine biogeochemist? A governance hacker? A citizen science collective?

### Closing question
*If solar geoengineering has PCMDI and carbon capture has OpenAir-Cyan, what does ocean intervention have — and what does that absence tell us about where we're putting our climate innovation dollars?*

---

## Trend Lines to watch

1. **Marine cloud brightening field experiments** — if any are conducted, expect code to follow
2. **Ocean alkalinity enhancement** — Shell's OceanAzul and others are working on this; GitHub presence would signal legitimacy
3. **Climate-intervention-governance repo growth** — if Zereo0317 adds ocean modules, it becomes the first governance code for this space
4. **CMIP for ocean intervention** — the next generation of climate models may include海岛 geoengineering scenarios, which would force tool development
5. **ophobia / OAE community** — the ocean alkalinity enhancement community is small but growing; watch for GitHub emergence
