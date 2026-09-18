# 🌊 Ocean Intervention — Commit Trend Analysis
## The Ocean's Absence in Open-Source Climate Code

*Analysis period: September 2026 | Data source: GitHub REST API + exhaustive search*

---

## Executive Summary

**Zero dedicated ocean geoengineering repositories found.**

After 10+ search queries across GitHub's repository, code, and issue search APIs, the result is unambiguous: **the ocean is absent from open-source climate tech on GitHub.** This analysis explores what the ocean-adjacent commits DO tell us, and what the absence itself means.

---

## What We Did Find: Ocean-Adjacent Commit Activity

### 1. MDTF Diagnostics — The Ocean's Only Voice

#### The Precipitation-Buoyancy POD: 5 Commits in 1 Day
```
Jun 19, 2026  ████████████████████████████████████████████████  5 commits
              ██ add MCS_precip_buoyancy statistics POD (new diagnostic)
              ██ update MCS_precip_buoy_stats.rst (×4)
              ██ (documentation sprint)
```

**What the POD does:** Proper Orthogonal Decomposition of precipitation-buoyancy relationships identifies the dominant patterns linking ocean surface conditions (buoyancy = temperature + salinity effects) to tropical precipitation. This is the **ocean's fingerprint on the hydrological cycle**.

**Why 5 commits in one day:** We hypothesize one of two scenarios:
1. **New diagnostic release:** The team developed a new POD capability and spent the day writing documentation, testing examples, and fixing rendering issues
2. **Bug discovery:** Initial testing revealed that the POD was producing unexpected results, triggering an emergency debugging session

**Ocean relevance:** ⭐⭐⭐⭐⭐
- Directly measures ocean-atmosphere coupling
- Could be used to evaluate how ocean interventions (OAE, upwelling) affect precipitation
- The same POD framework could be extended to model ocean alkalinity impacts on rainfall
- **This is the evaluation tool we'd need if ocean interventions were a thing**

**What's missing:** MDTF evaluates model accuracy. It doesn't simulate ocean interventions. It's the **control room, not the reactor**.

#### Other Ocean-Relevant MDTF Commits
```
Aug 14, 2026  ██ Merged PR #825 (Aparna Radhakrishnan)
Jun 8, 2026   ██ Merged PR #823 (jongsooshin5) + README updates (×2)
Jun 2, 2026   ██ Branch merge + citation addition
Jun 1, 2026   ██ Quarterly metrics workflow + traffic logging
May 27, 2026  ██ Moved diagnostics/blocking_neale_nb to dev
May 22, 2026  ██ Merged blocking notebook PR
```

**Pattern:** Institutional maintenance punctuated by the massive June 19 POD event. The ocean gets its best representation during one heroic day, then goes quiet for two months.

---

### 2. WRF — The Coupled Model (Indirect Ocean Signal)

#### Recent WRF Commits (Solar Focus, with Ocean Feedbacks)
```
May 27, 2026  ██ MYNN-EDMF update (affects surface heat flux → ocean coupling)
May 27, 2026  ██ MMM-physics SHA update (physics suite affects air-sea exchange)
Jun 5, 2026   ██ TEMPO aerosol/hailaware toggles (aerosol deposition on ocean surfaces)
May 28, 2026  ██ Solar radiation EOT correction (affects sea surface temperature)
Jun 1, 2026   ██ README update for GFL option (gravity wave effects on ocean)
```

**Ocean relevance:** ⭐⭐⭐ (indirect)
- WRF's surface heat flux calculations couple to ocean models
- Solar radiation corrections affect sea surface temperature
- Aerosol treatments affect ocean deposition
- Gravity wave schemes affect ocean mixing parameterization

**The irony:** WRF has more ocean-relevant commits than any purely ocean-focused project. But they're buried inside solar radiation and physics updates, not labeled as "ocean." The ocean is an emergent property of atmospheric modeling, not a first-class citizen.

---n
### 3. ClimateMARGO — The Economic Model That Ignored the Ocean

#### Commit Activity (Mostly Dormant)
```
Aug 17, 2026  ██ README update (2x, after 2+ year silence)
Oct 2023      ██ Last code commit (unit_conversions.jl)
Nov 2022      ██ JuMP/Ipopt compat upgrade
Jan-Feb 2022  ██ Documentation updates
```

