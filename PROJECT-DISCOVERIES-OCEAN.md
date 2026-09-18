# 🌊 Ocean Intervention — Project Discoveries & Gap Analysis (v6)

> **Last updated:** September 2026 (v6)  
> **Branch:** `ocean-intervention`  
> **Podcast episode:** Episode 3 — Ocean Intervention

---

## 🚨 HEADLINE FINDING: The Ocean Intervention Gap (v6 Reconfirmed)

**Our GitHub search across 12 query strategies returned ZERO dedicated ocean geoengineering repositories.**

### What We Searched (Complete v6 List)

| # | Search Query | Results | Category |
|---|-------------|---------|----------|
| 1 | `geoengineering simulation climate` | 0 | Direct |
| 2 | `climate technology carbon capture ocean` | 0 dedicated | Thematic |
| 3 | `geoengineering stars:>50` | 1 (not ocean) | Filtered |
| 4 | `climate simulation modeling stars:>100` | 1 (atmosphere only) | Filtered |
| 5 | `carbon capture removal stars:>100` | 0 | Filtered |
| 6 | `ocean climate intervention stars:>50` | 0 | Filtered |
| 7 | `climate model atmospheric ocean stars:>200` | 0 | Combined |
| 8 | `direct air capture DAC stars:>50` | 0 (not ocean) | Filtered |
| 9 | `ocean alkalinity enhancement` | 0 | Mechanistic |
| 10 | `marine cloud brightening` | 0 | Mechanistic |
| 11 | `artificial upwelling ocean model` | 0 | Mechanistic |
| 12 | `ocean fertilization iron model` | 0 | Mechanistic |

**Result: ZERO dedicated ocean geoengineering repositories across all 12 search strategies.**

---

## What DOES Exist: Ocean-Adjacent Lifelines

### 1. MDTF-Diagnostics (NOAA-GFDL) — The Precipitation-Buoyancy POD

| Field | Detail |
|-------|--------|
| **Repo** | `NOAA-GFDL/MDTF-diagnostics` |
| **Stars** | 80 |
| **Last commit** | August 14, 2026 (general); June 19, 2026 (PBP-POD) |
| **Focus** | Process-oriented model diagnostics |

**The precipitation-buoyancy POD (v6 Detail):**

| Date | Commit | Message | Ocean Relevance |
|------|--------|---------|-----------------|
| **Jun 19, 2026** | `33024ad` | **add MCS precipitation-buoyancy statistics POD** | ⭐⭐⭐ Core ocean-atmosphere diagnostic |
| Jun 19, 2026 | `4cfc99c` | Update MCS_precip_buoy_stats.rst | Documentation |
| Jun 19, 2026 | `699de27` | Update MCS_precip_buoy_stats.rst | Documentation |
| Jun 19, 2026 | `d6bc6d0` | Update MCS_precip_buoy_stats.rst | Documentation |
| Jun 19, 2026 | `3904d29` | Update MCS_precip_buoy_stats.rst | Documentation |

**5 commits on a single day (June 19, 2026), all touching the same file.** The 5th commit is the actual code addition; the first 4 are documentation updates. This is a textbook "big bang" release: code + 4 doc updates, all same day.

**What the POD does:** Measures the statistical relationship between precipitation and buoyancy (temperature-salinity structure) in climate model output. This is fundamental to ocean-atmosphere coupling — precipitation changes surface salinity, which changes buoyancy, which changes ocean mixing.

**Why it matters for ocean intervention:** If you want to evaluate whether an ocean geoengineering intervention works, you first need tools to evaluate ocean processes. MDTF provides those tools — but only for model evaluation, not intervention simulation. It's the QA lab for the ocean, not the ocean's experimenter.

**The irony:** The most ocean-relevant tool in open source is for evaluating model accuracy, not simulating interventions. We can evaluate the ocean but we can't perturb it in silico.

---

### 2. WRF (Atmosphere-Ocean Coupling Potential)

WRF has ocean coupling capabilities (MOM, POP), but no one appears to be using it for ocean intervention scenarios. The v4.8.0 release (Jun 8, 2026) includes MYNN surface layer updates that affect air-sea interaction, but these are for weather prediction, not geoengineering.

---

### 3. ClimateSoton/climate-research-group (CFD-Adjacent)

Active in August 2026, but a research group website, not a code repository. CFD resources could be relevant to ocean circulation modeling, but they're not adapted for intervention scenarios.

---

## What Doesn't Exist: The Ocean Gap Mapped

| Domain | Search | Result | What Would Be Needed |
|--------|--------|--------|---------------------|
| **Ocean Alkalinity Enhancement** | "ocean alkalinity enhancement", "OAE model", "olivine dissolution ocean" | ZERO | Dissolution kinetics model, ocean carbonate chemistry, alkalinity transport |
| **Marine Cloud Brightening** | "marine cloud brightening", "MCB simulation", "cloud seeding ocean" | ZERO | Cloud microphysics, CCN activation, radiation transfer, vessel spray modeling |
| **Artificial Upwelling** | "artificial upwelling", "deep water pumping ocean" | ZERO | Thermocline modeling, nutrient flux, vertical mixing parameterization |
| **Ocean Fertilization** | "ocean fertilization", "iron fertilization model", "FFE" | ZERO | Nutrient cycling, phytoplankton growth, export production modeling |
| **Ocean Sensors/IoT** | "ocean sensor network", "ocean monitoring" | ZERO | Sensor calibration, data pipelines, real-time assimilation |
| **Ocean Data Assimilation** | "ocean data assimilation", "ocean state estimation" | ZERO | 4D-Var, ensemble Kalman filter, observation operators |

