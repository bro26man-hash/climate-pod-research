# 🌊 Ocean Intervention — Project Discoveries

**Last Updated:** September 2026
**Research Round:** Second pass — expanded search, cross-theme analysis

---

## The Ocean Quadrant — The Gap

### ZERO DEDICATED REPOSITORIES FOR OCEAN GEOENGINEERING

After exhaustive searching across multiple query strategies in two research rounds:

| Search Query | Repos Found |
|--------------|-------------|
| ocean fertilization | 0 |
| ocean alkalinity enhancement | 0 |
| marine geoengineering | 0 |
| ocean intervention marine technology | 0 |
| ocean pH sensor monitoring | 0 ocean-specific |
| artificial upwelling ocean | 0 |
| seaweed kelp carbon farming | 0 |
| marine cloud brightening | 0 |
| ocean geoengineering CESM2 | 1 (documentation only) |

---

## The Only Ocean-Adjacent Finding

### jnickla1/CESM2geoeng_documentation — Paper Documentation

**What it is:** Documentation for the ocean geoengineering CESM2 paper. Not a codebase — a supplementary resource for a research publication.

**Why it's relevant:** CESM2 is one of the few Earth System Models that includes ocean biogeochemistry. If researchers are simulating ocean alkalinity enhancement or iron fertilization in CESM2, the documentation for that work is the closest thing to open-source ocean intervention code.

**Limitations:** It's documentation, not code. It describes what was done; it doesn't provide tools to do it yourself.

**Pattern:** The academic code lifecycle again — paper published, documentation shared, code not shared or not maintained.

---

## Cross-Theme Ocean Analysis

### What the Atmosphere Tools Have That Ocean Tools Don't

| Capability | Atmosphere (WRF, PCMDI) | Ocean |
|-----------|------------------------|-------|
| **Active simulation code** | ✅ WRF v4.8.0 | ❌ |
| **Model evaluation tools** | ✅ PCMDI v4.2.1 | ❌ |
| **Process diagnostics** | ✅ MDTF-diagnostics | ❌ |
| **Governance frameworks** | ✅ srm-forever, OOCC | ❌ |
| **Economic models** | ✅ Geo-DICE, ClimateMARGO | ❌ |
| **Hardware prototypes** | ✅ (SRM lacks this, but) | ❌ |
| **Active ocean models** | ⚠️ WRF has ocean modules, not intervention-focused | ❌ |
| **Ocean evaluation tools** | ⚠️ PCMDI has ocean metrics, not intervention-specific | ❌ |
| **Ocean diagnostics** | ⚠️ MDTF has precip-buoyancy POD only | ❌ |
| **Ocean governance frameworks** | ❌ | ❌ |
| **Ocean economic models** | ❌ | ❌ |

### Why the Gap?

**H1: Institutional Gatekeeping (Most Likely)**
- Ocean geoengineering research is concentrated at WHOI, Scripps, GEOMAR, IOC-UNESCO
- These institutions publish in closed journals and share data through institutional channels
- The culture of ocean science predates the open-source movement by decades
- Ocean researchers are at sea on ships, not at desks writing code

**H2: Governance & Liability**
- The London Convention/Protocol directly regulates ocean fertilization
- Scientists may self-censor to avoid regulatory scrutiny
- Ocean interventions have transboundary impacts — no single country can authorize them
- The legal risk of being associated with unregulated ocean experiments is real

**H3: Experimental Complexity Barrier (Structural)**
- SRM can be modeled with radiative transfer codes (srm-forever proves this)
- DAC can be prototyped in a garage (OpenAir-Cyan proves this)
- Ocean interventions require: ship time ($50K+/day), sensor deployments in remote waters, multi-year monitoring, and international coordination
- The barrier to GitHub-ready prototypes is astronomically higher

**The math:** A single ocean field experiment costs more than a decade of OpenAir-Cyan-type hardware development. The ROI on open-source ocean intervention tools is unclear for any individual researcher.

---

## What Would an Open-Source Ocean Intervention Project Look Like?

Based on patterns from the other two themes, a successful ocean geoengineering open-source project needs:

1. **Sensor design sharing** (like OpenAir-Cyan's hardware designs) — pH, pCO2, alkalinity sensors for monitoring experiments
2. **Data pipelines** (like PCMDI's evaluation tools) — open data formats for ocean carbonate chemistry measurements
3. **Modeling components** (like WRF's ocean modules) — executable models of ocean alkalinity enhancement, iron fertilization impacts
4. **Governance frameworks** (like srm-forever's transparency) — interactive tools showing legal/regulatory landscape
5. **Community infrastructure** — a maintained repo with multiple contributors, not a single-author ghost town

**The nearest feasible starting point:** Open ocean monitoring sensor designs + data pipelines. This is the DIY hardware equivalent for ocean science — shareable, buildable, and relevant without requiring a ship.

---

## The Ocean Gap in Context

| Theme | Active Repos | Top Stars | Ocean Repos? |
|-------|-------------|-----------|-------------|
| Solar Geoengineering | 6 | 133 | ❌ (no SRM-specific code) |
| Carbon Capture | 5+ | 85 | ❌ (no ocean DAC) |
| Ocean Intervention | 0 | 0 | ❌ (zero dedicated repos) |

**The ocean is the silence that speaks loudest.** Zero dedicated repos. Zero commits. Zero tools. Meanwhile, the atmosphere gets WRF (1,761 stars), PCMDI (133 stars), and MDTF (80 stars). The ocean gets... nothing.

---

## Episode Talking Points

1. **The ocean is the empty quadrant.** After exhaustive searching, there are zero dedicated ocean geoengineering repositories on GitHub. This isn't a technical gap — it's an institutional, legal, and structural one.

2. **The nearest tools are ocean-adjacent, not ocean-specific.** MDTF-diagnostics has the closest thing to ocean process diagnostics. PCMDI has ocean metrics. WRF has ocean physics modules. But none are designed for evaluating ocean interventions.

3. **The complexity barrier is real and structural.** A single ocean field experiment costs more than a decade of DIY hardware development. The ocean can't follow the OpenAir-Cyan model because the entry cost is 100x higher.

4. **The London Protocol may be causing self-censorship.** Ocean fertilization is regulated under the London Convention. Researchers might avoid sharing code that could be interpreted as preparatory for unregulated experiments.

5. **What would a first ocean-intervention repo look like?** Sensor designs for monitoring pH, pCO2, and alkalinity — shareable, buildable, and relevant without requiring a ship. Data pipelines for ocean carbonate chemistry. These are the DIY hardware equivalent for ocean science.

6. **The silence itself is a governance signal.** The absence of ocean intervention code on GitHub isn't just a research gap — it's a statement about who controls ocean governance and who's allowed to participate.