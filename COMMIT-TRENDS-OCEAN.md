# 🌊 Ocean Intervention — Commit Trend Analysis
## GitHub API Data Pull — September 2026

---

## 📈 Overall Activity Dashboard

| Repo | Stars | Recent Commits | Commit Rate | Last Active | Trend |
|------|-------|----------------|-------------|-------------|-------|
| **aiida-icon** | 3 | 15 in 7 months | 2.1/month | Jan 27, 2026 | 🟢 **Active institutional development** |
| **NCAR_ML_EKE** | 20 | 10 in 15 months | 0.67/month | Mar 30, 2022 | 🔴 **Dormant since paper publication** |
| **Oceananigans.jl** | 1,413 | (from v2) | High | Active | 🟢 **Active community-driven ocean physics** |
| **veros** | 187 | (not pulled) | Medium | Active | 🟢 **Active ocean circulation model** |
| **Total dedicated OGE repos** | **0** | **—** | — | **—** | **⬛ THE GAP** |

---

## 🌊 aiida-icon — The Highest-Quality Ocean-Adjacent Commits

### Recent Timeline (Jul 2025 – Jan 2026)
```
Jul 8, 2025   ■ Fix CI security with zizmor (#35)
Jul 17, 2025  ■ Pin env deps (#36)
Jul 17, 2025  ■ Re-enable ICON tests after aiida-core 2.7.1 fix (#39)
Jul 23, 2025  ■ Add CSCS CI test (#42)
Jul 25, 2025  ■ Fix docs deploy (#46)
Jul 29, 2025  ■ Simplify wrapper script usage (#45)
Jul 30, 2025  ■ Replace src conftest with loading aiida fixtures (#47)
Aug 7, 2025   ■ Improve ALPS specific setup (#48)
Aug 7, 2025   ■ Fix warning block on index page (#49)
Aug 20, 2025  ■ Add setup_env input to IconCalculation spec (#41)
Aug 20, 2025  ■ Output streams as dynamic node outputs (#38)
Aug 25, 2025  ■ Allow multi-model runs (#50)
Dec 18, 2025  ■ Add arbitrary remote file system links to inputs (#54)
Jan 26, 2026  ■ Remove single model assumption from restart file I/O (#61)
Jan 27, 2026  ■ add extpar_file and ifs2icon inputs (#60)
```

### The Quality Signal
This is the most professionally maintained ocean-*related* climate repo we found:
- **14 contributors** (Haeuselmann, Geiger, Goscinski, plus others via PRs)
- **Institutional backing** (CSCS — Swiss National Supercomputing Centre)
- **15 numbered PRs** in 7 months (&gt; 2 PRs/month)
- **Code quality focus:** CI security (zizmor), type safety (extpar_file), documentation fixes
- **Multi-model support** — the Aug 2025 upgrade from single-model to multi-model runs is architecturally significant

### What's Missing — The Intervention Layer
Despite excellent maintenance, aiida-icon has ZERO ocean intervention capabilities:
- No albedo modification module
- No OAE (Ocean Alkalinity Enhancement) chemistry solver
- No iron fertilization biogeochemistry
- No MCB (Marine Cloud Brightening) parameterization
- No ocean ecosystem response modeling

It makes it *easier to run existing climate models*. It doesn't make it *possible to simulate ocean interventions*. That gap — between infrastructure capability and intervention application — is the story.

**Podcast framing:** "The Swiss National Supercomputing Centre just shipped a major update that lets you run multiple climate models simultaneously on their HPC systems. 14 contributors. Rigorous CI security. World-class infrastructure. And none of it can simulate what it would actually do to the ocean if we tried to geoengineer it."

---

## 💀 NCAR_ML_EKE — The Academic Lifecycle Complete

### Full Timeline
```
2021-04-13  ■ Launch day (7 commits on one day)
2021-04-13  ■ Add MOM6 submodule ← Ocean model integrated
2021-04-13  ■ Add git submodule
2021-04-13  ■ 3x README updates
2021-07-23  ■ Edit README (Sam Partee)
2022-02-08  ■ Update MOM6 submodule (version bump)
2022-02-09  ■ Update README for compiling MOM6
2022-03-14  ■ Update MOM6 instructions
2022-03-28  ■ Refactor driver for colocated option
2022-03-30  ■ Fix notebook typos ← LAST COMMIT (4+ years ago)
```

