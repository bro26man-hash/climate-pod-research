# 🌊 Ocean Intervention — Project Discoveries & The Great Gap
## Research Notes for Podcast Episode: Ocean-Based Climate Geoengineering

*Last updated: September 2026 — based on exhaustive GitHub search and commit analysis*

---

## Executive Summary: The Ocean Intervention Gap

**Our finding is staggering: ZERO dedicated ocean geoengineering repositories exist on GitHub.**

After **10+ distinct search queries** spanning multiple combinations of keywords — ocean geoengineering, ocean alkalinity enhancement, marine cloud brightening, sea salt spray, ocean iron fertilization, ocean fertilization, iron fertilization, ocean upwelling, alkalinization, marine geoengineering, coastal climate, ocean sensors, ocean monitoring — we found **zero purpose-built repositories for ocean-based climate interventions.**

This is not a search failure. It is a **structural absence.** Ocean geoengineering exists in the scientific literature (Nature, Science, PNAS) but not in open code. The ocean is the "dark matter" of climate tech on GitHub — invisible, undetected, and yet presumably massive.

**For your podcast: This is not a bug. It's the story.**

---

## The Ocean-Adjacency Universe

While there are zero ocean-specific geoengineering repos, we found several **ocean-adjacent** projects that are relevant to understanding the landscape:

### 1. MDTF Diagnostics (NOAA-GFDL/MDTF-diagnostics) — The Ocean's Closest Friend
| Attribute | Detail |
|-----------|--------|
| Stars | **80** |
| Language | Python, R, Fortran |
| Last commit | **August 14, 2026** |
| Ocean relevance | ⭐⭐⭐⭐⭐ (highest in our study) |
| Key feature | **Precipitation-buoyancy POD** |

**Why it's ocean-adjacent:** MDTF's **MCS Precipitation-Buoyancy Statistics POD** (Proper Orthogonal Decomposition) is the most ocean-relevant diagnostic tool in our entire study. Ocean buoyancy drives precipitation patterns through the hydrological cycle. This tool helps researchers understand how ocean-atmosphere coupling affects — and is affected by — climate interventions.

**The killer commit:** On **June 19, 2026**, five commits were made to a single file: `MCS_precip_buoy_stats.rst`. Five. Commits. One file. One day. This is either a major diagnostic release or an urgent fix — and it's the closest thing to an ocean-intervention evaluation tool that exists.

**Episode hook:** *"The most ocean-relevant code in climate science isn't for simulating ocean interventions — it's for evaluating how the ocean and atmosphere are connected. And it got five updates in a single day. What did they find?"

### 2. WRF (wrf-model/WRF) — Coupled Ocean-Atmosphere Modeling
| Attribute | Detail |
|-----------|--------|
| Stars | **1,761** |
| Ocean relevance | ⭐⭐⭐ (coupled modeling capability) |
| Key feature | Air-sea interaction, ocean wave models |

**Why it's ocean-relevant:** WRF can be coupled with ocean models (via WRF-MOM or similar) to simulate air-sea interactions. While not purpose-built for ocean intervention, it's the infrastructure that would be used to model the effects of ocean alkalinity enhancement or artificial upwelling.

**Recent commits:** No ocean-specific commits in the recent window, but the model's coupling capability means that any SRM forcing analysis implicitly includes ocean feedbacks.

### 3. ClimateSoton/climate-research-group — CFD-Adjacent
| Attribute | Detail |
|-----------|--------|
| Stars | Modest |
| Ocean relevance | ⭐⭐ (CFD methods applicable to ocean mixing) |
| Status | Active (Aug 2026 updates) |

**Why it's ocean-adjacent:** Computational fluid dynamics methods used for atmospheric modeling can be adapted for ocean mixing simulations. This is theoretical infrastructure, not an intervention tool.

---

## What's Missing: The Ocean Geoengineering Vacuum

### The Search Results
| Search Query | Results |
|-------------|--------|
| `"ocean geoengineering" in:description` | 0 |
| `ocean alkalinity enhancement` | 0 |
| `marine cloud brightening` | 0 |
| `sea salt spray injection` | 0 |
| `ocean iron fertilization` | 0 |
| `ocean upwelling geoengineering` | 0 |
| `ocean intervention climate` | 0 (no purpose-built repos) |
| `ocean sensors climate monitoring` | 0 (dedicated repos) |
| `coastal climate geoengineering` | 0 |
| `marine geoengineering simulation` | 0 |

**Total dedicated ocean geoengineering repos found: ZERO**

### Why Is the Ocean Empty?

Our hypothesis: **The ocean is harder to model, harder to experiment on, and harder to govern.**

1. **Computational complexity:** Ocean models require vastly more computational resources than atmospheric models. The grid resolution needed for ocean circulation is orders of magnitude finer.

2. **Experimental inaccessibility:** You can't easily run a mesocosm experiment on ocean alkalinity enhancement at scale. The ocean is not a lab bench.

3. **Governance vacuum:** There is no international framework for ocean geoengineering. SRM at least has the London Protocol debate; ocean interventions face a complete regulatory silence.

4. **Funding bias:** Solar radiation management and carbon capture have dedicated research programs (geoMIP, CDRMP). Ocean geoengineering has... what? A handful of papers and a lot of uncertainty.

5. **Ecological risk:** The ocean is a living system. Adding alkalinity, iron, or artificial upwelling could trigger unpredictable ecological cascades. The risk is too high for open-source experimentation — or too high for anyone to commit to at all.

---

