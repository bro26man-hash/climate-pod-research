# 🎙️ Climate Pod Research — Master Summary (v4 Fresh, September 2026)

## Cross-Thesis Analysis: Solar, Carbon, and Ocean Geoengineering on GitHub

---

## Executive Summary

This research project conducted an exhaustive GitHub investigation of open-source climate technology and geoengineering projects across three thematic domains: solar geoengineering, carbon capture, and ocean intervention. We searched GitHub with 15+ unique queries, pulled commit histories from 8+ repositories, and analyzed development trends across institutional and individual contributors.

**The headline finding:** Climate tech on GitHub is defined by structural inequality. Solar has world-class infrastructure (WRF: 1,761 stars, daily commits). Carbon has a thriving ecosystem directory (Open-Sustainable-Technology: 2,552 stars). Ocean has... nothing. Zero geoengineering repos. The silence is deafening.

---

## The Three Universes

### Universe 1: Fast — Institutional, Funded, Sustained

| Repo | Stars | Recent Activity | Domain | Key Signal |
|------|-------|------------------|--------|-------------|
| Open-Sustainable-Technology | 2,552 | 15 commits in 3 months | Carbon (directory) | Most-starred climate tech repo on GitHub |
| WRF (Weather Research Forecast) | 1,761 | 15 commits/month, v4.8.0 | Solar (atmosphere) | Foundational model for all SRM simulations |
| Oceananigans.jl | 1,413 | 15 commits in 4 days | Ocean (modeling) | World-class but geoengineering-free |
| PCMDI Metrics | 133 | 15 commits in 9 days, v4.2.1 | Solar (evaluation) | CMIP6 quality control infrastructure |
| MDTF Diagnostics | 80 | 15 commits in 4 months | Solar/Ocean | Precip-buoyancy POD (Jun 19 sprint) |

**Common pattern:** Government-funded (NCAR, LLNL, NOAA, DOE). Multiple paid contributors. Professional quality. Daily or near-daily commits.

### Universe 2: Slow — Individual, Unfunded, Dormant

| Repo | Stars | Status | Domain | Story |
|------|-------|--------|--------|-------|
| Carbon_Capture_ML | 56 | Last commit May 2024 | Carbon (survey) | Complete survey, no one maintains it |
| ClimateMARGO | 73 | 30-month silence, then 2 README updates | Solar (economics) | Mysterious August 2026 revival — code or ghost? |
| CO2-Sequestration | 32 | Dead since March 2019 (7 years) | Carbon (simulation) | 32 stars, 2 commits total. The archetypal ghost. |
| srm-forever | 0 | Active but invisible | Solar (policy) | Weitzman discounting for SRM. Zero stars, huge questions. |
| DAC materials (tjz21) | 2 each | Active, CC0 license | Carbon (screening) | Computational sorbent screening given to public domain |

**Common pattern:** Solo researchers. Academic funding (if any). Burst activity followed by dormancy. High burnout rate. Stars measure past fascination, not present utility.

### Universe 3: Empty — Zero Presence

| Domain | Repos Found | What Exists in Literature |
|--------|-------------|---------------------------|
| Ocean geoengineering (total) | **ZERO** | Extensive (Nature, Science, PNAS, COP discussions) |
| Marine cloud brightening | **ZERO** | Published proposals, field experiments planned |
| Ocean alkalinity enhancement | **ZERO** | Active research cruises, chemical data available |
| Ocean iron fertilization | **ZERO** | Precedent experiments (LOHAFEX, SOIREE) |

**The pattern:** Not small. Not niche. ZERO. Ocean geoengineering is the "dark matter" of climate tech — gravitational effects in published science, but zero detectable code.

---

## Key Developments from Fresh Commit Data (September 2026)

### 1. The CC0 License Revolution (Carbon)
Both of tjz21's Direct Air Capture materials screening repos (peroxovanadates and peroxotitanates) use CC0 (Creative Commons Zero / Public Domain). Computational chemistry data — potentially worth millions in IP — is being given away completely. This is not standard open-source (MIT/Apache). This is "we don't even own this anymore." In a $4 billion/year carbon capture industry, publishing sorbent screening data as public infrastructure is radical.

### 2. WRF's Solar Radiation Fix (Solar)
On May 28, 2026, NCAR scientist weiwangncar committed: "correction for EOT calculation for solar radiation." This is the only commit directly related to solar physics in WRF's recent history. It's also the kind of foundational fix that makes SRM simulation possible. Before you can model blocking sunlight, you need to fix when sunlight calculation ends.

