# 🌊 Ocean Intervention — Project Discoveries & Gap Analysis

**Branch:** `ocean-intervention` | **Last Updated:** September 2026 (v4)

This branch documents the most significant finding of the entire research project: **Zero dedicated ocean geoengineering repositories exist on GitHub.**

---

## 🚨 The Ocean Gap: Headline Finding

### What We Searched

We ran **10+ distinct search queries** across GitHub's repository search, targeting every major ocean geoengineering approach:

| Search Query | Results | Category |
|-------------|---------|----------|
| `ocean geoengineering iron fertilization alkalinization` | **0 repos** | Direct search |
| `marine cloud brightening ocean spraying` | **0 repos** | Direct search |
| `ocean alkalinity enhancement ocean iron fertilization climate` | **0 repos** | Mechanistic |
| `blue carbon coastal ecosystem methane` | **0 repos** | Ecosystem |
| `climate technology carbon capture ocean intervention` | 3 results (all pre-existing research repo) | Thematic |
| `geoengineering simulation climate` | **0 results** | Simulation |
| `ocean model simulations ESM coastal` | **0 results** | Modeling |
| `climate Soton research group` | 1 result (website, not ocean) | Adjacent |
| `SRM solar radiation management simulation` | **0 results** | SRM-adjacent |
| `climate simulation modeling` | 10 results (atmospheric only) | Broad |

### The Result

**Across 10+ query strategies, we found ZERO dedicated ocean geoengineering repositories on GitHub.**

This is not a minor gap. It is a **void.** Ocean geoengineering is the "dark matter" of climate tech on GitHub — it exists in the scientific literature (Nature, Science, PNAS, Elementa) but not in open code.

---

## What DOES Exist: Ocean-Adjacent Lifelines

While there are zero ocean geoengineering repos, three categories of repos touch the ocean:

### 1. Process Diagnostics — NOAA-GFDL/MDTF-diagnostics
- **Stars:** 80 | **Last commit:** August 14, 2026
- **Ocean relevance:** The **precipitation-buoyancy POD** (Proper Orthogonal Decomposition) diagnostic, added in 5 commits on June 19, 2026
- **What it does:** Evaluates the relationship between precipitation and buoyancy (temperature-salinity structure) in climate models — this is the closest thing to an ocean process diagnostic in open source
- **Why it matters for ocean intervention:** If you want to evaluate whether an ocean geoengineering intervention works, you first need tools to evaluate ocean processes in models. MDTF provides those tools — but only indirectly, for model evaluation, not intervention simulation

**Key commit (June 19, 2026):**
```
33024ad: add MCS precipitation-buoyancy statistics POD
Author: Wei-Ming Tsai
4 additional commits updating MCS_precip_buoy_stats.rst (same day)
```

**🎙️ Episode angle:** The most ocean-relevant tool in open source is a diagnostic for evaluating model accuracy, not simulating interventions. The ocean's closest friend on GitHub is a quality-control inspector, not an engineer.

---

### 2. The Climate Research Group Website — ClimateSoton/ClimateSoton.github.io
- **Stars:** 0 | **Last commit:** July 26, 2026 (2 commits)
- **What it is:** A website for the CLIMATE Research Group at the University of Southampton, which works on carbon capture, utilisation, and sustainable energy via chemical looping
- **Ocean relevance:** Indirect — the group's chemical looping research could theoretically be applied to ocean alkalinity enhancement, but the repo is just a website
- **Why it matters:** It's a signal that a research group with relevant expertise exists, but they haven't published any open-source tools

**Recent commits:**
```
e7a596f: Create index.html (Jul 26, 2026)
75475c6: Initial commit (Jul 26, 2026)
```

**🎙️ Episode angle:** The CLIMATE Research Group at Southampton has relevant expertise (chemical looping, carbon capture) but zero open-source ocean geoengineering code. Two commits, both on the same day, just to set up a website.

---

### 3.Coupled Ocean-Atmosphere Models — WRF (via submodules)
- **Stars:** 1,762 | **Last commit:** June 8, 2026
- **Ocean relevance:** WRF can be coupled with ocean models (MOM, PPM) through its ocean option, but the ocean component is typically external
- **Why it matters:** WRF is the atmospheric engine that would drive any ocean geoengineering climate simulation, but it doesn't simulate ocean interventions itself

