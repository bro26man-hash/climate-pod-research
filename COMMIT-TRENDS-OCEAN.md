# 🌊 Ocean Intervention — Commit Trend Analysis

> Updated: September 2026 | 10+ search queries, 14+ ocean-adjacent commits analyzed

---

## Executive Summary

Ocean intervention is the **empty quadrant** of climate tech on GitHub. Across 10+ search queries and systematic review of ocean-adjacent repositories, we found **zero dedicated ocean geoengineering code repositories**. The ocean's voice in the open-source climate tech ecosystem is indirect — transmitted through evaluation diagnostics (MDTF), atmospheric models (WRF), and pure ocean dynamics code (Oceananigans.jl). None of these simulate interventions.

---

## Trend 1: The Precipitation-Buoyancy POD — The Ocean's Only Voice

### Why This Single Diagnostic Matters More Than Any Ocean Repo
- **5 commits on June 19, 2026** — the most intense single-day development in the entire ocean theme
- **What it does:** Evaluates whether climate models correctly simulate the coupling between ocean buoyancy (temperature/saltiness stratification) and precipitation patterns
- **Why it's the ocean's voice:** Ocean interventions (OAE, iron fertilization, MCB) would disrupt the air-sea exchange of heat, salt, and CO2. The precip-buoyancy POD is how you'd detect whether those disruptions are modeled correctly. It provides the **evaluation framework** that ocean intervention models need before they can be trusted.
- **Who maintains it:** NOAA-GFDL (Geophysical Fluid Dynamics Laboratory) — the same lab that produced the hurricane model and is a cornerstone of US climate modeling infrastructure
- **Institutional signal:** 5 commits in one day means someone at GFDL prioritized this tool. It's not a side project; it's a flagship diagnostic.
- **🎙️ Podcast insight:** The most ocean-relevant code in the entire GitHub climate tech ecosystem is an evaluation tool, not a simulation tool. We evaluate the ocean more than we intervene in it.

---

## Trend 2: The Atmospheric Gateway (WRF's Ocean Connection)

### How Ocean Signals Enter the Code World Through WRF
- **10 recent commits** including v4.8.0 release and solar radiation fixes
- **Ocean connection:** WRF's air-sea flux parameterizations control how energy and moisture exchange between ocean and atmosphere. Any ocean intervention would alter these fluxes (e.g., OAE changes ocean CO2 uptake, MCB changes solar heating of the ocean surface).
- **Why it matters:** WRF is the "gene" through which ocean intervention signals propagate into the climate modeling ecosystem. You can't simulate an ocean intervention without modeling its effect on air-sea fluxes.
- **🎙️ Podcast insight:** The ocean doesn't have its own repo. It speaks through WRF. The atmospheric model is the ocean's proxy in the code world.

---

## Trend 3: The Pure Ocean Universe (Oceananigans.jl)

### Beautiful Code, No Intervention
- **1,413 stars** (from v2 analysis) — the most popular pure ocean simulation code on GitHub
- **What it does:** Models ocean turbulence, internal waves, mixing, and stratification using Julia. State-of-the-art computational fluid dynamics for the ocean.
- **What it doesn't do:** Simulate any geoengineering intervention. No OAE module. No iron fertilization. No MCB. No restoration.
- **Why it matters:** Oceananigans provides the **pristine ocean baseline**. Before you can simulate what happens when you add alkalinity to the sea, you need a model of the sea itself. Oceananigans is that model.
- **🎙️ Podcast insight:** Oceananigans is the ocean's self-portrait. It shows the ocean as it is, not as we might change it. The gap between "model the ocean" and "simulate intervening in the ocean" is the governance gap.

---

## Trend 4: The Marine Renewable Energy Contrast