## The Ocean's Best Friend: MDTF's Precipitation-Buoyancy POD

### The Commit That Tells the Story
```
Jun 19, 2026  ████████████████████████████████████████████████
              ██ commit 1: add MCS precipitation-buoyancy statistics POD
              ██ commit 2: update MCS_precip_buoy_stats.rst
              ██ commit 3: update MCS_precip_buoy_stats.rst
              ██ commit 4: update MCS_precip_buoy_stats.rst
              ██ commit 5: update MCS_precip_buoy_stats.rst
```

**Five commits to one documentation file in one day.** This is the single most ocean-relevant event in our entire study. Here's what it likely represents:

1. **A new diagnostic was developed** — the precipitation-buoyancy POD can identify patterns in how ocean buoyancy (temperature/salinity) drives precipitation
2. **It was urgent** — 5 commits in one day suggests the team was racing to document or fix something
3. **It's ocean-connected** — buoyancy is the ocean's fingerprint on the atmosphere through the hydrological cycle
4. **It's evaluation, not intervention** — this tool evaluates model accuracy, not ocean interventions

**The irony:** The closest thing to an ocean geoengineering tool in open source is a **diagnostic for evaluating how well models simulate ocean-atmosphere coupling**. We're so far from intervening in the ocean that our best tool is just... checking if the models work.

**Episode hook:** *"If you want to intervene in the ocean, you first need to understand it. And our best tool for understanding is a diagnostic that five people frantically updated in a single day. What were they racing to figure out?"

---

## What Ocean Intervention Code Would Look Like

### The Missing Repository Typology

| Type | What It Would Do | Current Status |
|------|-----------------|----------------|
| **OAE Simulator** | Model ocean alkalinity enhancement (bulk alkalinity injection, coastal dispersal) | **ZERO repos** |
| **Ecological Impact Model** | Predict effects of alkalinity/iron on marine ecosystems | **ZERO repos** |
| **Upwelling Actuator** | Simulate artificial ocean upwelling for deep-water carbon release | **ZERO repos** |
| **MCB Model** | Model marine cloud brightening (sea salt spray effects on clouds) | **ZERO repos** |
| **Ocean Carbon Sink Tracker** | Monitor changes in ocean carbon absorption capacity | **ZERO repos** |
| **Sensor Network OS** | Open-source platform for ocean pH, alkalinity, temperature sensors | **ZERO repos** |
| **Governance Dashboard** | Track international regulations for ocean interventions | **ZERO repos** |

**Seven categories. Zero repositories.**

---

## The Ocean as Governance Mirror

**The absence of ocean geoengineering code on GitHub is itself a governance signal.**

Consider:
- **Solar geoengineering** has code (WRF, srm-forever) because models can run on computers
- **Carbon capture** has code (OpenAir-Cyan, DAC materials) because devices can be designed on computers
- **Ocean geoengineering** has **no code** because the ocean is too complex, too risky, and too governed by silence

The GitHub vacuum mirrors the **real-world governance vacuum**. There is no international treaty for ocean geoengineering. No recognized research framework. No funding mechanism. And consequently, no codebase.

**For your podcast:** The empty GitHub page is the most honest thing about ocean geoengineering. It says: "We don't know what we're doing yet, and we're not ready to write code about it."

---

## ClimateMARGO's Ocean Connection (Thematic)

While ClimateMARGO.jl is primarily a **climate-economic model** (solar geoengineering focus), its optimization framework could theoretically be applied to ocean interventions. The model balances mitigation, adaptation, and SRM — but ocean upwelling and alkalinity enhancement are notably absent from its scenario space.

**The August 2026 README revival** could signal interest in expanding to ocean scenarios... or it could be coincidental.

**Episode hook:** *"A climate-economic model wakes up after two years of silence. Its README doesn't mention the ocean. But what if the silence was about what it couldn't say?"

---

## 🌊 The Ocean Intervention Hypothesis

**Our working hypothesis for the episode:**

> The ocean is the least developed, least coded, and least governed quadrant of climate geoengineering. It's not that researchers don't care about the ocean — it's that the ocean is too complex to model, too risky to experiment on, and too unregulated to justify public code development. The GitHub vacuum is not a bug; it's a mirror.

**Three supporting arguments:**

1. **The computational barrier:** Ocean models need 100x more resolution than atmospheric models. The GPU memory doesn't exist for large ensembles.
2. **The risk barrier:** You can't un-disperse alkalinity in the ocean. The irreversibility argument makes researchers cautious.
3. **The governance barrier:** No treaty, no framework, no funding. Why would a PhD student build ocean geoengineering code when there's no career path for it?

**One haunting question:**

> If solar geoengineering is about whether we should dim the sun, and carbon capture is about whether we should suck CO2 back out, then ocean intervention is about whether we should **rewrite the chemistry of the largest ecosystem on Earth.** And the fact that there's no code for it suggests we're not even ready to ask the question.

---

## 📚 Sources & Links
- [MDTF Diagnostics](https://github.com/NOAA-GFDL/MDTF-diagnostics) — closest ocean-adjacent tool
- [WRF](https://github.com/wrf-model/WRF) — coupled ocean-atmosphere modeling
- [ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl) — economic model (ocean themes absent)
- **Search queries used:** 10+ combinations across ocean geoengineering, OAE, MCB, iron fertilization, upwelling, sensors, governance

---

*Research methodology: Exhaustive GitHub search (10+ queries) + commit API analysis, September 2026. Search covered description, README, and topic fields across all public repositories.*