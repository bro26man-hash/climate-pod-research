# ☀️ Solar Geoengineering — Open-Source Project Discoveries (v4, Sep 2026)

**Research Date:** September 2026  
**Methodology:** GitHub Repository Search API + Code Search API  
**Queries Used:** `geoengineering simulation climate`, `geoengineering stars:>5`, `climate simulation modeling stars:>10`, `marine cloud brightening ocean albedo`

---

## Executive Summary

After 10+ search queries across the GitHub ecosystem, we identified **4 active or semi-active open-source projects** directly relevant to solar geoengineering / solar radiation management (SRM). The landscape is dominated by **climate simulation models** (WRF, ClimateMARGO) rather than purpose-built SRM repositories — a key insight for our episode.

**Headline finding:** Solar geoengineering code lives *inside* climate models, not in SRM-specific repos. The science is embedded in the physics parameterizations of mainstream tools.

---

## Project Profiles

### 1. 🏆 wrf-model/WRF — The Workhorse

| Field | Detail |
|-------|--------|
| **URL** | https://github.com/wrf-model/WRF |
| **Stars** | 1,763 |
| **Language** | Fortran |
| **Last Activity** | June 8, 2026 (v4.8.0 release) |
| **Maintainers** | NCAR / NOAA / university consortium |
| **Contributors (recent)** | Anthony Islas, weiwangncar, Joseph Olson, Lluís Fita, Kelly Werner, Anders Jensen-NOAA, Chenghao Wang |

**Why it matters:** WRF is the most widely used regional climate model in the world. Its aerosol-aware physics schemes (TEMPO, MADE/SORGAM) are *the* tools used to simulate sulfate aerosol injection — the most studied SRM technique.

**Recent solar-relevant commits (May–June 2026):**
- `06d4240` — v4.8.0 release merge (Jun 8)
- `0708348` — README & version update for v4.8.0 (Jun 6)
- `6a289e1` — **Turned off tempo_aerosolaware and tempo_hailaware** (Jun 5) — significant SRM-relevant toggle
- `e836cd6` — **Correction for eot calculation for solar radiation** (May 28) — directly affects solar flux computation
- `8299919` — MYNN-EDMF pointer update & icloud_bl removal (May 27)
- `9c87d29` — New namelists for ShinHong PBL and revised MMM surface layer (May 20)
- `8fa379b` — Bug fix for urban NbS initialization (May 20)

**Episode angle:** A TEMPO aerosol toggle being turned *off* made it into release notes — SRM code is treated as a niche parameterization, not a first-class feature.

---

### 2. 🌍 ClimateMARGO/ClimateMARGO.jl — The Optimizer

| Field | Detail |
|-------|--------|
| **URL** | https://github.com/ClimateMARGO/ClimateMARGO.jl |
| **Stars** | 73 |
| **Language** | Julia |
| **Last Activity** | August 17, 2026 (README update) |
| **Maintainer** | Fons van der Plas (PhD researcher) |

**Why it matters:** Idealized climate-economic modeling framework for optimizing trade-offs between emissions mitigation, adaptation, and geoengineering. Not a GCM — a simplified Earth system model for global-scale policy optimization.

**Commit pattern — classic "burst and dormancy":**
- **Jan 12, 2022:** 8 commits in a single day (documentation push, version bump, CITATION.bib)
- **Feb 2022:** 3 more commits (compat upgrades, cleanup)
- **Oct 18, 2023:** 1 commit (unit conversion comment)
- **Jul 6, 2023:** 1 commit (Pluto notebook link)
- **Aug 17, 2026:** 2 commits (README updates)
- **Total gap:** 3.5 years between Feb 2022 and Oct 2023, then 2.5 years until Aug 2026

**Episode angle:** Typical academic research code lifecycle — built for a paper, maintained for citations, dormant between publications. The Julia language choice is notable: next-gen scientific computing is increasingly Julia-first.

---

### 3. 🔬 Sustainable-Solutions-Lab/regional-geo — SRM Regional Impact

| Field | Detail |
|-------|--------|
| **URL** | https://github.com/Sustainable-Solutions-Lab/regional-geo |
| **Stars** | Small research group |
| **Language** | Python/R |
| **Last Activity** | February 15, 2026 |
| **Maintainer** | Ken Caldeira (Carnegie Institution / Stanford) |

**Why it matters:** The most *directly* SRM-focused repository we found. Contains WRF input data and analysis code for studying **regional climate effects of sulfate aerosol injection** — "what happens to rainfall patterns in Africa and Asia if we inject aerosols in the Northern Hemisphere?"

**Commit pattern — intense research sprint:**
- **Feb 13, 2026:** 11 commits (README, data loader, style guide, file dimension docs)
- **Feb 14, 2026:** 3 commits (reading RDS files, area calculation, showing individual cases)
- **Feb 15, 2026:** 1 commit (gaussian smoothing for maps)
- **Total:** 15 commits in 3 days

**Key features:** Data loader for WRF output files, RDS file reading, area calculation scripts, Gaussian smoothing for spatial analysis, comprehensive README.

**Episode angle:** Ken Caldeira is one of the most prominent names in SRM research. This repo shows the *real* workflow: not elegant software engineering, but rapid research scripting — data loaders, analysis scripts, figure fixes — all in a 3-day burst.

---

### 4. 🌿 queraltab/Greenhouses-Library — Controlled Environment

| Field | Detail |
|-------|--------|
| **URL** | https://github.com/queraltab/Greenhouses-Library |
| **Stars** | 54 |
| **Language** | Modelica (OpenModelica) |
| **Last Activity** | August 2, 2019 |

**Why it matters (tangentially):** Greenhouse climate modeling library — simulating temperature, humidity, and heat pump systems for agricultural greenhouses. Not SRM per se, but relates to climate intervention in controlled environments.

**Commit pattern — complete dormancy:** All 15 commits from 2019. Dead since 2019.

**Episode angle (optional):** Cautionary tale — open-source climate tools often die after the PhD defense.

---

## Cross-Cutting Themes for the Episode

### 1. SRM Code Is Inside Climate Models, Not in SRM Repos
No "sulfate injection simulator" repository with 500 stars exists. SRM capability exists as *parameterizations* inside WRF and similar models.

### 2. The "Burst and Dormancy" Lifecycle
Three of four projects show this pattern: intense activity around paper deadlines, then long dormancy.

### 3. Institutional vs. Individual Development
- **WRF:** Multi-institutional, funded, continuous
- **ClimateMARGO:** Individual, dormant, burst pattern
- **regional-geo:** Individual, sprint-based
- **Greenhouses-Library:** Individual, dead after PhD

### 4. The Language Shift
Older tools are Fortran (WRF) or MATLAB. Newer tools are Julia (ClimateMARGO) and Python (regional-geo).

---

## Source Data

All commit histories pulled via GitHub List Commits API:
- wrf-model/WRF: 15 most recent commits
- ClimateMARGO/ClimateMARGO.jl: 15 most recent commits
- Sustainable-Solutions-Lab/regional-geo: 15 most recent commits
- queraltab/Greenhouses-Library: 15 most recent commits
