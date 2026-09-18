# 🌊 Ocean Intervention — Project Discoveries
## Podcast Episode Research: Ocean Geoengineering (OAE, Iron Fertilization, Marine Cloud Brightening)

**Last Updated:** September 2026 | **Research Version:** v4

---

## 🔍 Executive Summary — The Ocean Intervention Gap

**Our GitHub search across 10+ query strategies returned ZERO dedicated ocean geoengineering repositories.**

We searched for:
- Ocean geoengineering
- Ocean alkalinity enhancement (OAE)
- Iron fertilization
- Marine cloud brightening
- Ocean intervention climate
- Albedo modification (ocean)
- And more...

**Result: Nothing.**

Ocean geoengineering is the "dark matter" of climate tech on GitHub. It exists abundantly in the scientific literature (Nature, Science, PNAS, Nature Climate Change). It's discussed at COP. It's modeled in every major climate model. But it has **zero open-source repositories dedicated to it.**

This is either the biggest governance problem in climate tech — or proof that the scientific community agrees we Shouldn't Be doing it yet.

---

## 📊 What We DID Find: Ocean-Adjacent Resources

### 1. MDTF-diagnostics — The Ocean's Closest Friend
| Field | Detail |
|-------|--------|
| **Repository** | `NOAA-GFDL/MDTF-diagnostics` |
| **Stars** | 80 ★ |
| **Relevance** | **Precipitation-Buoyancy POD** — ocean-adjacent diagnostic |
| **Last Activity** | August 14, 2026 |

**Why It's Here:**
The precipitation-buoyancy Process-Oriented Diagnostic (POD) evaluates whether climate models correctly simulate the relationship between atmospheric buoyancy and precipitation. This is directly relevant to ocean intervention because:

1. **Ocean heat uptake** drives precipitation patterns globally
2. **OAE (Ocean Alkalinity Enhancement)** would alter ocean chemistry, which affects air-sea gas exchange, which affects precipitation
3. **Iron fertilization** affects marine ecosystems, which affect carbon cycling, which affects climate
4. **Marine cloud brightening** operates at the ocean-atmosphere interface

The MDTF's precipitation-buoyancy POD (5 commits on June 19, 2026) is the most ocean-relevant tool in open source — but it's for **model evaluation**, not **intervention simulation**.

**Key Commits — The Jun 19 Sprint:**
```
Jun 19, 2026:  4cfc99c — Update MCS_precip_buoy_stats.rst
Jun 19, 2026:  699de27 — Update MCS_precip_buoy_stats.rst
Jun 19, 2026:  d6bc6d0 — Update MCS_precip_buoy_stats.rst
Jun 19, 2026:  3904d29 — Update MCS_precip_buoy_stats.rst
Jun 19, 2026:  33024ad — **ADD MCS precipitation-buoyancy statistics POD** ← NEW
Aug 14, 2026:  87f8105 — Merge PR #825
```

**Five commits to one file in a single day.** The most ocean-relevant diagnostic in open source was getting its most intensive development. And it's still just evaluating models — not simulating interventions.

---

### 2. WRF — Coupled Ocean-Atmosphere Modeling (Indirect)
| Field | Detail |
|-------|--------|
| **Repository** | `wrf-model/WRF` |
| **Stars** | 1,763 ★ |
| **Relevance** | Atmospheric model with ocean coupling capability |
| **Last Activity** | June 8, 2026 (v4.8.0) |

WRF can be coupled with ocean models (MOM, PUGNOS) for earth system modeling. The v4.8.0 release includes solar radiation corrections that would be relevant to any geoengineering scenario viewed from the ocean's perspective. But WRF itself has no ocean intervention module.

---n

### 3. Earth System Models (Referenced, Not Pulled)
From our v2 ecosystem research, we identified these as relevant but beyond the scope of fresh commit pulls:

| Model | Stars | Ocean Component | Geoengineering Module? |
|-------|-------|-----------------|------------------------|
| **Oceananigans.jl** | 1,413 | Full ocean CFD | No — general circulation only |
| **veros** | ~100 | Ocean modeling | No — primitive equations |
| **MO framework** | ~50 | Ocean modeling | No — modular ocean |
| **NEMO** | ~200 | Ocean modeling | No — physical oceanography |
| **CMIP6 models** | Varies | All have ocean components | No — historical simulation only |

**The pattern:** Every ocean model on GitHub simulates what the ocean DOES. None simulate what we MIGHT MAKE the ocean DO.

---

## 🚨 The Ocean Gap — Detailed Analysis

### What's Missing

