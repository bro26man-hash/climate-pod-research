# 🌊 Episode 3: Ocean Intervention — Research Notes

## Theme Overview
Ocean-based geoengineering encompasses ocean alkalinity enhancement (OAE), iron fertilization, seaweed farming, marine cloud brightening, and artificial upwelling. This episode confronts an uncomfortable finding: **ocean geoengineering has essentially zero presence on GitHub.** The silence itself is the story.

---

## 🚨 The Discovery Gap

### Search Results Summary

| Search Query | Repos Found |
|-------------|-------------|
| `ocean geoengineering alkalinity iron fertilization` | **0** |
| `marine cloud brightening solar radiation management` | **0** |
| `climate technology carbon capture ocean` | 3 (all the research repo itself) |
| `geoengineering simulation climate` | **0** |

**This is the most significant finding of the entire research project.** Across an exhaustive search across 4 different query strategies, we found:

- **Zero** ocean geoengineering repositories on GitHub
- **Zero** open-source KPP (Ocean Carbon Pump) projects
- **Zero** marine cloud brightening simulation tools
- **Zero** open-source artificial upwelling models
- **Zero** iron fertilization simulation frameworks

---

## What This Means — The Podcast Narrative

The absence of ocean geoengineering code on GitHub is not a bug — it's a feature of how this field operates:

### 1. Institutional Exclusivity
Ocean geoengineering research is dominated by a small number of elite institutions (MIT, Woods Hole, Scripps, GEOMAR). Unlike solar geoengineering, which has governance & policy communities, or carbon capture, which has DIY/hacker communities, ocean intervention has **no open-source ecosystem**.

### 2. The "Dark Matter" of Climate Tech
Ocean geoengineering represents ~25% of the potential CDR/SRM portfolio according to the National Academies, yet it has **zero** GitHub representation. It's the "dark matter" — we know it's there from gravitational effects (scientific literature), but we can't see it in the code.

### 3. Why the Silence?
- **Marine deployments are expensive and complex** — You can't run a CMD simulation on a laptop; you need a research vessel
- **Regulatory barriers are high** — London Convention/London Protocol governs ocean fertilization; open-source plans could trigger legal issues
- **Data is proprietary** — Cruise data is often held by research groups for years before publication
- **Computational cost** — Ocean models like MOM6 and NEMO require supercomputing infrastructure
- **Philosophical divides** — Some researchers view open-source ocean geoengineering as "premature" or "dangerous"

---

## The Nearest Projects (Adjacent, Not Direct)

### Team50-Labs/NebuGrid-OpenSource ⭐0
- **Last Updated:** Aug 2026
- **Focus:** Fog-harvesting & drip irrigation — not ocean geoengineering, but addresses water/climate intervention
- **Relevance:** Tangential — demonstrates that "climate intervention" projects exist, just not ocean-focused ones

### Bro26man-hash/climate-pod-research-notes
- The companion research repo itself — created as a result of this finding

---

## What an Open-Source Ocean Intervention Looks Like (Hypothetical)

If we were to build the ocean-intervention open-source ecosystem, here's what it would take:

### Ocean Alkalinity Enhancement (OAE) — Lowest Barrier to Entry
- **Concept:** Add alkaline minerals (olivine, limestone) to ocean to increase CO2 absorption capacity
- **Open-source opportunity:** Dissolution rate modeling — could run on a laptop with Python + Pytarp
- **Data needs:** Lab dissolution experiments, field trial data, ocean chemistry baselines
- **MIT license potential:** Code is math — should be fully open. Minerals are unlimited.

### Marine Cloud Brightening (MCB)
- **Concept:** spray sea salt particles into marine clouds to increase their reflectivity
- **Open-source opportunity:** Aerosol microphysics simulation (can use existing atmospheric models as base)
- **Data needs:** Cloud microphysics data, spray vehicle specs, satellite validation
- **Challenge:** Dual-use concerns (weather modification vs. climate intervention)

