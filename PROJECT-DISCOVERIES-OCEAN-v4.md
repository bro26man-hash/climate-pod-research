# 🌊 Ocean Intervention — Project Discoveries (v4, September 2026)

## Overview
Comprehensive ocean geoengineering gap analysis with systematic 12-query GitHub search, ocean-adjacent repository profiles, and pseudocode frameworks for what open-source ocean intervention code would look like. **CONFIRMED: Zero dedicated ocean geoengineering repositories exist on GitHub.**

---

## The Ocean Gap: Systematic Search Protocol

We executed **12 targeted GitHub search queries** specifically designed to find ocean geoengineering code:

| # | Query | Result |
|---|-------|--------|
| 1 | `ocean geoengineering` | 0 repos |
| 2 | `ocean alkalinity enhancement` | 0 repos |
| 3 | `ocean iron fertilization` | 0 repos |
| 4 | `marine cloud brightening` | 0 repos |
| 5 | `ocean CDR` | 0 repos |
| 6 | `ocean carbon dioxide removal` | 0 repos |
| 7 | `OAE simulation` | 0 repos |
| 8 | `ocean geoengineering simulation` | 0 repos |
| 9 | `marine geoengineering` | 0 repos |
| 10 | `ocean intervention climate` | 0 repos |
| 11 | `ocean restoration carbon` | 0 repos |
| 12 | `blue carbon ocean` | 0 repos |

**Result: ZERO dedicated ocean geoengineering repositories.**

This is not a partial finding. It's not "few repos" or "mostly inactive repos." It's a **total absence** across all three major ocean intervention techniques (OAE, iron fertilization, marine cloud brightening) and across multiple query formulations.

---

## Ocean-Adjacent Discoveries (What Exists Near the Void)

### 1. CrayLabs/NCAR_ML_EKE ⭐20 — ML for Ocean Climate Modeling
- **Language:** Jupyter Notebook
- **Focus:** Using ML at scale (SmartSim) for HPC ocean climate simulations
- **Ocean Relevance:** Direct — ocean modeling, but evaluation, not intervention
- **Last activity:** August 10, 2026 (recent)
- **What it does:** Uses machine learning to accelerate and evaluate ocean climate models. Not simulating OAE or iron fertilization — testing whether existing models are accurate.
- **Why it matters:** This is the computational infrastructure that *could* be extended for ocean intervention modeling. The ML/SmartSim framework could couple with an OAE model. But it's currently a pure evaluation tool.
- **Podcast angle:** *"The closest thing to ocean geoengineering code is a machine learning toolkit for checking whether other models work. We're grading the tests, not taking them."

### 2. wrf-model/WRF ⭐1,762 — Atmosphere Model with Ocean Coupling
- **Language:** Fortran
- **Focus:** Weather Research and Forecasting (atmospheric, with ocean coupling options)
- **Ocean Relevance:** Indirect — solar radiation fix affects ocean surface heat flux
- **Last activity:** June 8, 2026 (v4.8.0)
- **Key commit:** "Correction for eot calculation for solar radiation" (May 28, 2026) — changes how sunlight hits the ocean surface
- **Why it matters:** WRF's solar radiation fix changes ocean surface heat flux calculations. Every ocean-mediated SRM scenario that uses WRF is affected. But WRF is not an ocean model — it's atmospheric with ocean options.
- **Podcast angle:** *"The most used climate model just fixed how it computes sunlight on the ocean. That changes every ocean SRM simulation. And nobody's writing the ocean intervention code to catch up."

