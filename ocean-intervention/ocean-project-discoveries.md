# 🌊 Ocean-Based Geoengineering — Open-Source Project Discoveries

*Research pulled from GitHub: September 2026*

---

## The Big Finding: A Near-Empty Repository

The most striking discovery from this research round is the **structural absence** of dedicated ocean geoengineering repositories on GitHub. Unlike solar geoengineering (which has ClimateMARGO, climate_analogs, sai-climate-tradeoffs) and carbon capture (which has OpenCarbon, peroxovanadates, electro-swing DAC), ocean intervention has almost no standalone open-source codebase.

This is not an accident — it's a story about **experimental complexity, governance sensitivity, and institutional siloing**. Ocean geoengineering research (ocean alkalinity enhancement, iron fertilization, seaweed cultivation) lives in marine science institutions, not software developer communities. The podcast *must* foreground this finding.

---

## Existing Repositories (Thin Slice)

### 1. Team50-Labs/NebuGrid-OpenSource
| Field | Detail |
|---|---|
| **Language** | Not specified |
| **Stars / Forks** | 0 ⭐ / 0 🍴 |
| **Last Updated** | 5 Aug 2026 |
| **URL** | https://github.com/Team50-Labs/NebuGrid-OpenSource |

**What it does:** Fog-harvesting and drip irrigation systems — water extraction from coastal fog, paired with precision irrigation. Related to ocean-intervention-adjacent water management in arid coastal regions.

**Why it matters for the podcast:** This is the **closest proxy** for ocean-adjacent open-source climate tech on GitHub. It's not ocean geoengineering per se, but it couples coastal fog (an ocean-atmosphere process) with sustainable water infrastructure. The 0 stars and 5 Aug 2026 update show it's a small, active project trying to solve water scarcity at the ocean-land boundary. It could anchor a segment on "what ocean-related climate tech actually exists in the open."

---

### 2. protontypes/open-sustainable-technology (Hydrosphere/Ocean sections)
| Field | Detail |
|---|---|
| **Language** | Multi-language |
| **Stars / Forks** | 2,552 ⭐ / 330 🍴 |
| **Last Updated** | 9 Sep 2026 |
| **URL** | https://github.com/protontypes/open-sustainable-technology |

**What it does:** The "Hydrosphere" category includes subsections for:
- **Freshwater and Hydrology**
- **Ocean Models** — links to openoceancolor, HYCOM, ROMS, MOM, NEMO, and other ocean circulation models
- **Waves and Currents**
- **Ocean Carbon and Temperature** — links to projects tracking ocean carbon uptake
- **Coastal and Reefs** — links to coral reef monitoring and restoration tools
- **Ocean and Hydrology Data Access**

**Why it matters for the podcast:** The hydrosphere section of open-sustainable-technology is **the only curated list of open-source ocean modeling tools on GitHub**. Notably, it links to operational/commercial ocean models (HYCOM, ROMS, NEMO) but **no ocean geoengineering models**. The absence is deafening: the tools for modeling ocean circulation exist; the tools for modeling ocean *intervention* (alkalinity enhancement, iron fertilization, SST reduction via cloud brightening over oceans) are missing. This vacuum is the podcast's smoking gun.

---

### 3. prashaant1926/open-earth-digital-twin-simulation
| Field | Detail |
|---|---|
| **Language** | TeX (scientific paper + LaTeX) |
| **Stars / Forks** | 0 ⭐ / 0 🍴 |
| **Last Updated** | 10 Oct 2025 |
| **URL** | https://github.com/prashaant1926/open-earth-digital-twin-simulation |

**What it does:** An agent-based modeling platform for Earth's major environmental systems using real-time public data. The repository is structured as a full scientific research pipeline: concept → literature → hypothesis → data → experiment → analysis → paper. Includes a LaTeX manuscript (paper.tex).

**Why it matters for the podcast:** This is an **Earth system digital twin** — exactly the kind of modeling infrastructure needed to simulate ocean intervention scenarios. But the code is in LaTeX and agent-based modeling, not in the Fortran/C/MPI codes that would actually run on supercomputers. The single commit (Oct 2025) is an initialization — it's a research outline as much as runnable code. Still, the structure of the repo (Co-Sci methodology, JSON hypothesis/experiment tracking) is a model for how ocean intervention research *could* be organized if the open-source community took it seriously.

---

## Why the Ocean Intervention Gap Exists

