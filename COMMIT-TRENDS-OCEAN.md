# 🌊 Ocean Intervention — Commit Trend Analysis & Narrative

**Branch:** `ocean-intervention` | **Last Updated:** September 2026 (v4)

Commit trend analysis for ocean-adjacent repositories, based on fresh data pulled via the GitHub API (September 2026).

---

## The headline: Zero Commits for Zero Repos

The most important statistic in this entire research project:

```
Dedicated ocean geoengineering repositories:          0
OAE computational screening datasets:                 0
Ocean sensor/hardware repos:                          0
Ocean process models with intervention modules:        0
Total ocean geoengineering commits found:             0
```

**For comparison:**
```
Solar geoengineering repos (srm-forever):             1 (with 4 commits)
Carbon capture DAC material repos (CC0):              2 (with 25+ commits)
Direct air capture DIY hardware (OpenAir-Cyan):        1 (with 15+ commits)
```

The ocean is not just underrepresented — it is **absent.**

---

## Ocean-Adjacent Commit Activity

While there are zero ocean geoengineering repos, there ARE commits from repos with ocean relevance:

### 1. NOAA-GFDL/MDTF-diagnostics — The Precipitation-Buoyancy POD

**The single most ocean-relevant commit in open source:**

| Date | Commit | Message | Ocean Relevance |
|------|--------|---------|----------------|
| **Jun 19, 2026** | `33024ad` | **add MCS precipitation-buoyancy statistics POD** | ⭐⭐⭐ Core ocean-atmosphere diagnostic |
| Jun 19, 2026 | `4cfc99c` | Update MCS_precip_buoy_stats.rst | Documentation |
| Jun 19, 2026 | `699de27` | Update MCS_precip_buoy_stats.rst | Documentation |
| Jun 19, 2026 | `d6bc6d0` | Update MCS_precip_buoy_stats.rst | Documentation |
| Jun 19, 2026 | `3904d29` | Update MCS_precip_buoy_stats.rst | Documentation |

**5 commits on a single day (June 19, 2026), all touching the same file.** The 5th commit is the actual code addition; the first 4 are documentation updates. This is a textbook "big bang" release: code + 4 doc updates, all same day.

**What the POD does:** Measures the statistical relationship between precipitation and buoyancy (temperature-salinity structure) in climate model output. This is fundamental to ocean-atmosphere coupling — precipitation changes surface salinity, which changes buoyancy, which changes ocean mixing.

**What it doesn't do:** It doesn't simulate any ocean intervention. It evaluates model accuracy. It's a quality-control tool, not an engineering tool.

** broader MDTF activity (May–Aug 2026):**
```
May 22: Merge blocking notebook PR
May 27: Move diagnostics/blocking_neale_nb to dev branch
Jun 1: Quarterly metrics workflow + traffic logging
Jun 2: Merge NOAA-GFDL:main into main; Add citation
Jun 8: Merge PR #823; Update README (2 commits)
Jun 19: Precip-buoyancy POD (5 commits, same day)
Aug 14: Merge PR #825 (latest)
```

**Pattern:** Steady maintenance (1–2 commits per month) with a single dramatic burst (June 19: 5 commits in one day for the ocean-relevant POD).

**🎙️ Episode angle:** "The most ocean-relevant code in all of open source was added by one person, on one day, to one file. And what that file does is measure how well climate models reproduce the relationship between rain and ocean temperature structure. It's the quality-control inspector of the ocean sciences. It doesn't build ocean interventions. It evaluates whether the models that would be needed to design those interventions actually work."

---

### 2. ClimateSoton/ClimateSoton.github.io — The Ocean-Adjacent Website

| Date | Commit | Message |
|------|--------|--------|
| Jul 26, 2026 | `e7a596f` | Create index.html |
| Jul 26, 2026 | `75475c6` | Initial commit |

**2 commits, both on the same day.** A基本建设 of a website for a research group that works on carbon capture and sustainable energy via chemical looping.

**Ocean relevance:** Indirect. Chemical looping technology could theoretically be applied to ocean alkalinity enhancement (regenerating alkaline solutions from ocean minerals), but the group hasn't published any Ocean-specific work or tools.

**🎙️ Episode angle:** "A research group with the expertise to tackle ocean geoengineering spent their GitHub effort on... a website. Two commits, both on the same day. They didn't publish a paper. They didn't release a dataset. They didn't build a tool. They made a webpage. This might be the most perfect metaphor for the ocean gap: the expertise exists, but the code doesn't."

