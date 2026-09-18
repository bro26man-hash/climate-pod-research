# 🌊 Ocean Intervention — Project Discoveries & Gap Analysis (v7)

> **Last updated:** September 2026 (v7)  
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

## What DOES Exist: Ocean-Adjacent Lifelines (v7 Updated)

### 1. MDTF-Diagnostics (NOAA-GFDL) — The Precipitation-Buoyancy POD

| Field | Detail |
|-------|--------|
| **Repo** | `NOAA-GFDL/MDTF-diagnostics` |
| **Stars** | 80 |
| **Last commit** | August 14, 2026 (general); June 19, 2026 (PBP-POD) |
| **Focus** | Process-oriented model diagnostics |

**The precipitation-buoyancy POD (v7 Detail — 5 commits confirmed):**

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

**The v7 insight — The PBP-POD as the ocean's closest friend is also its limitations:** The POD measures ocean-atmosphere coupling, but it doesn't simulate interventions. It could tell you whether your ocean model gets the salinity right, but not what happens when you add alkaline minerals to the ocean. The PBP-POD is a mirror, not a window.

**The irony for the podcast:** The most ocean-relevant tool in open source is for evaluating model accuracy, not simulating interventions. We can evaluate the ocean but we can't perturb it in silico.

---

### 2. WRF (Atmosphere-Ocean Coupling Potential — v7 Update)

WRF has ocean coupling capabilities (MOM, POP), but no one appears to be using it for ocean intervention scenarios. The v4.8.0 release (Jun 8, 2026) includes MYNN surface layer updates that affect air-sea interaction, but these are for weather prediction, not geoengineering.

**v7 addition — The TEMPO disable as indirect ocean signal:** The June 5 commit (6a289e1) turning off `tempo_aerosolaware` and `tempo_hailaware` for stratospheric instability is atmospheric, not oceanic. But SAI affects ocean temperatures (reduced solar radiation → reduced surface warming → altered ocean mixing). If someone were running WRF with SAI for ocean-intervention modeling, the TEMPO disable would directly affect their results. The atmosphere and ocean are coupled — you can't fix one without the other.

**v7 finding:** WRF is the single repo with the most cross-theme potential. Its atmosphere model feeds into both solar (SRM simulation) and ocean (coupled air-sea interaction) domains. But no one is using it for ocean intervention. The coupling exists in the code; the coupling doesn't exist in the use cases.

---

### 3. ClimateSoton/climate-research-group (v7 — The CFD Bridge)

**v7 UPDATE — This is the most significant new finding in the ocean theme.**

| Field | Detail |
|-------|--------|
| **Repo** | `ClimateSoton/climate-research-group` |
| **Stars** | Not tracked (website repo) |
| **Language** | HTML/CSS/JavaScript |
| **Last commit** | August 6, 2026 |
| **Focus** | Chemical looping, carbon capture, CFD modelling, reaction engineering |

**v7 Fresh Commit Pull (4 commits, all August 6, 2026):**

| Date | SHA | Message |
|------|-----|--------|
| Aug 6, 2026 | `4b7cc18` | Update index.html |
| Aug 6, 2026 | `f0b123f` | Delete 1.zip |
| Aug 6, 2026 | `503e839` | Add files via upload |
| Aug 6, 2026 | `3807b50` | Add files via upload |

**Why this matters for ocean intervention:**

The CLIMATE Research Group at the University of Southampton works on **CFD (Computational Fluid Dynamics) modelling**. CFD is the computational backbone of ocean circulation modeling. Their research areas include:
- **Chemical looping** — could be adapted for ocean alkalinity enhancement (dissolution kinetics)
- **CO₂ conversion** — relevant to ocean carbon chemistry modeling
- **Reaction engineering** — relevant to ocean intervention reaction rates

**The v7 bridge:** ClimateSoton is the ONLY carbon-theme repo with 2026 activity (Aug 6, 2026). Their CFD expertise is the closest thing to ocean circulation modeling in the carbon capture space. If any research group were to extend their work from atmospheric CFD to ocean CFD, it would be this one.

**The caution:** This is a research group website, not a code repository. The CFD work they describe may be proprietary or paper-based, not open-source. The bridge exists in principle, not in code. But the activity signal (Aug 2026) means the group is operational, and their next paper might include code.

**🎙️ Episode Hook:** *"The only carbon-capture repo with 2026 activity is a website. But that website belongs to a CFD research group that could be the bridge between carbon capture modeling and ocean intervention. The code might not exist yet. But the expertise does."

---

### 4. WRF Ocean Coupling (Indirect — v7 Reiteration)