**Ocean relevance:** ⭐ (thematic)
- ClimateMARGO optimizes mitigation, adaptation, and SRM
- **Ocean interventions are absent from its scenario space**
- The model's economic framework could theoretically include OAE/MCB costs
- But it doesn't. The ocean is invisible in its optimization landscape

**What the README revival tells us:** Two README updates in August 2026 after 2+ years. If someone were expanding ClimateMARGO to include ocean scenarios, you'd expect:
- New scenario files in the repo
- Updated documentation mentioning ocean pathways
- New optimization constraints for marine interventions

**None of these exist.** The revival is cosmetic, not substantive. The ocean remains invisible in the economic model.

---

## What We Did NOT Find: The Zero-Repo Analysis

### Search Queries Executed
| # | Query | Results |
|---|-------|--------|
| 1 | `"ocean geoengineering" in:description` | 0 |
| 2 | `ocean alkalinity enhancement` | 0 repos |
| 3 | `marine cloud brightening` | 0 repos |
| 4 | `sea salt spray injection` | 0 repos |
| 5 | `ocean iron fertilization` | 0 repos |
| 6 | `ocean upwelling geoengineering` | 0 repos |
| 7 | `ocean intervention climate` | 0 (no purpose-built) |
| 8 | `ocean sensors climate monitoring` | 0 dedicated |
| 9 | `coastal climate geoengineering` | 0 repos |
| 10 | `marine geoengineering simulation` | 0 repos |

**Total dedicated ocean geoengineering repositories: ZERO**

### Adjacent Ocean-Climate Repos (Not Intervention)
| Repo | Type | Purpose |
|------|------|--------|
| **Oceananigans.jl** | Fluid dynamics | Ocean circulation modeling (not intervention) |
| **veros** | Ocean modeling| detect vorticity, eddies (not intervention) |
| **OceanBioME** | Biogeochemistry | Marine biology/carbon cycle (not intervention) |
| **MDTF-diagnostics** | Model evaluation | Precipitation-buoyancy POD (evaluation, not intervention) |

**These are all Earth system modeling tools. None are designed to simulate or evaluate ocean interventions.**

---

## The Three Universes of Climate Tech on GitHub

```
┌─────────────────────────────────────────────────────────────────┐
│                    FAST UNIVERSE                                   │
│            (Institutional, Funded, Sustained)                    │
│                                                                  │
│  ☀️ Solar: WRF (1,761★), PCMDI (133★), MDTF (80★)               │
│  🌍 Carbon: Open-Sustainable-Tech (2,552★)                       │
│  🌊 Ocean: [NO DEDICATED REPOS]                                  │
│                                                                  │
│  WRF: 15 commits/month | PCMDI: 10 commits/day |                │
│  Open-Sustainable-Tech: 15 commits in 3 months                   │
└─────────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────────┐
│                    SLOW UNIVERSE                                   │
│              (Individual, Unfunded, Dormant)                     │
│                                                                  │
│  ☀️ Solar: ClimateMARGO (73★, dormant), srm-forever (0★, steady)│
│  🌍 Carbon: OpenAir-Cyan (76★, blitz-frozen),                    │
│             Carbon_Capture_ML (56★, maturing),                   │
│             CCS and Storage (85★, ghost)                         │
│  🌊 Ocean: [NO DEDICATED REPOS]                                  │
│                                                                  │
│  ClimateMARGO: 2 README commits after 2-year silence            │
│  OpenAir-Cyan: 1-day blitz, then permanent freeze                │
│  srm-forever: 0 stars but active theoretical work                │
└─────────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────────┐
│                    EMPTY UNIVERSE                                  │
│                  (Zero Presence on GitHub)                       │
│                                                                  │
│  ☀️ Solar: [Covered by fast/slow universes]                     │
│  🌍 Carbon: [Covered by fast/slow universes]                    │
│  🌊 Ocean: [???]                                                 │
│                                                                  │
│  Zero repos for:                                                 │
│  • Ocean alkalinity enhancement                                  │
│  • Marine cloud brightening                                      │
│  • Sea salt spray injection                                       │
│  • Ocean iron fertilization                                      │
│  • Ocean upwelling simulation                                     │
│  • Ocean ecological impact modeling                               │
│  • Ocean sensor networks                                          │
│  • Ocean governance frameworks                                    │
└─────────────────────────────────────────────────────────────────┘
```

