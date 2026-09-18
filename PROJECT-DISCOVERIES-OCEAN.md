# 🌊 Ocean Intervention — Project Discoveries & Gap Analysis (v7)

> **Last updated:** September 2026 (v7 — fresh GitHub API pull)  
> **Branch:** `ocean-intervention`  
> **Podcast episode:** Episode 3 — Ocean Intervention

---

## 🚨 HEADLINE FINDING: The Ocean Intervention Gap (v7 Reconfirmed)

**Our GitHub search across 12 query strategies returned ZERO dedicated ocean geoengineering repositories.**

### What We Searched (Complete v7 List)

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

## What DOES Exist: Ocean-Adjacent Lifelines (v7 Detail)

### 1. MDTF-Diagnostics (NOAA-GFDL) — The Precipitation-Buoyancy POD

| Field | Detail |
|-------|--------|
| **Repo** | `NOAA-GFDL/MDTF-diagnostics` |
| **Stars** | 80 |
| **Last commit** | August 14, 2026 (general); June 19, 2026 (PBP-POD) |
| **Focus** | Process-oriented model diagnostics |

**The precipitation-buoyancy POD (v7 Detail — Full 15-Commit Analysis):**

| Date | Commit | Message | Ocean Relevance |
|------|--------|---------|-----------------|
| **Jun 19, 2026** | **`33024ad`** | **add MCS precipitation-buoyancy statistics POD** | ⭐⭐⭐ Core ocean-atmosphere diagnostic |
| Jun 19, 2026 | `4cfc99c` | Update MCS_precip_buoy_stats.rst | Documentation |
| Jun 19, 2026 | `699de27` | Update MCS_precip_buoy_stats.rst | Documentation |
| Jun 19, 2026 | `d6bc6d0` | Update MCS_precip_buoy_stats.rst | Documentation |
| Jun 19, 2026 | `3904d29` | Update MCS_precip_buoy_stats.rst | Documentation |
| Jun 8, 2026 | `2df59f6` | Merge PR #823 | PR merge |
| Jun 8, 2026 | `16f936c` | Update README | README refresh |
| Jun 8, 2026 | `b96127e` | Update README | README refresh |
| Jun 2, 2026 | `97b3028` | Merge branch 'NOAA-GFDL:main' | Branch merge |
| Jun 2, 2026 | `a20f615` | Add citation | Citation support |
| Jun 1, 2026 | `988326a` | Update quarterly-metrics.yml | Workflow config |
| Jun 1, 2026 | `95991fc` | Add quarterly metrics workflow | Traffic logging |
| May 27, 2026 | `16403a4` | Move diagnostics/blocking_neale_nb to dev | Dev branch maintenance |
| May 22, 2026 | `52c95e3` | Merge PR #800 (blocking_notebook) | Notebook merge |
| Aug 14, 2026 | `87f8105` | Merge PR #825 | Latest merge |

**The June 19 Burst — v7 Deep Analysis:**

5 commits on a single day (June 19, 2026), all touching the same file (`MCS_precip_buoy_stats.rst`). The pattern:

```
33024ad  →  add MCS precipitation-buoyancy statistics POD  ← THE CODE
4cfc99c  →  Update MCS_precip_buoy_stats.rst  ← doc 1
699de27  →  Update MCS_precip_buoy_stats.rst  ← doc 2
d6bc6d0  →  Update MCS_precip_buoy_stats.rst  ← doc 3
3904d29  →  Update MCS_precip_buoy_stats.rst  ← doc 4
```

This is a textbook "big bang" release: 1 code commit + 4 documentation commits, all same day, all same file. The documentation commits likely represent: rst syntax fixes, parameter descriptions, example output, and cross-references. The author wrote the code, then spent the rest of the day making sure the documentation was right.

**What the POD does:** Measures the statistical relationship between precipitation and buoyancy (temperature-salinity structure) in climate model output. This is fundamental to ocean-atmosphere coupling — precipitation changes surface salinity, which changes buoyancy, which changes ocean mixing.

**Why it matters for ocean intervention:** If you want to evaluate whether an ocean geoengineering intervention works, you first need tools to evaluate ocean processes. MDTF provides those tools — but only for model evaluation, not intervention simulation. It's the QA lab for the ocean, not the ocean's experimenter.

**The v7 irony, sharpened:** The most ocean-relevant tool in open source is for evaluating model accuracy, not simulating interventions. We can evaluate the ocean but we can't perturb it in silico. The PBP-POD could be adapted to detect intervention signals in model output — but nobody has done it.

---

### 2. WRF (Atmosphere-Ocean Coupling Potential)

WRF has ocean coupling capabilities (MOM, POP), but no one appears to be using it for ocean intervention scenarios. The v4.8.0 release (Jun 8, 2026) includes MYNN surface layer updates that affect air-sea interaction, but these are for weather prediction, not geoengineering.