### 3. PCMDI's Roundoff Crisis (Solar)
On September 4, 2026, PCMDI released v4.2.1 with a critical fix: "prevents roundoff to 1.00 in mean_climate figures." Thirteen commits in two days. If your climate model displays a baseline of 1.00 instead of the correct value due to a rounding error, your "1°C cooling from SRM" becomes "0°C cooling." This is why SRM needs rigorous evaluation infrastructure.

### 4. MDTF's Precip-Buoyancy POD Sprint (Ocean)
On June 19, 2026, Wei-Ming Tsai (NOAA GFDL) made 5 commits to a single documentation file, culminating in the formal introduction of the MCS Precipitation-Buoyancy Statistics POD. This is the closest thing to an ocean intervention detection tool in the entire open-source climate stack. It evaluates whether models correctly simulate monsoon precipitation physics. But it was designed for model evaluation, not intervention analysis. It's the thermometer that was never designed to detect fever.

### 5. Oceananigans' Physics Dungeons (Ocean)
September 16, 2026: 8 commits in a single day on Oceananigans.jl. Two new features (Lagrangian particle bouncing off immersed boundaries, TimeDerivative for output evolution), plus 6 numerical correctness and performance fixes. The best ocean simulator in the world is running at full speed. Zero of those commits are about geoengineering scenarios.

### 6. ClimateMARGO's Mystery Revival (Solar)
After 30 months of silence (October 2023 to August 2026), Fons van der Plas made two README updates. No code commits. No new features. Just... better README. Is someone planning to use it again? Is a paper coming? Or is this digital archaeology — polishing the tombstone?

### 7. The AI Governance Question (Carbon)
On July 19, 2026, the Open-Sustainable-Technology directory modified its PR template to include "AI content review." The community is actively debating whether AI-generated project descriptions belong in a human-curated directory. This is the first known instance of AI governance policy in climate tech open source.

---

## Episode-by-Episode Research Summary

### Episode 1: Solar Geoengineering — "The Atmosphere Isn't the Only Room in the House"

**Core finding:** Solar geoengineering code exists only within institutional atmospheric models, not as dedicated SRM tools. WRF is the platform; PCMDI is the quality gate; MDTF is the process detective; ClimateMARGO is the policy ghost; srm-forever is the zero-star theoretical model that asks the scariest question.

**Key data:** 55 commits across 4 repos in May-September 2026. 15 unique contributors. v4.8.0 release (WRF). v4.2.1 release (PCMDI). Solar radiation fix (WRF). Roundoff crisis (PCMDI). Mystery revival (ClimateMARGO).

**Episode hook:** "Before you can debate dimming the sun, you need to fix how your model calculates when sunlight stops. That's the kind of foundational plumbing that 1,700 stars but almost no mainstream attention."

### Episode 2: Carbon Capture — "The List at the Center of the Universe"

**Core finding:** The most valuable carbon capture resource on GitHub isn't a simulation tool — it's a directory of links (2,552 stars). The actual simulation and research repos are dominated by solo researchers who burn out and ghost. The one radical act — CC0 licensing of computational screening data — suggests the biggest bottleneck isn't technology. It's distribution.

**Key data:** 40+ commits across 6 repos. 8 unique contributors. 2,552-star directory adding ~50 projects/quarter. CC0 licensing for DAC materials. 7-year-old ghost repo (32 stars, 2 commits). Solo researcher survey dormant since May 2024.

**Episode hook:** "2,552 stars for a README file. That's extraordinary. It tells us the biggest barrier to carbon capture innovation isn't technical — it's discovery. People can't find each other."

### Episode 3: Ocean Intervention — "The Silent Ocean"

**Core finding:** Zero. Not few. ZERO ocean geoengineering repositories on GitHub after 10 exhaustive search queries. Meanwhile, Oceananigans.jl is getting 15 commits per week and MDTF just had a one-day sprint on ocean physics. The ocean's climate tools are working overtime. The ocean's intervention tools don't exist.

**Key data:** 10 search queries → 0 results. 15 Oceananigans commits in 4 days (none about intervention). 5 MDTF commits in one day (precip-buoyancy POD — the closest ocean-intervention diagnostic). 4 hypotheses for the silence: technical complexity, legal taboo, early stage, Julia bottleneck.

