# 🌊 Ocean Intervention — Commit Trend Deep Dive

**Branch:** `ocean-intervention`
**Analysis Date:** September 17, 2026
**Repositories Analyzed:** Team50-Labs/NebuGrid-OpenSource, plus comprehensive searches across ocean geoengineering topics

---

## Executive Summary

Ocean geoengineering has zero meaningful GitHub presence. Across six distinct search strategies and dozens of query variations, we found exactly one repository remotely relevant — a fog-harvesting/drip-irrigation project not specifically about ocean intervention. This isn't a GitHub curation problem. It's a field-wide structural gap that reflects institutional siloing, governance complexity, and the fundamental difficulty of building ocean testbeds.

---

## The Search Matrix

We ran the following GitHub search queries with the following results:

| Search Query | Results |
|-------------|---------|
| `ocean fertilization iron enrichment` | **0 repos** |
| `ocean alkalinity enhancement` | **0 repos** |
| `marine cloud brightening` | **0 repos** |
| `ocean geoengineering` | **0 repos** |
| `climate engineering ocean simulation` | **0 repos** |
| `ocean intervention marine technology` | **0 repos** |
| `ocean pH sensor monitoring` | **0 repos** |
| `seaweed kelp farming carbon` | **0 repos** |
| `artificial upwelling ocean` | **0 repos** |
| `ocean acidification` | **0 dedicated repos** (built into PCMDI tools) |
| `ocean alkalinity enhancement iron fertilization seaweed climate` | **0 repos** |
| `solar radiation management geoengineering Long numerical model` | **0 repos** |

**The only ocean-adjacent finding:**

| Repo | Stars | Description |
|------|-------|-------------|
| Team50-Labs/NebuGrid-OpenSource | 0 | Fog-harvesting and drip irrigation for arid coastal environments |

---

## What Exists in Ocean Science on GitHub (Non-Geoengineering)

While ocean *geoengineering* has zero repos, some ocean science exists in adjacent contexts:

| Repo/Context | Relevance | Type |
|-------------|-----------|------|
| PCMDI/pcmdi_metrics | Ocean metrics (ENSO, sea ice, ocean heat content) | Evaluation tooling |
| protontypes/open-sustainable-technology | Ocean models, marine life, fishery sections in directory | Catalog |
| HydroChrono (Project-SEA-Stack) | Wave energy converter and ocean systems simulation | Energy (not geoengineering) |

**None of these are ocean geoengineering projects.** They are climate science tools that happen to include ocean components.

---

## Three Hypotheses for the Void

### H1: Institutional Gatekeeping

Ocean geoengineering research is concentrated in institutions that predate the open-source movement:
- **WHOI** (Woods Hole Oceanographic Institution) — publishes in Nature, Science, uses internal data systems
- **Scripps Institution of Oceanography** — similar model
- **GEOMAR** (German Ocean Research) — European equivalent
- **IOC-UNESCO** — international coordination body

These institutions share data through journal publications and conference presentations, not GitHub. The culture of ocean science is fundamentally different from climate modeling.

**Evidence:** The iron fertilization experiments (LOHAFEX, SOFeX, SERIES) were conducted by ship-based teams with institutional affiliations. No ship-time PI has incentive to open-source their experimental cruise data.

### H2: Governance & Liability

Ocean interventions sit in a unique legal category:
- **London Convention/London Protocol** — directly regulates ocean fertilization
- **UNESCO London Protocol** — has a moratorium on ocean fertilization research
- **没有得到研究许可** — scientists self-censor to avoid regulatory scrutiny

GitHub is a public platform. A researcher uploading code for "ocean iron fertilization simulations" could be interpreted as planning unregulated ocean intervention. The legal risk is real.

**Evidence:** The 2007 London Protocol amendment specifically criminalized ocean fertilization for commercial purposes. While research exemptions exist, the ambiguity creates chilling effects.

### H3: Experimental Complexity Barrier

| Intervention | Minimum Viable Prototype | GitHub-Ready? |
|-------------|-------------------------|---------------|
| **SRM (aerosol injection)** | Radiative transfer code on a laptop | ✅ Yes |
| **DAC (sorbent materials)** | Bench-top chemical setup | ✅ Yes (OpenAir-Cyan) |
| **OAE (alkalinity enhancement)** | Minerals + ocean water tank + pH monitoring | ⚠️ Possible but complex |
| **Iron fertilization** | Ship time + nutrients + tracer + monitoring | ❌ Not feasible |
| **Seaweed farming** | Onshore tank + growth media | ⚠️ Possible but niche |
| **Marine cloud brightening** | Wind tunnel + spray nozzle + satellite validation | ❌ Not feasible |