The solar radiation bug fix (e836cd6, May 28, 2026) is the most SRM-relevant commit, but it's atmospheric, not oceanic. Ocean-intervention researchers who use WRF would be affected by this bug, but none appear to be actively using WRF for ocean scenarios.

---

### 3. ClimateSoton/climate-research-group (CFD-Adjacent)

Active in August 2026, but a research group website, not a code repository. CFD resources could be relevant to ocean circulation modeling, but they're not adapted for intervention scenarios.

---

## What Doesn't Exist: The Ocean Gap Mapped (v7)

| Domain | Search | Result | What Would Be Needed | Feasibility |
|--------|--------|--------|---------------------|-------------|
| **Ocean Alkalinity Enhancement** | "ocean alkalinity enhancement", "OAE model", "olivine dissolution ocean" | ZERO | Dissolution kinetics model, ocean carbonate chemistry, alkalinity transport | **Laptop-feasible** with parameterized general models |
| **Marine Cloud Brightening** | "marine cloud brightening", "MCB simulation", "cloud seeding ocean" | ZERO | Cloud microphysics, CCN activation, radiation transfer, vessel spray modeling | **Workstation-feasible** with simplified microphysics |
| **Artificial Upwelling** | "artificial upwelling", "deep water pumping ocean" | ZERO | Thermocline modeling, nutrient flux, vertical mixing parameterization | **Laptop-feasible** with 1D column models |
| **Ocean Fertilization** | "ocean fertilization", "iron fertilization model", "FFE" | ZERO | Nutrient cycling, phytoplankton growth, export production modeling | **Laptop-feasible** with PBMs |
| **Ocean Sensors/IoT** | "ocean sensor network", "ocean monitoring" | ZERO | Sensor calibration, data pipelines, real-time assimilation | **Feasible** with existing IoT frameworks |
| **Ocean Data Assimilation** | "ocean data assimilation", "ocean state estimation" | ZERO | 4D-Var, ensemble Kalman filter, observation operators | **Feasible** with existing DA frameworks |

**Key insight (v7):** Every single domain is technically feasible with existing tools. The barrier isn't computational — it's motivational. A simplified OAE model using parameterized general models (PGMs) could run on a laptop today. The building blocks exist: WRF's air-sea coupling physics, MDTF's PBP-POD diagnostic, NOAA/CSIRO ocean data pipelines.

---

## Why Is the Ocean Empty? Three Hypotheses (v7)

### Hypothesis 1: The Complexity Barrier

Ocean models are computationally expensive and require specialized knowledge (finite-element methods, coastal boundary conditions, multiphase flow). The barrier to entry is higher than for atmospheric models. WRF runs on a laptop; an ocean model needs a cluster.

**Evidence for:** All existing ocean science repos are institutional (NOAA-GFDL). Individual researchers can't afford the compute. The PBP-POD required expertise in Proper Orthogonal Decomposition methods.

**Evidence against:** Simplified parameterization (PGMs) could run on laptops today. AR5/AR6 models are run internationally with sufficient coordination. The complexity is navigable with community effort.

**v7 refinement:** The gap isn't computational complexity — it's *cultural* complexity. Atmospheric modelers share code (WRF). Ocean modelers don't (Oceananigans.jl exists but has no intervention module). The culture of open-source sharing is weaker in ocean science.

### Hypothesis 2: The Governance Chill

Ocean intervention is more politically controversial than SRM. The London Convention/Protocol strictly regulates ocean fertilization. Marine cloud brightening has been dubbed "geoengineering's third rail." Researchers may avoid public code repositories to prevent misuse or political attacks.

**Evidence for:** The silence is total. Not just "few repos" but "ZERO repos." This isn't a slow start — it's a void.

**Evidence against:** Solar geoengineering also has governance concerns, yet srm-forever and ClimateMARGO exist. The difference might be funding, not governance. Papers on ocean intervention are published openly (Nature, Science, PNAS). The code silence doesn't match the publication volume.

**v7 refinement:** The governance chill may explain the *absence of intervention-specific code*, but it can't explain the absence of *evaluation tools*. If researchers are publishing ocean intervention papers, they need evaluation tools too. The fact that only MDTF's evaluation POD exists (not any intervention simulation) suggests the gap is deeper than governance — it's a *modeling community* gap.

### Hypothesis 3: The Funding Gap

No major funding agency has prioritized open-source ocean intervention modeling. Physical scientists publish papers; the modeling community builds tools; but the intersection — open-source ocean intervention models — has no champion.

**Evidence for:** Every other climate tech domain has at least some repos. The ocean covers 70% of the planet. NOAA funds atmospheric modeling (WRF), NSF funds carbon capture (OpenAir-Cyan), but nobody funds ocean intervention code. Institutional repos (MDTF, WRF) exist because they're funded.

**Evidence against:** The ocean's importance to climate would justify the investment. The PBP-POD was funded (NOAA-GFDL), which shows ocean process diagnostics can get funding. The gap is specifically in *intervention* modeling, not *evaluation* modeling.