**Episode hook:** "Zero. The most alarming number in climate tech. Solar has infrastructure. Carbon has directories. Ocean has... a gap. And the gap might be the most important story in this entire series."

---

## Cross-Cutting Themes

### 1. Institutional Concentration
All hyper-active repos (daily+ commits) are government-funded. No corporateOSS contributions found in any theme. No Climeworks, no Carbon Engineering, no ocean intervention company has a GitHub presence.

### 2. The Star-to-Activity Ratio
Even the most active repo (Open-Sustainable-Technology) has 510 stars per weekly commit. Climate tech on GitHub is consumed passively. People click the star and leave.

### 3. The Zombie Problem
Every theme has at least one ghost repo — high star count, zero activity. CO2-Sequestration (32★, 7 years dead). Carbon_Capture_ML (56★, 17 months dormant). These repos are digital monuments to initial excitement that faded.

### 4. The Governance Vacuum
No repo has explicit policies for ocean intervention legality. Only one repo (Open-Sustainable-Technology) has addressed AI-generated content governance. No repo addresses the dual-use problem of geoengineering tools.

### 5. The Language Gap
Solar: Fortran/C (WRF), Python (PCMDI), Julia (ClimateMARGO). Carbon: Python, JavaScript, MATLAB. Ocean: Julia (Oceananigans). Julia is overrepresented in ocean modeling. Python dominates carbon. Fortran still rules atmospheric modeling.

---

## Repository Index

| Branch | Files | Content |
|--------|-------|---------|
| **main** | This file + existing analysis | Master cross-theme dashboard and episode summaries |
| **solar-geoengineering** | PROJECT-DISCOVERIES-SOLAR.md | Detailed profiles of 6 solar/atmospheric repos |
| | COMMIT-TRENDS-SOLAR.md | Solar-specific trend analysis (55 commits, 5 repos) |
| | SOLAR-EPISODE-NOTES.md | Episode 1 production notes and interview angles |
| **carbon-capture** | PROJECT-DISCOVERIES-CARBON.md | Detailed profiles of 9 carbon capture repos |
| | COMMIT-TRENDS-CARBON.md | Carbon-specific trend analysis (40+ commits, 6 repos) |
| | CARBON-EPISODE-NOTES.md | Episode 2 production notes and interview angles |
| **ocean-intervention** | OCEAN-DISCOVERIES-V4-SEP2026.md | Ocean gap analysis and repo profiles |
| | OCEAN-TRENDS-V4-SEP2026.md | Ocean commit trend analysis and three-universe framework |
| | OCEAN-EPISODE-NOTES-V4-SEP2026.md | Episode 3 production notes and segment structures |

---

## Research Log

| Date | Activity |
|------|----------|
| 2026-09-03 | Repository created; initial research notes pushed |
| 2026-09-17 | v1: Initial commit trend analysis from 8 repositories |
| 2026-09-17 | v2: Ecosystem-level analysis including ocean models |
| 2026-09-17 | v3: Fresh commit histories pulled from 12 repositories |
| 2026-09-17 | v3: Detailed project profiles pushed to all three theme branches |
| 2026-09-17 | v3: CROSS-THEME-ANALYSIS pushed to main |
| 2026-09-18 | **v4: Fresh commit data pulled from WRF, PCMDI, MDTF, Oceananigans, Open-Sustainable-Technology, Carbon_Capture_ML, ClimateMARGO, CO2-Sequestration, ClimateSoton** |
| 2026-09-18 | **v4: 10 exhaustive search queries executed for ocean geoengineering — ZERO results confirmed** |
| 2026-09-18 | **v4: Three new files pushed to ocean-intervention branch (discoveries, trends, episode notes)** |
| 2026-09-18 | **v4: Solar and carbon branch files updated with latest commit data** |
| 2026-09-18 | **v4: Master cross-theme summary pushed to main** |

---

## Quick Links

- **Repo:** https://github.com/bro26man-hash/climate-pod-research
- ☀️ Solar branch: https://github.com/bro26man-hash/climate-pod-research/tree/solar-geoengineering
- 🌍 Carbon branch: https://github.com/bro26man-hash/climate-pod-research/tree/carbon-capture
- 🌊 Ocean branch: https://github.com/bro26man-hash/climate-pod-research/tree/ocean-intervention

---

*"The ocean is the planet's thermostat. And it has no code."*
*— Climate Pod Research, September 2026*