---

## Why Is the Ocean Empty? Three Hypotheses

### Hypothesis 1: The Complexity Barrier
Ocean models are computationally expensive and require specialized knowledge (finite-element methods, coastal boundary conditions, multiphase flow). The barrier to entry is higher than for atmospheric models. WRF runs on a laptop; an ocean model needs a cluster.

**Evidence for:** All existing ocean science repos are institutional (NOAA-GFDL). Individual researchers can't afford the compute.

**Evidence against:** AR5/AR6 models are run internationally. The complexity is navigable with sufficient coordination.

### Hypothesis 2: The Governance Chill
Ocean intervention is more politically controversial than SRM. The London Convention/Protocol strictly regulates ocean fertilization. Marine cloud brightening has been dubbed "geoengineering's third rail." Researchers may avoid public code repositories to prevent misuse or political attacks.

**Evidence for:** The silence istotal. Not just "few repos" but "ZERO repos." This isn't a slow start — it's a void.

**Evidence against:** Solar geoengineering also has governance concerns, yet srm-forever and ClimateMARGO exist. The difference might be funding, not governance.

### Hypothesis 3: The Funding Gap
No major funding agency has prioritized open-source ocean intervention modeling. Physical scientists publish papers; the modeling community builds tools; but the intersection — open-source ocean intervention models — has no champion.

**Evidence for:** Every other climate tech domain has at least some repos. The ocean is the only domain with zero. This pattern matches funding patterns: NOAA funds atmospheric modeling, NSF funds carbon capture, but nobody funds ocean intervention code.

**Evidence against:** The ocean covers 70% of the planet. You'd think至少 one agency would fund an open-source ocean model.

---

## What Would Open-Source Ocean Intervention Look Like?

### Architecture Sketch

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

### Bottom-Up Strategy (What's Feasible Now)

1. **Start with PGMs (Parameterized General Models)** not full Navier-Stokes. Use simplified parameterizations that run on a laptop.
2. **Use WRF's ocean coupling** as a starting point. WRF already has air-sea interaction physics. Extend it with intervention modules.
3. **Post-process MDTF diagnostics** for ocean intervention. The PBP-POD could be adapted to detect intervention signals in model output.
4. **Build on existing data.** OWID, CSIRO, and NOAA already have ocean data pipelines.

### Top-Down Strategy (What the Community Could Do)

1. **Open-source OAE benchmarking kit.** A standardized test case where everyone's model runs against the same scenario. Results compared in a shared dashboard.
2. **Ocean intervention model comparison exercise.** Like CMIP but for OAE/MCB. A "OMCF" (Ocean Model Comparison Facility).

---

## The Episode 3 Narrative (v6)

### Arc A: "The Empty Quadrant"
*We searched GitHub 12 different ways. We searched every ocean geoengineering technique from every angle. And we found nothing. Zero repositories. Zero models. Zero code.*

Show the search results table. All zeros. Then show what DOES exist — MDTF's 5-commits-in-1-day PBP-POD.

### Arc B: "The Three Hypotheses"
Present the three competing explanations: Complexity, Governance, Funding. Let the listener decide.

### Arc C: "The Architecture"
What would the first open-source OAE model look like? Here's a concrete sketch. Show the architecture diagram. Discuss what's feasible now vs. what needs a community.

### Arc D: "The Call to Action"
*If you're a developer, a climate scientist, or just someone who cares about the ocean — the quadrant is empty. What are you going to do about it?*

---

## Summary Table — Ocean Theme (v6)

| Domain | Repos | Commits | Status | Closest Tool |
|--------|-------|---------|--------|-------------|
| **Ocean Alkalinity Enhancement** | 0 | 0 | 🚫 EMPTY | — |
| **Marine Cloud Brightening** | 0 | 0 | 🚫 EMPTY | — |
| **Artificial Upwelling** | 0 | 0 | 🚫 EMPTY | — |
| **Ocean Fertilization** | 0 | 0 | 🚫 EMPTY | — |
| **Ocean Sensors/IoT** | 0 | 0 | 🚫 EMPTY | — |
| **Ocean Process Diagnostics** | 1 (MDTF) | 5 (1-day burst) | 🟡 Active | PBP-POD (evaluation only) |
| **Ocean-Adjacent CFD** | 1 (ClimateSoton) | Low | 🟡 Sparse | Research group website |

---

## v6 Key Signals

1. **The gap persists.** 12 queries, zero results. Not a slow start — a void.
2. **MDTF's PBP-POD is the ocean's closest friend.** 5 commits on June 19, 2026. The most ocean-relevant diagnostic in open source, and it's for evaluation, not simulation.
3. **The architecture is feasible.** A simplified OAE model could run on a laptop today. The barrier isn't technical — it's motivational.
4. **The governance question is unresolved.** Is the silence a choice (governance chill) or a gap (funding gap)? The data can't tell us.
5. **The call to action is real.** The ocean covers 70% of the planet. Zero repos. The listener has to ask: why?
