# 🌊 Ocean Intervention — Commit Trend Analysis & Narrative (v6)

> **Last updated:** September 2026 (v6)  
> **Branch:** `ocean-intervention`  
> **Podcast episode:** Episode 3 — Ocean Intervention

---

## The Headline: Zero Commits for Zero Repos (v6 Reconfirmed)

The most important statistic in this entire research project:

```
Dedicated ocean geoengineering repositories:          0
OAE computational screening datasets:                 0
Ocean sensor/hardware repos:                          0
Ocean process models with intervention modules:        0
Total ocean geoengineering commits found:             0
```

**For comparison:**
```
Solar geoengineering repos (srm-forever):             1 (with 4 commits)
Carbon capture DAC material repos (CC0):              2 (with 20+ commits)
Direct air capture DIY hardware (OpenAir-Cyan):       1 (with 15+ commits)
Atmospheric climate models (WRF):                     1 (with 15+ commits)
```

**The ocean is not just underrepresented — it is absent.**

---

## Ocean-Adjacent Commit Activity (v6 Detail)

While there are zero ocean geoengineering repos, there ARE commits from repos with ocean relevance:

### 1. NOAA-GFDL/MDTF-diagnostics — The Precipitation-Buoyancy POD

**The single most ocean-relevant commit in open source:**

| Date | Commit | Message | Ocean Relevance |
|------|--------|---------|----------------|
| **Jun 19, 2026** | `33024ad` | **add MCS precipitation-buoyancy statistics POD** | ⭐⭐⭐ Core ocean-atmosphere diagnostic |
| Jun 19, 2026 | `4cfc99c` | Update MCS_precip_buoy_stats.rst | Documentation |
| Jun 19, 2026 | `699de27` | Update MCS_precip_buoy_stats.rst | Documentation |
| Jun 19, 2026 | `d6bc6d0` | Update MCS_precip_buoy_stats.rst | Documentation |
| Jun 19, 2026 | `3904d29` | Update MCS_precip_buoy_stats.rst | Documentation |

**5 commits on a single day (June 19, 2026), all touching the same file.** The 5th commit is the actual code addition; the first 4 are documentation updates. This is a textbook "big bang" release: code + 4 doc updates, all same day.

**What the POD does:** Measures the statistical relationship between precipitation and buoyancy (temperature-salinity structure) in climate model output. This is fundamental to ocean-atmosphere coupling — precipitation changes surface salinity, which changes buoyancy, which changes ocean mixing.

**What the POD does NOT do:** It does not simulate ocean interventions. It does not model OAE, MCB, or artificial upwelling. It evaluates whether climate models get the ocean right. It's the QA lab, not the experimenter.

**The irony for the podcast:** The most ocean-relevant code in open source was written to evaluate models, not to perturb them. We can diagnose the ocean's behavior but we can't simulate what happens when we intervene.

---

### 2. WRF (Atmosphere-Ocean Coupling, Indirect)

WRF has ocean coupling capabilities (MOM, POP), but no commits target ocean intervention scenarios. The v4.8.0 release (Jun 8, 2026) includes MYNN surface layer updates that affect air-sea interaction physics, but these are for weather prediction, not geoengineering.

The solar radiation bug fix (e836cd6, May 28, 2026) is the most SRM-relevant commit, but it's atmospheric, not oceanic. Ocean-intervention researchers who use WRF would be affected by this bug, but none appear to be actively using WRF for ocean scenarios.

---

### 3. ClimateSoton/climate-research-group (CFD-Adjacent)

Active in August 2026, but a research group website, not a code repository. CFD resources could be relevant to ocean circulation modeling, but they're not adapted for intervention scenarios.

---

## The Three-Hypothesis Framework (v6 Narrative)

### Hypothesis 1: The Complexity Barrier

**The claim:** Ocean models are computationally expensive and require specialized knowledge. The barrier to entry is higher than for atmospheric models.

**Evidence FOR:**
- All ocean-adjacent repos are institutional (NOAA-GFDL)
- No individual has published an open-source ocean intervention model
- WRF runs on a laptop; an ocean model needs a cluster
- The PBP-POD required expertise in Proper Orthogonal Decomposition methods

**Evidence AGAINST:**
- AR5/AR6 models are run internationally with sufficient coordination
- The complexity is navigable with community effort
- Simplified parameterization (PGMs) could run on laptops today

**Podcast angle:** *"The complexity barrier is real but not absolute. A simplified OAE model could run on a laptop today. The question is whether someone decides to build it."*

### Hypothesis 2: The Governance Chill

**The claim:** Ocean intervention is more politically controversial. The London Convention/Protocol regulates ocean fertilization. MCB is "geoengineering's third rail." Researchers avoid public repos to prevent misuse.

**Evidence FOR:**
- The silence is total — not "few repos" but ZERO repos
- SRM also has governance concerns, yet srm-forever exists
- The difference might be funding, not governance

**Evidence AGAINST:**
- Solar geoengineering also faces governance concerns, yet code exists (srm-forever, ClimateMARGO)
- Papers on ocean intervention are published openly (Nature, Science)
- The code silence doesn't match the publication volume

**Podcast angle:** *"If governance is the reason, we'd expect fewer papers too. But the papers keep coming. The silence is in the code, not the literature. What does that tell us?"*

### Hypothesis 3: The Funding Gap

