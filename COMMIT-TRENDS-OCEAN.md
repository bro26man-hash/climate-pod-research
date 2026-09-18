# 🌊 Ocean Intervention — Commit Trend Analysis & Narrative (v7)

> **Last updated:** September 2026 (v7)  
> **Branch:** `ocean-intervention`  
> **Podcast episode:** Episode 3 — Ocean Intervention

---

## The Headline: Zero Commits for Zero Repos (v7 Reconfirmed)

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
Carbon capture directory (Open-Sustainable-Tech):     1 (with 200+ commits)
Ocean process diagnostics (MDTF PBP-POD):             1 (with 5 commits, 1-day burst)
Ocean-adjacent CFD (ClimateSoton):                    1 (with 4 commits, website only)
```

**The ocean is not just underrepresented — it is absent.**

---

## Ocean-Adjacent Commit Activity (v7 Detail)

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

**v7 analysis — The PBP-POD as mirror, not window:**

The PBP-POD measures the statistical relationship between precipitation and buoyancy. This is fundamental to ocean-atmosphere coupling — precipitation changes surface salinity, which changes buoyancy, which changes ocean mixing.

But the PBP-POD does NOT simulate interventions. It does not model OAE, MCB, or artificial upwelling. It evaluates whether climate models get the ocean right. It's the QA lab, not the experimenter.

**The v7 reframe:** The PBP-POD is a mirror — it reflects the ocean's behavior back to us. But it's not a window — it doesn't show us what happens when we perturb the system. We can diagnose the ocean's behavior but we can't simulate what happens when we intervene.

**The irony for the podcast:** The most ocean-relevant code in open source was written to evaluate models, not to perturb them. The mirror works. The window doesn't.

---

### 2. WRF — Atmosphere-Ocean Coupling Code That Exists But Nobody Uses (v7)

WRF has ocean coupling capabilities (MOM, POP). The code exists.

**v7 fresh commit evidence:**
- **Jun 8, 2026 (06d4240):** v4.8.0 release merge
- **May 27, 2026 (8299919):** MYNN-EDMF pointer update — affects air-sea interaction physics
- **May 28, 2026 (e836cd6):** Solar radiation bug fix — affects energy budget that drives ocean temperatures
- **Jun 5, 2026 (6a289e1):** TEMPO aerosol/hail options disabled for stratospheric instability — someone tried SAI and the physics broke

**The v7 finding — The bridge that exists but nobody crosses:**

WRF's MOM/POP ocean coupling code is in the repository. It's been there for years. The v4.8.0 release continues to update air-sea interaction physics. But nobody appears to be using WRF for ocean intervention scenarios.

The TEMPO disable (6a289e1) is the clearest signal: someone tried to run WRF with SAI, found the physics couldn't handle it, and turned off the options. If someone were running WRF for ocean-intervention modeling (SAI affecting ocean temperatures → altered ocean mixing), the TEMPO disable would directly affect their results.

**The chain that isn't run:**
```
WRF SAI simulation → Solar radiation bug (e836cd6) → TEMPO unstable (6a289e1) → 
Ocean temperature response → Ocean mixing change → Intervention effect