### Marine Energy Has Tools. Marine Geoengineering Has Nothing.
- **MHKiT-Python:** A proper tooling ecosystem for marine energy (tidal, wave) has data processing, QC, and resource assessment tools
- **Oceananigans:** A sophisticated ocean dynamics simulation framework
- **Ocean geoengineering:** Zero repos
- **The contrast:** Marine *energy* (harvesting the ocean) has a full software stack. Marine *intervention* (manipulating the ocean) has nothing. The difference is intention: energy extraction is acceptable; environmental manipulation is not.
- **🎙️ Podcast insight:** The contrast between MHKiT's tooling and the ocean geoengineering void is the governance story in a single comparison. We code for what we harvest. We don't code for what we manipulate.

---

## The Ocean Gap: A Quantitative Summary

| Search Strategy | Queries | Dedicated Repos Found |
|----------------|---------|----------------------|
| Direct geoengineering terms | 3 ("ocean geoengineering", "marine geoengineering simulation", "ocean intervention climate model") | 0 |
| Specific OAE-only | 3 ("ocean alkalinity enhancement", "ocean liming", "seaweed farming climate") | 0 |
| Iron fertilization & blue carbon | 2 ("ocean iron fertilization", "blue carbon restoration") | 0 |
| Marine cloud brightening | 1 ("marine cloud brightening") | 0 |
| Ocean carbon removal (ocean-specific) | 1 ("ocean carbon removal open source") | 0 |
| **Total** | **10+** | **0** |

---

## The Deep Ocean vs. The Shallow Ocean

Our search reveals a stratification pattern that mirrors the ocean itself:

| Depth | GitHub Equivalent | What's There |
|-------|------------------|-------------|
| **Surface (Sunlit)** | Atmospheric models (WRF), Evaluation tools (PCMDI, MDTF) | Well-lit, well-funded, lots of code |
| **Mesopelagic (Twilight)** | Ocean dynamics (Oceananigans), Marine energy (MHKiT) | Interesting but not intervention-focused |
| **Bathypelagic (Midnight)** | **Ocean geoengineering** | **Completely dark. Zero code. Zero visitors.** |

---

## 🔑 Key Takeaways for the Podcast

1. **The ocean is the silent quadrant** — 10+ searches, zero repos. The gap is the headline.
2. **MDTF's precip-buoyancy POD is the ocean's only voice** — 5 commits in one day, the most ocean-relevant tool in open source, and it's an evaluator, not a simulator.
3. **WRF is the atmospheric gateway** — ocean signals enter the code world through air-sea flux calculations, not dedicated ocean tools.
4. **Oceananigans shows the pristine ocean** — no interventions modeled, just the sea as it is.
5. **Marine energy vs. marine geoengineering** — MHKiT has a full stack; ocean manipulation has nothing. The contrast is the governance story.
6. **The silence is a signal** — is it cowardice (governance fear)? Complexity (too hard)? Data scarcity (can't model what we can't observe)? Or is it wisdom (maybe we shouldn't be coding ocean interventions yet)?

---

## 🎙️ Episode Narrative Arc

**Opening:** "We searched GitHub 10 different ways looking for ocean geoengineering code. We found zero. Not one repository. This is the most surprising finding in our entire research."

**Act 1 — The Void:** Document the gap. Show the search queries. Count the zeros. Establish that ocean intervention is the "dark matter" of climate tech.

**Act 2 — The Indirect Voice:** Trace how ocean science does exist in code — through MDTF's POD (the evaluator), WRF (the atmospheric gateway), and Oceananigans (the pure dynamics). The ocean speaks, but only through proxies.

**Act 3 — The Governance Hypothesis:** Ask why the gap exists. Is it fear? Complexity? Funding? The cultural resistance to "manipulating the sea" vs. "harvesting the sea" (MHKiT's tools).

**Act 4 — The Blueprint:** What would the first ocean intervention codebase look like? OAE module, MCB module, OIF module, blue carbon module, and an evaluation framework like MDTF but for interventions.

**Close:** "The blank page is the most important finding. The ocean is where the climate is most turbulent, most complex, and most silent in the code world. That silence is itself a signal. What are we waiting for?"

---

*Data source: GitHub API commit data and systematic search queries, September 2026.*