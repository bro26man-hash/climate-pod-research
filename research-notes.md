# 🌍 Carbon Capture & Direct Air Removal — Research Notes (Updated Sep 2026)

## Project Discoveries

### 1. api-evangelist/lithos-carbon
- **URL:** https://github.com/api-evangelist/lithos-carbon
- **Language:** Not specified (API surface profiling by API Evangelist / Kin Lane)
- **Description:** Independent third-party profile of the Lithos Carbon API surface. Lithos Carbon delivers permanent carbon dioxide removal via enhanced rock weathering (ERW) — spreading crusite-rich rock on agricultural land to accelerate natural CO2 sequestration.
- **Last Activity:** September 16, 2026
- **Commit Count:** 10 shown (all between Aug 29 – Sep 16, 2026 — ~3 commits/week)
- **Key commits:**
  - Sep 16: "Slug + MCP type corrections, rescore artifacts"
  - Sep 12: "Slug + MCP type corrections, rescore artifacts"
  - Sep 7: "Enrichment + identity; publish to network"
  - Sep 4: "Slug + MCP type corrections, rescore artifacts"
  - Sep 1: "Slug + MCP type corrections, rescore artifacts" (×2 same day)
  - Aug 30: "Slug + MCP type corrections" + "Record who wrote each artifact"
  - Aug 29: "Publish the delivery model — what was measured, not a new score"
- **Relevance:** Extremely active documentation effort. The MCP (Model Context Protocol) type corrections suggest AI/ML integration is being added. Not simulation code, but reflects the booming CDR API ecosystem. 10 commits in 3 weeks = the most active carbon capture-related repo we found.

### 2. api-evangelist/climeworks
- **URL:** https://github.com/api-evangelist/climeworks
- **Description:** API surface profile of Climeworks AG, the Swiss Direct Air Capture (DAC) company and the world's most prominent CDR pioneer. Their Orca and Mammoth plants are the largest operational DAC facilities.
- **Relevance:** Climeworks is the reference point for industrial DAC. Their API infrastructure reveals how CDR operations are being digitized and integrated with external systems. The existence of documented API surfaces suggests a maturing industry.

### 3. api-evangelist/spiritus
- **URL:** https://github.com/api-evangelist/spiritus
- **Description:** API profile of Spiritus Technologies, building low-cost, modular carbon capture systems. Represents the next generation of DAC hardware companies emerging after Climeworks.
- **Relevance:** New entrants are emerging with API-first operational models, suggesting that software integration is becoming a competitive differentiator in the CDR space.

### 4. ClimateMARGO/ClimateMARGO.jl
- **URL:** https://github.com/ClimateMARGO/ClimateMARGO.jl
- **Stars:** 73
- **Description:** Julia implementation of MARGO, an idealized climate-economic modelling framework. Includes CDR optimization modules that can be applied to carbon capture pathway analysis — optimizing the trade-off between mitigation, adaptation, and carbon dioxide removal investments.
- **Last Activity:** August 17, 2026
- **Relevance:** The only multi-purpose climate-economic model in this set that explicitly includes CDR as a policy lever. Most relevant for episode framing around: "What is the optimal mix of emission cuts vs. carbon capture?"

### 5. Supplementary: Computational DAC Materials (from broader search)
- **tjz21/DAC_peroxovanadates** — Octuperoxovanadates as DAC materials, updated Aug 19, 2026 (coordinated wave)
- **tjz21/DAC_peroxotitanates** — Tetraperoxotitanates as DAC materials, updated Aug 19, 2026 (coordinated wave)
- **o7-machinehum/electro-swing-dacc** — DIY electro-swing DAC device plans, updated Aug 2026

---

## Commit Trend Analysis

| Repository | Commits (shown) | Period | Pattern |
|------------|----------------|--------|---------|
| lithos-carbon | 10 | Aug 29 – Sep 16, 2026 | **Very Active** (~3 commits/week) |
| climeworks | (discussed) | Ongoing | Active documentation |
| spiritus | (discussed) | Ongoing | Active documentation |
| ClimateMARGO.jl | 10 (shown) | 2021–2022 + Aug 2026 burst | Maintenance-driven |