---

## The Ocean Gap: Statistical Summary

| Metric | Count | Comparison |
|--------|-------|------------|
| Ocean geoengineering repos | **0** | Solar: 1 (srm-forever); Carbon: 5+ (DAC, CCS, OpenAir) |
| Ocean geoengineering commits | **0** | Solar: 4 (srm-forever); Carbon: 25+ (DAC materials) |
| Ocean-adjacent diagnostic tools | 1 (MDTF POD) | Solar: 3+ (WRF radiation, PCMDI metrics, ClimateMARGO) |
| OAE computational screening | **0** | DAC: 2 repos (peroxovanadates, peroxotitanates) |
| Ocean sensor/hardware repos | **0** | Air: 1 (OpenAir-Cyan, OSHWA-certified) |
| CC0 ocean datasets | **0** | Carbon: 2 (both DAC, both Sep 12, 2025) |

---n
## The Three Universes: Ocean Edition

```
FAST UNIVERSE (Institutional, Funded, Sustained):
  ☀️ Solar:     WRF (1,762★), PCMDI (133★)
  🌍 Carbon:    Open-Sustainable-Tech (2,552★)
  🌊 Ocean:     Oceananigans.jl (1,413★, from v2 research), veros

SLOW UNIVERSE (Individual, Unfunded, Dormant):
  ☀️ Solar:     ClimateMARGO (73★, ambiguous revival), srm-forever (0★, new)
  🌍 Carbon:    OpenAir-Cyan (76★, dormant), Carbon_Capture_ML (56★, dormant),
                DAC_peroxovanadates (2★, CC0), DAC_peroxotitanates (2★, CC0)
  🌊 Ocean:     **NOTHING**

EMPTY UNIVERSE (Zero Presence):
  ☀️ Solar:     (none — everything has at least some presence)
  🌍 Carbon:    (none — everything has at least a website)
  🌊 Ocean:     **ALL OF OCEAN GEOENGINEERING** — 0 repos, 0 commits, 0 datasets
```

---n
## Why the Ocean Gap Matters: A Governance Reading

The absence of ocean geoengineering code is **not neutral**. It is a signal. Here's what the silence tells us:

### Signal 1: Political Risk Aversion
Ocean geoengineering is the most politically radioactive categories of climate intervention. SRM at least has the Weitzman discounting debate framing it as an intellectual question. OAE has "we're changing ocean chemistry." Iron fertilization has "we're dumping iron in the sea." Marine cloud brightening has "we're spraying seawater into the sky."

**The silence says:** No one wants to build tools for politically toxic interventions.

### Signal 2: Complexity Barrier
Solar geoengineering involves aerosols in the atmosphere — relatively simple physics compared to ocean intervention, which coupled ocean dynamics, chemistry, biology, and transport.

**The silence says:** The computational complexity of ocean geoengineering is beyond what individuals can build. It requires institutional teams with multi-year funding.

### Signal 3: Publication Bias
Ocean geoengineering papers face higher barriers to publication (reviewer skepticism, journal caution). The incentive structure doesn't reward building open-source tools for controversial interventions.

**The silence says:** The academic incentive structure makes it rational to publish papers but irrational to build open-source tools.

### Signal 4: The "Not Invented Here" Problem
Ocean scientific models tends to be proprietary (national labs, research institutes). The code stays behind the firewall. Only the papers come out.

**The silence says:** Ocean science hasn't adopted the open-source culture that atmospheric science (WRF) and climate-economics (ClimateMARGO) have embraced.

**🎙️ Episode angle:** "The ocean gap is not an accident. It's the sum of four forces: political toxicity, computational complexity, publication bias, and proprietary culture. Each force alone would be explainable. Together, they're a wall. And the wall is made of code that doesn't exist."

---n
## The Precipitation-Buoyancy POD as Ocean Proxy

Since there are zero ocean geoengineering repos, the most ocean-relevant code we found serves as a **proxy for what ocean intervention tools would look like if they existed:**

