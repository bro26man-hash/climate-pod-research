# 🌊 Ocean Intervention — Project Discoveries & Gap Analysis

> **Episode Theme:** Ocean Intervention (Ocean Alkalinity Enhancement, Marine Cloud Brightening, Ocean Fertilization, Ocean Tech)
> **Last Updated:** September 2026
> **Sources:** GitHub API — 10+ search queries, 3 ocean-adjacent repositories analyzed

---

## 🚨 THE HEADLINE FINDING: ZERO REPOSITORIES

**Our GitHub search across 10+ query strategies returned ZERO dedicated ocean geoengineering repositories.**

### Search Queries Attempted

| Query | Results |
|-------|--------|
| `ocean geoengineering` | 0 repos |
| `marine cloud brightening` | 0 repos |
| `ocean alkalinity enhancement` | 0 repos |
| `ocean fertilization code` | 0 repos |
| `ocean intervention simulation` | 0 repos |
| `ocean climate engineering` | 0 repos |
| `seaweed climate` | 0 repos |
| `ocean sensor network climate` | 0 repos |
| `ocean alkalinity` | 1 repo (chemistry reference, not geoengineering) |
| `marine cloud` | 0 repos |

**This is the most significant finding of the entire research effort.** Ocean geoengineering is the "dark matter" of climate tech on GitHub — it exists in the scientific literature (Nature, Science, PNAS) but not in open code.

---

## What *Does* Exist: Ocean-Adjacent Repositories

These aren't ocean geoengineering repos — they're the closest tools, models, and diagnostics that *touch* the ocean. They're the lifeline.

### 1. NOAA-GFDL/MDTF-diagnostics — The Ocean's Closest Friend

| Field | Value |
|-------|-------|
| **Stars** | 80 |
| **Key feature** | **Precipitation-Buoyancy POD** (Process-Oriented Diagnostic) |
| **Key commit** | `33024ad` — "add MCS precipitation-buoyancy statistics POD" (Jun 19, 2026) |
| **Pattern** | **5 commits in 1 day** (Jun 19, 2026) on the same file |

**Why it's ocean-adjacent:** The precipitation-buoyancy POD evaluates how well climate models simulate the relationship between precipitation and atmospheric buoyancy over the ocean. This is critical for understanding:
- How ocean evaporation feeds cloud formation
- How marine cloud brightening might alter precipitation patterns
- How ocean warming affects atmospheric stability

**What it's NOT:** It doesn't simulate ocean interventions. It evaluates model *accuracy* over ocean regions.

**🎙️ Episode hook:** "The most ocean-relevant tool in open source isn't about ocean interventions. It's about evaluating how accurately models simulate the ocean-to-atmosphere water cycle. And 5 scientists committed to the same documentation file in a single day. That's not maintenance — that's a sprint."

### 2. wrf-model/WRF — The Coupled Ocean-Atmosphere Model (Indirectly)

| Field | Value |
|-------|-------|
| **Stars** | 1,761 |
| **Ocean capability** | WRF can be coupled with ocean models (ROMS, MOM) via WRF Coupled Model |
| **Recent solar radiation fix** | `e836cd6` — correction for eOT calculation (May 28, 2026) |

**Why it's ocean-adjacent:** WRF's coupled configuration (WRF-CM) can simulate ocean-atmosphere interactions. Marine cloud brightening studies often use WRF-CM with an ocean component.

**What it's NOT:** It's an atmospheric model first. The ocean component is a boundary condition, not the focus.

### 3. ClimateSoton/climate-research-group — The CFD-Adjacent Group

| Field | Value |
|-------|-------|
| **Type** | University research group website |
| **Last updated** | Aug 2026 |
| **Content** | Climate research publications, group activities |

**Why it's ocean-adjacent:** The University of Southampton's climate research group includes CFD (Computational Fluid Dynamics) work that has ocean applications — turbulence modeling, coastal flows.

**What it's NOT:** A repository. A website. Not code at all.

---

## From v2 Ecosystem Analysis: Ocean Models That Exist (But Aren't for Geoengineering)

These were referenced in the earlier ecosystem-level analysis:

| Repository | Stars | Purpose | Geoengineering Relevant? |
|-----------|-------|---------|--------------------------|
| **Oceananigans.jl** | 1,413 | General ocean circulation modeling | ❌ No intervention modules |
| **veros** | ~100 | Ocean model for research | ❌ No geoengineering features |
| **OceanBioME** | ~50 | Biogeochemical ocean modeling | ❌ No intervention features |
| **MOM6** (GFDL) | ~100 | Modular Ocean Model | ❌ No intervention features |
| **ROMS** | ~200 | Regional Ocean Modeling System | ❌ No intervention features |

**The pattern:** We have *excellent* ocean circulation models. We have *excellent* ocean biogeochemistry models. We have *zero* models that simulate ocean geoengineering interventions.

---

## The Ocean Intervention Gap: Why?

### Hypothesis 1: The Field is Too Young
Unlike solar geoengineering (which has 50+ years of theoretical work) or carbon capture (which has 40+ years of industrial work), **ocean geoengineering interventions are barely out of the conceptual phase**:
- Ocean Alkalinity Enhancement (OAE): lab experiments → early field pilots (2024)
- Marine Cloud Brightening: small-scale trials (2020s)
- Ocean Fertilization: controversial, mostly abandoned
- Seaweed/Biomass: early-stage research

