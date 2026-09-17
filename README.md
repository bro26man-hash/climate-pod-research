# 🌊 Ocean Intervention — Episode Research Notes

**Podcast Theme:** Ocean-Based Geoengineering — Alkalinity Enhancement, Iron Fertilization, Seaweed & More
**Branch:** `ocean-intervention`
**Last Updated:** September 2026

---

## 🎙️ Episode Angle

**This is the biggest story the GitHub data reveals: the ocean geoengineering quadrant is essentially empty.** Our search across GitHub for ocean alkalinity enhancement, iron fertilization, marine cloud brightening, and seaweed-based interventions returned almost nothing. The experimental complexity, governance sensitivity, and institutional siloing of ocean research create the largest open-source gap in all of climate technology. This isn't just a podcast episode — it's a fundamental finding about how climate innovation gets organized on the internet.

---

## 🔍 Project Discoveries

### The Ocean Quadrant — What We Found

| Repo | Stars | Forks | Language | Last Commit | Description |
|------|-------|-------|----------|-------------|-------------|
| **[Team50-Labs/NebuGrid-OpenSource](https://github.com/Team50-Labs/NebuGrid-OpenSource)** | 0 | 0 | — | Aug 20, 2026 | Fog-harvesting and drip irrigation system for arid coastal environments. Not ocean geoengineering per se, but the only ocean-adjacent project found. |

### Related Cross-Theme Projects (Not Ocean-Specific)

| Repo | Stars | Theme | Relevance |
|------|-------|-------|-----------|
| **[PCMDI/pcmdi_metrics](https://github.com/PCMDI/pcmdi_metrics)** | 133 | Solar | Ocean metrics evaluation (ENSO, sea ice) — the closest thing to ocean simulation in open source |
| **[prashaant1926/open-earth-digital-twin-simulation](https://github.com/prashaant1926/open-earth-digital-twin-simulation)** | 0 | Solar | Agent-based Earth systems — could eventually model ocean interventions |

### What We Couldn't Find

| Topic | Expected Presence | Actual Presence |
|-------|-------------------|-----------------|
| **Ocean Alkalinity Enhancement (OAE)** | Multiple repos; mineral weathering kits, sensor networks | **Zero dedicated repos** |
| **Iron Fertilization** | At least 1-2 legacy repos from 2000s experiments | **Zero repos** |
| **Marine Cloud Brightening (MCB)** | Cloud model integrations, spray mechanism designs | **Zero repos** |
| **Artificial upwelling/downwelling** | Pump designs, energy analysis | **Zero repos** |
| **Seaweed/kelp farming for carbon** | Growth models, LCA tools | **Zero repos** |
| **Ocean acidification monitoring** | pH sensor networks, data analysis | **Zero repos** (built into PCMDI tools) |

---

## 📊 Commit Trend Analysis

### The Finding: Ocean Geoengineering Has No GitHub Footprint

Unlike solar geoengineering (PCMDI, 133★; srm-forever, 4 commits) or carbon capture (OpenAir-Cyan, 76★; peroxovanadates, computational chemistry wave), **ocean intervention has zero meaningful open-source presence on GitHub.** This was confirmed by searching across multiple query strategies:

1. **Direct searches** for "ocean fertilization," "ocean alkalinity enhancement," "marine geoengineering" returned zero results.
2. **Broader searches** for "ocean intervention marine technology" returned zero results.
3. **Related searches** for "ocean monitoring pH sensor" returned nothing ocean-specific.

### What This Tells Us — Three Hypotheses

**H1: Institutional Gatekeeping.** Ocean geoengineering research is concentrated in a handful of institutions (WHOI, Scripps, IOC-UNESCO, GEOMAR) that publish in closed journals and share data through institutional channels, not GitHub. The culture of ocean science predates the open-source movement.

**H2: Governance & Liability.** Ocean interventions carry unique legal and governance complexity — the London Convention/London Protocol regulate ocean fertilization directly. The risk of being associated with unregulated ocean experiments may deter public code sharing.

**H3: Experimental Complexity Barrier.** SRM can be modeled with radiative transfer codes. DAC can be prototyped in a garage (OpenAir-Cyan). Ocean interventions require ship time, sensor deployments in remote waters, and multi-year monitoring — the barrier to "GitHub-ready" prototypes is enormously higher.

### Trending Implications:
- 🚨 **Ocean intervention is the "dark matter" of climate tech on GitHub** — it exists in the scientific literature but not in open code
- 🔮 **Digital twin approaches** (Open Earth Digital Twin, CMIP6 evaluation) may be the first open-source path to ocean modeling
- ⚠️ **The governance story dominates the technical story** — any ocean geoengineering episode must address why open source hasn't followed
- 🔮 **Ocean alkalinity enhancement** is the most promising near-term ocean intervention; its absence from GitHub is itself a finding

---

## 🎙️ Key Episode Questions

1. **Why is ocean geoengineering invisible on GitHub?** The answer isn't technical — it's institutional, legal, and cultural. What would it take to change that?
2. **What would an "open-source ocean alkalinity" project look like?** Open data from alkalinity addition experiments, open sensor designs for pH monitoring, open modeling of carbonate chemistry — but who would run it?
3. **Is the absence itself a governance signal?** The silence on GitHub may reflect the London Protocol's restrictions on ocean fertilization research — scientists self-censor to avoid regulatory scrutiny.
4. **Can digital twins prepare the ground?** If we can model ocean systems in silico (PCMDI metrics, Earth digital twins) before physical deployment, that might lower the governance risk enough to attract open-source development.
5. **What's the difference between ocean research that can be open-sourced vs. that which can't?** Sensor designs and data pipelines are shareable; actual ocean experiments are not. Where's the line?

---

## 🔗 Related Resources
- **London Protocol on Ocean Fertilization:** http://www.loml.org/
- **WHOI Ocean Climate Change Institute:** https://www.whoi.edu/scientific/oci/
- **IOC-UNESCO Ocean Science:** https://www.unesco.org/en/ocean-science
- **PCMDI Metrics (ocean metrics):** http://pcmdi.llnl.gov/research/metrics/
- **Co-Sci Open Earth Digital Twin:** https://co-sci.org
- **OpenAir-Cyan (the only ocean-adjacent DAC project):** https://openair-collective.github.io/openair-cyan/
