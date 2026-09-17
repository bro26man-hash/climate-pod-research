# 🌊 Ocean Intervention — Research Notes (Updated Sep 2026)

## Project Discoveries

### 1. CrayLabs/NCAR_ML_EKE
- **URL:** https://github.com/CrayLabs/NCAR_ML_EKE
- **Language:** Jupyter Notebook
- **Stars:** 20
- **Contributors:** Andrew Shao, Sam Partee (NCAR)
- **Description:** "Using Machine Learning at Scale in HPC Simulations with SmartSim: An Application to Ocean Climate Modeling." Demonstrates applying machine learning (via SmartSim AI+HPC orchestration) to accelerate ocean climate simulations using the MOM6 ocean model and CESM2 framework.
- **Last Activity:** March 30, 2022
- **Commit Count:** 10 shown (4 in 2022, 6 in 2021 — activity concentrated in paper publication period)
- **Key commits:**
  - Mar 30, 2022: "Fix notebook typos (#10)"
  - Mar 28, 2022: "Refactor driver to support colocated option (#9)"
  - Mar 14, 2022: "Update MOM6 instructions and submodule"
  - Feb 9, 2022: "Update README for compiling MOM6"
  - Feb 8, 2022: "Update MOM6 submodule"
  - Jul 2021 + Apr 2021: Multiple README updates + LICENSE creation
- **Relevance:** The closest thing to open-source ocean climate simulation tooling. ML+HPC fusion could eventually make ocean geoengineering simulations tractable — but this repo predates that application and doesn't address OAE, iron fertilization, or other marine interventions directly.

### 2. jnickla1/CESM2geoeng_documentation
- **URL:** https://github.com/jnickla1/CESM2geoeng_documentation
- **Language:** Not specified
- **Description:** Documentation for the ocean geoengineering CESM2 paper. The CESM2 (Community Earth System Model v2) is the most sophisticated Earth system model capable of simulating ocean-based geoengineering scenarios including Marine Cloud Brightening (MCB), Ocean Alkalinity Enhancement (OAE), and Arctic MCB.
- **Last Activity:** Repository is **EMPTY** — no commits, no files, no code.
- **Relevance:** The existence of this empty repo — linked from a published scientific paper — is the most significant finding in this entire research effort. The simulation code likely exists within the main CESM2 repository under an undocumented geoengineering component, but no one has extracted, documented, or maintained geoengineering-specific ocean modules.

### 3. No Dedicated Ocean Geoengineering Repositories Found

After extensive searching across **multiple query strategies** including:
- "ocean geoengineering" → 0 dedicated repos
- "ocean alkalinity enhancement" → 0 dedicated repos
- "iron fertilization simulation" → 0 dedicated repos
- "marine cloud brightening" → 0 dedicated repos
- "seaweed geoengineering" → 0 dedicated repos
- "ocean computing climate" → Adjacent only (NCAR_ML_EKE)
- "climate intervention ocean" → Adjacent only (CESM2geoeng_doc — empty)

...no open-source repositories specifically implementing ocean geoengineering simulations were found.

### 4. Tangentially Relevant (from broader search)
- **protontypes/open-sustainable-technology** (2,546★) — Umbrella directory that may catalog ocean-related projects hidden within
- **Team50-Labs/NebuGrid-OpenSource** — Smart fog-harvesting system, water-cycle analog but not ocean geoengineering

---

## The Ocean Intervention Gap — Full Analysis

### The Core Finding
Ocean geoengineering is the "dark matter" of climate tech on GitHub — it exists in the scientific literature but not in open code.

### Evidence Table

| Search Strategy | Repos Found |
|----------------|-------------|
| "ocean geoengineering" | 0 dedicated repos |
| "ocean alkalinity enhancement" | 0 dedicated repos |
| "iron fertilization simulation" | 0 dedicated repos |
| "marine cloud brightening" | 0 dedicated repos |
| "seaweed geoengineering" | 0 dedicated repos |
| "ocean computing climate" | Adjacent only (NCAR_ML_EKE) |
| "climate intervention ocean" | Adjacent only (CESM2geoeng_doc — empty) |

### Why This Matters

1. **Governance Vacuum:** If no one has built open-source tools for ocean geoengineering, who sets the technical standards? The silence on GitHub mirrors the silence in international governance frameworks. The London Convention/London Protocol governing ocean fertilization has no digital compliance tools.

2. **Barrier to Entry:** Without open models, small research teams and developing nations cannot participate in ocean geoengineering research. This centralizes expertise in a handful of well-funded institutions (NCAR, GFDL, ETH Zurich, GEOMAR Kiel) and effectively makes ocean geoengineering a tool of the Global North.

3. **Reproducibility Crisis:** Scientific papers on ocean geoengineering (e.g., the CESM2 geoengineering paper) lack accompanying code or data repositories. Results are impossible to verify, reproduce, or build upon. Fundamentally at odds with open science principles.

4. **Comparison With Other Domains:**