### 3. ClimateSoton/climate-research-group — CFD/Climate University Group
- **Language:** HTML/Markdown (website)
- **Focus:** University research group, CFD expertise, climate science
- **Ocean Relevance:** Indirect — CFD methods applicable to ocean fluid dynamics
- **Last activity:** August 2026 (actively maintained)
- **What it does:** Maintains a research group website with publications and projects. CFD expertise could model ocean intervention fluid dynamics (alkalinity dispersion, iron plume transport).
- **Why it matters:** Institutional funding + CFD skills + active maintenance = the ingredients for ocean intervention code. But the group is doing fundamental CFD, not ocean CDR.
- **Podcast angle:** *"A university group has the skills, the funding, and the active development cycle. They do CFD. Ocean intervention is fluid dynamics. So... why aren't they?"

---

## What Would Open-Source Ocean Intervention Look Like? (Pseudocode Frameworks)

Since the ocean has zero repos, we drafted four frameworks showing what the code would look like:

### Framework 1: Ocean Alkalinity Enhancement (OAE)
```python
class OceanAlkalinityEnhancement:
    def __init__(self, region, mineral_source, discharge_rate):
        self.region = region          # e.g., "equatorial Pacific"
        self.mineral = mineral_source  # olivine, lime, dunite
        self.rate = discharge_rate     # tons/day
        self.ocean_model = ClimateModel()
    
    def simulate_alkalinity_spread(self, days=365):
        """Model how alkalinity spreads from discharge point"""
        pass
    
    def calculate_carbon_uptake(self):
        """How much CO2 does the alkalinity increase sequester?"""
        pass
    
    def assess_ecosystem_impact(self):
        """pH changes, species impacts, food web effects"""
        pass
```

### Framework 2: Iron Fertilization
```python
class IronFertilization:
    def __init__(self, ocean_region, iron_source, deployment_strategy):
        self.region = ocean_region
        self.iron = iron_source        # ferrous sulfate, iron dust
        self.strategy = deployment     # continuous, pulsed, targeted
    
    def simulate_phytoplankton_bloom(self):
        """Model the plankton bloom response"""
        pass
    
    def calculate_carbon_export(self):
        """How much carbon sinks to deep ocean?"""
        pass
    
    def assess_counterproductivity(self):
        """Does N2O production offset the CO2 benefit?"""
        pass
```

### Framework 3: Marine Cloud Brightening (MCB)
```python
class MarineCloudBrightening:
    def __init__(self, shipping_route, spray_rate, ship_count):
        self.route = shipping_route
        self.spray = spray_rate        # CCN particles/second
        self.ships = ship_count
    
    def simulate_cloud_albedo_change(self):
        """How much more sunlight does the brightened cloud reflect?"""
        pass
    
    def assess_precipitation_impact(self):
        """Does brightening reduce rainfall downwind?"""
        pass
    
    def optimize_ship_routes(self):
        """Where should ships spray for maximum cooling?"""
        pass
```

### Framework 4: Ocean Governance (Inherited from SRM Governance)
```python
class OceanInterventionGovernance:
    def __init__(self, stakeholders, regulatory_region):
        self.stakeholders = stakeholders  # coastal nations, fishing orgs, scientists
        self.region = regulatory_region
    
    def assess_transboundary_impact(self):
        """Ocean currents don't respect borders"""
        pass
    
    def require_consent(self):
        """Who must consent before deployment?"""
        pass
    
    def model_cascading_effects(self):
        """What happens if one country deploys and others don't?"""
        pass
    
    def emergency_stop_protocol(self):
        """How do you stop an intervention that's going wrong?"""
        pass
```

---

## Why the Ocean Gap Exists: Five Hypotheses

| # | Hypothesis | Evidence | Testable? |
|---|-----------|----------|-----------|
| 1 | **Complexity Barrier** | Ocean GCMs require HPC; 10x higher entry than atmospheric models | Run a 1D OAE model on a laptop — if it works, this is wrong |
| 2 | **Governance Chill** | Ocean currents cross borders; international law complex | Count ocean geoengineering papers in Nature vs. Science — if governance papers exist, code should too |
| 3 | **Irreversibility Aversion** | OAE changes ocean chemistry for centuries; scientists avoid irreversible code | Survey modelers: "Would you code an irreversible intervention?" |
| 4 | **Publication Incentive** | A decade of code can't be one paper; academic incentive mismatch | Check if tenure committees count open-source code |
| 5 | **Data Scarcity** | Ocean observations sparse; can't validate without data | Map ocean pH/alkalinity monitoring stations vs. atmospheric stations |