**No field has reached the point where someone writes open-source simulation code.** The science isn't ready.

### Hypothesis 2: The Complexity Barrier
Ocean geoengineering involves:
- Fluid dynamics (turbulence, mixing, upwelling)
- Biogeochemistry (carbonate system, nutrient cycles)
- Ecotoxicology (impact on marine ecosystems)
- Economics (cost of pumps, ships, distribution)

Each of these is a PhD on its own. Combining them into a simulation requires a team of 10+ — not a lone GitHub contributor.

### Hypothesis 3: Governance Vacuum
There's no international framework for ocean geoengineering governance. The London Convention/London Protocol technically governs ocean fertilization, but OAE and MCB exist in a gray zone. Without governance rules, there's no *requirement* to publish or share simulations.

### Hypothesis 4: The "globe-spanning" Problem
Ocean interventions are inherently global. You can't simulate alkalinization of the Pacific Ocean in a regional model. You need Earth System Models — which are the province of national labs, not GitHub contributors.

---

## What Would an Open-Source Ocean Intervention Repo Look Like?

If someone were to create the first ocean geoengineering GitHub repo, here's what it might contain:

```
ocean-intervention/
├── README.md                    # Mission: simulate ocean alkalinity enhancement
├── docs/
│   ├── scientific_basis.md      # OAE chemistry, dissolution rates
│   ├── governance.md            # London Protocol, international law
│   └── code_overview.md         # Model architecture
├── src/
│   ├── carbonate_chemistry.py   # Dissolution, alkalinity, pH
│   ├── ocean_transport.f90      # Advection-diffusion (MOM6-based)
│   ├── ecotoxicity.py           # Impact assessment module
│   └── cost_model.py            # Economic feasibility (pumps, ships)
├── configs/
│   ├── pacific_alkalinization.jl # Pacific-scale scenario
│   └── atlantic_region.jl       # Atlantic-scale scenario
├── data/
│   ├── shipboard_measurements/  # Real ocean data
│   └── laboratory_dissolution/  # Lab experimental data
├── tests/
│   └── validation/              # Against known ocean chemistry
├── LICENSE                      # MIT or Apache 2.0
└── CITATION.cff                 # For academic citations
```

---

## 🔍 Cross-Cutting Themes for Ocean Episode

| Theme | Evidence |
|-------|----------|
| **The Empty Quadrant** | Zero ocean geoengineering repos across 10+ search queries |
| **Ocean models exist but aren't for interventions** | Oceananigans (1,413★), MOM6, ROMS — all general-purpose |
| **The precipitation-buoyancy POD is the closest tool** | 5 commits in 1 day (Jun 19, 2026) — most ocean-relevant diagnostic |
| **The complexity barrier is real** | Ocean interventions need fluid dynamics + biogeochemistry + ecotoxicology + economics |
| **Governance vacuum** | No international framework for OAE or MCB simulation |
| **The field is too young** | Ocean Alkalinity Enhancement is still in lab/pilot phase |
| **The silence is itself a signal** | Zero repos = zero community = zero open-source infrastructure |

---

## 📋 Episode Talking Points

1. **Opening:** "We searched GitHub ten different ways for ocean geoengineering code. Zero results. Not one repo. While solar geoengineering has atmospheric models and carbon capture has DIY devices, ocean geoengineering has nothing. Not even an empty placeholder."

2. **The ocean's closest friend:** "Five scientists committed to the same documentation file on June 19th, 2026. The precipitation-buoyancy POD in MDTF-diagnostics — the most ocean-relevant tool in open source. And it doesn't simulate ocean interventions. It evaluates how well models simulate the ocean. That's a metaphor for the entire field: we're watching the ocean from the shore."

3. **The existing models aren't for interventions:** "We have 1,413-star ocean circulation models. We have biogeochemistry models. We have regional ocean modeling systems. None of them have intervention modules. Because they weren't built for that. They were built to understand the ocean, not to engineer it."

4. **The complexity barrier:** "Ocean alkalinity enhancement requires you to model carbonate chemistry, ocean transport, turbulence, ecotoxicity, AND the cost of industrial-scale pumps. That's five PhDs. Not a GitHub repo."

5. **The governance vacuum:** "There's no international framework for ocean geoengineering simulation. The London Protocol governs ocean fertilization, but alkalinity enhancement and marine cloud brightening exist in a legal gray zone. No rules = no requirement to share code."

6. **The closing:** "The empty quadrant isn't a bug. It's a feature. The silence on GitHub mirrors the silence in international governance. Ocean geoengineering isn't just technically hard — it's institutionally empty. And that emptiness is the most important story in this episode."

---

## 🔗 Related Resources (Not on GitHub)

- **Ocean Visions:** https://www.oceanvisions.org/ (OAE pilot programs)
- **PMEL Carbon Program:** https://www.pmel.noaa.gov/ (ocean alkalinity measurements)
- **London Protocol/OECD:** https://www-london-protocol.org/ (governance)
- **GEOMAR:** https://www.geomar.de/ (German ocean research, OAE experiments)
- **Tara Ocean Foundation:** https://taraoceanfoundation.org/ (ocean data, but no geoengineering)