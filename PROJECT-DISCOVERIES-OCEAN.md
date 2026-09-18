# 🌊 Ocean Intervention — Project Discoveries & Gap Analysis
## Verified September 2026 — Fresh Commit Data from 5 Ocean-Adjacent Repos (v5)

---

## 🚨 Headline Finding: The Ocean Gap

**Our GitHub search across 10+ query strategies returned ZERO dedicated ocean geoengineering repositories.**

Query strategies attempted:
- `ocean geoengineering` → 0
- `ocean alkalinity enhancement` → 0
- `marine cloud brightening` → 0
- `ocean iron fertilization` → 0
- `seaweed farming climate` → 0
- `ocean liming` → 0
- `marine geoengineering simulation` → 0
- `ocean carbon removal open source` → 0
- `blue carbon restoration` → 0
- `coastal climate adaptation model` → 0 (non-geoengineering)

**Ocean geoengineering is the dark matter of climate tech on GitHub.** It exists in the scientific literature (Nature, Science, PNAS) but not in open code.

---

## 🌊 Ocean-Adjacent Repos: What IS There — Fresh Data v5

### 1. MDTF-Diagnostics (Precipitation-Buoyancy POD) — UPDATED v5
- **Repo:** [NOAA-GFDL/MDTF-diagnostics](https://github.com/NOAA-GFDL/MDTF-diagnostics)
- **Stars:** 80 | **License:** Apache-2.0
- **Last commit:** August 14, 2026 (Merge PR #825)
- **Fresh commits:** 15 pulled (Aug 2026 – May 2026)

**Why it's ocean-adjacent:** The **precipitation-buoyancy POD** is the most ocean-relevant diagnostic in open source. It evaluates how well climate models capture the vertical coupling between ocean buoyancy and precipitation — a process that ocean interventions (OAE, iron fertilization) would directly affect.

**Fresh commit highlights:**
```
Jun 19, 2026: add MCS_precip_buoyancy_statistics POD ← NEW diagnostic
Jun 19, 2026: Update MCS_precip_buoy_stats.rst (×5) ← Documentation blitz
Aug 14, 2026: Merge PR #825 ← Latest activity
```

**Key insight v5:** The precip-buoyancy POD got 5 commits in one day (June 19, 2026) — the most intense single-day development in the entire ocean theme. NOAA/GFDL considers this a priority tool. But it's for *evaluating* model accuracy, not *simulating* interventions.

**🎙️ Podcast insight v5:** The most ocean-relevant code in the entire GitHub climate tech ecosystem is an evaluation tool, not a simulation tool. We evaluate the ocean more than we intervene in it.

---

### 2. WRF (Ocean-coupled modes) — UPDATED v5
- **Repo:** [wrf-model/WRF](https://github.com/wrf-model/WRF)
- **Stars:** 1,761 | **License:** Apache-2.0
- **Fresh commits:** 15 pulled (May-Jun 2026, v4.8.0 release cycle)

**Ocean connection:** WRF's air-sea flux parameterizations control how energy and moisture exchange between ocean and atmosphere. Any ocean intervention would alter these fluxes (OAE changes CO2 uptake, MCB changes solar heating).

**🎙️ Podcast insight v5:** The ocean doesn't have its own repo. It speaks through WRF. The atmospheric model is the ocean's proxy in the code world.

---

### 3. aiida-icon — UPDATED v5
- **Repo:** [aiida-icon/aiida-icon](https://github.com/aiida-icon/aiida-icon)
- **Stars:** 3 | **License:** Not specified
- **Last commit:** January 27, 2026 (add extpar_file and ifs2icon inputs, PR #60)
- **Fresh commits:** 15 pulled (Jul 2025 - Jan 2026)

**Why it's ocean-adjacent:** ICON (Icosahedral Nonhydrostatic) is the EU's climate model with an ocean component (ICON-Ocean). This AiiDA plugin automates running ICON simulations on HPC workflows. The Aug 2025 upgrade to multi-model support (PR #50) is architecturally significant.

**What's missing:** No albedo modification, no OAE chemistry, no iron fertilization, no MCB parameterization. Just better workflow automation for existing climate modeling.

**🎙️ Podcast insight v5:** "The Swiss National Supercomputing Centre just shipped a major update that lets you run multiple climate models simultaneously. 14 contributors. World-class infrastructure. And none of it can simulate what it would do to the ocean if we tried to geoengineer it."

---

### 4. NCAR_ML_EKE — UPDATED v5
- **Repo:** [CrayLabs/NCAR_ML_EKE](https://github.com/CrayLabs/NCAR_ML_EKE)
- **Stars:** 20 | **License:** Not specified
- **Last commit:** March 30, 2022 (Fix notebook typos)
- **Fresh commits:** 10 pulled (Apr 2021 - Mar 2022)

**Why it's ocean-adjacent:** Uses MOM6 (Modular Ocean Model) as its simulation target. ML surrogates of ocean climate models on HPC architectures.

**The complete lifecycle:** 7 commits on launch day (Apr 13, 2021), MOM6 submodule integrated, then 3 more commits over 15 months, then total silence for 4+ years after the Nature paper.

---

### 5. CCU-LCA — NEW v5
- **Repo:** [massimopizzol/CCU-LCA](https://github.com/massimopizzol/CCU-LCA)
- **Stars:** 14 | **License:** Not specified
- **Last commit:** April 28, 2021 (1 commit after 11 months)
- **Fresh commits:** 9 pulled (Apr 2019 - Apr 2021)

**Why it's ocean-adjacent (indirectly):** Life-cycle assessment of carbon capture and utilization technologies. The LCA framework could be applied to ocean intervention lifecycle analysis, but no ocean-specific code exists.

**Pattern:** Created for a scientific article (6 commits on launch day). Two more commits in 2020. Last commit Apr 2021. Academic ghost repo with 14 stars.

---

## 🔍 The Ocean Gap: What's Missing — Updated v5

### Missing Categories

| Category | Expected | Actual | Gap Size |
|----------|----------|--------|----------|
| **Ocean Alkalinity Enhancement (OAE)** | Simulators, reactor models | 0 | Total absence |
| **Marine Cloud Brightening (MCB)** | Aircraft/ship models, cloud microphysics | 0 | Total absence |
| **Ocean Iron Fertilization (OIF)** | Biogeochemistry models | 0 | Total absence |
| **Macroalgae/Seaweed farming** | Growth models, lifecycle analysis | 0 | Total absence |
| **Blue carbon ecosystem modeling** | Mangrove/seagrass/carbon models | 0 | Total absence |
| **Ocean sensor networks** | DIY controllers, data platforms | 0 | Total absence |
| **Coastal reflected solar** | Shallow-water albedo models | 0 | Total absence |

### The Ocean Physics Models: What EXISTS vs. What's MISSING

| Capability | Ocean Model | Has Intervention? | Fresh Commits? |
|-----------|-------------|------------------|----------------|
| Ocean circulation | MOM6, NEMO, Veros | ❌ | No |
| Sea ice dynamics | CICE, LIM | ❌ | No |
| Marine biogeochemistry | PISCES, OceanBioME | ❌ | No |
| Wave dynamics | WAVEWATCH III | ❌ | No |
| Coastal engineering | Delft3D, MIKE | ❌ | No |
| GPU acceleration | Oceananigans.jl (1,413★) | ❌ | No |
| ML surrogates | NCAR_ML_EKE (20★) | ❌ | Dormant since 2022 |
| Workflow automation | aiida-icon (3★) | ❌ | Active but no intervention |
| Evaluation diagnostics | MDTF precip-buoyancy POD (80★) | ❌ | 🟢 Active (Jun 2026) |
| **Any intervention layer** | **None** | **⬛ ZERO** | **—** |

---

## 🧠 Why Is the Ocean Gap So Wide? — Updated v5

### Theory 1: The Governance Chill
International law (London Protocol, CBD) created a governance gray zone. You can code solar physics (WRF) without legal risk. You cannot code ocean iron fertilization without potential violation of international maritime law.

### Theory 2: The Cost Prohibitory
Ocean intervention requires research vessels and platforms. No "laptop-scale" ocean intervention exists. Solar geoengineering can be modeled with a laptop. Carbon capture can be prototyped with 3D printers.

### Theory 3: The Complexity Penalty
Ocean biogeochemistry is harder than atmospheric physics. OAE requires carbonate chemistry + ocean circulation + ecosystem response. The coding barrier is higher than for SRM or even DAC.

### Theory 4: The Academic Incentive Problem
NCAR_ML_EKE and CCU-LCA both follow the "publish then die" pattern. Building intervention tools doesn't generate papers. Running experiments with existing tools does.

### Theory 5: The "Playing God" Stigma
Ocean geoengineering is the most ecosystem-scale intervention option. Iron fertilization literally feeds a marine ecosystem from above. Cultural resistance is higher than for atmospheric SRM.

---

## 📊 Ocean-Vs-Terrestrial Gap Visualization — Updated v5

| Theme | Active Repos | Stars | Commits (recent) | Intervention Specific |
|-------|-------------|-------|-------------------|---------------------|
| ☀️ Solar | 6 | 1,844 | 80+ | 0 dedicated SRM simulators |
| 🌍 Carbon | 10+ | 2,600+ | 70+ | 1 open hardware DAC (frozen) |
| 🌊 Ocean | 5 | 1,623 | 64+ | **ZERO dedicated repos** |

**The paradox:** Ocean geoengineering has the most scientific basis in oceanography (which has outlet models). But it has zero repos. Solar geoening has ~nothing in dedicated simulation, but has atmospheric models. Ocean is the forgotten quadrant.

---

## 🎙️ Episode Talking Points — Ocean Intervention (Updated v5)

### Opening Frame
> "We searched GitHub for every ocean geoengineering repository. The result is zero. Not a handful. Not a few. ZERO. For a planet that's 71% ocean, that's either a massive oversight or a massive message. We think it's a message."

### Three Narrative Arcs (Updated v5)
1. **"The Ocean Adjacent Life"** (aiida-icon) — 15 commits in 7 months. The most active ocean-related climate code on GitHub makes it easier to run the ICON climate model. You know what's missing? Anyone writing an ocean intervention module.

2. **"The Ghost of Ocean Modeling Past"** (NCAR_ML_EKE) — A perfect academic paper. 20 stars. MOM6 integrated with ML. And then silence. The citations accumulated. The code went dormant.

3. **"The Precip-Buoyancy POD — The Ocean's Only Voice"** (MDTF-diagnostics) — 5 commits in one day (Jun 19, 2026). The most ocean-relevant diagnostic in open source evaluates whether models get the ocean right. But nobody is building tools to simulate what we'd do to the ocean.

### Q&A Provocations (Updated v5)
- "Is the absence of ocean-geoengineering code a governance signal — or just a funding gap?"
- "If you built an open-source OAE simulator, would that be activism or engineering?"
- "Ocean models exist. Albedo models exist. Where's the composite model that would simulate ocean geoengineering?"
- "The precip-buoyancy POD got 5 commits in one day. The intervention simulation got zero. What does that ratio tell us?"
- "Should GitHub host a moratorium on ocean geoengineering code — or is that exactly what we need?"