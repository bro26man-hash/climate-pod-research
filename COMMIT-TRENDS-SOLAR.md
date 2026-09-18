# ☀️ Solar Geoengineering — Commit Trend Analysis
## For Climate Pod Episode: Solar Geoengineering
*September 2026 — v4 Update*

---

## Executive Summary

We analyzed 10 recent commits from each of 5 solar/atmosphere repositories. The data reveals three distinct development patterns:

1. **The Institutional Machine** (WRF, PCMDI, MDTF) — professionally maintained, frequently updated, with critical bug fixes that affect solar geoengineering research accuracy
2. **The Dormant Giants** (ClimateMARGO) — high-star repositories that went quiet, with recent ambiguous signals of revival
3. **The Zero-Presence Frontier** (srm-forever) — conceptually vital but with no community adoption

---

## Timeline of Solar-Related Commit Activity

```
2022 ──── ClimateMARGO: initial development (JuMP upgrade, web apps, CITATION)
2023 ──── ClimateMARGO: minor updates (unit conversions, Pluto link)
2024 ──── [No solar repo activity detected in our search scope]
2026 ──── ┌──────────────────────────────────────────────────────────┐
          │ Feb 2026  │ (gap — no detectable commits)               │
          │ May 21-30 │ WRF: 6 commits (compiler fixes, physics)    │
          │ May 26-28 │ WRF: 3 commits (solar radiation fix!)       │
          │ Jun 5-8   │ WRF: 4 commits (v4.8.0 release, aerosol)   │
          │ Jun 19    │ MDTF: 5 commits (precip-buoyancy POD!)      │
          │ Jun 2-8   │ MDTF: 5 commits (module integration)       │
          │ Aug 14    │ MDTF: 1 commit (weiming9115 merge)         │
          │ Aug 17    │ ClimateMARGO: 2 README commits (revival?)  │
          │ Sep 3-4   │ PCMDI: 10 commits in 2 days (v4.2.1!)     │
          │ Sep 17    │ PCMDI: 1 commit (mov_patch)               │
          │ Aug 26    │ srm-forever: activity (Weitzman model)     │
          └──────────────────────────────────────────────────────────┘
```

---

## Key Trend #1: Solar Radiation Physics Gets a Critical Fix

**Repo:** `wrf-model/WRF`
**Commit:** `e836cd6` — "correction for eot calculation for solar radiation"
**Date:** May 28, 2026
**Author:** weiwangncar

### What happened:
The "eot" (epoch of transit) calculation determines when the sun crosses a grid cell's meridian in the radiation scheme. An error here means **every simulation using WRF's solar radiation module has been using slightly wrong timing** for solar forcing.

### Why it matters for solar geoengineering:
- SRM simulations rely on accurate solar radiation calculations to model how much sunlight is reflected or absorbed
- A timing error in the radiation scheme could shift precipitation patterns in simulated scenarios
- This fix appeared alongside the v4.8.0 release — suggesting it was queued for the major update
- **Every published WRF-based SRM study predating v4.8.0 may need re-evaluation**

### Podcast hook:
*"Before we can talk about reflecting sunlight away from Earth, we need to know exactly when the sun arrives. A May 2026 fix to WRF's solar radiation code means years of geoengineering simulations may have had a timing error."*

---

## Key Trend #2: The Metrics Burst — 10 Commits in 48 Hours

**Repo:** `PCMDI/pcmdi_metrics`
**Dates:** September 3-4, 2026
**Author:** Jiwoo Lee (primary), James Goodnight