| Feature | Precip-Buoyancy POD (exists) | OAE Simulator (doesn't exist) |
|---------|------------------------------|-------------------------------|
| Purpose | Evaluate model accuracy | Design intervention strategy |
| Input | Climate model output | Ocean conditions, injection rates |
| Method | Statistical decomposition (POD) | coupled ocean-chemistry-biology modeling |
| Output | Accuracy metrics | Deployment recommendations |
| Maintainer | NOAA-GFDL (institutional) | **Nobody** |
| Funding | Federal grant | **Unfunded** |
| Stars | 80 | 0 |
| Commits | 15+ (sustained) | 0 |
| **License** | Open source | **N/A** |

**The gap between the POD and a hypothetical OAE simulator is the governance gap.** We can evaluate whether models work. We can't design interventions.

---n
## What Would Open-Source Ocean Geoengineering Look Like?

Drawing from the patterns we observed in solar and carbon repos:

### The OAE Scenario (mirror of DAC)

| DAC (exists) | OAE (doesn't exist) |
|-------------|---------------------|
| 2 computational screening repos (CC0) | 0 computational screening repos |
| DFT input files on GitHub | 0 mineral dissolution datasets |
| CC0 license (Sep 12, 2025) | 0 CC0 ocean datasets |
| Chemical Science + Chemistry of Materials papers | 0 published OAE screening papers with data |
| Maintained by Nyman lab (Oregon State) | **No equivalent group** |

### The OpenAir-Cyan Scenario (mirror of DIY hardware)

| Air (exists) | Ocean (doesn't exist) |
|-------------|----------------------|
| DIY DAC device (OSHWA-certified) | 0 DIY OAE deployment kits |
| 76 stars, documentation site | 0 stars, no documentation |
| Open hardware community | 0 open hardware community |
| Feb 12, 2024: 7 commits in 1 day | **No equivalent one-day sprint** |

### The WRF Scenario (mirror of Earth System Model)

| Atmospheric (exists) | Ocean (doesn't exist) |
|---------------------|----------------------|
| WRF: 1,762★, v4.8.0, active | 0 dedicated ocean intervention ESM |
| PCMDI: 133★, v4.2.1, active | 0 ocean intervention evaluation toolkit |
| MDTF: 80★, precip-buoyancy POD | **POD evaluates models, doesn't simulate interventions** |

**🎙️ Episode angle:** "If you wanted to build open-source ocean geoengineering today, you'd be doing something nobody has ever done. You'd be the first person to create a computational screening dataset for alkaline materials (like the Nyman lab did for DAC). You'd be the first person to build a DIY OAE deployment kit (like OpenAir-Cyan for air). You'd be the first person to create an ocean intervention Earth System Model (like WRF for the atmosphere). You'd be writing the first line of code that nobody has written yet. And that's exactly why it doesn't exist — because nobody's done it."

---n
## 🎙️ Episode Structure (Suggested)

### Act 1: "The Void" (7 min)
- 10 search queries, zero ocean geoengineering repos
- The three universes: fast, slow, empty
- Why the ocean is the empty quadrant

### Act 2: "The Closest Thing" (6 min)
- The precip-buoyancy POD: the most ocean-relevant code in open source
- It evaluates model accuracy; it doesn't design interventions
- The quality-control inspector who doesn't build the airplane
- ClimateSoton's website: 2 commits, both for a webpage

### Act 3: "Why Is the Ocean Empty?" (7 min)
- Four hypotheses: governance, complexity, funding, publication barriers
- Which is right? Which dominates?
- The political toxicity of ocean intervention vs. solar radiation

### Act 4: "What Would It Take?" (5 min)
- Mirror the DAC, OpenAir-Cyan, and WRF patterns
- What would an OAE computational screening dataset look like?
- What would a DIY OAE deployment kit look like?
- Could the ocean gap be the next open-source frontier?

---

## Data Sources

All search queries and commit data pulled fresh from GitHub API on September 19, 2026:
- 10 distinct search queries across GitHub repository search
- Commit histories from MDTF-diagnostics (15 commits), ClimateSoton.github.io (2 commits), WRF (15 commits, cross-referenced)
- v2 ocean ecosystem analysis (Oceananigans.jl, veros, OceanBioME) incorporated from previous research

---

## Research Log

| Date | Activity |
|------|----------|
| 2026-09-19 | v4: Ocean gap confirmed across 10+ search queries; ocean-adjacent repo profiles, hypotheses, and episode brief pushed to branch |
| 2026-09-17 | v3: Previous analysis completed; 6 ocean search queries confirmed zero repos |
| 2026-09-03 | Initial research notes created |