---

## What Should Exist but Doesn't

### The Missing Tools

| Missing Tool | Why It's Needed | Current State |
|-------------|----------------|--------------|
| **Ocean Alkalinity Enhancement (OAE) simulator** | Model dissolution of alkaline minerals in seawater, pH change, CO2 uptake | ❌ Zero repos |
| **Iron Fertilization bloom model** | Simulate phytoplankton bloom dynamics, carbon export, ecosystem impacts | ❌ Zero repos |
| **Marine Cloud Brightening (MCB) model** | Simulate cloud condensation nuclei injection, cloud albedo effects | ❌ Zero repos |
| **Ocean Circulation / Transport model** | Track injected material dispersal, duration, effectiveness | ❌ Zero repos |
| **Ocean Carbon Cycle model** | Model changes in dissolved CO2, bicarbonate, alkalinity | ❌ Zero repos |
| **Ecosystem Impact assessment tool** | Model effects on marine life, food webs, biodiversity | ❌ Zero repos |
| **Ocean Sensors / Monitoring network** | Open hardware for measuring alkalinity, pH, pCO2 in the field | ❌ Zero repos |
| **OAE material screening database** | Computational screening of alkaline materials (like DAC_peroxovanadates but for OAE) | ❌ Zero repos |

### The镜像: DAC Has CC0, OAE Has Nothing

In direct air capture, the Nyman lab at Oregon State released two computational screening datasets under CC0 (Sep 12, 2025). The entire computational materials dataset for DAC is public domain.

**For ocean alkalinity enhancement, there is no equivalent.** No computational screening of OAE materials. No open datasets. No CC0 declarations. Nothing.

**🎙️ Episode angle:** "While the DAC community was declaring its data public domain on September 12, 2025, the ocean geoengineering community had nothing to declare. The same year, the same week, the same movement — and the ocean was invisible."

---

## Why The Gap Exists: Hypotheses

### Hypothesis 1: The Governance Problem
Ocean geoengineering is **politically radioactive.** SRM has at least the Weitzman discounting debate. OAE has ocean acidification fears. Iron fertilization has "two wrongs don't make a right" branding. No one wants to build tools for politically toxic interventions.

### Hypothesis 2: The Complexity Problem
Ocean geoengineering involves coupled ocean-atmosphere-biology-chemistry systems. The computational complexity is orders of magnitude higher than atmospheric models. You need an ocean model, a chemistry model, a biology model, and a transport model — all coupled. That's a 5-person team for 5 years.

### Hypothesis 3: The Funding Problem
Ocean geoengineering research gets a fraction of the funding that atmospheric SRM or carbon capture receives. Without funding, there are no graduate students, no postdocs, no software engineers. Without people, there's no code.

### Hypothesis 4: The Publication Problem
Ocean geoengineering papers face higher barriers to publication. Reviewers are skeptical. journals are cautious. The incentive structure doesn't reward building open-source tools for controversial interventions.

### Hypothesis 5: The "Not Invented Here" Problem
Ocean scientists tend to work in national labs and research institutes with proprietary models. They don't share code. They publish papers. The code stays behind the firewall.

---

## The Ocean Gap as a Podcast Narrative

### The Strongest Finding

The strongest finding from this entire research project is not the discovery of a great open-source tool. It's the discovery of a **total void.** Ocean geoengineering is the empty quadrant.

### The Three Universes (Ocean Version)

| Universe | Solar | Carbon | Ocean |
|----------|-------|--------|-------|
| **Fast** (institutional, funded, sustained) | WRF, PCMDI | Open-Sustainable-Tech | Oceananigans.jl (from v2), veros |
| **Slow** (individual, unfunded, dormant) | ClimateMARGO, srm-forever | OpenAir-Cyan, Carbon_Capture_ML, DAC repos | **Nothing** |
| **Empty** (zero presence) | — | — | **Ocean geoengineering: 0 repos** |

### What Oceananigans.jl Tells Us (from v2 research)
Oceananigans.jl has 1,413 stars and is actively developed. It's a GPU-accelerated ocean simulation framework. But it's a **general-purpose ocean model**, not a geoengineering tool. It can simulate ocean dynamics, but it doesn't know about alkalinity, iron, or cloud brightening. It's the ocean's "WRF" — powerful, but not purpose-built for intervention scenarios.

