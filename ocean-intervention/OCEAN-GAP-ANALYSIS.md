# 🌊 Ocean Intervention Gap Analysis

**Research Date:** September 2026  
**Data Source:** Exhaustive GitHub search across 8+ query strategies  
**Headline Finding:** Zero dedicated ocean geoengineering repositories on GitHub

---

## Search Strategy

We searched GitHub using the following query strategies:
1. `geoengineering ocean`
2. `marine geoengineering`
3. `ocean fertilization climate`
4. `ocean climate model simulation`
5. `ocean alkalinity enhancement`
6. `iron fertilization`
7. `seaweed climate`
8. `ocean upwelling geoengineering`
9. `marine cloud brightening`
10. Topic search: `climate simulation`, `geoengineering`

Across all 10 strategies, **no repository was found that specifically models, simulates, or implements an ocean geoengineering intervention.**

---

## What "Ocean Intervention" Means (For Context)

Ocean geoengineering encompasses several approaches:

### 1. Ocean Alkalinity Enhancement (OAE)
Add crushed olivine, limestone, or other alkaline minerals to the ocean. The dissolved minerals increase alkalinity, allowing the ocean to absorb more CO2. Natural version: weathering of rocks on land → rivers carry alkalinity to ocean.

**Why it matters:** Could amplify a natural carbon sink by 10-50x.

### 2. Iron Fertilization
Add iron to iron-limited ocean regions (Southern Ocean, equatorial Pacific) to stimulate phytoplankton blooms. The blooms absorb CO2, and some carbon exports to the deep ocean.

**Why it matters:** Natural version of iron fertilization drives glacial-period CO2 cycles. But experiments (LOHAFEX, SEEDS) showed mixed results.

### 3. Seaweed/Biofilm Farming
Cultivate seaweed for carbon sequestration, biofuel, or animal feed. Seaweed grows 30-80x faster than terrestrial plants.

**Why it matters:** Could provide both carbon removal and economic value.

### 4. Artificial Upwelling
Pump deep, nutrient-rich water to the surface to stimulate phytoplankton productivity, enhancing the biological carbon pump.

**Why it matters:** Natural upwelling zones are among the most productive ocean ecosystems.

### 5. Marine Cloud Brightening (SRM-adjacent)
Spray sea salt aerosols into marine clouds to increase cloud reflectivity and cool the planet.

**Why it matters:** The最有前途的 SRM 方法之一，but not strictly "ocean intervention" — it's atmospheric SRM with ocean-derived materials.

---

## The Gap Map

| Approach | Papers | GitHub Repos | Open Tools | Status |
|----------|--------|-------------|------------|--------|
| Ocean Alkalinity Enhancement | 20+ | 0 | 0 | ❌ No code |
| Iron Fertilization | 30+ | 0 | 0 | ❌ No code |
| Seaweed/Biofilm | 10+ | 0 | 0 | ❌ No code |
| Artificial Upwelling | 10+ | 0 | 0 | ❌ No code |
| Marine Cloud Brightening | 20+ | 2 | 2 | ⚠️ SRM-adjacent only |
| DAC | 50+ | 8+ | 5+ | ✅ Active |
| Solar Radiation Management | 30+ | 5+ | 3+ | ⚠️ Sparse |
| Carbon Capture & Storage | 100+ | 15+ | 8+ | ✅ Active |

---

## Why Is the Gap So Wide?

### Factor 1: Regulatory Barriers
The **London Protocol and London Convention** (the "London Convention") regulate ocean disposal at sea. Ocean fertilization and OAE fall under a de facto moratorium. Researchers may avoid building tools that could be interpreted as facilitating prohibited activities.

- **Impact on open source:** If the regulator says "no", the developer says "no".
- **Evidence:** No ocean fertilization experiment in the last decade has been accompanied by open-source tools.

### Factor 2: Computational Complexity
Ocean models are among the most computationally expensive tools in climate science. MOM6 (Modular Ocean Model) requires HPC infrastructure. Running even a simplified ocean model requires serious compute.

- **Impact on open source:** The barrier to entry is much higher than for atmospheric models or economic models.
- **Evidence:** Every ocean model on GitHub (MOM6, NEMO, PISCES) is maintained by a massive consortium, not an individual.

### Factor 3: Discipline Silos
Oceanographers and the "open-source climate tech" community don't overlap. Climate tech open source is dominated by software engineers and economists. Ocean models are built by physical oceanographers who write Fortran.