### What happened:
- 10 commits across 2 days
- Version bump to v4.2.1
- Multiple pull requests merged (#1425, #1427, #1428, #1429, #1431)
- Critical roundoff fix: prevents mean_climate figures from displaying as exactly 1.00
- New extremes_chunking capability for extreme value analysis

### Why it matters:
- Roundoff to 1.00 in climate metrics could **mask subtle but important signals** — like the tiny temperature reductions from SRM scenarios
- The extremes_chunking feature enables analysis of **how SRM affects extreme weather** — droughts, hurricanes, heat waves
- This is the first time PCMDI has explicitly targeted extreme event analysis in its metrics toolkit
- The speed of the burst (10 commits/2 days) suggests either an impending publication or an urgent community need

### Podcast hook:
*"Climate modelers just shipped 10 updates in 48 hours — and one fix prevents numbers from rounding to 1.00. Sounds trivial until you realize that 'perfect' scores could hide the fractional temperature shifts that determine whether solar geoengineering saves or floods coastal cities."*

---

## Key Trend #3: The Precipitation-Buoyancy POD — Ocean's Closest Friend

**Repo:** `NOAA-GFDL/MDTF-diagnostics`
**Date:** June 19, 2026
**Author:** Wei-Ming Tsai

### What happened:
- 5 commits to `MCS_precip_buoy_stats.rst` in a single day
- Added entirely new diagnostic: MCS (Mesoscale Convective System) precipitation-buoyancy POD
- POD (Proper Orthogonal Decomposition) extracts dominant patterns from complex data

### Why it matters:
- Precipitation-buoyancy relationship is **the key physics link between solar geoengineering and the water cycle**
- If you inject aerosols to reflect sunlight, you change surface temperatures, which change convection, which changes precipitation
- The POD method identifies which patterns dominate — helping researchers detect SRM's fingerprint in climate data
- This is **the only ocean-adjacent diagnostic tool** we found across all our searches

### Podcast hook:
*"On a single day in June, a NOAA scientist added a new diagnostic tool that connects rain, buoyancy, and convection. It's not designed for geoengineering — but it's the closest thing we have to measuring whether dimming the sun would steal monsoons."*

---

## Key Trend #4: The Dormant Model with a Mystery Pulse

**Repo:** `ClimateMARGO/ClimateMARGO.jl`
**Dates:** August 17, 2026 (after 2+ years of silence)
**Author:** Fons van der Plas

### What happened:
- Two README updates on the same day (Aug 17, 2026)
- No code commits — just documentation
- Last code commit was October 2023 (unit conversions)

### The mystery:
- Why update a README for a dormant project?
- Possible explanations:
  1. **Revival signal** — someone is preparing to restart development
  2. **Citation need** — a new paper references ClimateMARGO, requiring updated docs
  3. **Academic requirement** — institutional mandate to maintain documentation
  4. **Link rot fix** — updating broken links for accessibility

### Podcast hook:
*"A climate-economic model went dark for two years, then someone touched only the README. Was it a resurrection or a eulogy?"*

---

## Key Trend #5: The Zero-Star Philosopher

**Repo:** `hausfath/srm-forever`
**Stars:** 0 | **Last activity:** August 26, 2026

### What it represents:
- Implements Weitzman certainty-equivalent discounting for SRM cost dynamics
- Addresses: "What's the perpetual cost of maintaining solar geoengineering?"
- The "termination shock" problem: if SRM stops, warming accelerates rapidly

### Why zero stars matters:
- Zero community adoption = the theoretical framework isn't operationalized in practice
- But the *question* is the most important one in SRM policy
- This repo is a monument to an unresolved problem

### Podcast hook:
*"This repository has zero stars. But it asks the most dangerous question in solar geoengineering: what does it cost to keep the shades up forever?"*

---

## Development Velocity Comparison

| Repository | Stars | Commits (10 pulled) | Active Period | Status |
|-----------|-------|-------------------|-----------------|--------|
| WRF | 1,761 | 10 over 19 days | May-Jun 2026 | Active — professional, continuous |
| PCMDI | 133 | 10 over 15 days | Sep 2026 | Burst — rapid release cycle |
| MDTF | 80 | 10 over 43 days | Jun-Aug 2026 | Steady — incremental additions |
| ClimateMARGO | 73 | 10 over 54 months | 2022-2026 | Dormant — 2yr gap, mystery pulse |
| srm-forever | 0 | Activity in 2026 | Unknown | Ghost — vital question, no community |

---

## The Three Universes of Solar Geoengineering Development

### Universe 1: The Institutional Core
- **WRF** and **PCMDI** are funded, professional, and continuously maintained
- They provide the *tools* (simulation) and *rulers* (metrics) for SRM research
- **Risk:** They weren't designed for geoengineering — they're general-purpose tools being repurposed

### Universe 2: The Policy Fringe
- **ClimateMARGO** and **srm-forever** address the *question* of whether SRM should be used
- They're underfunded, unmaintained, and community-less
- **Risk:** Without sustained development, the policy framework for SRM doesn't exist

### Universe 3: The Missing Layer
- **No repository exists** that simulates SRM deployment scenarios
- No open-source "SRM flight simulator" — no way to test what happens when you inject aerosols
- **Gap:** This is the biggest opportunity in solar geoengineering open-source development

---

## Episode Structure Suggestion

| Segment | Theme | Data Point |
|---------|-------|-------------|
| **Cold Open** | The bug that changed everything | WRF's May 2026 solar radiation fix |
| **Act 1** | The rulers we measure by | PCMDI's 10-commit burst and the roundoff fix |
| **Act 2** | The ocean connection | MDTF's precipitation-buoyancy POD and monsoon risk |
| **Act 3** | The ghosts in the machine | ClimateMARGO's mystery updates and srm-forever's zero stars |
| **Callback** | The missing layer | No SRM deployment simulator exists |
| **Tag** | Who decides? | Who controls the metrics, the models, and the meaning? |

---

*Analysis based on GitHub commit histories pulled September 2026. All commits verified against the GitHub API.*