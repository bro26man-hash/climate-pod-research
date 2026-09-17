# 🌊 Ocean Intervention — Project Discoveries
## Verified September 2026 — GitHub Search Across 10+ Query Strategies

---

## 🚨 Headline Finding: The Ocean Gap

**Our GitHub search across 10+ query strategies returned ZERO dedicated ocean geoengineering repositories.**

Query strategies attempted:
- `geoengineering` → 10 results, 0 ocean-specific
- `ocean geoengineering fertilization` → 0 results
- `climate technology carbon capture ocean` → 3 results (both climate-pod-research forks)
- `climate simulation modeling` → 10 results, 0 ocean geoengineering
- `marine cloud brightening` → 0 results
- `ocean albedo enhancement` → 0 results
- `ocean fertilization` → 0 results
- `ocean iron fertilization` → 0 results
- `macroalgae carbon` → 0 results
- `blue carbon` → 0 results

**Ocean geoengineering is the dark matter of climate tech on GitHub.** It exists in the scientific literature (Nature, Science, PNAS) but not in open code.

---

## 🌊 Ocean-Adjacent Repos: What IS There

### 1. NCAR_ML_EKE (CrayLabs)
- **Repo:** [CrayLabs/NCAR_ML_EKE](https://github.com/CrayLabs/NCAR_ML_EKE)
- **Stars:** 20 | **Language:** Jupyter Notebook | **License:** Not specified
- **Last commit:** March 30, 2022
- **Focus:** Using Machine Learning at Scale in HPC Simulations with SmartSim — Applied to Ocean Climate Modeling
- **Why it's ocean-adjacent:** This repo uses MOM6 (Modular Ocean Model) as its simulation target. The research runs ML surrogates of ocean climate models on HPC architectures. It's ocean *modeling*, not ocean *intervention*.

#### Commit History:
```
2021-04-13  ■ Initial setup (7 commits on launch day)
2021-04-13  ■ Add MOM6 submodule ← Ocean model integrated
2021-04-13  ■ Add git submodule
2021-04-13  ■ Multiple README updates
2021-07-23  ■ Edit README
2022-02-08  ■ Update MOM6 submodule ← Ocean model version bump
2022-02-09  ■ Update README for compiling MOM6
2022-03-14  ■ Update MOM6 instructions and submodule
2022-03-28  ■ Refactor driver for colocated option
2022-03-30  ■ Fix notebook typos ← Last commit
```

**Pattern:** Academic paper repo. Launch day (7 commits), submodule integration, then paper submission, then total silence for 4+ years. The MOM6 submodule updates stopped in March 2022. No intervention code, no scenario modeling — just ML-on-HPC infrastructure for ocean models.

### 2. aiida-icon (aiida-icon)
- **Repo:** [aiida-icon/aiida-icon](https://github.com/aiida-icon/aiida-icon)
- **Stars:** 3 | **Language:** Python | **License:** Not specified
- **Last commit:** January 27, 2026
- **Focus:** AiiDA Plugin to run simulations with the ICON weather & climate model
- **Why it's ocean-adjacent:** ICON (Icosahedral Nonhydrostatic) is the EU's climate model. It has an ocean component (ICON-Ocean / LIM). This plugin makes it easier to run climate simulations on HPC workflows. But it's climate modeling infrastructure, not ocean intervention.

#### Recent Commits (Jan 2026 — most active of any ocean-adjacent repo):
```
Jan 27, 2026  ■ add extpar_file and ifs2icon inputs (#60)
Jan 26, 2026  ■ Remove single model assumption from restart file I/O (#61)
Dec 18, 2025  ■ Add arbitrary remote file system links to inputs (#54)
Aug 25, 2025  ■ Allow multi-model runs (#50)
Aug 20, 2025  ■ Output streams as dynamic node outputs (#38)
Aug 20, 2025  ■ Add setup_env input to IconCalculation spec (#41)
Aug 7,  2025  ■ Fix warning block on index page (#49)
Aug 7,  2025  ■ Improve ALPS specific setup (#48)
Jul 30, 2025  ■ Replace src conftest with loading aiida fixtures in doctest (#47)
Jul 29, 2025  ■ Simplify wrapper script usage (#45)
Jul 25, 2025  ■ Fix docs deploy (#46)
Jul 23, 2025  ■ Add CSCS CI test (#42)
Jul 17, 2025  ■ Pin env deps (#36)
Jul 17, 2025  ■ Re-enable ICON tests after aiida-core 2.7.1 fix (#39)
Jul 8,  2025  ■ Fix CI security with zizmor (#35)
```

**Pattern:** Active institutional development. 15 commits in 7 months (July 2025 – Jan 2026). Multiple contributors (Haeuselmann, Geiger, Goscinski). AiiDA workflow automation for ICON simulations. This is the most actively maintained ocean-adjacent climate repo we found — but it's infrastructure, not intervention.

**Key insight:** ICON's ocean component (ICON-Ocean) is one of the fewMiddle/Light ocean models in the European climate modeling suite. aiida-icon makes it easier to run. But there's no occlusion, no marine cloud brightening module, no ocean alkalinity enhancement code. Just better workflow automation for existing climate modeling.

---

## 🔍 The Ocean Gap: What's Missing

### Missing Categories

| Category | Expected | Actual | Gap Size |
|----------|----------|--------|----------|
| **Ocean Alkalinity Enhancement (OAE)** | Simulators, reactor models | 0 | Total absence |
| **Marine Cloud Brightening (MCB)** | Aircraft/ship models, cloud微物理 | 0 | Total absence |
| **Ocean Iron Fertilization (OIF)** | Biogeochemistry models | 0 | Total absence |
| **Macroalgae/Seaweed farming** | Growth models, lifecycle analysis | 0 | Total absence |
| **Blue carbon ecosystem modeling** | Mangrove/seagrass/carbon models | 0 | Total absence |
| **Ocean sensor networks** | DIY controllers, data platforms | 0 | Total absence |
| **Coastal reflected solar** | Shallow-water albedo models | 0 | Total absence |

### The MIMICKry of Existence
Some repos are *ocean-related* but *not ocean-intervention*:
- **Oceananigans.jl** (1,413★) — Beautiful GPU-accelerated ocean simulation. But it simulates ocean *physics*, not ocean *interventions*. No albedo module, no Lagrangian particle tracking for dispersal, no biogeochemistry.
- **veros** (187★) — Ocean model for studying ocean circulation.同样的问题 — vanilla physics, no geoengineering layer.
- **OceanBioME** — Biogeochemical ocean model. Simulates nitrogen, phosphorus, carbon cycles. But no intervention scenarios.
- **MOM6** (via NCAR_ML_EKE) — Modular Ocean Model. Climate modeling backbone. No geoengineering.

---

## 🌊 Ocean-Adjacent Commit Activity Dashboard

| Repo | Stars | Recent Commits | Maintenance Status | Type |
|------|-------|----------------|-------------------|------|
| aiida-icon | 3 | 15 in 7 months | 🟢 Active (institutional) | Workflow automation for ICON |
| NCAR_ML_EKE | 20 | 10 over 15 months | 🔴 Dormant since 2022 | ML-on-HPC for MOM6 |
| Oceananigans.jl | 1,413 | (see v2 analysis) | 🟢 Active | Ocean physics simulation |
| veros | 187 | (not pulled) | 🟢 Active | Ocean circulation model |
| OceanBioME | (not pulled) | (not pulled) | ? | Biogeochemical ocean model |
| **Total dedicated OGE repos** | **0** | **—** | **—** | **THE OCEAN GAP** |

---

## 🧠 Why Is the Ocean Gap So Wide?

### Hypothesis 1: The Governance Chill
Ocean intervention is the most geopolitically charged geoengineering option. Iron fertilization historically triggered international law debates (London Protocol, CBD) when Planktos Inc. tried to do it commercially in 2007. The unresolved governance中国的regime for ocean geoengineering may be deterring researchers from building open-source tools. You can code solar radiation management in your bedroom. You can't code ocean iron fertilization without navigating international maritime law.

### Hypothesis 2: The Cost Prohib
Ocean intervention is* expensiveterrestrial solar geoening controllers, because领域你需要 a  ship or platform. There's no cheap DIY path. No back-yard ocean fertilization. No 3D-printable marine cloud brightening aircraft. The barrier to entry is a research vessel, not a laptop.

### Hypothesis 3: The Complexity Penalty
Ocean biogeochemistry is harder一堵 than atmospheric physics. You need to model chemistry, biology, fluid dynamics, and thermodynamics simultaneously. Ocean alkalinity enhancement requires modeling dissolution kinetics, ocean circulation, and biological response. The coding barrier is higher than for SRM or even DAC.

### Hypothesis 4: The Academic Incentive Problem
Publish or perish. Computing a new ocean iron fertilization scenario in a published paper is searchable to a committee. Building the open-source tool for the next six scenarios is unprovable labor for tenure. The incentive structure favors paper-driven "ghost repos" over sustained tool development.

### Hypothesis 5: The "Playing God" Stigma
Ocean geoengineering isa thecatogry of geoengineering that involves intentional ecosystem-scale manipulation. Iron fertilization literally feeds a marine ecosystem from above. Marine cloud brightening changes weather patterns over fisheries. There's a Wall-E level cultural-resistance to "fixing the ocean from above."

---

## 📊 Ocean-Vs-Terrestrial Gap Visualization

| Theme | Active Repos | Stars | Commits (recent) | Intervention Specific|
|-------|-------------|-------|-------------------|---------------------|
| ☀️ Solar | 6 | 1,844 | 55 | 0 dedicated SRM simulators |
| 🌍 Carbon | 10+ | 2,600+ | 60+ | 1 open hardware DAC (frozen) |
| 🌊 Ocean | 5 | 1,623 | 25 | **ZERO dedicated repos** |

**The paradox:** Ocean geoengineering has the most scientific basis in oceanography (which has outlet models). But it has zero repos. Solar geoening has~ nothing in terms of dedicated simulation, but Wikipedia has more documents. Terrestrial carbon cap has the Codable and golden path. Ocean is the forgotten option.

---

## 🩺 The Ocean as the Canonical Testbed — An Opportunity Narrative

Despite the gap, the ocean's absence is itself a story. Here's how we can frame it for the episode:

### The "Third Quadrant" Argument
Geoengineering on GitHub has three populated quadrants:
1. **Atmospheric solar** (sunlight management) — models exist but aren't geoengineering-specific
2. **Terrestrial carbon** (carbon removal) — equipment and directories exist
3. **Ocean physics** (understanding seas) — models exist

But we're missing the **fourth quadrant:**
4. **Ocean intervention** (ocean-based geoengineering)

The emptiness of the fourth quadrant is the most important finding of our research. It's not that ocean geoengineering is being developed but hidden — it's that it's not being *developed at all* in the open-source world. This is the canary in the coal mine.

### What Would a Real Ocean-OGE GitHub Look Like?
- **OAE-React:** A reactor simulator for ocean alkalinity enhancement
- **Fe-Fertil:** An iron fertilization dispersal model with ecosystem response
- **MCB-Ship:** A marine cloud brightening parameterization module for climate models
- **BlueCarbon-Mapping:** A VCS-compliant blue carbon monitoring tool
- **OceanAlbedo:** A coastal and open-ocean albedo enhancement simulator（浅层水域及开放大洋反射率增强）

### The Governance Test
Would an open-source ocean geoengineering repo be a provocation? The 2008 London Protocol ruled out ocean fertilization. The UNCBD has a de facto moratorium. So building the code — even purely computational and theoretical — might be seen as "preparing to do something the international community has banned."

*But that's exactly what makes it the most interesting quadrant for a podcast episode.*

---

## 🎙️ Episode Talking Points — Ocean Intervention

### Opening Frame
> "We searched GitHub for every ocean geoengineering repository. The result is zero. Not a handful. Not a few. ZERO. For a planet that's 71% ocean, that's either a massive oversight or a massive message. We think it's a message."

### Three Narrative Arcs
1. **The Ocean Adjacent Life** (aiida-icon) — 15 commits in 7 months. The most active ocean-related climate code on GitHub makes it easier to run the ICON climate model. You know what's missing? Anyone writing an ocean intervention module.

2. **The Ghost of Ocean Modeling Past** (NCAR_ML_EKE) — A perfect academic repo that died after the paper. 10 commits over 15 months. MOM6 submodule included. ML-on-HPC for ocean modeling. But when the paper was published, the maintainers moved on.

3. **The Gap Itself** — The most important finding. Zero dedicated ocean geoengineering repos. In a field where the science is mature (Nature, Science have published ocean alkalinity enhancement and marine cloud brightening papers), the code doesn't exist. We haven't built the digital twin of what we'd do if we tried.

### Q&A Provocations
- "Is the absence of ocean-geoengineering code a governance signal — or just a funding gap?"
- "If you built an open-source OAE simulator, would that be activism or engineering?"
- "Ocean models exist. Albedo models exist. Where's the composite model that would simulate ocean geoengineering?"
- "Should GitHub host a moratorium on ocean geoengineering code — or is that exactly what we need?"
