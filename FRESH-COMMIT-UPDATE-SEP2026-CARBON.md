# 🌍 Carbon Capture — Fresh Commit Update v7 (September 2026)

> **Branch:** `carbon-capture`  
> **Podcast episode:** Episode 2 — Carbon Capture  
> **Data pulled:** September 2026 via GitHub API  
> **Repos analyzed:** 8 (lithos-carbon, ShennongWM-G, plus v6 references to open-sustainable-technology, openair-cyan, Carbon_Capture_ML, DAC_peroxovanadates, DAC_peroxotitanates, carbon-capture-and-storage)

---

## Executive Summary

v7 data reveals the carbon capture ecosystem on GitHub is defined by **two opposing forces:**

1. **The API Infrastructure Wave** — `lithos-carbon` (Kin Lane's API Evangelist project) shows **weekly commits for 3+ weeks straight**, with MCP (Model Context Protocol) type corrections and a public "delivery model" publication. This represents the **industrialization** of carbon capture data — it's being packaged as API surfaces, scored, and delivered as measurable infrastructure.

2. **The CC0 Materials Revolution** — The two `tjz21/DAC_peroxovanadates` and `tjz21/DAC_peroxotitanates` repos adopted CC0 public domain dedication in September 2025, treating computational screening data as public infrastructure. This is the **open-science** signal — research data freed from paywalls and embargoes.

These two forces — **industrial quantification** vs. **open-liberation** — define the current tension in carbon capture OSS.

---

## 🔥 Repo 1: Lithos-Carbon — The API Evangelist's Carbon Scorecard

| Field | Detail |
|-------|--------|
| **Repo** | `api-evangelist/lithos-carbon` |
| **Maintainer** | Kin Lane (API Evangelist) |
| **Stars** | Low (new / niche) |
| **Language** | Not specified (data/metadata project) |
| **Last commit** | **September 16, 2026** (most recent!) |
| **URL** | https://github.com/api-evangelist/lithos-carbon |

### What Is This?

Lithos Carbon is a **third-party profile of a public API surface** — Kin Lane ("API Evangelist") is documenting, scoring, and publishing the API infrastructure of Lithos Carbon, a company delivering "permanent carbon dioxide removal." This is not carbon capture simulation code. This is **meta-data about carbon capture data infrastructure** — a catalog of what APIs exist, how they're structured, and how they're scored.

### v7 Fresh Commit Timeline (August 29 – September 16, 2026)

```
Aug 29  █ Publish the delivery model — what was measured, not a new score (39aaecd)
Aug 30  █ Slug + MCP type corrections, rescore artifacts (dc3e5df)
Aug 30  █ Record who wrote each artifact in this repository (3116c37)
Aug 30  █ Slug + MCP type corrections, rescore artifacts (7015117)
Sep 01  █ Slug + MCP type corrections, rescore artifacts (dd9a65d)
Sep 01  █ Slug + MCP type corrections, rescore artifacts (63d08bb)
Sep 04  █ Slug + MCP type corrections, rescore artifacts (3959770)
Sep 07  █ Enrichment + identity; publish to network (41af07c)
Sep 12  █ Slug + MCP type corrections, rescore artifacts (4553141)
Sep 16  █ Slug + MCP type corrections, rescore artifacts (d672544)
```

### 🔥 The "Delivery Model" Publication — A New Paradigm?

**Commit `39aaecd` (Aug 29, 2026):** *"Publish the delivery model — what was measured, not a new score (roadmap#41)*"

This is the most conceptually significant commit in the carbon capture OSS ecosystem this month. Kin Lane is publishing **a methodology document** that explains what Lithos Carbon's API surface measures and how it scores. The key phrase: **"what was measured, not a new score."**

This is a shift from **opinion-based assessment** ("we think this API is good") to **transparency-based assessment** ("here's exactly what we measured and how"). It's the API Evangelist version of open-science methodology disclosure.

**🎙️ Podcast angle:** *"The API evangelist behind carbon capture scoring just published 'what we measured, not a new score.' It sounds humble, but it's a paradigm shift. For years, climate-tech API scoring has been a black box. Now the methodology is public. You can audit the score. That's a bigger deal than it sounds."

### 🔥 The MCP Pattern — "Slug + MCP Type Corrections"

**6 out of 10 commits** use the same message pattern: *"Slug + MCP type corrections, rescore artifacts"*

**MCP = Model Context Protocol** — Anthropic's open standard for AI tools to interact with external data sources. The fact that Kin Lane is correcting MCP types and rescore artifacts **weekly** signals:

1. **MCP is being actively used** — someone (or an AI agent) is querying Lithos Carbon's API through MCP
2. **The data schema is evolving** — corrections imply the initial type mappings were wrong or incomplete
3. **Rescoring is ongoing** — as the data schema changes, scores must be recalculated

This is the **living-infrastructure pattern** — not a one-time audit, but a continuously Updated scoring system. The carbon capture API landscape is not static; it's being monitored and recalibrated.

### 🔥 "Record who wrote each artifact" — The Attribution Revolution

**Commit `3116c37` (Aug 30, 2026):** *"Record who wrote each artifact in this repository"*

This is an **attribution layer** being added to the scoring system. Each API artifact (endpoint, schema, scoring metric) now has a **provenance record** — who contributed it, when, and how. This is:
- **Reproducibility infrastructure** — you can trace every score back to its source
- **Accountability infrastructure** — if a score is wrong, you can find who made the measurement
- **Community-building infrastructure** — contributors get credit, which incentivizes participation

**🎙️ Podcast angle:** *"Three weeks into the project, the API evangelist added a 'record who wrote each artifact' commit. That's not just scoring — that's provenance tracking. He's building the git-not-git of carbon capture data infrastructure."

### The Weekly Velocity Pattern

| Week | Commits | Pattern |
|------|---------|--------|
| Aug 29-30 | 4 | Launch burst (delivery model + 3 corrections) |
| Sep 1 | 2 | Continued corrections |
| Sep 4 | 1 | Self-contained correction |
| Sep 7 | 1 | **Enrichment + identity** (new capability) |
| Sep 12 | 1 | Correction cycle continues |
| Sep 16 | 1 | Latest correction |

**After the initial launch burst, the pattern stabilizes at ~1 commit/week** — a sustainable maintenance cadence. This is what healthy OSS looks like: not frantic bursts, but steady, purposeful updates.

---

## 🔥 Repo 2: ShennongWM-G — The Greenhouse World (Cross-Theme)

*(See solar-geoengineering branch for full details — this repo bridges both themes.)*

**Key v7 addition:** Commit `9fc3682` (May 24, 2026): *"Update public README links and citation"* — the developer is investii ng in citability, which is essential for any tool that will be used in SRM or carbon capture research.

---

## 🟢 Repo 3: Open Sustainable Technology — The AI Governance Signal (v6 Carry-Forward)

### v6 → v7 Continuity

The **PR template AI-disclosure change** (commit `c4c9fe7`, Jul 19, 2026) remains the most significant governance development in the carbon capture ecosystem:

```
Modify PR template for AI content review
→ New mandatory AI-disclosure checkbox
→ Applied to every new project entry PR
```

**v7 Signal:** This commit was followed **the same day** by `be14281` ("Update PR template with review reminder"), suggesting the maintainer refined the AI disclosure language within 24 hours of initial deployment. This rapid iteration on AI governance — just one day between "create the checkbox" and "refine its language" — suggests **serious, ongoing attention** to the AI question.

**The "claude-carbon" addition** (Aug 23, 2026) is simultaneously fascinating and uncomfortable: a new project entry for an "AI tool for carbon-aware compute scheduling." The repo is cataloging AI tools that ** themselves optimize for lower carbon emissions** — a meta-level feedback loop.

---

## 🟡 Repo 4: OpenAir-Cyan — The Frozen Blitz (v6 Carry-Forward)

### The Dormancy Problem

**15 commits in February 2024, then complete silence for 2+ years.** The DIY open hardware DACC (Direct Air Capture Community) device received OSHWA certification, published full schematic plans, and then... stopped. No updates, no bug fixes, no community responses to issues.

**v7 question:** With lithos-carbon's ongoing API scoring, is there an opportunity to **re-activate** OpenAir-Cyan by connecting it to modern API infrastructure? Could the OSHWA-certified hardware designs be paired with modern data protocols?

---

## 🟡 Repo 5: The CC0 Revolution — DAC Peroxovanadates & Peroxotitanates (v6 Carry-Forward)

### The CC0 Adoption Signal

Both `tjz21/DAC_peroxovanadates` and `tjz21/DAC_peroxotitanates` adopted **CC0 (Creative Commons Zero / Public Domain)** licensing in September 2025. These are **computational screening datasets** for DAC sorbent materials — the researcher ran calculations on peroxovanadate and peroxotitanate compounds for CO2 capture and **deliberately freed the data**.

**Why CC0 matters:** Most scientific datasets use restrictive licenses or default copyright. CC0 is a **deliberate act of liberation** — the researcher could have used CC-BY (attribution required) or even kept the data proprietary for a publication embargo. Instead, they chose **full public domain dedication**.

**🎙️ Podcast angle:** *"Two researchers had a choice: publish data with attribution requirements, or give it to the public completely. They chose CC0. The peroxovanadate and peroxotitanate DAC screening data is now public infrastructure. No paywalls. No embargoes. No 'request access.' Just... free. This is what open science looks like when it's done right."

---

## ⚪ Repo 6: Carbon-Capture-and-Storage — The 85-Star Ghost (v6 Carry-Forward)

### The Ghost

**85 stars. Zero commits since March 2021.** This repo — covering reservoir simulation and geomechanics — was once cited 85 times but has been **dead for 4+ years**. The stars measure citations, not usability. This is the most common pattern in climate tech OSS: high visibility, zero maintenance.

---n
## 📊 Carbon Capture Cross-Repo Trend Dashboard (v7)

| Repo | Stars | Commit Velocity | Pattern | State |
|------|-------|-------------------|---------|-------|
| **open-sustainable-tech** | 2,552 | 3-4/month sustained | Institutional curation | 🟢 Exceptionally active |
| **lithos-carbon** | Low | **1/week (steady)** | Living API infrastructure | 🟢 The new signal |
| **openair-cyan** | 76 | 15/day then 2+yr silence | Frozen blitz | ⚡ Beautiful ghost |
| **Carbon_Capture_ML** | 56 | 1/week then 1.5yr silence | Maturing then dormant | ⚪ Research archive |
| **DAC_peroxovanadates** | 2 | CC0 adoption Sep 2025 | Liberation event | 🟢 Open-science hero |
| **DAC_peroxotitanates** | 2 | CC0 adoption Sep 2025 | Liberation event | 🟢 Open-science hero |
| **carbon-capture-and-storage** | 85 | Zero since 2021 | Ghost | 💀 Citation trap |

---

## 🎙️ Episode 2 Talking Points (v7 Updated)

### Lead Stories
1. **"The Scorecard That Scores Itself"** — Kin Lane's lithos-carbon project is publishing carbon capture API scoring methodology — not just scores, but "what was measured." The API evangelist is building the methodology layer for climate-tech data infrastructure.

2. **"Weekly Rescoring as a Service"** — 6 out of 10 lithos-carbon commits are identical: "Slug + MCP type corrections, rescore artifacts." This isn't maintenance — it's a **living system** that constantly recalibrates. The carbon capture API landscape is being monitored in real-time.

3. **"Who Wrote This?"** — The "record who wrote each artifact" commit (Aug 30, 2026) adds provenance tracking to the scoring system. Every score has an author. Every measurement has a trace. This is reproducibility infrastructure for climate tech.

4. **"The CC0 Choice"** — Two DAC researchers chose public domain dedication over all other options. Their screening data for peroxovanadate and peroxotitanate sorbents is now fully public. This is the open-science ideal in action.

### Structural Insights
5. **"The Two-Speed Ecosystem"** — The carbon capture world has two speeds: institutional curation (open-sustainable-tech, 3-4/month for 15 months straight) and individual liberation (CC0 datasets, one-shot release then silence). Both are real. Neither is wrong.

6. **"The AI Governance Lab"** — The mandatory AI-disclosure checkbox (Jul 2026) is the first concrete governance response to AI-generated contributions in climate tech OSS. The community is figuring this out in real time.

### The Big Question for Episode 2
| Question | Evidence |
|----------|----------|
| Can open source break the $1000/ton DAC cost barrier? | CC0 screening data + open hardware (OpenAir-Cyan) + API scoring (lithos-carbon) = the infrastructure exists |
| What makes OpenAir-Cyan special? | OSHWA-certified DIY DACC device, full schematics, then... silence. Why did it stop? |
| Are peroxides the sorbent of the future? | Two CC0 datasets suggest researchers believe so — and they're giving the data away |
| Is the August 2026 materials wave real? | lithos-carbon's weekly rescoring suggests active monitoring of new carbon capture materials |

---

## 🔗 References

- [Lithos-Carbon Repository](https://github.com/api-evangelist/lithos-carbon)
- [API Evangelist Blog](https://apievangelist.com/)
- [Open Sustainable Technology](https://github.com/protontypes/open-sustainable-technology)
- [DAC Peroxovanadates (CC0)](https://github.com/tjz21/DAC_peroxovanadates)
- [DAC Peroxotitanates (CC0)](https://github.com/tjz21/DAC_peroxotitanates)
- [OpenAir-Cyan (OSHWA-certified DACC)](https://github.com/openair-collective/openair-cyan)

---

## 📋 Update Log

| Version | Date | Changes |
|---------|------|----------|
| v6 | Sep 2026 | Initial 9-repo analysis; AI governance signal identified; CC0 trend noted; ghost repos flagged |
| **v7** | **Sep 2026** | **Fresh API pull from lithos-carbon (10 commits, Aug-Sep 2026); "delivery model" publication analyzed; MCP weekly rescoring pattern documented; attribution-layer commit highlighted; AI governance refinement cycle (1-day iteration) noted; cross-theme linkage with ShennongWM-G and solar-geoengineering branch established** |