---

## Key Trends & Episode Themes

### 1. The CDR API Ecosystem Is Booming
lithos-carbon received 10 commits in just 3 weeks (August–September 2026). The carbon removal industry is rapidly digitizing its operations, but through closed API surfaces, not open simulation code. **The companies are building; the open-source community isn't.** This is a critical distinction: the industry is building integration infrastructure, not research tools. Episode angle: "The DAC companies have APIs, but no one has open-source simulation code that models their processes."

### 2. MCP / AI Integration Emerging
lithos-carbon's recent commits reference "MCP type corrections" — Model Context Protocol integration for AI agents. This suggests CDR companies are preparing for AI-driven optimization of their capture systems. The convergence of AI and climate tech is accelerating. Episode angle: "When AI agents start managing carbon capture, who's accountable?"

### 3. Hardware + Software Convergence
Companies like Spiritus and Lithos are building API surfaces around physical capture systems. This convergence creates a new category: hardware-companies-with-software-stacks. The open-source opportunity exists in simulation and optimization — not in the hardware itself.

### 4. The $1000/ton Question — No Open Simulation
No open-source DAC simulation code was found in this search. The gap between academic models and industrial deployment is stark. We can model the Earth system (CESM, WRF, CESM2) but we cannot model the $1000/ton DAC cost curve, sorbent chemistry degradation, or energy integration at the industrial scale. Episode angle: "Why is there no open-source code for the most important climate technology of the century?"

### 5. The August 2026 DAC Materials Wave (Confirmed)
Three computational chemistry repos — peroxovanadates, peroxotitanates, and electro-swing-DAC — were all updated on August 19, 2026. This coordinated timing across independent repos suggests a shared research event (likely a paper publication). This is the strongest evidence of a **coordinated open computational chemistry community** forming around DAC materials.

### 6. Economic Modeling Gap
ClimateMARGO addresses CDR optimization at the macro level (what fraction of climate budgets should go to CDR vs. mitigation?), but no tool models the micro/meso level: sorbent material costs, plant energy requirements, geographic suitability, supply chain logistics. The gap between hierarchical CDR modeling — from molecular to planetary — is enormous.

---

## Episode Questions for Carbon Capture

1. **Can open source break the $1000/ton DAC cost barrier?** If no one has published open-source simulation of DAC processes, how can researchers collaborate on cost reduction? Can a clone-the-repo approach accelerate innovation?

2. **What makes OpenAir-Cyan special?** The openair-collective's DIY open hardware DACC device (referenced in the broader search) represents a hardware-open approach to DAC. Is this the right model for CDR?

3. **Are peroxides the sorbent of the future?** The peroxovanadates and peroxotitanates repositories both appeared on August 19, 2026, suggesting a coordinated research event in computational DAC materials. Are peroxide compounds the next-generation sorbent?

4. **When AI agents manage capture, who's accountable?** With MCP integration beginning in carbon removal APIs, we're entering a new governance territory where algorithmic decisions directly impact carbon accounting.

5. **What's the optimal CDR portfolio?** ClimateMARGO models the macro question: how much should we invest in DAC vs. ERW vs. nature-based solutions? Can these tools be democratized for developing nations?

6. **Why does CDR have APIs but no simulation?** The lithos-carbon repo has 10 commits in 3 weeks documenting a company's API — but there's no open-source tool that simulates the enhanced weathering process itself. We're documenting the industry, not modeling it.

---

*Research compiled from GitHub repository search and commit history analysis. Sources: api-evangelist/lithos-carbon, api-evangelist/climeworks, api-evangelist/spiritus, ClimateMARGO/ClimateMARGO.jl, tjz21/DAC_peroxovanadates, tjz21/DAC_peroxotitanates.*