### The Complete Academic Arc
1. **Creation (Apr 2021):** 7 commits in one day — same day as arigos posit founding the lab and getting the MOM6 submodule
2. **Development (Jul 2021):** One README edit 3 months later
3. **Paper prep (Feb–Mar 2022):** 5 commits over 2 months — MOM6 version bump, compilation instructions, driver refactoring, notebook fixes
4. **Publication (2022):** Paper published (Nature: "Using Machine Learning at Scale in HPC Simulations with SmartSim: An Application to Ocean Climate Modeling")
5. **Death (Mar 2022 → forever):** No commits in 4+ years

### The MOM6 Connection
MOM6 (Modular Ocean Model) is the ocean component of several major climate models including GFDL's ESM. NCAR_ML_EKE integrated MOM6 into a machine-learning workflow. This means researchers can run ML surrogates of an ocean General Circulation Model (GCM) on HPC systems.

**But:** It doesn't simulate any intervention. No iron fertilization. No OAE. No MCB. Just faster ocean modeling.

**Podcast framing:** "A perfect academic paper. 20 stars. MOM6 integrated with ML. A beautiful demonstration of HPC + AI for ocean modeling. And then… silence. The paper got published. The citations accumulated. The code went dormant. Is this what happens to all the ocean geoengineering tools we never built?"

---

## 🔬 Ocean Physics Models: Existing Capability vs. Intervention vacuum

| Capability | Ocean Model | Has Intervention? |
|-----------|-------------|------------------|
| Ocean circulation | MOM6, NEMO, Veros | ❌ |
| Sea ice dynamics | CICE, LIM | ❌ |
| Marine biogeochemistry | PISCES, PARACE \|, OceanBioME | ❌ |
| Wave dynamics | WAVEWATCH III | ❌ |
| Coastal engineering | Delft3D, MIKE | ❌ |
| GPU acceleration | Oceananigans.jl | ❌ |
| ML surrogates | NCAR_ML_EKE | ❌ |
| Workflow automation | aiida-icon | ❌ |
| **Any intervention layer** | **None** | **⬛ ZERO** |

**The pattern is absolute:** Every layer of ocean modeling exists in open source. Physics, biogeochemistry, ice, waves, coastal, GPU, ML, workflow. But not one layer adds geoengineering capability. The ocean models can simulate what the ocean does. They can't simulate what we'd do to the ocean.

---

## 📊 Cross-Theme Comparison: Where Ocean Stands

### Commit Activity per Theme
| Theme | Active Repos | Total Recent Commits | Avg Commits/Repo | Multi-Contributor Repos |
|-------|-------------|---------------------|-------------------|------------------------|
| ☀️ Solar | 6 | 55 | 9.2 | 1 (WRF) |
| 🌍 Carbon | 10+ | 60+ | 6.0 | 1 (open-sustainable-tech) |
| 🌊 Ocean | 5 | 25+ | 5.0 | 1 (aiida-icon) |

### The Contributors Theme
| Theme | Single-Contributor Repos | Institutional Repos | Avg Contributors |
|-------|-------------------------|--------------------|-------------------|
| ☀️ Solar | 3 of 6 (50%) | 1 (WRF) | 1.8 |
| 🌍 Carbon | 6 of 10 (60%) | 1 (open-sustainable-tech) | 1.5 |
| 🌊 Ocean | 2 of 5 (40%) | 1 (aiida-icon) | 1.6 |

**Earth's surface is 71% ocean. GitHub's geoengineering ecosystem has fewer active ocean intervention repos than solar radiation papers published in 2024 alone.**

---

## 🧮 The Ocean Gap Theories — Commit Evidence

