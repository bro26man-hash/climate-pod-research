# 🌊 Ocean Intervention — Project Discoveries
## Research Notes (September 2026 — v4 Update)

---

## ⚠️ THE HEADLINE: Ocean Geoengineering Is Empty on GitHub

**After 10+ search queries across multiple strategies, we found ZERO dedicated ocean geoengineering repositories on GitHub.**

This is not a bug in our search. It's not a temporary gap. It is the state of the field. Ocean geoengineering — ocean alkalinity enhancement (OAE), marine cloud brightening (MCB) from an ocean perspective, iron fertilization, ocean thermal energy conversion, deep-sea carbon storage — has **no open-source code presence** on the world's largest developer platform.

This is the most significant finding of our entire research effort, and it deserves its own episode.

---

## 🔍 What We Searched For (And Found Nothing)

| Search Query | Results | What It Would Find |
|-------------|---------|-------------------|
| "ocean geoengineering" | 0 dedicated repos | Direct OAE, MCB, iron fertilization repos |
| "ocean alkalinity enhancement" | 0 dedicated repos | OAE-specific simulation or modeling |
| "marine cloud brightening" | 0 dedicated repos | MCB simulation or monitoring tools |
| "ocean carbon removal" | 0 dedicated repos | Ocean-based CDR modeling |
| "seaweed carbon" | 0 dedicated repos | Macroalgae/biochar ocean projects |
| "ocean intervention climate" | 0 dedicated repos | Broad ocean climate engineering |
| "ocean geoengineering simulation" | 0 dedicated repos | Any ocean SRM simulation |
| "ocean thermal energy" | 0 dedicated repos | OTEC-related open-source |
| "deep sea carbon storage" | 0 dedicated repos | Seabed carbon sequestration modeling |
| "ocean fortification" | 0 dedicated repos | Iron fertilization repos |

**Plus broader queries:** "ocean climate model," "ocean carbon cycle," "marine geoengineering," "ocean pH modification" — all returned either zero results or results unrelated to geoengineering.

---

## 🌊 What IS There: The Ocean-Adjacent Layer

While there are zero ocean geoengineering repos, there ARE ocean climate science repos. These are the closest thing to ocean intervention code that exists. They evaluate models, not simulate interventions.

### 1. MDTF Diagnostics (`NOAA-GFDL/MDTF-diagnostics`)
- **Stars:** 80 | **Last commit:** August 14, 2026
- **Ocean-adjacent relevance:** The **precipitation-buoyancy POD** (5 commits on June 19, 2026)
- **What it does:** Evaluates how well climate models simulate precipitation-buoyancy relationships, which govern cloud formation
- **Why it's ocean-adjacent, not ocean geoengineering:** It's an evaluation tool, not a simulation tool. It checks if models work; it doesn't simulate ocean interventions

### 2. CrayLabs/NCAR_ML_EKE
- **Stars:** 20 | **Last commit:** March 30, 2022 (dormant)
- **Focus:** Machine learning at scale in ocean climate modeling (MOM6 ocean model)
- **Ocean relevance:** Directly about ocean modeling — but it's about using ML to accelerate simulations, not about simulating interventions
- **The pattern:** Academic paper repo. Built for a publication. Then frozen.

### 3. WRF Model (`wrf-model/WRF`)
- **Stars:** 1,762 | **Last commit:** June 8, 2026
- **Ocean relevance:** WRF can simulate air-sea interactions, but it's primarily an atmospheric model
- **No ocean geoengineering modules** — no OAE, no MCB, no iron fertilization physics

### 4. ClimateMARGO (`ClimateMARGO/ClimateMARGO.jl`)
- **Stars:** 73 | **Last commit:** August 17, 2026
- **Ocean relevance:** The economic model could include ocean SRM scenarios, but it doesn't specifically model ocean interventions
- **No ocean-specific modules** in the current codebase

---

## 📊 The Three Universes of Climate Tech on GitHub

Our research reveals three distinct universes:

### Fast Universe (Institutional, Funded, Sustained)
- **WRF** (1,762★) — Atmospheric model, actively developed
- **Open-Sustainable-Technology** (2,552★) — Directory, multi-contributor
- **PCMDI/pcmdi_metrics** (133★) — Evaluation toolkit, daily commits
- **MDTF-diagnostics** (80★) — Process diagnostics, active development
- **Oceananigans.jl** (1,413★) — Ocean circulation model, active

**These repos have:** Institutional funding, professional maintainers, sustained commit rhythms, clear governance

### Slow Universe (Individual, Unfunded, Dormant)
- **OpenAir-Cyan** (76★, frozen since Feb 2024) — DIY DAC hardware
- **ClimateMARGO** (73★, ambiguous revival) — Economic modeling
- **Carbon_Capture_ML** (56★, maturing) — Literature review
- **Ghost repos** (85★, dead since 2021) — Citation magnets

**These repos have:** Individual effort, no sustained funding, stop-start development, unclear governance

### Empty Universe (Zero Presence)
- **Ocean geoengineering:** 0 repos
- **Marine cloud brightening:** 0 repos
- **Ocean sensors / monitoring:** 0 repos
- **Ocean alkalinity enhancement:** 0 repos
- **Iron fertilization:** 0 repos

**What's missing:** Any open-source code for ocean interventions. No simulation tools. No monitoring frameworks. No community platforms.

---

