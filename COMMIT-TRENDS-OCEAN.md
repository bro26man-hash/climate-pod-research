# Ocean Intervention — Commit Trend Analysis

**Last Updated:** September 2026
**Source Repositories Analyzed:** Team50-Labs/NebuGrid-OpenSource, plus cross-theme analysis of PCMDI/pcmdi_metrics, wrf-model/WRF, prashaant1926/open-earth-digital-twin-simulation

---

## The Ocean Quadrant — Finding

### ZERO DEDICATED REPOSITORIES

After exhaustive searching across multiple query strategies:

| Search Query | Results |
|--------------|--------|
| ocean fertilization | 0 repos |
| ocean alkalinity enhancement | 0 repos |
| marine geoengineering | 0 repos |
| ocean intervention marine technology | 0 repos |
| ocean pH sensor monitoring | 0 ocean-specific repos |
| artificial upwelling ocean | 0 repos |
| seaweed kelp carbon farming | 0 repos |
| marine cloud brightening | 0 repos |

**The only ocean-adjacent project found:** Team50-Labs/NebuGrid-OpenSource (0 stars, Aug 2026) — fog-harvesting for arid coastal environments. Not ocean geoengineering per se.

---

## Cross-Theme Commit Histories

### PCMDI/pcmdi_metrics (133 stars) — Has Ocean Metrics

| Commit Date | Activity |
|-------------|----------|
| Sep 4, 2026 | v4.2.1 release (10 commits in 2 days) |
| Jun 8, 2026 | PR #825 merged |
| Jun 19, 2026 | MCS precipitation-buoyancy POD (ocean-relevant) |

**Key Insight:** PCMDI's v4.2.1 includes metrics for ENSO, sea ice, and ocean heat content — the closest thing to ocean simulation tooling that exists in open source. But these are evaluation tools, not intervention design tools.

### wrf-model/WRF (1,761 stars) — Ocean Physics in the Background

| Commit Date | Activity |
|-------------|----------|
| Jun 8, 2026 | v4.8.0 released |
| May 27, 2026 | MYNN-EDMF update (includes ocean boundary layer physics) |
| May 28, 2026 | Solar radiation correction (relevant to ocean surface energy budget) |

**Key Insight:** WRF includes ocean boundary layer physics and air-sea interaction modules, but these are climate model components — not tools for designing or evaluating ocean interventions.

### prashaant1926/open-earth-digital-twin-simulation — Future Potential

**Key Insight:** The agent-based Earth digital twin concept could eventually model ocean interventions, but it's currently a TeX manifesto, not a codebase.

---

## Three Hypotheses for the Ocean Gap

### H1: Institutional Gatekeeping (Most Likely)

**Evidence:**
- Ocean geoengineering research is concentrated in WHOI, Scripps, GEOMAR, IOC-UNESCO
- These institutions publish in closed journals and share data through institutional channels
- The culture of ocean science predates the open-source movement by decades
- The researchers who would build these tools are at sea on ships, not at desks writing code

**Supporting evidence:** The 85-star carbon-capture-and-storage repo (single author, single paper, then silence) shows academic projects die without institutional home. Ocean science is even more institutionally siloed.

### H2: Governance & Liability (Important)

**Evidence:**
- The London Convention/Protocol directly regulates ocean fertilization
- Scientists may self-censor to avoid regulatory scrutiny
- Ocean interventions have transboundary impacts — no single country can authorize them
- The legal risk of being associated with unregulated ocean experiments is real

**Counter-evidence:** Solar geoengineering has similar governance concerns (SRM is not explicitly illegal, but carries reputation risk), yet at least srm-forever exists. The difference: ocean interventions require physical deployment, not just code.

### H3: Experimental Complexity Barrier (Structural)

**Evidence:**
- SRM can be modeled with radiative transfer codes (srm-forever proves this)
- DAC can be prototyped in a garage (OpenAir-Cyan proves this)
- Ocean interventions require: ship time ($50K+/day), sensor deployments in remote waters, multi-year monitoring, and international coordination
- The barrier to GitHub-ready prototypes is astronomically higher

**The math:** A single ocean field experiment costs more than a decade of OpenAir-Cyan-type hardware development. The ROI on open-source ocean intervention tools is unclear for any individual researcher.

---

## Cross-Theme Comparison

| Theme | Active Repos | Top Stars | Commit Activity | Open-Source Maturity |
|-------|-------------|-----------|----------------|---------------------|
| Solar Geoengineering | 6 | 133 | Moderate (v4.2.1 burst) | No SRM-specific simulation code exists |
| Carbon Capture | 5+ | 85 | Bursty (Aug 2026 wave) | Materials science active, system design absent |
| Ocean Intervention | 0 | 0 | None | Complete absence |

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

## Updated Episode Questions

1. Why is ocean geoengineering invisible on GitHub? The answer is institutional, legal, and structural — not technical.
2. What would an open-source ocean alkalinity project look like? Sensor designs, data pipelines, and modeling components — but who would run it?
3. Is the silence itself a governance signal? The London Protocol restrictions may be causing self-censorship among researchers who might otherwise share code.
4. Can digital twins prepare the ground? If we can model ocean systems before physical deployment, that might lower the governance risk enough to attract open-source development.
5. What's different about ocean research that can be open-sourced vs. that which can't? Sensor designs and data pipelines are shareable; actual ocean experiments are not. Where's the line?
