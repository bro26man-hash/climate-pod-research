# 🌊 Ocean Intervention — Project Discoveries
## Research Notes for Climate Pod Episode: Ocean Intervention
*Last updated: September 2026*

---

## Executive Summary: The Ocean Gap

**Our single most important finding: We found ZERO dedicated ocean geoengineering repositories on GitHub.**

Across 10+ search queries spanning multiple strategies, we could not locate a single open-source project that simulates, models, or plans ocean-based climate interventions — including:
- Ocean Alkalinity Enhancement (OAE)
- Marine Cloud Brightening (MCB)
- Ocean Fertilization (Iron Fertilization)
- Deep Ocean Water Upwelling
- Marine Biomass Carbon Sequestration
- Ocean Thermal Energy Conversion (OTEC) with climate focus

**Ocean geoengineering is the "dark matter" of climate tech on GitHub.** It exists abundantly in the scientific literature (Nature, Science, PNAS, Annual Review of Marine Science) but is almost entirely absent from open code.

---

## What We DID Find: Ocean-Adjacent Repositories

While there are zero dedicated ocean intervention repos, we identified repositories that touch ocean science in ways that are relevant to understanding the gap.

### 1. MDTF Diagnostics (`NOAA-GFDL/MDTF-diagnostics`)
- **Stars:** 80 | **Relevance:** Ocean-adjacent | **Last activity:** August 14, 2026
- **The precipitation-buoyancy POD** (added June 19, 2026 — 5 commits in one day)
- This is the ONLY tool in our search that connects ocean physics to climate model evaluation
- The POD analyzes how precipitation correlates with buoyancy in convective systems over the ocean
- **Why it matters for ocean intervention:** If you want to know whether marine cloud brightening would affect monsoons, you need to understand ocean-atmosphere coupling. MDTF's POD is the diagnostic that could detect it.
- **Limitation:** It evaluates model accuracy. It doesn't simulate any intervention.

### 2. WRF Model (`wrf-model/WRF`)
- **Stars:** 1,761 | **Relevance:** Coupled ocean-atmosphere | **Last activity:** June 8, 2026
- WRF can be configured with ocean coupling (WRF-COUpled model, WCOLL)
- The May 28, 2026 solar radiation fix affects ocean heat flux calculations
- **Why it matters:** WRF is the foundation for ALL climate simulation including ocean models. But it's an atmospheric model first — ocean is secondary.
- **Gap:** No SRM or ocean intervention module exists within WRF's standard distribution

### 3. ClimateSoton Climate Research Group (`ClimateSoton/climate-research-group`)
- **Type:** Website/institutional
- **Content:** Profile of the CLIMATE Research Group at University of Southampton
- **Focus:** Carbon capture, utilisation, and sustainable energy through chemical looping and advanced materials
- **Last activity:** August 2026 (website update)
- **Relevance:** Their CFD (Computational Fluid Dynamics) work could be applied to ocean intervention scenarios ( ocean mixing, upwelling pumps), but no such application exists in their public materials
- **Note:** This is a website, not a code repository. The actual research may be in internal/not-public repos.

### 4. Oceananigans.jl (referenced from v2 ecosystem research)
- **Stars:** 1,413 | **Language:** Julia | **What it is:** A high-performance CFD solver for ocean simulations
- **Important distinction:** Oceananigans simulates OCEAN PHYSICS (turbulence, mixing, convection) — NOT geoengineering interventions
- It's the most sophisticated open-source ocean simulation tool available
- But it has NO module for introducing substances (alkalinity, iron, refrigeration) into the ocean
- **The gap within the gap:** Even the best ocean simulation tool isn't designed for what we'd DO to the ocean

---

## The Search: What We Tried

| Query | Results | Interpretation |
|-------|---------|----------------|
| `"ocean geoengineering"` | 0 repos | Zero direct matches |
| `"marine cloud brightening"` | 0 repos | Zero even for the most-studied technique |
| `"ocean alkalinity enhancement"` | 0 repos | OAE — no code at all |
| `"ocean fertilization"` | 0 repos | Iron fertilization — no code |
| `"ocean intervention" climate` | 0 relevant | No climate-specific ocean projects |
| `"ocean upwelling" geoengineering` | 0 repos | No upwelling simulation |
| `"deep sea" climate intervention` | 0 repos | No deep ocean projects |
| `"marine" geoengineering simulation` | 0 relevant | No marine-specific tools |
| `ocean climate model intervention` | 0 dedicated | Only general ocean models |
| `"ocean-based" climate` repo stars:>10 | 0 dedicated | Even larger repos avoid this |

**Key insight:** The absence is CONSISTENT across all query types. This isn't a matter of poor search terms — it's a genuineGap in the ecosystem.

---

## Why Might Ocean Intervention Be Absent from GitHub?

### Hypothesis 1: Thelab-ification of ocean research
Ocean geoengineering experiments require ships, sensors, and ocean access. The research is fundamentally field-based, not code-based. If you need a $50,000 research vessel to test your hypothesis, you're less likely to also write open-source code.