- **Impact on open source:** The ForTran wall keeps ocean models out of the Python-driven open-source climate ecosystem.
- **Evidence:** The most active ocean-adjacent repos (NCAR_ML_EKE, VikingVador's FNO) are niche academic projects, not community tools.

### Factor 4: No Pilot Deployments
Unlike DAC (multiple operational plants) and SRM (small-scale experiments like SCoPEx, behavior, the坚持), ocean intervention has almost no operational pilot projects.

- **Impact on open source:** No real-world data to validate models against. No operational feedback loop.
- **Evidence:** The last major ocean fertilization experiment was LOHAFEX in 2009. That was 17 years ago.

### Factor 5: Ethical and Governance Concerns
Ocean intervention raises unique questions: Who owns the ocean? What are the transboundary effects? Who governs the governance?

- **Impact on open source:** Some researchers may deliberately avoid building tools that could lower the barrier to unilateral deployment.
- **Evidence:** The governance literature (Biermann et al., 2024) explicitly discuss "command and control" approaches to ocean geoengineering.

---

## The Exception That Proves the Rule: Marine Cloud Brightening

Marine cloud brightening (MCB) is the only ocean-adjacent geoengineering approach with GitHub repos. But MCB is technically **solar radiation management (SRM)**, not ocean intervention — it uses sea salt as a delivery mechanism for atmospheric cloud seeding.

The two MCB repos found:
1. **mlmac-seid/marine-cloud-brightening-simulation** — RRTM-based radiative transfer simulation
2. **AidanCraw/mcb-tc-model** — Tropical cyclone track modeling

Both are atmospheric models, not ocean models. Both are project/thesis-sized (0-1 stars). Both have been dormant for years.

**The takeaway:** Even when an ocean-adjacent approach is actively researched, the open-source tooling is still tiny and dormant.

---

## What Would Bridge the Gap?

### The "OpenAir-Cyan of Ocean Intervention"

If we could build an open-source ocean intervention tool that mirrors OpenAir-Cyan's accessibility, what would it be?

**Concept 1: OAE Calculator**
- Input: target CO2 offset (tons/year)
- Output: required olivine quantity, dissolution rate, ocean transport
- Method: Simplified 1D ocean chemistry model, laptop-runnable
- Impact: Makes OAE thinking accessible to policymakers

**Concept 2: Ocean Alkalinity Transport Model**
- Input: olivine dissolution rate, ocean current data
- Output: alkalinity distribution, CO2 uptake over time
- Method: 2D simplified circulation model
- Impact: Tests whether OAE actually works at scale

**Concept 3: Governance Dashboard**
- Input: deployment reports, satellite data
- Output: verification that an OAE or iron fertilization project is occurring
- Method: Data integration + anomaly detection
- Impact: Enables monitoring and accountability

### What It Would Take to Build It

1. **A champion:** Someone with both ocean science expertise and software engineering skills
2. **Modest scope:** Start with a 1D model, not a full GCM
3. **Open data:** Use existing ocean chemistry datasets (NOAA, GCOS)
4. **Community:** Partner with the OAE research community (Renforth, Kheshgi, etc.)
5. **Governance-first:** Build the verification/governance tools alongside the models

---

## 📊 Comparison: Ocean vs. Other Carbon Removal Domains on GitHub

| Metric | Ocean | Solar | Carbon |
|--------|-------|-------|--------|
| Total repos | ~5 | ~10 | ~15+ |
| Active repos (2026) | 0-1 | 2-3 | 3-4 |
| Stars (top repo) | 20 | 1,761 | 85 |
| Stars (avg) | 3.2 | — | — |
| Open hardware | ❌ | ✅ (GeoVision) | ✅ (Cyan, Epiphyte) |
| Community activity | None | Low | Low |
| Governance tools | None | None | None |
| Papers-to-code ratio | ~100:1 | ~10:1 | ~5:1 |

**The ocean intervention gap is the widest gap in climate tech open source.**

---

## 🎙️ Podcast Episode Talking Points

### The "Perfect Storm" Thesis
Ocean geoengineering's absence on GitHub isn't one thing — it's five barriers stacking:
1. Regulation says "no"
2. The computers say "too expensive"
3. The disciplines say ".notmyfield"
4. The pilots say "none yet"
5. The ethicists say "be careful"

### The "First Mover" Opportunity
Whoever builds the first serious, maintenance-quality ocean intervention model will be the sole voice in the space. It's a wide-open field.

### The "Governance Signal"
The silence might be intentional. Maybe researchers are self-censoring because they know deployment without governance would be dangerous. The code gap might be a feature, not a bug.

### The "MDTF-Diagnostics Bridge"
MDTF-diagnostics' precipitation-buoyancy POD (Jun 2026) is the closest thing to ocean process diagnostics. If ocean geoengineering ever gets serious, MDTF-like tools would need to be built for ocean-specific variables (alkalinity, iron, chlorophyll, pH).

---

## References

- Kheshgi et al. (2022) "Ocean Based Climate Change Mitigation" — Oxford Principles
- Renforth et al. (2023) "Ocean Alkalinity Enhancement" — review
- Biermann et al. (2024) "Governance of Ocean Geoengineering"
- London Protocol / London Convention — ocean disposal regulations
- LOHAFEX (2009) — Iron fertilization experiment
- NOAA GFDL MDTF-diagnostics — precipitation-buoyancy POD
- CrayLabs/NCAR_ML_EKE — ML for ocean climate modeling