| Theme | # Repos Found | Top Repo Stars |
|-------|--------------|----------------|
| Solar Geoengineering | 4 | 4 (Legacy) + 73 (ClimateMARGO) |
| Carbon Capture + CDR | 4+ | 2,546 (directory) + active APIs |
| Ocean Intervention | 0+ | 0 (empty) |

5. **The Empty CESM2geoeng_documentation Story:** A published scientist created a GitHub repository for documenting ocean geoengineering simulations in CESM2, then abandoned it with zero files. The code may exist somewhere in the CESM2 main repo, undocumented and inaccessible. This is the pipeline: paper → empty repo → nothing. The ultimate expression of the gap.

### What Should Exist (But Doesn't)

| Intervention Type | Simulation Need | Status |
|-------------------|----------------|--------|
| **Ocean Alkalinity Enhancement (OAE)** | Dissolution rates, carbon sequestration efficiency, ocean chemistry changes, ecosystem impacts | No open code |
| **Iron Fertilization** | Phytoplankton bloom modeling, carbon export efficiency, food web cascades | No open code |
| **Seaweed / Marine Biomass** | Growth modeling, carbon sequestration calculations, ecosystem interactions | No open code |
| **Marine Cloud Brightening (MCB)** | Droplet activation, cloud microphysics, radiative effects, atmospheric coupling | No open code |
| **Coastal Upwelling** | Deep water nutrient transport, carbon pump efficiency, local ecosystem effects | No open code |

---

## Commit Trend Analysis

| Repository | Commits | Last Commit | Activity |
|------------|---------|-------------|----------|
| NCAR_ML_EKE | 10 (shown) | Mar 30, 2022 | Dormant — research completion |
| CESM2geoeng_documentation | 0 | Never created files | **Empty repo** |

### Key Trends

1. **Complete absence of ocean geoengineering code:** Across all search queries, zero dedicated ocean intervention repositories were found. This is not a niche gap; it's a void.

2. **Even adjacent fields are dormant:** NCAR_ML_EKE, the most relevant ocean climate modeling tool, hasn't been updated since March 2022. The ML+HPC ocean modeling community has dispersed after the paper publication.

3. **Paper → Empty repo → Nothing:** The CESM2 ocean geoengineering paper produced an empty GitHub repository. This suggests the simulation code exists only within the main CESM2 codebase, undocumented for geoengineering applications.

4. **The silence is itself a governance signal:** The absence of ocean geoengineering code on GitHub is not a technical accident; it reflects institutional caution, funding gaps, and political discomfort. The repo is empty because the field itself is empty of open-source infrastructure.

5. **The WRF ocean module paradox:** WRF (1,761★, actively updated) has an ocean coupling (WOF) but it models atmosphere-ocean interaction for weather forecasting — not ocean geoengineering scenarios. The most popular climate tool on Earth doesn't include intervention scenarios.

---

## Episode Questions for Ocean Intervention

1. **Why is ocean geoengineering the empty quadrant?** Of all the climate intervention domains, ocean intervention has the least open-source infrastructure. Is this a scientific challenge, a governance problem, or both?

2. **What would open-source OAE look like?** If you were going to build the first open-source ocean alkalinity enhancement simulation, what would you model? What data would you need? Who would you collaborate with?

3. **Is the silence itself a governance signal?** The London Convention governs ocean fertilization, but there are no digital compliance tools, no open models, no public data. Does the absence of code mean the absence of political will?

4. **Can ML unlock ocean geoengineering simulation?** NCAR_ML_EKE demonstrated ML+HPC for ocean climate modeling. Could the same techniques accelerate ocean intervention simulations? What would it take to apply SmartSim-style ML to OAE or MCB?

5. **Should we build it?** If ocean geoengineering simulation tools don't exist, should the podcast episode call for building them? Is open-source ocean intervention the next frontier — or should we focus on mitigation instead?

---

## What Would the First Open-Source Ocean Intervention GitHub Repo Look Like?

### Proposed: open-oae-simulator
- **Name:** `open-oae-simulator` or `oceancarbon-sim`
- **Language:** Python (accessible) + Julia (performance) for heavy computations
- **Modules:**
  - Carbonate chemistry solver (OAE dissolution kinetics)
  - Ocean transport model (alkalinity spreading)
  - Ecosystem impact model (phytoplankton, benthic effects)
  - Carbon sequestration accounting (net vs. gross)
  - Scenario runner (different deployment scales)
- **Data:** Publicly available ocean chemistry data (NOAA, ETH Zurich)
- **License:** MIT or Apache 2.0
- **Governance:** Multi-institutional (GEOMAR, WHOI, MIT) advisory board

### Why It Doesn't Exist Yet
1. No one has done it (the gap itself is the finding)
2. Funding doesn't support tool development — it supports publications
3. Institutional risk aversion — no lab wants to be associated with "ocean manipulation code"
4. Complexity — the first version would be simplified and maybe not credible

---

*Research compiled from GitHub repository search and commit history analysis. Sources: CrayLabs/NCAR_ML_EKE, jnickla1/CESM2geoeng_documentation, protontypes/open-sustainable-technology.*