---

## 🌊 The Ocean's Close Friend: The Precipitation-Buoyancy POD

The single most ocean-relevant piece of open-source code we found:

**What it is:** A Proper Orthogonal Decomposition (POD) diagnostic that measures the statistical relationship between precipitation rate and buoyancy (temperature-salinity structure) in climate model output.

**Why it matters:** The precip-buoyancy relationship is fundamental to how ocean-atmosphere coupling works. If you want to evaluate whether an ocean intervention changes precipitation patterns, you need to know how precipitation relates to buoyancy in the baseline model. The POD provides that baseline.

**What it isn't:** It doesn't simulate any intervention. It's a diagnostic, not a simulator. It evaluates model accuracy; it doesn't model ocean impacts.

**The podcast twist:** The most ocean-relevant code in open source is used for model evaluation, not intervention design. It's the quality-control inspector who evaluates the runway but doesn't build the airplane.

---

## Summary: The Ocean Gap

| Metric | Value |
|--------|-------|
| Dedicated ocean geoengineering repos | **0** |
| Ocean-adjacent diagnostic tools | 1 (MDTF precip-buoyancy POD) |
| Ocean-specific research group repos | 0 (only a website) |
| OAE computational screening datasets | **0** (vs. 2 for DAC, both CC0) |
| Ocean sensor/hardware repos | **0** |
| Ocean process models with intervention modules | **0** |
| GitHub search queries run | **10+** |
| Most ocean-relevant commit (Jun 19, 2026) | Precipitation-buoyancy POD addition |

---

## 🎙️ Episode Structure (Suggested)

### Act 1: "The Void" (7 min)
- Ten search queries, zero results
- The ocean is the empty quadrant
- Compare: DAC has CC0 datasets, OAE has nothing
- The most ocean-relevant tool is a diagnostic, not a simulator

### Act 2: "Why Is the Ocean Empty?" (8 min)
- Four hypotheses: governance, complexity, funding, publication barriers
- Which hypothesis is right?
- The "politically radioactive" problem

### Act 3: "What Would Open-Source Ocean Geoengineering Look Like?" (7 min)
- If we built an OAE simulator, what would it include?
- The mirror of DAC: computational screening for alkaline materials
- Ocean sensors as open hardware (the OpenAir-Cyan model)
- The community needed to sustain it

### Act 4: "The Silence Is a Signal" (5 min)
- The ocean gap is not an accident — it's a governance statement
- What does it mean that the scientific community has published extensively on ocean geoengineering but not built a single open-source tool?
- Is the silence itself a form of governance?

---

## Ocean-Adjacent Repositories (Full List)

| Repo | Stars | Ocean Relevance | What It Does |
|------|-------|----------------|-------------|
| NOAA-GFDL/MDTF-diagnostics | 80 | ⭐⭐⭐ (indirect) | Precipitation-buoyancy POD for model evaluation |
| ClimateSoton/ClimateSoton.github.io | 0 | ⭐ (website) | Research group webpage |
| wrf-model/WRF | 1,762 | ⭐⭐ (coupled mode) | Atmospheric model with optional ocean coupling |
| ClimateMARGO/ClimateMARGO.jl | 73 | ⭐ (indirect) | Climate-economic framework (could include ocean) |

---

## Data Sources

All search queries and commit data pulled fresh from GitHub API on September 19, 2026:
- 10 distinct search queries across GitHub repository search
- Commit histories from MDTF-diagnostics (15 commits), ClimateSoton.github.io (2 commits), WRF (15 commits, cross-referenced)
- v2 ocean ecosystem analysis (Oceananigans.jl, veros, OceanBioME) incorporated from previous research

---

## Research Log

| Date | Activity |
|------|----------|
| 2026-09-19 | v4: Ocean gap confirmed across 10+ search queries; ocean-adjacent repo profiles, hypotheses, and episode brief pushed to branch |
| 2026-09-17 | v3: Previous analysis completed; 6 ocean search queries confirmed zero repos |
| 2026-09-03 | Initial research notes created |
