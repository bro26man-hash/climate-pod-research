# ☀️ Solar Geoengineering — Commit Trend Analysis
## Trend Summary from 5 Repositories (September 2026 — v4 Update)

---

## Executive Summary

Fresh commit data was pulled from 5 solar/atmosphere repositories on September 18, 2026. The key finding: **solar geoengineering development is split between two universes — the high-activity institutional models (WRF, PCMDI, MDTF) that provide the evaluation infrastructure, and the dormant/niche academic repos that attempt direct SRM simulation but lack sustained development.**

The most significant trend: **solar radiation physics is being actively maintained, but SRM-specific simulation tools are absent.** We have world-class tools to evaluate whether a model can simulate climate; we lack comparably sophisticated tools to simulate an SRM intervention.

---

## Trend 1: Institutional Thunder — The PCMDI/WRF/MDTF Complex

### The Data

| Repo | Total Commits Pulled | Time Span | Avg Commits/Week |
|------|---------------------|-----------|------------------|
| WRF | 15 | ~1 month (May–Jun 2026) | ~3.75/wk |
| PCMDI | 15 | ~17 days (Sep 1–17, 2026) | ~6.0/wk |
| MDTF | 15 | ~2.5 months (May–Aug 2026) | ~2.1/wk |

### What This Tells Us

**PCMDI's September 4 release day is the standout event.** 10 commits in a single day — version bump, roundoff fix, dask optimization, SVD stability. This is what a mature open-source climate tool looks like at release time: focused, surgical, institutional.

**WRF's v4.8.0 is the solar-relevant milestone.** The May 28 solar radiation EOT correction and the June 5 aerosol parameterization changes are the commits that directly affect SRM simulation capacity. These aren't SRM-specific commits — they're general improvements that happen to be critical for SRM researchers.

**MDTF's June 19 precip-buoyancy POD is the ocean's closest connection.** Five commits to one file on one day. This is the most ocean-relevant diagnostic in open-source climate science, and it just happened.

### The Pattern

These three repos share a pattern: **institutional funding → sustained development → mature tooling → community dependence.** PCMDI is funded by the U.S. Department of Energy. WRF is funded by NOAA and NCAR. MDTF is funded by NOAA GFDL. Their commit rhythms reflect institutional priorities, not individual enthusiasms.

### 🎙️ Talking Point
"The solar geoengineering evaluation infrastructure is world-class. PCMDI, WRF, and MDTF are funded, maintained, and actively developed. But they share a common blind spot: they evaluate models, they don't simulate interventions. The SRM simulation layer is missing."

---

## Trend 2: The Ghost Revival — ClimateMARGO's Ambiguous Signal

### The Data

| Period | Commits | Type | Signal |
|--------|---------|------|--------|
| Jan 2022 | 8 | Code + docs | Active development peak |
| Feb 2022 | 2 | Code + docs | Continued activity |
| Nov 2022 | 2 | Code | Last real code commits |
| Jul 2023 | 1 | Doc (Pluto link) | Dormancy begins |
| Oct 2023 | 1 | Doc (comment) | Dormancy deepens |
| Aug 2026 | 2 | README only | ??? |

### What This Tells Us

ClimateMARGO's pattern is the **"academic ghost repo"** archetype: active development for a paper, then disappearance when the paper is published, then mysterious README updates years later with no code changes.

The August 2026 README updates are especially intriguing because:
1. They come after 2+ years of complete silence
2. They're documentation-only — no code, no tests, no issue responses
3. They could signal someone is preparing to use the model for a new study
4. Or they could just be citation management (updating a DOI link, adding a reference)

**The provocative question for the episode:** Is ClimateMARGO's revival a real signal of renewed geoengineering economic modeling interest, or is it just a researcher updating their citation page before a paper submission?

### 🎙️ Talking Point
"ClimateMARGO went dormant for 2 years, then its README got updated twice in one day. Is this the quiet prelude to a major policy moment? Or is this academic ghosting at its most ambiguous?"

---

## Trend 3: The Zero-Star Theorist — srm-forever's Conceptual Weight

### The Data

The srm-forever repository applies the Weitzman (1998) certainty-equivalent discounting framework to SRM cost dynamics. The question it addresses:

**"What is the social cost of committing to maintain SRM for centuries?"**

This is not a simulation tool. It's a theoretical framework — a mathematical argument about the cost structure of perpetual SRM maintenance.

### Why It Matters

- Zero stars, but conceptually critical
- The Weitzman framing is increasingly cited in SRM governance discussions
- It highlights the "commitment problem" — SRM must be maintained continuously, unlike decarbonization which is a one-time transition
- If SRM is stopped, temperatures rebound rapidly. The cost of "never stopping" is central to the governance question.