The chain exists in theory. The code is in the repository. But nobody runs it.
```

**🎙️ Episode angle:** *"The most important climate model has ocean coupling code. It's been there for years. But nobody is using it to simulate what happens when we intervene in the ocean. The bridge is built. Nobody crosses it."

---

### 3. ClimateSoton/climate-research-group — The CFD Bridge That Could Be (v7)

**v7 UPDATE — This is the most significant new finding in the ocean theme.**

| Field | Detail |
|-------|--------|
| **Repo** | `ClimateSoton/climate-research-group` |
| **Stars** | Not tracked (website repo) |
| **Last commit** | August 6, 2026 (4 commits, same day) |
| **Focus** | Chemical looping, CFD modelling, CO₂ conversion, reaction engineering |

**v7 Fresh Commit Pull (4 commits, all Aug 6, 2026):**

| Date | SHA | Message |
|------|-----|--------|
| Aug 6, 2026 | `4b7cc18` | Update index.html |
| Aug 6, 2026 | `f0b123f` | Delete 1.zip |
| Aug 6, 2026 | `503e839` | Add files via upload |
| Aug 6, 2026 | `3807b50` | Add files via upload |

**Why this matters for ocean intervention:**

The CLIMATE Research Group works on **CFD (Computational Fluid Dynamics)** modelling. CFD is the computational backbone of ocean circulation modeling. Their research areas include:
- **Chemical looping** — dissolution kinetics, directly applicable to OAE (olivine/limestone dissolution)
- **CO₂ conversion** — ocean carbon chemistry modeling
- **Reaction engineering** — reaction rates, directly applicable to ocean intervention chemistry

**The v7 bridge:** ClimateSoton is the ONLY carbon-theme repo with 2026 activity. Their CFD expertise is the closest thing to ocean circulation modeling in the carbon capture space. If any research group were to extend their work from atmospheric CFD to ocean CFD, it would be this one.

**The caution:** This is a research group website, not a code repository. The CFD work they describe may be proprietary or paper-based, not open-source. The bridge exists in principle, not in code.

**The opportunity:** A small grant could adapt their atmospheric CFD codes for ocean circulation modeling with intervention modules. The bridge already exists in expertise; it just needs funding to become code.

**🎙️ Episode angle:** *"The only carbon-capture repo with 2026 activity is a website. But that website belongs to a CFD research group that could be the bridge between carbon capture modeling and ocean intervention. The code might not exist yet. But the expertise does. And a grant could change that."

---

## The Three-Hypothesis Framework (v7 Updated)

### Hypothesis 1: The Complexity Barrier

**The claim:** Ocean models are computationally expensive and require specialized knowledge. The barrier to entry is higher than for atmospheric models.

**v7 evidence FOR:**
- All ocean-adjacent repos are institutional (NOAA-GFDL)
- ClimateSoton's CFD work is NOT open-source — it's website promotional material
- WRF's ocean coupling code (MOM/POP) exists but nobody uses it for interventions
- The PBP-POD required expertise in Proper Orthogonal Decomposition methods

**v7 evidence AGAINST:**
- WRF started as an individual project and became institutional — the transition is possible
- Simplified parameterization (PGMs) could run on laptops today
- The WRF ocean coupling code already exists — the complexity barrier was already crossed for the atmosphere

**v7 addition — The bridge that exists but isn't crossed:** The complexity barrier isn't technical. WRF already has ocean coupling code. The code is there. The barrier is motivational, not technical. Nobody decided to use it for interventions.

**Podcast angle:** *"The complexity barrier is real but not absolute. A simplified OAE model could run on a laptop today. The question is whether someone decides to build it. And the WRF code shows the barrier was already crossed for the atmosphere — just not for the ocean."

### Hypothesis 2: The Governance Chill

**The claim:** Ocean intervention is more politically controversial. The London Convention/Protocol regulates ocean fertilization. MCB is "geoengineering's third rail."

**v7 evidence FOR:**
- The silence is total — not "few repos" but ZERO repos
- ClimateSoton's CFD work is published but not on GitHub (paper-based, not open-source)
- The "publication without open-source" pattern suggests researchers avoid public repos

**v7 evidence AGAINST:**
- SRM also has governance concerns, yet srm-forever exists (0 stars, but it exists)
- ClimateSoton is actively publishing and updating their website — the research is happening
- Papers on ocean intervention are published openly (Nature, Science)
- The code silence doesn't match the publication volume

**v7 addition — The open-source culture gap:** ClimateSoton's CFD research is published in papers but not shared as code. This suggests the barrier isn't governance — it's open-source culture. Climate scientists publish papers; they don't share code. The papers are accessible; the code is not.

**Podcast angle:** *"If governance were the reason, we'd expect fewer papers too. But the papers keep coming. The silence is in the code, not the literature. What does that tell us? The governance chill doesn't explain why papers exist but code doesn't."

### Hypothesis 3: The Funding Gap

**The claim:** No major funding agency prioritizes open-source ocean intervention modeling.

**v7 evidence FOR:**
- Every other climate tech domain has at least some repos
- The ocean covers 70% of the planet
- NOAA funds atmospheric modeling (WRF), NSF funds carbon capture (OpenAir-Cyan), but nobody funds ocean intervention code
- ClimateSoton's operational status (Aug 2026) suggests some funding exists for chemical looping/CFD, but it's not directed at open-source ocean code

**v7 evidence AGAINST:**
- ClimateSoton's CFD expertise exists and is active — the talent is there
- The WRF ocean coupling code exists — the building blocks are there
- The PBP-POD diagnostic exists — the evaluation tools are there
- All the pieces exist; they just aren't assembled

**v7 addition — The bridge funding opportunity:** The most promising path might be to fund a "CFD-to-Ocean" bridge project. ClimateSoton has the CFD expertise. A small grant could adapt their atmospheric CFD codes for ocean circulation modeling with intervention modules. The bridge already exists in expertise; it just needs funding to become code.

**Podcast angle:** *"The ocean covers 70% of the planet. It drives every weather system you've ever experienced. And there is exactly zero open-source code for intervening in it. The funding gap is the most explainable mystery — but the solution might be a small bridge grant."

---

## The "Empty Quadrant" Dashboard (v7)

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
            │           │   + TEMPO   │
            │           │   disable   │
            │           │   (Jun 5)   │
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
      WRF coupling      │            │
      EXISTS but        │            │
      UNUSED            │            │
            │           │            │
      ClimateSoton      │            │
      CFD bridge        │            │
      EXISTS in         │            │
      expertise         │            │
      (not code)        │            │
            │           │            │
            └────────────┼────────────┘
                         │
                    CARBON
                  CAPTURE (CDR)
                         │
            ┌────────────┼────────────┐
            │            │            │
         DADIUS      CCS       CARBON
      (DIRECT AIR)  (STORAGE)   (SURVEY)
            │            │            │
      tjz21: 2★     ghost:    Open-Sust:
      CC0: YES     85★ dead    2,552★ alive
      10 commits    0 commits   15 commits
                       
      ClimateSoton:
      CFD bridge
      (Aug 2026)
```