### 1. Experimental Complexity
Ocean geoengineering requires **ocean-going vessels, large volumes of reagent (e.g., olivine sand for alkalinity enhancement), satellite monitoring, and years of observation**. You can't "fork" an ocean experiment the way you fork a code repository. The fundamental invisibility of the experiment to software developers creates the repository gap.

### 2. Governance Sensitivity
SAF (stratospheric aerosol injection) has its governance debates, but ocean intervention (especially iron fertilization) faced a **moratorium** after the famous 2012 Haida Salmon Restoration Corp. incident, where a company dumped 100 tonnes of iron sulfate into the Pacific without authorization. The governance stigma — "ocean geoengineering = rogue experimentation" — scares away institutional developers who would otherwise open-source the modeling tools.

### 3. Institutional Siloing
Ocean science is funded by marine institutes (Woods Hole, Scripps, GEOMAR, CSIRO Marine) with **closed procurement cultures**. The computational oceanographers who build models like MOM, NEMO, and HYCOM work at institutions that don't prioritize open-source software infrastructure (unlike, say, the climate-modeling community around E3SM or CESM). The "open" in their work means open data (CMIP6, satellite observations), not open experiment design.

### 4. The "Empty Quadrant" Narrative
Across GitHub, climate tech maps as a 2×2 matrix:

|  | Open Source | Closed/Proprietary |
|---|---|---|
| **Solar Geoengineering** | ClimateMARGO, climate_analogs, sai-climate-tradeoffs | GFDL models, NCAR CESM |
| **Carbon Capture** | OpenCarbon, peroxovanadates, electro-swing DAC | Climeworks, Carbon Engineering |
| **Ocean Intervention** | **Almost nothing** | Almost everything |
| **Energy/Atmosphere** | Thousands of repos (pvlib, windpowerlib, PyPSA) | Utility-scale models |

The ocean intervention cell is the **only genuinely empty quadrant**. There is no SRM-zeroDAC-zero energy-capture cell and no solar-zero ocean-zero cell — but the ocean intervention cell is truly vacant.

---

## What Ocean Intervention Would Need to Go Open-Source

### Tiered Approach

**Tier 1 — Open Data & Observation (Lowest Barrier)**
- Open ocean alkalinity monitoring (Buoy-based pH,Ω sensors with public API)
- Open seaweed/kelp growth monitoring (satellite + ground-truth datasets)
- Open iron fertilization observational datasets (WHERE, EIFEX, LOHAFEX data revived)
- GitHub equivalent: a `marine-geoengineering-data` organization hosting FAIR datasets

**Tier 2 — Open Modeling (Medium Barrier)**
- Open ocean alkalinity perturbation models (coupled from existing CESM/MOM frameworks)
- Open iron fertilization bloom prediction models
- Open seaweed carbon sequestration lifecycle models
- GitHub equivalent: a `ocean-geoengineering-models` repo with Docker container for reproducible runs

**Tier 3 — Open Experiment Design (Highest Barrier)**
- Open protocol templates for small-scale mesocosm experiments
- Open tracking of governance/regulatory approvals per experiment
- Open stakeholder engagement records (indigenous communities, fishing industries)
- GitHub equivalent: `ocean-geoengineering-experiments` as an ethical research framework, not a code repo

---

## Podcast Episode Angle

### The Hook
*"We can simulate solar geoengineering in open code, we can design DIY carbon capture machines — but where's the open-source ocean geoengineering? The answer reveals why the ocean is the final frontier of climate technology, and why the gap between what we model and what we deploy might be the most dangerous one."*

### Key Questions for the Episode
1. **Where is the code?** — The structural absence of ocean geoengineering repositories is the most striking finding of this research round.
2. **Why does the gap exist?** — A combination of experimental complexity (you can't fork an ocean), governance trauma (Haida incident moratorium), and institutional siloing (marine science cultures aren't software-engineer cultures).
3. **What would open-source ocean intervention look like?** — A three-tiered path: open data first, open models second, open experiment design third. None of this exists today.
4. **What's the ethical dimension?** — Open-source ocean geoengineering could democratize governance (many stakeholders monitoring) or accelerate rogue experiments (anyone with a boat and olivine). The code can't answer this — only institutions can.
5. **What's the role of the podcast listener?** — Listeners who care about ocean intervention can start by contributing datasets, not models. The GitHub entry point for ocean geoengineering is a FAIR dataset, not a Fortran codebase.

### Bottom Line
The ocean intervention gap is not a technical problem — it's a **governance, cultural, and ethical** problem that happens to manifest as a software/open-source problem. Any podcast that only talks about GitHub code will miss the deeper story. The code absence is a symptom; the ocean governance absence is the disease.