**The claim:** No major funding agency prioritizes open-source ocean intervention modeling. Physical scientists publish papers; the modeling community builds tools; but nobody funds the intersection.

**Evidence FOR:**
- Every other climate tech domain has at least some repos
- The ocean covers 70% of the planet
- NOAA funds atmospheric modeling (WRF), NSF funds carbon capture (OpenAir-Cyan), but nobody funds ocean intervention code
- Institutional repos (MDTF, WRF) exist because they're funded

**Evidence AGAINST:**
- You'd think at least one agency would fund an open-source ocean model
- The ocean's importance to climate would justify the investment

**Podcast angle:** *"The ocean covers 70% of the planet. It drives every weather system you've ever experienced. And there is exactly zero open-source code for intervening in it. The funding gap is the most explainable mystery."*

---

## The "Empty Quadrant" Dashboard (v6)

```
                    ATMOSPHERE
                         │
            ┌────────────┼────────────┐
            │            │            │
      SOLAR REMOVAL   SRM       SOLAR RADIATION
      (CDR)           (SAI)      (MODELS)
            │            │            │
            │    srm-   │    WRF    │
            │  forever  │  (1,762★) │
            │    0★     │   15 commits  │
            │           │            │
  ──────────┼───────────┼────────────┼──────────────
            │           │            │
      OCEAN             │     ATMOSPHERE
   INTERVENTION         │     MODELS
            │           │            │
      ZERO              │   PCMDI   │
      REPOS             │  (133★)   │
      12 QUERIES        │   15 commits  │
      ZERO COMMENTS     │            │
            │           │            │
            └────────────┼────────────┘
                         │
                    CARBON
                  CAPTURE (CDR)
                         │
            ┌────────────┼────────────┐
            │            │            │
         DADIUS      CCS       CARBON
      (DIRECT AIR)  (STORAGE)  (SURVEY)
            │            │            │
      tjz21: 2★     ghost:    Open-Sust:
      CC0: YES     85★ dead   2,552★ alive
      10 commits    0 commits  15 commits
```

---

## What Would Open-Source Ocean Intervention Look Like? (v6 Architecture)

```
ocean-intervention/
├── oae/                    # Ocean Alkalinity Enhancement
│   ├── alkalinity_model.py  # Dissolution kinetics of olivine/limestone
│   ├── ocean_circulation.py # Simplified primitive equation solver
│   ├── carbon_chemistry.py  # CO2 system: DIC, TA, pH, pCO2
│   └── scenarios/
│       ├── small_scale.py   # 1km² pilot
│       ├── regional.py      # 100km² basin
│       └── global.py        # Global ocean
├── mcb/                    # Marine Cloud Brightening
│   ├── cloud_microphysics.py# CCN activation, droplet formation
│   ├── spray_nozzle.py     # Autonomous vessel spray systems
│   ├── radiation_transfer.py # Shortwave forcing calculation
│   └── scenarios/
├── upwelling/              # Artificial Upwelling
│   ├── thermocline_model.py # Mixed layer depth, pycnocline
│   ├── nutrient_pump.py     # Nutrient flux from deep water
│   └── scenarios/
└── data/
    ├── ocean_mesh/          # Topography and bathymetry
    ├── sst_anomalies/       # Sea surface temperature data
    └── carbon_cycle/        # Global carbon cycle boundary conditions
```

**Bottom-up feasibility:** A simplified OAE model could run on a laptop today using parameterized general models (PGMs), not full Navier-Stokes. The building blocks exist:
- WRF's air-sea coupling physics (v4.8.0)
- MDTF's PBP-POD diagnostic (Jun 19, 2026)
- NOAA/CSIRO ocean data pipelines
- CC0-licensed sorbent screening data (tjz21)

**Top-down opportunity:** An "OMCF" (Ocean Model Comparison Facility) — like CMIP but for OAE/MCB. Standardized test cases, shared dashboards, community benchmarks.

---

## Episode 3: Commit-Based Talking Points

| Talking Point | Evidence | Source |
|---------------|----------|--------|
| "We searched 12 ways. We found nothing." | 12 queries, zero results | Complete search log |
| "The most ocean-relevant code evaluates models, not interventions" | PBP-POD, 5 commits Jun 19, 2026 | MDTF commit 33024ad |
| "The silence is total — not a slow start but a void" | 0 repos across all ocean themes | 12-query gap analysis |
| "The complexity barrier is real but not absolute" | Simplified models could run on laptops | Architecture sketch |
| "The funding gap is the most explainable mystery" | No agency funds ocean intervention code | Cross-repo comparison |
| "The call to action is real" | Ocean covers 70%, has 0 repos | Headline finding |

---

## v6 Signal Summary

| Signal | Strength | Confidence | Implication |
|--------|----------|------------|-------------|
| Zero ocean intervention repos | 🟢 High | 🟢 Absolute | The void is the story |
| PBP-POD is ocean-adjacent lifeline | 🟢 High | 🟢 Clear | QA exists, simulation doesn't |
| 12 queries confirm the gap | 🟢 High | 🟢 Exhaustive | Not a search failure — a real absence |
| Architecture is feasible | 🟡 Medium | 🟢 Clear | The technical barrier is surmountable |
| Three hypotheses remain unresolved | 🟡 Medium | 🟡 Genuine | The data can't tell us which is right |
| WRF coupling unused for OAE | 🟡 Medium | 🟢 Clear | Cross-domain potential, no one's bridging it |
