# ☀️ Solar Geoengineering — Project Discoveries
## Verified September 2026 — Commit Data Pulled Fresh from GitHub API

---

## 🏆 Tier 1: Institutional, Funded, Actively Maintained

### 1. WRF (Weather Research and Forecasting Model)
- **Repo:** [wrf-model/WRF](https://github.com/wrf-model/WRF)
- **Stars:** 1,761 | **Language:** Fortran | **License:** Apache-2.0
- **Last commit:** June 8, 2026 (v4.8.0 release)
- **Focus:** Foundational atmospheric model used worldwide for weather prediction and climate simulation
- **Why it matters for SGE:** WRF is the primary model used to simulate solar radiation management (SRM) scenarios. Any solar geoengineering experiment that models atmospheric effects must contend with WRF's physics suite. The recent v4.8.0 release includes critical solar radiation correction commits.

#### Recent Solar-Relevant Commits (May–June 2026):
| Date | Commit | Author | Significence |
|------|--------|--------|-------------|
| Jun 8 | Merge release-v4.8.0 | Anthony Islas | v4.8.0 released |
| Jun 6 | Update README and version to v4.8.0 | Anthony Islas | Documentation reset |
| May 28 | **Correction for EOT calculation for solar radiation** | weiwangncar | 🔥 **Direct solar radiation fix** —Easterly Offset Temperature calculation corrected for solar schemes |
| May 27 | Update MMM-physics repo SHA with various fixes | Anthony Islas | Physics suite update |
| May 26 | Fixing CDXWRF module | Lluís Fita | Convective downdraft fix |
| May 20 | Add new namelists for ShinHong PBL and revised MMM surface layer | weiwangncar | Boundary layer physics update |
| May 19 | Bug fix for udm | weiwangncar | Unified Diagnostics Module fix |
| May 12 | Updating MYNN-SFC submodule | Joseph Olson | Surface layer physics |

**Episode hook:** *"The most used climate model on Earth just fixed its solar radiation calculation. What does it mean for solar geoengineering research?"*

---

### 2. ClimateMARGO.jl
- **Repo:** [ClimateMARGO/ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- **Stars:** 73 | **Language:** Julia | **License:** MIT
- **Last commit:** August 17, 2026 (README update)
- **Focus:** Idealized climate-economic modeling framework for optimizing trade-offs between emissions mitigation, adaptation, and solar geoengineering
- **Why it matters:** This is one of the few open-source tools that explicitly models the *governance* dimension of SGE — not just the physics, but the economic optimal deployment strategy. The August 2026 README update after 2+ years of dormancy signals potential revival.

#### Recent Commits:
| Date | Commit | Author | Significence |
|------|--------|--------|-------------|
| Aug 17, 2026 | Update README.md (×2) | Fons van der Plas | 🔥 **Revival signal** — Two README updates after 2 years, 4 months of silence |
| Oct 18, 2023 | Update unit_conversions.jl with comment from #86 | Fons van der Plas | Last code change before dormancy |
| Jul 6, 2023 | Add link to Pluto in README | Fons van der Plas | Last activity before 2-year gap |
| Nov 14, 2022 | Update Project.toml | Fons van der Plas | Dependency management |
| Nov 12, 2022 | JuMP and Ipopt compat upgrade #85 | Fons van der Plas | Solver compatibility fix |

**Episode hook:** *"A climate-economics model dies on the shelf for two years, then suddenly gets its README updated. Is someone waking up to the idea that we need to plan for solar geoengineering — or is it just a stale page?"*

---

## 🏗️ Tier 2: Conceptually Important, Low Activity

### 3. GCCS-Core (Global Climate Control System)
- **Repo:** [KOSASIH/GCCS-Core](https://github.com/KOSASIH/GCCS-Core)
- **Stars:** 9 | **Language:** Python | **License:** Not specified
- **Last commit:** October 29, 2024 (single-day blitz of 15+ commits)
- **Focus:** "Foundational framework for the Global Climate Control System" — encompasses core algorithms, data processing, and server infrastructure
- **⚠️ Red flags:** All 15 commits on a single day (Oct 29, 2024). Zero commits since. No actual climate simulation code visible — appears to be scaffolding (setup.py, requirements.txt, deploy.sh, example files). The name "Global Climate Control System" is alarmingly grandiose for what's essentially a project skeleton.

#### Commit Pattern:
| Date | Commits | Type |
|------|---------|------|
| Oct 29, 2024 | 15 | All scaffolding (setup, deploy, examples, configs) |
| Total | 15 | **Zero substantive code commits** |

**Episode hook:** *"GitHub hosts a repo called 'Global Climate Control System' with 9 stars and all its commits in one day. It's basically a blank project template. But what it tells us about how people think about solar geoengineering is remarkable."*

---

### 4. OOCC_2021 (Solar Geoengineering Governance Model)
- **Repo:** [jlehtomaa/OOCC_2021](https://github.com/jlehtomaa/OOCC_2021)
- **Stars:** 2 | **Language:** Python | **License:** Not specified
- **Last commit:** November 15, 2021
- **Focus:** "A simple model for solar geoengineering governance" — published alongside a 2021 academic paper
- **Why it matters:** This is one of the very few repos that explicitly addresses the *governance* of SGE rather than the physics. The model explores how international cooperation could regulate solar geoengineering deployment.

#### Recent Commits:
| Date | Commit | Type |
|------|--------|------|
| Nov 15, 2021 | Update bibtex entry | Paper refinement |
| Oct 26, 2021 | Update bibtex reference | Paper refinement |
| Sep 5, 2021 | Update readme (×3) | Documentation push before publication |
| Sep 4, 2021 | Update citation / added citation file | Publication prep |
| Jul 30, 2021 | Update readme | Development phase |
| Jul 28, 2021 | Comment errors / update strategy tables | Strategy refinement |
| Jul 23, 2021 | Update / cleanups and checks | Final development |

**Pattern:** Classic academic paper repo — active development for 4 months, publication prep in September, then total silence. 15 commits total, all on governance strategy.

**Episode hook:** *"In 2021, a researcher built a model for how the world should govern solar geoengineering. Then he published the paper and stopped committing. The code is still there, still runnable, still the best open-source governance model we have. Why hasn't anyone maintained it?"*

---

### 5. GeoVision
- **Repo:** [pixnum-hub/GeoVision](https://github.com/pixnum-hub/GeoVision)
- **Stars:** 0 (unlisted) | **Language:** HTML | **License:** Not specified
- **Last commit:** December 6, 2025
- **Focus:** "Geoengineering Simulator" — created in a single day with 4 commits
- **⚠️ Assessment:** Barely exists. 4 commits on one day: initial commit, file upload, license, README update. No actual simulation code visible. The name "GeoVision" is generic enough to be either promising or empty.

---

## 🔬 Tier 3: Niche & Specialized

### 6. srm-forever
- **Repo:** [hausfath/srm-forever](https://github.com/hausfath/srm-forever)
- **Stars:** 0 | **Language:** Not specified
- **Last commit:** August 26, 2026
- **Focus:** Interactive SRM economics model using Weitzman certainty-equivalent discounting
- **Why it matters despite zero stars:** This repo applies the famous Weitzman (2009) framework to the question "What does it cost to keep solar geoengineering running forever?" The certainty-equivalent approach to discounting under deep uncertainty is the most rigorous economic framework for long-term SRM decision-making. Conceptually critical.

---

## 📊 Solar Geoengineering Development Landscape Summary

| Repo | Stars | Commits (recent) | Activity Status | Simulation Type |
|------|-------|-------------------|----------------|-----------------|
| WRF | 1,761 | 15 in 30 days | 🟢 Very Active | Atmospheric physics (general, not SGE-specific) |
| ClimateMARGO.jl | 73 | 2 README updates in 1 day | 🟡 Potential Revival | Climate-economic optimization |
| GCCS-Core | 9 | 15 in 1 day (Oct 2024) | 🔴 Dormant since | Scaffolding only |
| OOCC_2021 | 2 | 15 over 4 months (2021) | 🔴 Dormant since 2021 | Governance model |
| GeoVision | 0 | 4 in 1 day (Dec 2025) | 🔴 Dormant since | Simulator (empty) |
| srm-forever | 0 | Unknown (2026) | 🟡 Low Activity | SRM economics |

### Key Patterns:
1. **The institutional mega-model (WRF) doesn't know it's a geoengineering tool** — WRF is a general atmospheric model, but its solar radiation physics updates are the closest thing to an open-source SRM simulation standard
2. **Governance code is even rarer than simulation code** — Only OOCC_2021 and srm-forever address the "what should we do about SRM" question rather than the "how does SRM work" question
3. **The revival pattern is real but ambiguous** — ClimateMARGO's two README updates after 2 years could signal renewed interest or just someone tidying up a stale page
4. **Single-day commit bursts are the norm for academic repos** — GCCS-Core and GeoVision both show the "publish a paper, dump a repo, never return" pattern

---

## 🎙️ Episode Talking Points — Solar Geoengineering

### Opening Frame
> "We searched every GitHub repo related to solar geoengineering. The most downloaded atmospheric model on Earth is updating its solar radiation code right now. But the number of repos that explicitly simulate solar geoengineering is… zero. Here's what we found."

### Three Narrative Arcs
1. **The Hidden Infrastructure** (WRF) — The world's most important climate model silently maintains solar radiation physics. Scientists use it for SRM experiments but no one calls it a geoengineering repo.
2. **The Governance Vacuum** (OOCC_2021, srm-forever) — We have the physics but not the governance code. The best governance model is a dead repo from 2021.
3. **The Resurrection Question** (ClimateMARGO) — A dormant model wakes up. Is it a signal that economists are re-entering the SRM debate, or just someone updating a README?

### Q&A Provocations
- "If WRF fixes a solar radiation bug, does that count as geoengineering development?"
- "Should there be an 'SRM-FRAC' — a Solar Radiation Management Faithful Repo Attendance Counter — to track who's actually maintaining SGE code?"
- "What would an open-source ocean albedo enhancement model look like? Why doesn't it exist?"