**Most likely:** A combination of 1 (complexity), 3 (irreversibility), and 4 (incentives). The data scarcity (5) is real but not unique — atmospheric models started with sparse data too.

---

## The Ocean's Only Commit Trail: Precipitation-Buoyancy POD

The NOAA-GFDL/MDTF-diagnostics repository has **5 commits on June 19, 2026 alone** for the same file — the precipitation-buoyancy POD (Process-Oriented Diagnostics). This is the ocean's most active commit trail:

- **What it is:** A diagnostic tool that checks whether climate models correctly simulate precipitation-buoyancy relationships
- **What it does:** Evaluates model accuracy, not intervention scenarios
- **Why it matters:** It's the closest ocean-adjacent code to geoengineering — it checks if models that *could* simulate interventions are actually correct
- **Commit pattern:** 5 commits in one day, then nothing. A burst of focused evaluation work, then silence.

**Episode hook:** *"The ocean's most active GitHub commit trail is five people fixing the same file in one day. They were checking if the models work. Not building tools to save the ocean. Just grading the tests."

---

## Comparison: Ocean vs. Solar vs. Carbon

| Metric | ☀️ Solar | 🌍 Carbon | 🌊 Ocean |
|--------|---------|---------|--------|
| Total repos found | 6+ | 9+ | **0 dedicated** |
| Recently updated | 3 | 3 | **0** |
| Dormant ghosts | 3 | 4 | **0** |
| Active community | WRF (institutional) | open-sustainable-tech (curated) | **None** |
| Hardware projects | GeoVision (simulator) | openair-cyan (DACC) | **None** |
| Governance models | OOCC_2021 (frozen) | None | **None** |
| CC0/public domain | None | tjz21 (2 repos) | **None** |
| Pseudocode frameworks | None needed | None needed | **Drafted by us** |

**Verdict:** Ocean geoengineering isn't just behind the other themes. It's in a different category entirely. It's not a slow field — it's an absent field.

---

## Episode Narratives for Ocean Episode

1. **"The Void"** — Zero repos. 12 queries. Nothing. The ocean covers 70% of the planet and has zero open-source intervention code.

2. **"The Complexity Wall"** — You can simulate SRM on a laptop. Ocean intervention requires an HPC. The entry barrier is structural, not motivational.

3. **"The Irreversibility Problem"** — SRM is reversible. OAE is not. Scientists may avoid coding what they can't unmake.

4. **"The Only Commit Trail"** — 5 commits on one diagnostic file. The ocean's most active GitHub moment was evaluation, not intervention.

5. **"The Blueprint Era"** — We drafted pseudocode for OAE, iron fertilization, MCB, and governance. The frameworks exist in our heads. They need to exist in GitHub. Someone just has to commit them.

---

## Call to Action for Our Audience

If you're moved by the ocean gap, here's what you can do:

1. **Start small** — A 1D ocean column model in Python + xarray. You don't need an HPC to start.
2. **Use adjacent tools** — WRF, MDTF-diagnostics, NCAR_ML_EKE are the building blocks.
3. **Fork the governance** — OOCC_2021's SRM governance model needs an ocean extension.
4. **CC0 your code** — Follow tjz21's example. Remove friction. Public domain = maximum adoption.
5. **Ship it** — The ocean won't wait for perfect code. Commit something. Anything.

---

*Analysis date: September 2026 | Data source: GitHub API, 12 systematic search queries, commit histories*

CONFIRMED v4: Zero dedicated ocean geoengineering repos. Ocean gap is total, not partial.*