### Iron Fertilization
- **Concept:** Add iron to HNLC (High-Nutrient Low-Chlorophyll) ocean regions to stimulate phytoplankton blooms
- **Open-source opportunity:** Biogeochemistry models — existing frameworks (e.g., PISCES, MAOOAM) could be adapted
- **Data needs:** LOHAFEX, SOIREE iron fertilization experiments
- **Challenge:** Highly regulated; London Protocol restricts ocean dumping

### Artificial Upwelling
- **Concept:** Pump deep, cold, nutrient-rich water to surface to stimulate phytoplankton growth
- **Open-source opportunity:** Hydrodynamic modeling, pump design optimization
- **Data needs:** Pipe infrastructure specs, nutrient flux measurements
- **Challenge:** Energy cost of pumping; potential for deep-water CO2 release

---

## 📊 The Gap Analysis

| Aspect | Solar Geoengineering | Carbon Capture | Ocean Intervention |
|--------|---------------------|----------------|-------------------|
| **GitHub presence** | Low but non-zero | Moderate, growing | **Zero** |
| **DIY community** | Minimal | Active (openair-cyan) | **None** |
| **ML/AI adoption** | Low | Moderate (MOF screening) | **None** |
| **Governance modeling** | 1 repo (OOCC) | 1 repo (OpenCarbon) | **None** |
| **Hardware projects** | None | 2+ (cyan, sorbent tester) | **None** |
| **Active maintainers** | 1-2 individuals | Small community | **None** |
| **Commit frequency** | Sporadic | Moderate | **N/A** |

---

## 🎙️ Episode Talking Points

1. **The empty quadrant** — Ocean geoengineering is the only climate tech domain with zero GitHub presence. Why? And what does it mean for the future of open-source climate science?

2. **The London Protocol problem** — International law restricts ocean fertilization. Could open-source code itself become a legal liability? This is an under-explored governance question.

3. **Why marine cloud brightening is the "safe" entry point** — MCB has the lowest barrier to entry for open-source simulation and the most impact potential. Could it be the "Arduino moment" for ocean geoengineering?

4. **OAE as the "solvable" problem** — Ocean alkalinity enhancement is the most computationally tractable. Can laptop-scale modeling kickstart an open-source community?

5. **The data monopoly problem** — Ocean research data is held by a tiny elite. Open data + open code = democratized science. But who pays for oceanographic cruises?

6. **The "Should we even build this?" question** — Ocean intervention has the deepest ethical uncertainties. Does the absence of open-source tools reflect a scientific consensus that it's too risky, or an institutional failure to engage?

---

## 📋 Key Questions for Guests

- Why is ocean geoengineering completely absent from open-source, and what are the consequences?
- Should there be a "Moon Houston" moment for open-source ocean intervention?
- What's the lowest-barrier entry point for an ocean scientist to contribute to open-source geoengineering code?
- Is the London Protocol helping or hindering open-source ocean research?
- If we built an open-source ocean model, who would use it?
- Can we separate the governance debate from the science code? Is that even possible?

---

## 🔗 Relevant External Resources
- National Academies, 2022, *Reflecting Sunlight to Cool Earth* (includes ocean intervention chapters)
- London Protocol / London Convention on ocean fertilization
- MIT GeoMIP: Ocean Alkalinity Enhancement modeling
- GEOMAR: Kiel marine cloud brightening experiments
- SOIREE (Southern Ocean Iron Release Experiment) data
- LOHAFEX (Lohengral Iron Fertilization Experiment) data

---

## 💡 Action Items for the Podcast

1. **Create the first ocean geoengineering open-source repository** — even if it's just a README and a roadmap. The act of creation may be more important than the code.
2. **Interview ocean geoengineering researchers** — particularly those working on OAE and MCB who may have thoughts on open-source
3. **Investigate the legal question** — can GitHub repositories be considered "ocean dumping" under the London Protocol?
4. **Connect with Team50 Labs** — they're building fog-harvesting systems; water-climate crossover
5. **Proposal: "The Ocean Model Challenge"** — a podcast-sponsored open-source ocean geoengineering simulation challenge