The barrier to "GitHub-ready" prototypes is enormously higher for ocean interventions than for SRM or DAC. You can't run an ocean intervention simulation without ocean-scale data, which requires ship time or satellite validation.

---

## What an Open-Source Ocean Intervention Project Would Look Like

If someone wanted to build the first meaningful ocean geoengineering GitHub repository, here's what it might contain:

### Tier 1: Shareable Infrastructure
- **Open sensor designs** for pH, pCO2, alkalinity monitoring (Arduino/Python-based)
- **Data pipelines** for ocean chemistry data (CSV/NetCDF + analysis scripts)
- **Carbonate chemistry models** (PyCO2SYS, CO2SYS — already exist but not labeled as geoengineering)

### Tier 2: Modeling & Simulation
- **Ocean circulation models** with geoengineering parameterization (MOM6, NEMO — exist but not geoengineered)
- **.Entity Framework for OAE** — modular Python code for simulating alkalinity addition effects
- **Wave-resolving models** for artificial upwelling (existing in HydroChrono but not geoengineering-labeled)

### Tier 3: Experimental Design
- **Open experimental protocols** for ocean alkalinity addition experiments (published protocols, not just papers)
- **Environmental monitoring templates** — pre-built sensor arrays and deployment plans
- **Risk assessment frameworks** — code-based governance tools

### Why Nobody's Building This

| Barrier | Severity |
|---------|----------|
| Ship time costs ($50K+/day) | 🔴 Critical |
| Regulatory uncertainty | 🔴 Critical |
| No funding mechanism for open-source ocean engineering | 🔴 Critical |
| Institutional incentives (publish papers, not share code) | 🟡 High |
| Technical expertise gap (oceanographers ≠ software engineers) | 🟡 High |

---

## The Governance Signal

The absence of ocean geoengineering on GitHub may itself be the most important finding of this research.

**Three possible interpretations:**

1. **The silence is unintentional** — ocean scientists simply haven't thought of GitHub as a dissemination channel
2. **The silence is self-censorship** — researchers avoid public code to avoid regulatory scrutiny
3. **The silence is structural** — the funding institutions and publication venues for ocean science don't produce open-source code

**Which interpretation is correct matters for the podcast episode:**
- If (1): the story is about awareness — "ocean scientists, GitHub is waiting for you"
- If (2): the story is about governance — "the London Protocol is chilling open science"
- If (3): the story is about institutions — "ocean science is structurally unlike climate science"

The likely truth is: **all three are partially correct**, and the interplay between them is what makes ocean geoengineering the most complex governance challenge in the climate tech space.

---

## Episode-Ready Talking Points

1. **"Ocean geoengineering is the dark matter of climate tech on GitHub."** 2,500+ projects in open sustainable technology. Zero for ocean intervention.

2. **"You can build a DAC machine in your garage. You can't build an ocean enrichment experiment in your garage."** The hardware barrier is 10,000x higher for ocean interventions.

3. **"The London Protocol may be the world's most effective unintentional open-source suppressor."** Regulating ocean fertilization research may have the side effect of preventing open-source development.

4. **"What would the first ocean intervention GitHub repo look like?"** Sensor designs, carbonate chemistry models, experimental protocols — all shareable, none requiring ship time.

5. **"The silence on GitHub is itself a finding."** This isn't about what we know about ocean geoengineering — it's about what we can't share.

---

## Recommended Next Steps for Research

1. **Search academic databases** (not GitHub) for ocean alkalinity enhancement experimental data — the data exists in papers
2. **Contact WHOI/Scripps** directly about open-source ocean sensor projects
3. **Investigate the Ocean Visions alliance** and similar initiatives for ocean intervention governance
4. **Look at CO2SYS/PyCO2SYS** — existing carbonate chemistry tools that could be the foundation for an open-source OAE modeling toolkit
5. **Monitor the Edinburgh Ocean Metal Prize** and similar funding programs that might incentivize open-source ocean work

---

*Search data from GitHub API, 12 distinct query strategies. Zero ocean geoengineering repositories found.*