### 🎙️ Talking Point
"This repo has zero stars, but it asks the most important question in SRM economics: what does it cost to keep the sun shield up forever? And the answer might change how we think about who controls the thermostat."

---

## Trend 4: The Evaluation Gap — Where SRM Simulation Should Be

### What We Found

Across all 5 repos, we find:
- **World-class model evaluation tools** (PCMDI metrics, MDTF diagnostics)
- **World-class atmospheric modeling** (WRF physics suite)
- **Economic modeling frameworks** (ClimateMARGO, Geo-DICE)
- **Curated directories** (Awesome Geoengineering)

What we **don't** find:
- Open-source SRM simulation models (no "simulate stratospheric aerosol injection" repo with active development)
- Cloud brightening simulation tools (no "marine cloud brightening model" repo)
- Coupled ocean-atmosphere SRM tools (no repo that models the ocean response to SRM)
- Interactive SRM scenario tools (no "try SRM in a browser" repo — except the dormant srm-forever)

### The Hypothesis

The evaluation gap exists because:
1. SRM is politically controversial — funding for simulation tools is harder to obtain
2. The IPCC has not yet included SRM scenarios in its assessment reports, reducing institutional demand
3. The someone-else's-problem dynamic: atmospheric scientists evaluate models, but SRM specialists are a tiny community
4. The governance inhibitors: simulating SRM might be seen as advocating for it

### 🎙️ Talking Point
"We have better tools to evaluate whether a climate model works than we do to simulate what happens if we try to engineer the climate. The evaluation gap is real, and it's telling us something about what the scientific community is — and isn't — allowed to do."

---

## Trend 5: The Aerosol Parameterization Signal

### The Key Commit

**WRF, June 5, 2026:** "Turn off tempo_aerosolaware and tempo_hailaware in Registry (#2346)"

This commit disables two aerosol-aware schemes in the WRF TEMPO physics package. The implications:
- TEMPO is used for air quality and atmospheric chemistry modeling
- Disabling aerosol-aware schemes may indicate numerical instability or accuracy issues
- For SRM researchers, aerosol parameterization is critical: any error in aerosol forcing propagates directly into cooling predictions

### The Deeper Pattern

WRF's cyclical development pattern shows that aerosol physics is an active area of improvement: MYNN-EDMF updates (May 27), ShinHong PBL namelists (May 20), MMM surface layer revisions (May 20). Each of these affects how aerosols interact with clouds, radiation, and turbulence.

### 🎙️ Talking Point
"The most important solar geoengineering code you'll never read is a commit that turns off two aerosol flags. Because when you're simulating what happens when you block the sun, you'd better get the aerosol physics right."

---

## 📊 Trend Dashboard

```
                    Weekly Commit Velocity (approximate)

WRF     ████████████████████████████████████  3.75/wk  [INSTITUTIONAL]
PCMDI   ████████████████████████████████████████████████  6.0/wk  [INSTITUTIONAL]
MDTF    ██████████████████████████████  2.1/wk  [INSTITUTIONAL]
ClimateMARGO  ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  0.05/wk  [DORMANT]
srm-forever ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  ?/wk    [THEORETICAL]
```

**Legend:** █ = active code development | ░ = dormant or documentation-only

---

## 🔮 What to Watch

1. **WRF v4.8.0 adoption** — Will SRM researchers migrate to the new physics suite? The aerosol changes may force re-evaluation of existing simulation setups.

2. **PCMDI v4.2.1 usage** — The roundoff fix and dask optimizations will enable larger, more precise SRM evaluation studies. Watch for citations in 2027 IPCC reports.

3. **MDTF precip-buoyancy POD extension** — Will this diagnostic be extended to Marine Cloud Brightening scenarios? The June 19 commits are a starting point.

4. **ClimateMARGO's second README update** — Is this a real revival or a citation update? Check back in 3 months for code commits.

5. **srm-forever's theoretical framework** — If Weitzman discounting enters mainstream SRM governance discussions, this repo's 0-star obscurity will seem ironic.

---

*Data source: GitHub API commit histories pulled September 18, 2026. All timestamps in UTC. Commit counts may include merge commits and documentation updates.*

**Research log:** v4 update — fresh commit data from 5 solar/atmosphere repositories. Previous versions (v1–v3) used aggregated search results without API verification.

**Next steps:** Search for SRM-specific repositories using targeted queries ("stratospheric aerosol injection", "marine cloud brightening", "solar radiation management simulation"). Contact PCMDI maintainer Jiwoo Lee for potential interview.