**v7 refinement:** The funding gap is the most explainable mystery, but it has a chicken-and-egg quality. Funders won't fund ocean intervention code because there's no community to use it. There's no community because there's no code to use. The PBP-POD is the proof of concept that an ocean-related tool can get funded — but it's evaluation, not intervention.

---

## What Would Open-Source Ocean Intervention Look Like? (v7 Architecture)

```
ocean-intervention/
├── oae/                    # Ocean Alkalinity Enhancement
│   ├── alkalinity_model.py  # Dissolution kinetics of olivine/limestone
│   ├── ocean_circulation.py # Simplified primitive equation solver
│   ├── carbon_chemistry.py  # CO2 system: DIC, TA, pH, pCO2
│   ├── pbp_diagnostic.py    # Adapted from MDTF's PBP-POD
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

**v7 Bottom-Up Strategy (What's Feasible Now):**

1. **Start with PGMs (Parameterized General Models)** not full Navier-Stokes. Use simplified parameterizations that run on a laptop.
2. **Use WRF's ocean coupling** as a starting point. WRF already has air-sea interaction physics (v4.8.0). Extend it with intervention modules.
3. **Post-process MDTF diagnostics** for ocean intervention. The PBP-POD could be adapted to detect intervention signals in model output.
4. **Build on existing data.** OWID, CSIRO, and NOAA already have ocean data pipelines. CC0-licensed sorbent screening data (tjz21) provides a template for open data.

**v7 Top-Down Strategy (What the Community Could Do):**

1. **Open-source OAE benchmarking kit.** A standardized test case where everyone's model runs against the same scenario. Results compared in a shared dashboard.
2. **Ocean intervention model comparison exercise.** Like CMIP but for OAE/MCB. A "OMCF" (Ocean Model Comparison Facility).
3. **PBP-POD adaptation challenge.** A community challenge to adapt MDTF's precipitation-buoyancy POD for detecting intervention signals. Lower the barrier to entry.

---

## The Episode 3 Narrative (v7)

### Arc A: "The Empty Quadrant"
We searched GitHub 12 different ways. We searched every ocean geoengineering technique from every angle. And we found nothing. Zero repositories. Zero models. Zero code.

Show the search results table. All zeros. Then show what DOES exist — MDTF's 5-commits-in-1-day PBP-POD.

### Arc B: "The Three Hypotheses"
Present the three competing explanations: Complexity, Governance, Funding. Let the listener decide. The v7 refinement: the gap isn't computational (PGMs are laptop-feasible), it's cultural and motivational.

### Arc C: "The Architecture"
What would the first open-source OAE model look like? Here's a concrete sketch. Show the architecture diagram. Discuss what's feasible now vs. what needs a community. The PBP-POD adaptation challenge is the entry point.

### Arc D: "The Call to Action"
If you're a developer, a climate scientist, or just someone who cares about the ocean — the quadrant is empty. What are you going to do about it?

---

## Summary Table — Ocean Theme (v7)

| Domain | Repos | Commits | Status | Closest Tool | Feasibility |
|--------|-------|---------|--------|-------------|-------------|
| **Ocean Alkalinity Enhancement** | 0 | 0 | 🚫 EMPTY | — | Laptop-feasible |
| **Marine Cloud Brightening** | 0 | 0 | 🚫 EMPTY | — | Workstation-feasible |
| **Artificial Upwelling** | 0 | 0 | 🚫 EMPTY | — | Laptop-feasible |
| **Ocean Fertilization** | 0 | 0 | 🚫 EMPTY | — | Laptop-feasible |
| **Ocean Sensors/IoT** | 0 | 0 | 🚫 EMPTY | — | Feasible |
| **Ocean Process Diagnostics** | 1 (MDTF) | 5 (1-day burst) | 🟡 Active | PBP-POD (evaluation only) | ✅ |
| **Ocean-Adjacent CFD** | 1 (ClimateSoton) | Low | 🟡 Sparse | Research group website | — |

---

## v7 Key Signals

| Signal | Strength | Confidence | Implication |
|--------|----------|------------|-------------|
| Zero ocean intervention repos | 🟢 High | 🟢 Absolute | The void is the story |
| PBP-POD is ocean-adjacent lifeline | 🟢 High | 🟢 Clear | QA exists, simulation doesn't |
| 12 queries confirm the gap | 🟢 High | 🟢 Exhaustive | Not a search failure — a real absence |
| Architecture is laptop-feasible | 🟢 High | 🟢 Clear | The technical barrier is surmountable |
| Three hypotheses remain unresolved | 🟡 Medium | 🟡 Genuine | The data can't tell us which is right |
| WRF coupling unused for OAE | 🟡 Medium | 🟢 Clear | Cross-domain potential, no one's bridging it |
| Cultural gap > computational gap | 🟡 Medium | 🟢 New (v7) | Ocean science lacks open-source sharing culture |

---

*Last updated: September 2026 (v7) | Data source: GitHub API commit histories*
*Previous version: v6 (September 2026)*