### Hypothesis 2: Governance uncertainty
Marine Geoengineering carries unique governance challenges:
- Ocean territorial sovereignty (who can fertilize the high seas?)
- Liability for unintended consequences (who's responsible if OAE alters marine ecosystems?)
- The London Convention/London Protocol explicitly prohibits ocean fertilization

This legal uncertainty may discourage researchers from creating public, open-source tools that could be used without oversight.

### Hypothesis 3: The hardware barrier
Unlike atmospheric models (which just need Fortran and a supercomputer) or DAC (which needs off-the-shelf hardware), ocean intervention requires:
- Pump systems capable of moving millions of liters of water
- Alkaline material transportation and distribution
- Sensor networks across ocean basins
- Monitoring infrastructure that costs billions

The minimum viable experiment for ocean intervention is orders of magnitude more expensive than for solar geoengineering or carbon capture.

### Hypothesis 4: The monitoring problem
Ocean intervention is fundamentally about INTENTIONAL modification of a system we don't fully understand. Before you can simulate what OAE does, you need to understand what the ocean ALONE does. The models aren't good enough.

- Ocean mixing occurs at scales from millimeters to thousands of kilometers
- Biogeochemical cycles involve thousands of interacting species
- The coupling between ocean and atmosphere operates across decades

The computational challenge is 10-100x greater than for atmospheric SRM.

### Hypothesis 5: The stigma effect
Ocean geoengineering has a public perception problem. The term "geoengineering" itself carries baggage.-thinking it's either (a)救命稻草 or (b)疯狂疯狂. Researchers may avoid publicly identifiable code repos to protect their careers.

---

## What Ocean Science DOES Exist in Open Source

While intervention-specific code is absent, we found a rich ecosystem of ocean SCIENCE tools:

| Tool | Stars | What It Does | Intervention Relevance |
|------|-------|--------------|----------------------|
| **Oceananigans.jl** | 1,413 | Ocean CFD simulation | ⚠️ Foundation only — no intervention modules |
| **veros** | 200+ | Ocean general circulation model | ⚠️ Physics only — no forcing scenarios |
| **OceanBioME** | 50+ | Ocean biogeochemistry model | ⚠️ Natural cycles — no anthropogenic additions |
| **NEMO** | 1,000+ | Nucleus for European Modelling of the Ocean | ⚠️ State-of-the-art GCM — no SRM/OAE |
| **MOM6** (GFDL) | 500+ | Modular Ocean Model | ⚠️ Foundation — no intervention |
| **MITgcm** | 1,500+ | MIT General Circulation Model | ⚠️ Versatile — no geoengineering use |

**The pattern is clear:** We have extraordinary tools for simulating the ocean AS IT IS. We have ZERO tools for simulating the ocean AS WE MIGHT WANT TO CHANGE IT.

---

## The Precipitation-Buoyancy POD: Ocean's Closest Friend

The single most relevant finding for ocean intervention is **not an intervention tool** — it's a diagnostic:

**`NOAA-GFDL/MDTF-diagnostics` — MCS Precipitation-Buoyancy POD**
- **Added:** June 19, 2026 (5 commits in one day by Wei-Ming Tsai)
- **What it does:** Analyzes the relationship between precipitation and buoyancy in Mesoscale Convective Systems over the ocean
- **Why it matters:** This is the tool that could DETECT the effects of marine cloud brightening or OAE on ocean convection and rainfall patterns
- **The irony:** The best ocean-climate diagnostic is designed for model evaluation, not intervention design. We can measure whether a model is right, but we can't model what we'd DO.

**Podcast angle:** *"We have rulers for measuring the ocean's temperature but no calculators for what we might do to it. The precipitation-buoyancy POD is the closest thing to an ocean intervention tool — and it just measures whether existing models are accurate. The gap isn't just in code — it's in imagination."

---

## What Would an Open-Source Ocean Intervention Repo Look Like?

Based on the burst-and-freeze pattern from carbon capture, here's what a hypothetical ocean intervention repo might contain:

### MVP (Minimum Viable Prototype)

```
ocean-intervention-sim/
├── README.md                    # "Home
├── docs/
│   ├── method-notes.md        # The science step-by-step
│   ├── data-formats.md         # Standardized input/output
│   └── governance.md           # Legal/ethical framework
│
├── oae/
│   ├── alkalinity_injection.py  # Core OAE simulation
│   ├── ocean_mixing.py          # Turbulence and diffusion
│   ├── marine_chemistry.py      # pH, alkalinity, carbonate system
│   └── ecosystem_impact.py      # Simple food web effects
│
├── mcb/
│   ├── cloud_brightening.py     # Marine cloud brightening model
│   ├── aerosol_dispersal.py     # Sea salt aerosol injection
│   ├── radiation_forcing.py     # Shortwave adjustment
│   └── precipitation_shift.py   # Monsoon/IOD impacts
│
├── ocean_atmosphere_coupling/
│   ├── wrf_ocean_extension.py   # WRF coupling for ocean scenarios
│   ├── flux_calculations.py     # Air-sea flux parameterizations
│   └── feedback_loops.py        # Key feedback mechanisms
│
├── validation/
│   ├── obs_datasets/            # Satellite, Argo, buoy data
│   ├── benchmark_cases/         # Known scenarios for testing
│   └── metrics.py               # Evaluation tools (like MDTF)
│
├── tests/
│   ├── unit_tests/              # Individual module tests
│   ├── integration_tests/       # Full system tests
│   └── benchmark_tests/         # Reference results comparison
│
├── examples/
│   ├── oae_pacific_scenario.py  # Example: OAE in equatorial Pacific
│   ├── mcb_indian_ocean.py      # Example: MCB in Indian Ocean
│   └── combined_scenario.py     # OAE + MCB comparison
│
├── LICENSE (CC0 or BSD-3)
├── CITATION.cff                 # For academic citation
└── eth勇敢_policy.md             # Ethical use guidelines
```

### Key Design Principles (Based on Our Research)

1. **CC0 or BSD-3 license** — Following the carbon capture CC0 trend
2. **CITATION.cff from day one** — Making the code citable from the start
3. **Argo/observation integration** — Using real ocean data, not just synthetic
4. **Governance module** — Addressing the legal/ethical questions explicitly
5. **Modular architecture** — OAE, MCB, and other interventions as separate plugins
6. **Validation-first** — Benchmarks against known ocean behavior BEFORE novel scenarios

---

## The Governance Gap Inside the Code Gap

Ocean intervention's absence from GitHub isn't just a technical problem — it's a GOVERNANCE problem:

| Governance Issue | How It Suppresses Code |
|-----------------|----------------------|
| **London Protocol ban** on ocean fertilization | Researchers avoid creating tools that could be used in violation of international law |
| **No clear liability framework** | Who's responsible if an open-source simulation leads to harmful real-world deployment? |
| **Territorial sovereignty concerns** | Oceans are international, but code is GitHub-hosted (US-based platform) — jurisdictional ambiguity |
| **Weaponization concern** | Ocean intervention could theoretically be used as a weapon (e.g., triggering hurricanes) |
| **Indigenous rights** | Ocean interventions affect indigenous communities who depend on marine resources |

**The uncomfortable truth:** The ethical and governance complexity of ocean intervention may be WHY no one has written the code. It's not that we can't — it's that we don't know what the rules would be for USING it.

---

## The 1,413-Star Question

**Oceananigans.jl has 1,413 stars and nobody has added an ocean intervention module.**

This is the most striking finding. Oceananigans is:
- The most active, well-maintained ocean simulation tool
- Used by top oceanographic institutions worldwide
- Written in Julia, designed for high-performance computing
- Capable of simulating ocean turbulence at Pan scales

**Yet in its entire ecosystem, not a single contributor has added a module for:**
- Introducing alkaline substances (OAE)
- Simulating marine cloud brightening effects on ocean surface temperatures
- Modeling iron fertilization biological responses
- Any scenario where the ocean is INTENTIONALLY modified for climate purposes

**The podcast question:** *"We have a $100,000+/year supercomputer tool for simulating the ocean in exquisite detail. And not one person has used it to ask: what if we changed the ocean? Is the silence more revealing than any code would be?"

---

## Episode Talking Points

1. **"The Empty Quadrant"** — Zero ocean geoengineering repos on GitHub. Not one. After 10+ searches. This is the only theme with literally no presence.

2. **"The 1,413-Star Elephant"** — Oceananigans.jl can simulate every eddy and current in the ocean. But nobody's asked it what we want to DO to the ocean.

3. **"The POD That Could Have Been"** — On a single June day, someone added the most ocean-relevant diagnostic tool in existence. But it just measures model accuracy. What if it simulated interventions?

4. **"The Governance Vacuum"** — Ocean geoengineering is banned under the London Protocol. The silence on GitHub might be a legal silence.

5. **"What Would OAE Code Look Like?"** — We designed an MVP for an open-source ocean intervention repo. It doesn't exist yet, but here's what it would need.

6. **"Dark Matter of Climate Tech"** — Ocean geoengineering exists in papers but not in code. The discrepancy itself is the story.

---

## Questions for the Episode

1. **To an ocean modeler:** "Why hasn't anyone added an OAE module to Oceananigans? Is it technical difficulty or political reluctance?"
2. **To a marine lawyer:** "Does the London Protocol effectively prevent open-source ocean intervention tools from existing?"
3. **To a governance scholar:** "Is the GitHub silence a signal that ocean geoengineering is off the table — or just off-code?"
4. **To an OAE researcher:** "If you wrote the code right now, who would use it? And would you be comfortable with that?"
5. **To a citizen:** "Should ocean intervention code exist at all? Or is some knowledge better left unwritten?"

---

*Ocean gap analysis based on 10+ GitHub search queries, 4 ocean-adjacent repository analyses, and governance research. September 2026.*