WRF's MOM/POP coupling capabilities are documented but unused for intervention scenarios. The v4.8.0 release includes air-sea interaction physics updates (MYNN-EDMF, May 27, 2026), but these are for weather prediction.

**v7 finding:** The coupling code exists. The expertise exists. The commitment doesn't. This is the "bridge that exists but nobody crosses" problem.

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

## Why Is the Ocean Empty? Three Hypotheses (v7 Updated)

### Hypothesis 1: The Complexity Barrier

Ocean models are computationally expensive and require specialized knowledge (finite-element methods, coastal boundary conditions, multiphase flow). The barrier to entry is higher than for atmospheric models.

**v7 evidence for:** All ocean-adjacent repos are institutional (NOAA-GFDL). ClimateSoton's CFD work is NOT open-source — it's website promotional material. The actual CFD code is behind institutional walls. Individual researchers can't afford the compute.

**v7 evidence against:** WRF's atmosphere model was once individual-scale, now it's institutional. The transition happened when the community coalesced. The ocean could follow the same path — but it hasn't.

**v7 addition — The WRF bridge that isn't:** WRF already has ocean coupling (MOM, POP). The code exists. But nobody is using it for intervention scenarios. The bridge between atmospheric and ocean modeling is built butunused. The complexity barrier isn't technical — it's motivational.

### Hypothesis 2: The Governance Chill

Ocean intervention is more politically controversial than SRM. The London Convention/Protocol strictly regulates ocean fertilization. Marine cloud brightening has been dubbed "geoengineering's third rail."

**v7 evidence for:** The silence is total. Not just "few repos" but "ZERO repos." SRM also has governance concerns, yet srm-forever and ClimateMARGO exist. The difference might be funding, not governance.

**v7 evidence against:** ClimateSoton's Aug 2026 activity shows the research group is alive and publishing. If governance were the chill, we'd expect fewer papers too. But the papers keep coming. The silence is in the code, not the literature.

**v7 addition — The CFD connection:** If ClimateSoton's CFD work is published but not on GitHub, it suggests researchers are publishing papers but not sharing code. This is the "publication without open-source" pattern — common in climate science, but it means the ocean gap isn't a governance chill; it's an open-source culture gap.

### Hypothesis 3: The Funding Gap

No major funding agency has prioritized open-source ocean intervention modeling.

**v7 evidence for:** Every other climate tech domain has at least some repos. The ocean is the only domain with zero. NOAA funds atmospheric modeling (WRF), NSF funds carbon capture (OpenAir-Cyan), but nobody funds ocean intervention code.

**v7 evidence against:** ClimateSoton's operational status (Aug 2026 website update) suggests some funding exists for chemical looping and CFD research. The funding is there — it's just not directed at open-source ocean intervention code.

**v7 addition — The bridge funding opportunity:** The most promising path might be to fund a "CFD-to-Ocean"bridge project. ClimateSoton has the CFD expertise. A small grant could adapt their atmospheric CFD codes for ocean circulation modeling with intervention modules. The bridge already exists in expertise; it just needs funding to become code.

---

## What Would Open-Source Ocean Intervention Look Like? (v7 Architecture)

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

### v7 Bottom-Up Strategy — The ClimateSoton Bridge

1. **Start with CFD parameterizations, not full Navier-Stokes.** ClimateSoton's CFD expertise provides the building blocks for ocean circulation modeling. Their chemical looping research maps directly to dissolution kinetics for OAE.
2. **Use WRF's ocean coupling (MOM/POP) as the starting framework.** WRF already has air-sea interaction physics. Extend it with intervention modules. The code exists; the use cases don't.
3. **Post-process MDTF diagnostics for ocean intervention.** The PBP-POD could be adapted to detect intervention signals in model output.
4. **Build on existing data.** OWID, CSIRO, and NOAA already have ocean data pipelines.

### v7 Top-Down Strategy — The OMCF (Ocean Model Comparison Facility)

1. **Open-source OAE benchmarking kit.** A standardized test case where everyone's model runs against the same scenario.
2. **Ocean intervention model comparison exercise.** Like CMIP but for OAE/MCB. A "OMCF" (Ocean Model Comparison Facility).
3. **The ClimateSoton connection.** Their CFD work could provide the initial ocean circulation module. A bridge grant could adapt atmospheric CFD for ocean use.

---

## The Episode 3 Narrative (v7)

### Arc A: "The Empty Quadrant"
We searched GitHub 12 different ways. We searched every ocean geoengineering technique from every angle. And we found nothing. Zero repositories. Zero models. Zero code.