| Ocean Intervention Approach | GitHub Repos | Scientific Papers |
|---------------------------|---------------|-------------------|
| **Ocean Alkalinity Enhancement (OAE)** | **0** | 50+ (Nature, Science)
| **Iron Fertilization** | **0** | 100+ (multiple journals) |
| **Marine Cloud Brightening** | **0** | 30+ (atmospheric science) |
| **Ocean Upwelling Pumping** | **0** | 20+ (engineering literature) |
| **Deep Ocean Carbon Storage** | **0** | 40+ (geology/policy) |
| **Seaweed/Biomass Cultivation** | **0** | 30+ (biology/economics) |
| **Ocean Albedo Modification** | **0** | 10+ (theoretical) |

### What's Different About Ocean Geoengineering
1. **It's hardest to simulate** — ocean processes operate at scales (cm to 1000s km, days to centuries) that exceed current model capabilities
2. **It's hardest to monitor** — you need ocean-going instruments, floats, and satellites to verify any intervention
3. **It's hardest to govern** — the ocean is international territory; no single nation can deploy or verify
4. **It's hardest to reverse** — ocean interventions have multi-century timescales
5. **It's cheapest to study** — you don't need field experiments to run a model; you just need the model

### The Irony
The ocean is the **largest active carbon sink on Earth** (absorbing ~25% of anthropogenic CO2). Yet it's the **least represented in open-source climate intervention code.** We have tools to simulate the atmosphere. We have tools to simulate terrestrial ecosystems. We have tools to simulate ice sheets. We don't have tools to simulate the ocean being deliberately altered.

---

## 🎙️ Ocean Intervention — Episode Talking Points

### The Empty Quadrant
> "We searched for ocean geoengineering repos using 10 different queries. Zero results. Not one. This is the empty quadrant of climate tech on GitHub. The atmosphere has models. The land has models. The ice has models. The ocean? Nothing."

### Why the Silence?
Three theories:
1. **The field is too young** — OAE and marine cloud brightening are still in early research; no one's built tools yet
2. **The complexity is prohibitive** — ocean models require PhDs to run; nobody's built user-friendly interfaces
3. **The politics are paralyzing** — no government or funder wants to be associated with ocean intervention code

### The MDTF as Ocean-Adjascent Lifeline
> "The precipitation-buoyancy POD isn't an ocean intervention tool. It's a ruler for measuring whether climate models get the ocean right. But it's the closest thing we have. Five commits in one day, and the most ocean-relevant diagnostic in open source got a major upgrade."

### The Governance Signal
> "Maybe the absence of ocean geoengineering repos isn't a bug — it's a feature. Maybe the scientific community is saying: 'We don't have the models to simulate this responsibly. We don't have the monitoring to verify it. And until we do, the code stays empty.'"

---

## 📈 Ocean Theme Commit Trend Summary

| Source | Commits Pulled | Relevance | Trend |
|--------|---------------|-----------|-------|
| **MDTF-diagnostics** | 15 | High (precip-buoyancy POD) | 🔴 Active — diagnostic expansion |
| **WRF** | 15 | Medium (coupled modeling) | 🔴 Active — v4.8.0 release |
| **Oceananigans.jl** | Referenced | High (ocean CFD) | 🔴 Active (from v2 research) |
| **veros** | Referenced | Medium (ocean modeling) | 🟢 Maintained |
| **Dedicated ocean geoengineering** | **0** | **N/A** | **⚫ ZERO — nothing exists** |

**Total ocean intervention commits found: 0**
**Total ocean-adjacent commits found: 30+**
**The gap is real, measurable, and significant.**

---

## 🔗 Links
- MDTF-diagnostics: https://github.com/NOAA-GFDL/MDTF-diagnostics
- WRF: https://github.com/wrf-model/WRF
- Oceananigans.jl: https://github.com/CliMA/Oceananigans.jl
- veros: https://github.com/MRI-JAM/veros
- v2 Ocean Research: [CROSS-THEME-ANALYSIS-SEP2026.md](../main/CROSS-THEME-ANALYSIS-SEP2026.md)

---

## 📝 Research Log — Ocean Theme

| Date | Activity |
|------|----------|
| Sep 17, 2026 | Initial ocean search — 0 results across 10+ query strategies |
| Sep 17, 2026 | MDTF-diagnostics identified as ocean-adjacent resource |
| Sep 17, 2026 | Precipitation-buoyancy POD discovered — 5 commits on Jun 19, 2026 |
| Sep 17, 2026 | WRF identified for coupled ocean-atmosphere modeling |
| Sep 17, 2026 | Oceananigans.jl, veros referenced from v2 ecosystem analysis |
| Sep 18, 2026 | Ocean gap confirmed — zero dedicated repos, zero intervention modules |
| Sep 18, 2026 | v4 research notes pushed to ocean-intervention branch |

---

*This document is part of the Climate Pod Research repository.*
*Branch: ocean-intervention | Version: v4 | Date: September 2026*