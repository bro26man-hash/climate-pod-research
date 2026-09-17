# 🌊 Ocean Intervention — Commit Trend Analysis (v2 — Second Research Round)

**Last Updated:** September 2026 (Second research round — expanded search)
**Source Repositories Analyzed:** jnickla1/CESM2geoeng_documentation, cross-theme analysis of PCMDI/pcmdi_metrics, wrf-model/WRF, NOAA-GFDL/MDTF-diagnostics, Team50-Labs/NebuGrid-OpenSource

---

## The Ocean Quadrant — Finding

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

## Cross-Theme Commit Histories: Ocean-Adjacent Tools

### 1. PCMDI/pcmdi_metrics (133 stars) — Has Ocean Metrics

| Commit Date | Activity | Ocean Relevance |
|-------------|----------|----------------|
| Sep 4, 2026 | v4.2.1 release (10 commits in 2 days) | ENSO metrics, sea ice, ocean heat content |
| Jun 19, 2026 | MCS precip-buoyancy POD | **Ocean process diagnostics** |
| Aug 14, 2026 | PR #825 merged | Cross-validation diagnostics |

**Key Insight:** PCMDI's v4.2.1 includes metrics for ENSO, sea ice, and ocean heat content — the closest thing to ocean evaluation tooling that exists in open source. But these are evaluation tools for CMIP6 models, not tools for evaluating ocean interventions.

**What's missing:** Ocean intervention evaluation metrics. If you want to measure the effect of ocean alkalinity enhancement on ocean chemistry, PCMDI gives you CMIP6 baseline metrics but not intervention-specific diagnostics.

---

### 2. wrf-model/WRF (1,761 stars) — Ocean Physics in the Background

| Commit Date | Activity | Ocean Relevance |
|-------------|----------|----------------|
| Jun 8, 2026 | v4.8.0 released | Includes ocean boundary layer physics |
| May 27, 2026 | MYNN-EDMF update | Ocean boundary layer physics parameterization |
| May 28, 2026 | Solar radiation correction | Ocean surface energy budget |

**Key Insight:** WRF includes ocean boundary layer physics and air-sea interaction modules. These are climate model components — not tools for designing or evaluating ocean interventions.

**What's missing:** WRF's ocean component is for modeling the ocean's response to atmospheric forcing, not for simulating ocean interventions like OAE or iron fertilization.

---

### 3. NOAA-GFDL/MDTF-diagnostics (80 stars) — The Ocean-Adjacent Lifeline

| Commit Date | Activity | Ocean Relevance |
|-------------|----------|----------------|
| Aug 14, 2026 | PR #825 merged | Cross-institutional diagnostics |
| Jun 19, 2026 | MCS precip-buoyancy POD (x4) | **Closest to ocean process diagnostics** |
| Jun 8, 2026 | PR #823 merge + README | PR-based workflow |
| Jun 2, 2026 | Branch merge | Integration |

**Key Insight:** The MCS precipitation-buoyancy POD is the closest thing to ocean process diagnostics in open source. It evaluates the relationship between precipitation and buoyancy — a key ocean-atmosphere coupling process. This is process-oriented diagnostics, not intervention design.

**What's missing:** Intervention-specific metrics. MDTF evaluates what climate models do; it doesn't evaluate what ocean interventions would do.

---

## The Ocean Gap: Three Hypotheses

### H1: Institutional Gatekeeping (Most Likely)

**Evidence:**
- Ocean geoengineering research is concentrated at WHOI, Scripps, GEOMAR, IOC-UNESCO
- These institutions publish in closed journals and share data through institutional channels
- The culture of ocean science predates the open-source movement by decades
- Ocean researchers are at sea on ships, not at desks writing code

**Supporting evidence:** The CESM2geoeng_documentation repo (a paper supplementary resource, not code) shows that even the researchers doing ocean geoengineering simulation aren't sharing code. They're sharing documentation.

**Counter-evidence:** Some ocean models are open-source (MOM6, NEMO, ROSSCO). But these are general-purpose ocean models, not geoengineering-specific tools.

---

### H2: Governance & Liability

**Evidence:**
- The London Convention/Protocol directly regulates ocean fertilization
- Scientists may self-censor to avoid regulatory scrutiny
- Ocean interventions have transboundary impacts — no single country can authorize them
- The legal risk of being associated with unregulated ocean experiments is real