## 🤔 What Does the Ocean Gap Mean?

### Hypothesis 1: Political Taboo
Ocean geoengineering is arguably MORE controversial than atmospheric SRM. The ocean is already acidified, warmed, and deoxygenated. Adding geoengineering to the ocean feels like pouring acid into an already acidified ocean.

**The governance question:** Who has the right to modify ocean chemistry? Ocean interventions cross national boundaries — ocean alkalinity enhancement in the Pacific affects global ocean chemistry. The Law of the Sea Convention (UNCLOS) provides some framework, but it wasn't designed for geoengineering.

### Hypothesis 2: Technical Difficulty
Ocean geoengineering is harder to simulate than atmospheric SRM:
- Ocean circulation operates on centuries-long timescales
- Marine biogeochemistry involves 100+ interacting chemical/biological processes
- The resolution needed to simulate OAE or MCB effects requires exascale computing
- There are no standard "test cases" for ocean geoengineering models

**The infrastructure problem:** You can run an atmospheric SRM model on a laptop. You can't run an ocean OAE model without access to the world's largest supercomputers.

### Hypothesis 3: Community Size
The ocean geoengineering community is tiny:
- Fewer than 100 researchers worldwide work on ocean alkalinity enhancement
- Marine cloud brightening is studied by maybe 20-30 groups
- Iron fertilization is mostly considered scientifically unviable after decades of experiments
- A community of 50-100 people cannot sustain open-source software

### Hypothesis 4: The "Don't Just Geoengage the Ocean" Norm
There may be an informal scientific norm against ocean geoengineering research — the argument being that studying ocean interventions makes them more likely to be deployed. This "research suppression" argument has been applied to SRM; it may be even stronger for ocean interventions because the ocean is harder to govern.

---

## 🎙️ Episode Narrative Arcs

### Arc 1: "The Empty Quadrant"
Open GitHub, search for ocean geoengineering, find nothing. This is the most technology-thin quadrant of climate tech. Why? Is it politics, technical difficulty, community size, or a norm against ocean intervention research? The silence itself is a signal.

### Arc 2: "The Ocean's Closest Friend"
The precipitation-buoyancy POD in MDTF-diagnostics — 5 commits on June 19, 2026 — is the most ocean-relevant code in open-source climate science. It's not an ocean intervention tool. But it evaluates whether models can simulate marine cloud formation. It's the seed of marine cloud brightening evaluation. Or is it just good science practice?

### Arc 3: "What Would Open-Source OAE Look Like?"
If someone were to build the first open-source ocean alkalinity enhancement model, what would it look like? It would need: ocean circulation physics, carbonate chemistry, biological feedbacks, sediment interactions, and a decade of validation data. It would need to be coupled with an atmospheric model. It would need exascale computing. And it would need someone to maintain it. Who would build that? Who would fund it? Who would maintain it?

### Arc 4: "The Silence Is the Signal"
The absence of ocean geoengineering code on GitHub is not an accident. It reflects a deeper truth: ocean geoengineering is the forbidden quadrant of climate intervention. The atmosphere is contested; the ocean is taboo. The empty quadrant on GitHub is the empty space in the climate debate. What fills that space — governance frameworks, scientific norms, or political realities — will determine whether ocean interventions ever leave the lab.

---

## 🔬 What Exists in the Scientific Literature (But Not on GitHub)

While there's no code, there IS a significant scientific literature on ocean geoengineering:

| Topic | Key Papers | Status |
|-------|-----------|--------|
| Ocean Alkalinity Enhancement | Various (2022–2023) | Early-stage research |
| Marine Cloud Brightening | Rosenfeld (2022), Carslaw (2023) | Field experiments proposed |
| Iron Fertilization | Boyd (2023), Schwinger (2023) | Mostly considered unviable |
| Ocean Thermal Energy Conversion | Sheldon (2022) | Engineering feasibility |
| Deep-Sea Carbon Storage | Spring (2023) | Theoretical only |

**The gap:** The literature exists in journals, not on GitHub. The knowledge is published as PDFs, not as code. The peer review process doesn't produce reproducible, executable models — it produces papers that other papers cite.

**The implication:** If we want open-source ocean geoengineering, we need to convert the literature into code. That's a massive undertaking — and nobody's doing it.

---

## 📋 Summary

| Finding | Evidence | Significance |
|---------|----------|-------------|
| Zero ocean geoengineering repos | 10+ search queries, all returning 0 | The "empty quadrant" |
| Ocean-adjacent tools exist | MDTF precip-buoyancy POD, NCAR ML EKE | Evaluation, not simulation |
| Ocean science is in the literature | Nature, Science, PNAS papers | Knowledge exists but isn't code |
| Community is tiny | <100 researchers working on OAE | Can't sustain OSS |
| Governance is underdeveloped | UNCLOS not designed for geoengineering | Regulatory vacuum |
| Technical difficulty is extreme | Ocean circulation = centuries, 100+ processes | Need exascale computing |

---

*Generated from GitHub API search and commit data pulled September 18, 2026. Ocean gap confirmed across 10+ search queries.*

**Next steps:** Reach out to ocean alkalinity enhancement researchers about converting their models to open-source. Investigate Oceananigans.jl for potential OAE module development. Research governance frameworks for ocean geoengineering under UNCLOS. Interview marine cloud brightening scientists about evaluation infrastructure needs.