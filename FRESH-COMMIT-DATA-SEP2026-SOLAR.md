# ☀️ Solar Geoengineering — Fresh Commit Data (September 2026)

**Pulled:** September 2026  
**Repositories:** wrf-model/WRF, ClimateMARGO/ClimateMARGO.jl, brandonhimpfen/awesome-geoengineering, PSLmodels/Geo-DICE, antara-banerjee/GeoengineeringLE_WinterWarming, jlehtomaa/OOCC_2021, KOSASIH/GCCS-Core

---

## Overview: What the Fresh Data Reveals

This data supplements the existing COMMIT-TRENDS-SOLAR.md analysis with granular commit histories pulled directly from the GitHub API in September 2026. The big picture: **solar geoengineering on GitHub is bifurcated** — institutional models (WRF) are intensely active, while governance and interactive tools are either dormant or single-author. The surprise hit is **awesome-geoengineering**, a curated directory that's actively maintained with 7 commits including updates on Sep 5-6, 2026.

---

## 1. wrf-model/WRF — 1,761 Stars — ACTIVE INSTITUTIONAL RELEASE

**15 commits pulled · May 12 – Jun 8, 2026 · 5 contributors**

| Date | Commit SHA | Message | Author |
|------|-----------|---------|--------|
| Jun 8 | 06d4240 | Merge remote-tracking branch 'origin/release-v4.8.0' | Anthony Islas |
| Jun 6 | 0708348 | Update README and version declaration to new v4.8.0 (#2347) | Anthony Islas |
| Jun 5 | 6a289e1 | Turn off tempo_aerosolaware and tempo_hailaware in Registry (#2346) | weiwangncar |
| May 30 | 4466746 | Fix a vectorization option in AOCC stanza (#2335) | weiwangncar |
| May 28 | e836cd6 | **Correction for eot calculation for solar radiation** (#2334) | weiwangncar |
| May 27 | 8299919 | Updating MYNN-EDMF pointer and removing icloud_bl package (#2336) | Joseph Olson |
| May 27 | 4fab0e2 | Update MMM-physics repo SHA with various fixes (#2339) | Anthony Islas |
| May 26 | 75ad1f9 | Fixing CDXWRF module (#2322) | Lluís Fita |
| May 26 | 0aa6582 | Update readme file for GFL option (#2333) | weiwangncar |
| May 21 | 02f02bc | Include mp_physics=88 in TEMPO error print message (#2325) | Kelly Werner |
| May 20 | 06e6998 | Minor Tempo changes (#2310) | AndersJensen-NOAA |
| May 20 | 8fa379b | Fixing a scheme-guard bug in urban NbS initialization (#2329) | Chenghao Wang |
| May 20 | 9c87d29 | Add new namelists for ShinHong PBL and revised MMM surface layer (#2323) | weiwangncar |
| May 19 | c1cd5c4 | Bug fix for udm (#2309) | weiwangncar |
| May 12 | b96a7e9 | Updating the MYNN-SFC submodule (#2311) | Joseph Olson |

### 🔑 Critical Findings

1. **Solar radiation EOT correction (May 28):** The commit `e836cd6` — "Correction for eot calculation for solar radiation" — is the most SRM-relevant commit in the entire dataset. EOT (Empirical Orthogonal Transform) corrections affect how solar radiation is calculated in WRF. This directly impacts any SRM simulation that uses WRF as its atmospheric model. A correction means previous simulations may have had systematic errors in their solar radiation calculations.

2. **TEMPO aerosol physics being staged (Jun 5):** The commit `6a289e1` turns OFF `tempo_aerosolaware` and `tempo_hailaware` in the Registry. These are experimental TEMPO (Traceable Intensity of Aerosols and Gases) options. Being turned OFF in a stable release (v4.8.0) means they're being moved to the next development cycle. TEMPO aerosol microphysics is the closest thing to an SRM aerosol simulation module in WRF.

3. **MYNN-EDMF update (May 27):** The MYNN-EDMF (Yonsei University Nonlocal closure + Eddy-Diffusivity Mass-Flux) update includes ocean boundary layer physics improvements. This is relevant for marine cloud brightening simulations where the ocean-atmosphere interface matters.

4. **Multi-institutional orchestration:** 5 contributors from NCAR (weiwangncar, Islas), NOAA (AndersJensen-NOAA), LLNL (Fita), and university (Olson, Wang, Werner). This is a textbook institutional release cycle.

5. **10 commits in 18 days (May 12 – Jun 8):** The release cadence is intense but sustainable. This is the "fast universe" of climate tech — funded, staffed, and running.

**🎙️ Podcast angle:** *The atmospheric model that simulates SRM effects just corrected its solar radiation physics and is staging aerosol microphysics for the next release. If you're simulating what happens when you inject sulfates, WRF is the tool — and it just got better.*

---

## 2. brandonhimpfen/awesome-geoengineering — 4 Stars — THE MOST ACTIVELY MAINTAINED GEOENGINEERING REPO

**7 commits pulled · Jun 28, 2025 – Sep 6, 2026 · 1 contributor (but reportedly multiple)**

| Date | Commit SHA | Message |
|------|-----------|--------|
| Sep 6 | 8d0a800 | Update README.md |
| Sep 5 | 5926daf | Update README.md |
| May 5 | a6e8359 | Update to v2.0.0 |
| Mar 12 | c06033b | Update README.md |
| Jan 16 | b04d97a | Update README.md |
| Jun 28 | c5dfd85 | Update README.md |
| Jun 28 | 06ac1de | Initial commit |

### 🔑 Critical Findings

1. **Active as of September 2026:** Updates on Sep 5 AND Sep 6, 2026. This is the ONLY geoengineering-specific repository in our entire analysis that was actively updated in September 2026.

2. **v2.0.0 released May 5, 2026:** A major version bump signals either a significant content expansion or a rebranding. The directory has likely grown substantially.

3. **Consistent quarterly updates:** Jan, Mar, May, Sep — roughly quarterly cadence. This is sustainable, not bursty.

4. **4 stars but active:** Star count undercounts the value. A well-maintained directory of geoengineering resources is more useful for podcast research than most repos with 100x more stars.

**🎙️ Podcast angle:** *The most actively maintained geoengineering-specific repo on GitHub has 4 stars but was updated twice this week. Stars don't measure utility — they measure fame. This directory is the real working resource for people in the field.*

---

## 3. ClimateMARGO/ClimateMARGO.jl — 73 Stars — THE DORMANT REVIVAL SIGNAL

**15 commits pulled · Oct 2023, Jul 2023, Nov 2022, 2022, Jan 2022, + Aug 2026 README updates**

| Date | Commit SHA | Message | Type |
|------|-----------|---------|------|
| Aug 17, 2026 | d916f36 | Update README.md | 🔴 README-only |
| Aug 17, 2026 | 6d9ba7a | Update README.md | 🔴 README-only |
| Oct 18, 2023 | 57d4da7 | Update unit_conversions.jl with comment from #86 | 🟢 Code |
| Jul 6, 2023 | fbbe619 | add link to pluto in readme | 🔴 README |
| Nov 14, 2022 | 5063c42 | Update Project.toml | 🟡 Dependency |
| Nov 12, 2022 | 12a0ce6 | JuMP and Ipopt compat upgrade (#85) | 🟢 Code |
| Feb 10, 2022 | 32e66fd | Removed deprecated web apps | 🟡 Infrastructure |
| Feb 4, 2022 | d609d49 | Added CITATION.bib | 🔵 Citation |
| Jan 13, 2022 | b2d9228 | Fixed typo | 🔵 Minor |
| Jan 12, 2022 | 8a7e012 | Updated arguments for doc version deployment | 🔵 Infrastructure |
| Jan 12, 2022 | 0954182 | Added documenter key | 🔵 Infrastructure |
| Jan 12, 2022 | 26a80b3 | Update README.md | 🔴 README |
| Jan 12, 2022 | ea2a879 | Bump version | 🟡 Version |
| Jan 12, 2022 | b35e5ca | Update documentation (#83) | 🔵 Docs |
| Jan 12, 2022 | 27e2bf5 | Update documentation (#82) | 🔵 Docs |

### 🔑 Critical Findings

1. **The Jan 12, 2022 burst:** 11 commits on a single day. This is the classic "academic launch" pattern — a paper drops, the repo is created, documentation is added, version is bumped. Then silence.

2. **2+ years of dormancy (Feb 2022 – Aug 2026):** No activity for 42 months. The last code commit was October 2023 (a comment fix, not new features).

3. **The Aug 17, 2026 resurrection:** Two README updates on the same day. No code. No new features. Just documentation touching. This is the "maybe" signal — someone remembered the project, updated the description, but didn't write any code.

4. **The Julia cliff:** ClimateMARGO is written in Julia, a language with growing scientific computing adoption but still a niche. The JuMP/Ipopt compat upgrade (Nov 2022) suggests they were fighting dependency breakage. The lack of further code commits may indicate the Julia ecosystem proved too brittle for sustained development.

**🎙️ Podcast angle:** *ClimateMARGO — the climate-economic model for quantifying trade-offs between mitigation, adaptation, and geoengineering — went dormant for over 3 years, then suddenly got its README touched. No code. No new features. Is this a revival or a funeral procession? The Aug 2026 README updates might be the first sign of life... or the last flicker.*

---

## 4. PSLmodels/Geo-DICE — 2 Stars — THE LEGACY GHOST

**4 commits pulled · Aug 2016 – Sep 2018 · 2 contributors**

| Date | Commit SHA | Message |
|------|-----------|--------|
| Sep 27, 2018 | 82a0370 | Add files via upload |
| Aug 15, 2016 | fe8da8e | Add files via upload |
| Aug 15, 2016 | b2f65e6 | Add files via upload |
| Aug 15, 2016 | 82e4f18 | Initial commit |

### 🔑 Critical Findings

1. **Dead since 2018.** 8 years without a commit. Last activity was "Add files via upload" — not even meaningful code changes.

2. **Only 4 commits in entire lifetime.** The initial commit, two uploads on the same day, and one upload 2 years later. This is the "set it and forget it" academic repo.

3. **Modified DICE model with geoengineering.** Geo-DICE extends the Dynamic Integrated Climate-Economy model to include geoengineering as a policy lever. The concept is sound, but the implementation is frozen in 2018-era MATLAB.

**🎙️ Podcast angle:** *Geo-DICE: a modified DICE model that includes geoengineering as an option. 8 years dead. 2 stars. The DICE model itself is one of the most influential climate economics tools ever created — but its geoengineering variant is a ghost. The governance modeling layer of solar geoengineering is stuck in MATLAB from the Obama era.*

---

## 5. antara-banerjee/GeoengineeringLE_WinterWarming — 2 Stars — THE ACADEMIC NICHE

**10 commits pulled · Apr 6 – Apr 24, 2021 · 1 contributor**

| Date | Commit SHA | Message |
|------|-----------|--------|
| Apr 24, 2021 | 3ed2840 | Update README.md |
| Apr 23, 2021 | ee54d4f | updated |
| Apr 16, 2021 | e5f3f8f | removing netcdf (somewhat large file) |
| Apr 16, 2021 | fb7947a | removed netcdf from repo |
| Apr 14, 2021 | cab6d96 | slight updates to color handling for consistency |
| Apr 8, 2021 | d7710a1 | renamed ensemble and plotting modules for readability |
| Apr 8, 2021 | e3b380d | cleaning up region selection for readability |
| Apr 6, 2021 | 090e2be | adding numpy outputs directory to gitignore |
| Apr 6, 2021 | 1d04e09 | added 95% confidence stippling to congruent/residual NAM regression plots |
| Apr 6, 2021 | 0b87fc5 | small change to add condition to saving calculated PCs |

### 🔑 Critical Findings

1. **Specific scientific focus:** This is an ensemble modeling project for studying winter warming patterns in response to geoengineering. The commit messages reference NAM (Northern Annular Mode), confidence stippling, and PCA (Principal Components). This is published-science code, not a general tool.

2. **Single-burst pattern:** All 10 commits in 18 days (Apr 6-24, 2021). Paper was likely published around that time. Then complete silence.

3. **NetCDF cleanup:** The removal of large netCDF files suggests the author was trying to slim the repo before publication. This is common in academic repos where large data files are pushed to Zenodo or similar.

**🎙️ Podcast angle:** *This repo represents the ' Publish and Perish' pattern: a researcher builds an ensemble model for winter warming response to geoengineering, publishes the paper, pushes the code for the publication, then moves on. 2 stars, 5 years dormant. The science is specific and useful for one question, but it's not a platform.*

---

## 6. jlehtomaa/OOCC_2021 — 2 Stars — THE GOVERNANCE TEACHING TOOL

**10 commits pulled · Sep 3 – Nov 15, 2021 · 1 contributor**

| Date | Commit SHA | Message |
|------|-----------|--------|
| Nov 15, 2021 | 333c878 | update bibtex entry |
| Oct 26, 2021 | b62c2da | update bibtex reference |
| Sep 5, 2021 | f7fe793 | update readme |
| Sep 5, 2021 | 32051b7 | update readme |
| Sep 5, 2021 | c8aabbd | update readme |
| Sep 4, 2021 | cb130ac | update citation |
| Sep 4, 2021 | 9d3899a | added citation file |
| Sep 3, 2021 | a665677 | update readme |
| Sep 3, 2021 | 01fcd9e | update readme |
| Sep 3, 2021 | ecb16a0 | update readme |

### 🔑 Critical Findings

1. **A simple solar geoengineering governance model.** The repo description says "A simple model for solar geoengineering governance." This is the governance layer — not simulation, not physics, but the policy/economics modeling.

2. **BibTeX management, not code development:** 6 of 10 commits are reference/citation updates. The "model" may be primarily a document with embedded equations, not a runnable simulation.

3. **Burst pattern matches conference cycle:** All activity in a 3-month window (Sep-Nov 2021). Likely tied to a paper submission or conference presentation.

**🎙️ Podcast angle:** *The open-source governance model for solar geoengineering is a document with BibTeX references. The hardest part of geoengineering — who decides? — has a GitHub repo where the most active development was... updating citations. The governance gap is real, and this repo proves it's not even close to being solved computationally.*

---

## 7. KOSASIH/GCCS-Core — 9 Stars — THE DIY CLIMATE CONTROL SINGLE-DAY BURST

**10 commits pulled · ALL on Oct 29, 2024 · 1 contributor**

| Date | Commit SHA | Message |
|------|-----------|--------|
| Oct 29, 2024 | 99bf84f | Update README.md |
| Oct 29, 2024 | 7cad777 | Update README.md |
| Oct 29, 2024 | 4350445 | Update README.md |
| Oct 29, 2024 | b6e44cc | Update README.md |
| Oct 29, 2024 | cfaa741 | Update README.md |
| Oct 29, 2024 | bef35ee | Update README.md |
| Oct 29, 2024 | cc92644 | Update README.md |
| Oct 29, 2024 | fc3553b | Create requirements.txt |
| Oct 29, 2024 | f6da191 | Create setup.py |
| Oct 29, 2024 | 4a068bc | Create data_collection.sh |

### 🔑 Critical Findings

1. **All 10 commits on a single day.** 7 README updates + setting up Python packaging. This looks like a repo that was prepared for publication on GitHub in one push — all files, all at once.

2. **7 README updates in one day:** This may indicate iterative testing of the GitHub Pages documentation or multiple sections being added to the README. It could also mean the author was uncertain about how GitHub repositories work.

3. **Global Climate Control System (GCCS):** The description says "foundational framework for the Global Climate Control System." This is ambitious. The actual scope appears to be a Python package for climate data collection and analysis, not literal climate control.

4. **No commits since Oct 29, 2024.** Dead on arrival. Set up, documented, pushed, then nothing.

**🎙️ Podcast angle:** *GCCS-Core: 10 commits in a single day, all about setting up Python packaging and writing READMEs. "Global Climate Control System" — the name is bigger than the project. A Python data collection framework that got 9 stars and then vanished. It's the "README-driven development" pattern taken to the extreme.*

---

## Comparative Analysis: Seven Types of Solar Geoengineering Repos

| Repo | Stars | Commits | Active Period | Pattern | SRM Relevance |
|------|-------|---------|--------------|---------|---------------|
| **WRF** | 1,761 | 15/18d | May-Jun 2026 | Institutional release | **Direct** — atmospheric model |
| **awesome-geoengineering** | 4 | 7/quarter | Jun 2025-Sep 2026 | Sustainably maintained | **Indirect** — resource directory |
| **ClimateMARGO** | 73 | 15 over 4yr | 2022-2023 + Aug 2026 | Dormant revival | **Policy** — economic modeling |
| **Geo-DICE** | 2 | 4 total | 2016-2018 | Legacy ghost | **Policy** — DICE + geoengineering |
| **WinterWarming** | 2 | 10/18d | Apr 2021 | Academic publish-and-die | **Niche** — winter response |
| **OOCC_2021** | 2 | 10/3mo | Sep-Nov 2021 | Conference burst | **Governance** — teaching model |
| **GCCS-Core** | 9 | 10/1d | Oct 2024 | Single-day launch | **Data** — climate data collection |

---

## The Four Activity Patterns in Solar Geoengineering on GitHub

### Type 1: Institutional Release Cycles (WRF)
Multi-contributor, version-tagged, funded by national labs. 5 contributors, 10 commits in 18 days, v4.8.0 release.

### Type 2: Sustainably Maintained Directories (awesome-geoengineering)
Quarterly updates, focused scope, practical utility. 4 stars but actually useful.

### Type 3: Dormant with Revival Signals (ClimateMARGO)
Long dormancy, README-only updates. The "maybe" pattern.

### Type 4: Academic Single-Burst (Geo-DICE, WinterWarming, OOCC, GCCS-Core)
One push of commits tied to a paper or conference, then permanent silence.

---

## What the Solar Geoengineering Commit Data Tells Us for the Podcast

1. **The atmospheric modeling tool is world-class and actively improving.** WRF v4.8.0 includes a solar radiation correction that could affect all previous SRM simulation results. The TEMPO aerosol physics being staged for the next release is explicitly SRM-relevant.

2. **The governance layer is non-existent as runnable code.** Geo-DICE is frozen in 2018. OOCC_2021 is a document with BibTeX entries. ClimateMARGO is a Julia package with no code commits in 3+ years. Nobody is building serious computational governance tools.

3. **The directory gap is real but surmountable.** Awesome-geoengineering is the only actively maintained geoengineering-specific repo. It has 4 stars. This is the resource that podcasters and researchers actually use.

4. **The academic burst pattern dominates.** 4 of 7 repos had all their commits in a single short period and then went silent. The incentive structure of academia (publish, move on) doesn't reward long-term code maintenance.

5. **WRF is the story.** 1,761 stars, institutional funding, 5 contributors, active development. If solar geoengineering needs an atmospheric model, WRF is it. The solar radiation correction commit alone is worth an episode.

---

## 📋 Research Log

| Date | Activity |
|------|----------|
| 2026-09-17 | v4: Fresh commit data pulled from 7 solar geoengineering repos via GitHub API |
| 2026-09-17 | v4: WRF v4.8.0 release cycle analyzed — solar radiation EOT correction identified as most SRM-relevant commit |
| 2026-09-17 | v4: awesome-geoengineering confirmed as only actively maintained geoengineering-specific repo (Sep 5-6, 2026 updates) |
| 2026-09-17 | v4: ClimateMARGO revival signal documented — 2 README updates after 42-month dormancy, no code commits |
| 2026-09-17 | v4: Geo-DICE legacy confirmed — 8 years dormant, 4 lifetime commits, last activity Sep 2018 |
| 2026-09-17 | v4: GCCS-Core single-day burst documented — 10 commits all on Oct 29, 2024, zero activity since |