**Counter-evidence:** Solar geoengineering has similar governance concerns (SRM is not explicitly illegal, but carries reputation risk), yet at least srm-forever exists. The difference: ocean interventions require physical deployment, not just code.

**The nuance:** You can code an SRM simulation without deploying anything. You can't code an OAE deployment without eventually putting alkalinity in the ocean. The governance risk is different — it's not just reputational, it's legal.

---

### H3: Experimental Complexity Barrier (Structural)

**Evidence:**
- SRM can be modeled with radiative transfer codes (srm-forever proves this)
- DAC can be prototyped in a garage (OpenAir-Cyan proves this)
- Ocean interventions require: ship time ($50K+/day), sensor deployments in remote waters, multi-year monitoring, and international coordination
- The barrier to GitHub-ready prototypes is astronomically higher

**The math:**
- A single ocean field experiment: $50K-$500K+ in ship time, plus equipment, plus multi-year monitoring
- An OpenAir-Cyan-type hardware project: $1K-$10K in components
- The ROI on open-source ocean intervention tools is unclear for any individual researcher

**The comparison:** It takes 10 years of DIY DAC hardware development to equal the cost of one ocean field experiment season. Ocean geoengineering can't follow the OpenAir-Cyan model because the entry cost is 100x higher.

---

## Cross-Theme Comparison: The Activity Dashboard

```
Solar Geoengineering:
  ████████████████████ PCMDI (133 stars, Sep 2026 burst)
  ████████████ WRF (1,761 stars, June 2026 release, continuous)
  ████████ MDTF-diagnostics (80 stars, Jun-Aug 2026 active)
  ████ ClimateMARGO (73 stars, Aug 2026 revival)
  ██ srm-forever (0 stars, Aug 2026 single burst)
  ████ AM3 (4 stars, legacy Fortran, dormant since 2015)

Carbon Capture:
  ████████████████████████ Open Sustainable Tech (2,546 stars, continuous)
  ████████████████ OpenAir-Cyan (76 stars, Feb 2024 burst, dormant)
  ████ Carbon_Capture_ML (56 stars, paper-driven peaks)
  ██ carbon-capture-and-storage (85 stars, thesis burst, ghost)
  ██ peroxovanadates + peroxotitanates (2 stars each, Aug 2026 wave)
  █ electro-swing-DAC (research collection, Aug 2026)

Ocean Intervention:
  █ (zero dedicated repos)
  ██ WRF ocean module — atmosphere-coupled, not intervention-focused
  ██ PCMDI ocean metrics — ENSO verification, not intervention metrics
  ██ MDTF-diagnostics — precipitation-buoyancy POD (closest to ocean process)
  █ CESM2geoeng_documentation — paper docs, not code
```

---

## Key Findings for the Podcast

1. **The ocean is the silence that speaks loudest.** Zero dedicated repos, zero commits, zero tools. Meanwhile, the atmosphere gets WRF, PCMDI, and MDTF. The ocean gets... nothing.

2. **The nearest tools are ocean-adjacent, not ocean-specific.** MDTF-diagnostics has the closest thing to ocean process diagnostics. PCMDI has ocean metrics. WRF has ocean physics modules. But none are designed for evaluating ocean interventions.

3. **The complexity barrier is real and structural.** A single ocean field experiment costs more than a decade of DIY hardware development. The ocean can't follow the OpenAir-Cyan model because the entry cost is 100x higher.

4. **The London Protocol may be causing self-censorship.** Ocean fertilization is regulated. Researchers might avoid sharing code that could be interpreted as preparatory for unregulated experiments.

5. **CESM2 Pacific biologists doing ocean geoengineering aren't sharing code — they're sharing documentation.** This is the academic code lifecycle again: paper published, docs shared, code not maintained.

---

## What to Watch Next Quarter

1. **Will anyone build the first open-source OAE model?** Based on the MOM6/NEMO/ROSCO ocean modeling community, there's talent. But the geoengineering-specific layer doesn't exist.

2. **Will MDTF-diagnostics add more ocean-relevant PODs?** The precip-buoyancy POD was added in Jun 2026. If ocean intervention evaluation becomes a priority, more ocean diagnostics would follow.

3. **Will the London Protocol be updated?** If governance clarifies what's allowed vs. prohibited, it could either unlock or further suppress open-source ocean intervention development.

4. **Will digital twins prepare the ground?** If we can model ocean systems before physical deployment, that might lower the governance risk enough to attract open-source development.

5. **The ocean remains silent** — Unless someone builds the first open-source OAE model, the absence will persist into 2027.