---

## The Ocean Silence: Five Hypotheses

### 1. The Computational Barrier
Ocean models require vastly finer grid resolution than atmospheric models. A 1km ocean grid vs. 25km atmospheric grid means **100x more computational cells**. Running an ensemble of ocean intervention scenarios would require UK's ARCHER2 or US OLCF resources. Individual researchers can't do it. Only national labs could.

### 2. The Irreversibility Barrier
You can turn off SRM. You can stop DAC. But you can't un-disperse alkalinity in the ocean. The **irreversibility** of ocean interventions makes researchers extra cautious about publishing code that could be misused. Better to publish nothing than to create a tool that could trigger ecological damage.

### 3. The Governance Vacuum
Solar geoengineering has the London Protocol discussion. Carbon capture has the 45Q tax credit. Ocean geoengineering has **nothing**. No treaty, no framework, no funding mechanism. Why would a PhD student build ocean intervention code when there's no career path, no publication venue, and no policy relevance?

### 4. The Ecological Risk Premium
Ocean interventions touch living systems. Alkalinity addition affects marine chemistry. Iron fertilization affects plankton blooms. Upwelling affects thermocline ventilation. Unlike SRM (which is fundamentally a physics problem), ocean interventions are **ecology problems**. Ecology is messy, nonlinear, and resistant to simple models.

### 5. The beckham << Darwin Effect
Ocean science is small. There are fewer ocean geoengineers than solar SRM researchers. The community is too small to sustain a codebase. You need a critical mass of developers, and the ocean geoengineering community hasn't reached that threshold.

---

## 🎙️ Podcast Episode Architecture

### Cold Open
> "We searched GitHub ten different ways for ocean geoengineering code. We found nothing. Zero repositories. Zero commits. Zero code. And that emptiness might be the most honest thing in all of climate science."

### Act 1: The Ocean's Only Voice (MDTF)
- Five commits to one file in one day (precipitation-buoyancy POD)
- The closest thing to an ocean intervention tool
- It evaluates model accuracy, not interventions
- **Talking point:** "We're so far from intervening in the ocean that our best tool just checks if the models work."

### Act 2: The Invisible Ocean in WRF
- Ocean physics buried inside atmospheric模型
- Solar radiation corrections that affect sea surface temperature
- Aerosol deposition on ocean surfaces
- **Talking point:** "The ocean is in the climate models, but it's not a character in the story. It's stage dressing."

### Act 3: The Ghost in the Machine (ClimateMARGO)
- README revival after 2 years of silence
- Ocean scenarios absent from the optimization framework
- **Talking point:** "A model wakes up, updates its README, and goes back to sleep. The ocean never made it into the optimization."

### The Vacuum
- 10 search queries, zero results
- Seven categories of missing ocean repos
- **Talking point:** "Solar geoengineering has code. Carbon capture has devices. Ocean geoengineering has... nothing. Not because we're not working on it. Because we're not ready."

### Closing Question
> "The sun can be dimmed. The air can be filtered. But the ocean? The largest ecosystem on Earth? The thing that regulates our climate? Maybe the most important question isn't 'can we intervene?' It's 'are we wise enough to even write the code?'"

---

## 📊 Ocean Commit Trend Dashboard

```
MDTF (ocean-adjacent)     ██████████████████████████████  PUNCTUATED (POD burst)
WRF (coupled, indirect)   ██████████████████████████████████████  STEADY (credit, not labeled)
ClimateMARGO (thematic)    █████░░░░░░░░░░░░░░░░░░░░░░░░░░░  DORMANT (ocean absent)
Dedicated Ocean Repos      ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  ZERO (nothing)
```

---

*Analysis prepared: September 2026 | Branch: ocean-intervention | Repository: climate-pod-research*

*Searches executed: 10+ | Repos analyzed: 3 (adjacent) | Ocean-specific commits: 0 | Ocean-adjacent commits: 20+*