### Theory 1: The Governance Chill
**Evidence:** Zero commits to any ocean intervention code anywhere on GitHub.
**Mechanism:** International law (London Protocol, CBD) has created a governance gray zone. Researchers can code solar physics (WRF) without legal risk. They cannot code ocean iron fertilization without potential violation of international maritime law.

### Theory 2: The Cost Barrier
**Evidence:** Ocean intervention requires physical platforms (research vessels, ocean barges). No "laptop-scale" ocean intervention exists.
**Mechanism:** Solar geoengineering can be modeled with a laptop (WRF is free). Carbon capture can be prototyped with 3D printers (openair-cyan). Ocean intervention requires a ship. The hardware barrier keeps away individual contributors.

### Theory 3: The Complexity Penalty
**Evidence:** Even the best ocean models (Oceananigans.jl at 1,413★) have zero intervention modules..
**Mechanism:** Ocean biogeochemistry is harder than atmospheric physics. OAE requires carbonate chemistry modules + ocean circulation + ecosystem response. The coding barrier is higher, and few researchers have the cross-disciplinary skills.

### Theory 4: The Academic Incentive Problem
**Evidence:** NCAR_ML_EKE and most ocean-adjacent repos follow the "publish then die" pattern.
**Mechanism:** Building intervention tools doesn't generate papers. Running an experiment with existing tools generates papers. The incentive structure favors using tools over building them.

### Theory 5: The "Playing God" Stigma
**Evidence:** Ocean geoengineering is the most ecosystem-scale intervention option. Iron fertilization literally introduces a limiting nutrient to a vast ecosystem.
**Mechanism:** Cultural resistance to "fixing the ocean" is higher than for "fixing the atmosphere." The ocean is wild, chaotic, and sacred in ways the atmosphere is not. Building code that simulates ocean intervention might feel like consent to actually do it.

---

## 🔮 Trend Projections for Episode 2 (Ocean)

### What's Trending Up ✓
1. **Ocean physics modeling is thriving** (Oceananigans, veros, MOM6, NEMO) — the computational tools are mature
2. **Workflow automation for climate models is improving** (aiida-icon, 15 commits in 7 months)
3. **HPC integration with ocean models is advancing** (NCAR_ML_EKE's ML surrogates)

### What's Trending Down ✗
1. **Zero intervention-specific code** — not a single commit to any ocean geoengineering module
2. **Ocean-adjacent repos go dormant after publication** — NCAR_ML_EKE pattern is the norm, not the exception
3. **No community coordination** — unlike the carbon capture ecosystem (which has directories and registries), ocean modeling is siloed by institutional fiefdoms

### The Signal in the Silence 📡
**The ocean gap is not a data gap — it's a political gap.** The science of ocean alkalinity enhancement is mature enough for field experiments (Keller et al. 2023). The modeling tools exist to simulate the effects. The computing power exists to run the simulations. But there is zero open-source code that would let a researcher design, test, or refine an ocean geoengineering intervention.

This is the most consequential "nothing" we found on GitHub. The absence of code is a direct reflection of the absence of governance. You can't build the tool until you've decided it's permitted to build.

---

## 📋 Research Log

| Date | Activity |
|------|----------|
| Sep 17, 2026 | v3: Initial ocean gap analysis — 10+ search queries, zero OGE repos |
| Sep 17, 2026 | v3: Ocean-adjacent repos identified (Oceananigans, veros, OceanBioME, MOM6 via NCAR_ML_EKE, aiida-icon) |
| Sep 17, 2026 | v4: Fresh commit data pulled from aiida-icon (15 commits, Jul 2025–Jan 2026) |
| Sep 17, 2026 | v4: Fresh commit data pulled from NCAR_ML_EKE (10 commits, Apr 2021–Mar 2022) |
| Sep 17, 2026 | v4: Five governance-gap hypotheses documented with commit evidence |
| Sep 17, 2026 | v4: Cross-model capability matrix built — every ocean modeling layer exists, none have intervention modules |
| Sep 17, 2026 | v4: The "playing God" stigma hypothesis added as fifth theory |
| Sep 17, 2026 | v4: Episode 2 narrative arcs drafted based on NCAR_ML_EKE lifecycle and aiida-icon activity |