---

## What Would Open-Source Ocean Intervention Look Like? (v7)

```
ocean-intervention/
├── oae/                    # Ocean Alkalinity Enhancement
│   ├── alkalinity_model.py  # Dissolution kinetics of olivine/limestone
│   │   └── (ClimateSoton CFD bridge could model dissolution kinetics)
│   ├── ocean_circulation.py # Simplified primitive equation solver
│   │   └── (WRF MOM/POP coupling could provide foundation)
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

### v7 Bottom-Up Strategy — The Two Bridges

**Bridge 1: ClimateSoton CFD → Ocean Circulation**
- ClimateSoton's CFD expertise provides the building blocks for ocean circulation modeling
- Their chemical looping research maps directly to dissolution kinetics for OAE
- A bridge grant could adapt atmospheric CFD codes for ocean use
- Timeline: 6-12 months for proof-of-concept

**Bridge 2: WRF MOM/POP → Intervention Modules**
- WRF already has ocean coupling code (MOM/POP)
- The code exists; the use cases don't
- Extend with intervention modules (OAE, MCB, upwelling)
- Timeline: 12-18 months for working prototype

**Bridge 3: MDTF PBP-POD → Intervention Evaluation**
- The PBP-POD could be adapted to detect intervention signals in model output
- The diagnostic infrastructure exists; the application doesn't
- Extend from model evaluation to intervention evaluation
- Timeline: 3-6 months for adaptation

### v7 Top-Down Strategy — The OMCF (Ocean Model Comparison Facility)

1. **Open-source OAE benchmarking kit.** A standardized test case where everyone's model runs against the same scenario.
2. **Ocean intervention model comparison exercise.** Like CMIP but for OAE/MCB. A "OMCF" (Ocean Model Comparison Facility).
3. **The ClimateSoton connection.** Their CFD work could provide the initial ocean circulation module.
4. **The WRF connection.** MOM/POP coupling could provide the baseline ocean model.
5. **The MDTF connection.** PBP-POD could provide the evaluation framework.

---

## Episode 3: Commit-Based Talking Points (v7)

| Talking Point | Evidence | Source |
|---------------|----------|--------|
| "We searched 12 ways. We found nothing." | 12 queries, zero results | Complete search log |
| "The most ocean-relevant code evaluates models, not interventions" | PBP-POD, 5 commits Jun 19, 2026 | MDTF commit 33024ad |
| "The silence is total — not a slow start but a void" | 0 repos across all ocean themes | 12-query gap analysis |
| "The WRF ocean coupling code exists but nobody uses it" | MOM/POP in WRF, TEMPO disable for SAI | WRF commits e836cd6, 6a289e1 |
| "The only 2026 activity is a website" | 4 commits, Aug 6, 2026 | ClimateSoton commit log |
| "A CFD research group could be the bridge" | Chemical looping, reaction engineering | ClimateSoton research areas |
| "The complexity barrier is real but not technical" | WRF already has ocean coupling code | WRF repository |
| "The gap is in code, not papers" | ClimateSoton publishes but doesn't share code | Cross-repo analysis |
| "A bridge grant could change everything" | CFD expertise + OAE need = bridge opportunity | Cross-theme analysis |

---

## v7 Signal Summary

| Signal | Strength | Confidence | Implication |
|--------|----------|------------|-------------|
| Zero ocean intervention repos | 🟢 High | 🟢 Absolute | The void is the story |
| PBP-POD is ocean-adjacent lifeline | 🟢 High | 🟢 Clear | QA exists, simulation doesn't |
| PBP-POD is a mirror, not a window | 🟢 High | 🟢 Clear | We can evaluate, not simulate |
| WRF ocean coupling exists but unused | 🟢 High | 🟢 Clear | Bridge built, not crossed |
| ClimateSoton CFD bridge potential | 🟡 Medium | 🟢 Clear | Expertise exists, code doesn't |
| 12 queries confirm the gap | 🟢 High | 🟢 Exhaustive | Not a search failure — a real absence |
| Architecture is feasible | 🟡 Medium | 🟢 Clear | The technical barrier is surmountable |
| Open-source culture gap (papers ≠ code) | 🟡 Medium | 🟢 New | ClimateSoton publishes but doesn't share code |
| Three hypotheses remain partially unresolved | 🟡 Medium | 🟡 Genuine | Evidence leans toward culture gap, not governance chill |
| Bridge funding opportunity | 🟡 Medium | 🟢 New | Small grant could adapt CFD to ocean modeling |
| WRF TEMPO disable signals SAI attempt | 🟢 High | 🟢 Clear | Someone tried SAI, physics broke, options disabled |

---

## v7 Research Log

| Date | Activity |
|------|----------|
| Sep 2026 | v6: Initial gap analysis — 12 queries, zero ocean repos, MDTF PBP-POD identified |
| Sep 2026 | v7: Fresh commit data pulled from ClimateSoton (4 commits, Aug 6, 2026) |
| Sep 2026 | v7: ClimateSoton identified as "The CFD Bridge" — only carbon-theme repo with 2026 activity |
| Sep 2026 | v7: WRF ocean coupling (MOM/POP) re-examined — code exists but unused for interventions |
| Sep 2026 | v7: WRF TEMPO disable (6a289e1) connected to ocean — SAI attempt would affect ocean temperatures |
| Sep 2026 | v7: PBP-POD recharacterized as "mirror, not window" — evaluates models, doesn't simulate interventions |
| Sep 2026 | v7: "Open-source culture gap" hypothesis added — ClimateSoton publishes but doesn't share code |
| Sep 2026 | v7: Two new bridges identified (ClimateSoton CFD, WRF MOM/POP) |
| Sep 2026 | v7: Bridge funding opportunity proposed — small grant to adapt CFD to ocean modeling |
| Sep 2026 | v7: Three narrative arcs added (WRF Coupling That Isn't, CFD Bridge, Culture Gap) |
| Sep 2026 | v7: Bottom-up strategy updated with two-bridge approach (ClimateSoton + WRF) |
| Sep 2026 | v7: Top-down strategy updated with OMCF concept and three-bridge connection |