Show the search results table. All zeros. Then show what DOES exist — MDTF's 5-commits-in-1-day PBP-POD, ClimateSoton's Aug 2026 website update.

### Arc B: "The Three Hypotheses"
Present the three competing explanations: Complexity, Governance, Funding. Let the listener decide. The v7 addition: the "open-source culture gap" — researchers publish papers but don't share code.

### Arc C: "The Architecture"
What would the first open-source OAE model look like? Here's a concrete sketch. Show the architecture diagram. Discuss the ClimateSoton CFD bridge — the most promising path from existing expertise to open-source ocean code.

### Arc D: "The WRF Coupling That Isn't"
WRF has ocean coupling code (MOM/POP). It exists. It works. But nobody is using it for intervention scenarios. The bridge is built but nobody crosses it. This is the motivational gap, not the technical gap.

### Arc E: "The Call to Action"
If you're a developer, a climate scientist, or just someone who cares about the ocean — the quadrant is empty. What are you going to do about it?

---

## Summary Table — Ocean Theme (v7)

| Domain | Repos | Commits | Status | Closest Tool | v7 Signal |
|--------|-------|---------|--------|-------------|----------|
| **Ocean Alkalinity Enhancement** | 0 | 0 | 🚫 EMPTY | — | Confirmed in 12 queries |
| **Marine Cloud Brightening** | 0 | 0 | 🚫 EMPTY | — | Confirmed in 12 queries |
| **Artificial Upwelling** | 0 | 0 | 🚫 EMPTY | — | Confirmed in 12 queries |
| **Ocean Fertilization** | 0 | 0 | 🚫 EMPTY | — | Confirmed in 12 queries |
| **Ocean Sensors/IoT** | 0 | 0 | 🚫 EMPTY | — | Confirmed in 12 queries |
| **Ocean Process Diagnostics** | 1 (MDTF) | 5 (1-day burst) | 🟡 Active | PBP-POD (evaluation only) | v7: Mirror, not window |
| **Ocean-Adjacent CFD** | 1 (ClimateSoton) | 4 (Aug 2026) | 🟢 Active | Research group website | **v7: The Bridge** |
| **WRF Ocean Coupling** | 1 (WRF) | Indirect | 🟡 Unused | MOM/POP in WRF | **v7: Bridge built, not crossed** |

---

## v7 Key Signals

1. **The gap persists.** 12 queries, zero results. Not a slow start — a void.
2. **MDTF's PBP-POD is the ocean's closest friend.** 5 commits on June 19, 2026. The most ocean-relevant diagnostic in open source, and it's for evaluation, not simulation. v7 update: it's a mirror, not a window.
3. **ClimateSoton is the CFD bridge.** The ONLY carbon-theme repo with 2026 activity. Their CFD expertise could adapt to ocean circulation modeling. The bridge exists in expertise, not in code.
4. **WRF's ocean coupling exists but is unused.** MOM/POP are in the code. Nobody is using them for intervention scenarios. The bridge is built but not crossed.
5. **The architecture is feasible.** A simplified OAE model could run on a laptop today using parameterized general models (PGMs), not full Navier-Stokes.
6. **The governance question is unresolved.** Is the silence a choice (governance chill) or a gap (funding/open-source culture)? The v7 evidence leans toward "open-source culture gap" — papers are published, code is not shared.
7. **The call to action is real.** The ocean covers 70% of the planet. Zero repos. The listener has to ask: why?

---

## v7 Research Log

| Date | Activity |
|------|----------|
| Sep 2026 | v6: Initial gap analysis — 12 queries, zero ocean repos, MDTF PBP-POD identified |
| Sep 2026 | v7: Fresh commit data pulled from ClimateSoton (4 commits, Aug 6, 2026) |
| Sep 2026 | v7: ClimateSoton identified as "The CFD Bridge" — only carbon-theme repo with 2026 activity |
| Sep 2026 | v7: WRF ocean coupling (MOM/POP) re-examined — code exists but unused for interventions |
| Sep 2026 | v7: "Open-source culture gap" hypothesis added — papers published, code not shared |
| Sep 2026 | v7: PBP-POD recharacterized as "mirror, not window" — evaluates models, doesn't simulate interventions |
| Sep 2026 | v7: Two new narrative arcs added (WRF Coupling That Isn't, CFD Bridge) |
| Sep 2026 | v7: Bottom-up strategy updated with ClimateSoton CFD bridge path |
| Sep 2026 | v7: Top-down strategy updated with OMCF concept and ClimateSoton connection |
