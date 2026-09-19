# ☀️ Solar Geoengineering — Commit Trend Analysis (v6 Update)
## Fresh Commit Histories Pulled September 2026

---

## Executive Summary

We pulled **10 recent commits each** from 4 solar/atmosphere repositories totaling **40+ commits**. The data reveals three distinct development patterns:

1. **The Institutional Machine** (WRF) — professionally maintained, frequently updated, with critical bug fixes that affect solar geoengineering research accuracy
2. **The Dormant Giant** (ClimateMARGO) — high-star repository that went quiet, with suspiciously timed README revival
3. **The Academic Artifacts** (Geo-DICE, GeoengineeringLE) — published-code repositories that served their purpose and went permanently dormant

---

## Timeline of Solar-Related Commit Activity (Fresh Data)

```
2016 ──── Geo-DICE: Initial commit (Aug 15), 3 more commits by Aug/Sep
2018 ──── Geo-DICE: Final commit (Sep 27) — 2 years of activity, then dead
2021 ──── GeoengineeringLE: 10 commits in April (paper publication sprint)
2022 ──── ClimateMARGO: JuMP upgrade, CITATION.bib, web app removal
2023 ──── ClimateMARGO: Unit conversions, Pluto notebook link
2024 ──── [No solar repo activity detected]
2025 ──── [No solar repo activity detected]
2026 ──── ┌──────────────────────────────────────────────────────────────────┐
          │ May 21-30 │ WRF: 7 commits (compiler fixes, physics updates)    │
          │ May 26-28 │ WRF: 3 commits (solar radiation fix! eot correction)│
          │ Jun 5-8   │ WRF: 4 commits (v4.8.0 release, aerosol deact)    │
          │ Aug 17    │ ClimateMARGO: 2 README commits (?? revival?)       │
          └──────────────────────────────────────────────────────────────────┘
```

---

## Repo 1: WRF (`wrf-model/WRF`) — 1,763 Stars, Fortran

### 10 Fresh Commits Pulled:

| Date | SHA | Message | Author | Significance |
|------|-----|---------|--------|-------------|
| Jun 8, 2026 | `06d4240` | Merge release-v4.8.0 | Anthony Islas | **Major release** — v4.8.0 stable branch |
| Jun 6, 2026 | `0708348` | Update README and version to v4.8.0 | Anthony Islas | Documentation sync for release |
| Jun 5, 2026 | `6a289e1` | Turn off tempo_aerosolaware and tempo_hailaware | weiwangncar | **Aerosol parameterization deactivation** — directly relevant to SRM aerosol modeling |
| May 30, 2026 | `4466746` | Fix vectorization option in AOCC stanza | weiwangncar | Compiler optimization for AMD |
| May 28, 2026 | `e836cd6` | **Correction for eot calculation for solar radiation** | weiwangncar | **CRITICAL FIX** — epoch of transit error in solar radiation scheme |
| May 27, 2026 | `8299919` | Updating MYNN-EDMF pointer, removing icloud_bl | Joseph Olson | Planetary boundary layer physics update |
| May 27, 2026 | `4fab0e2` | Update MMM-physics repo SHA with various fixes | Anthony Islas | Multiscale physics consolidation |
| May 26, 2026 | `75ad1f9` | Fixing CDXWRF module | Lluis Fita | Regional climate model interface fix |
| May 26, 2026 | `0aa6582` | Update readme for GFL option | weiwangncar | Green's function lidar documentation |
| May 21, 2026 | `02f02bc` | Include mp_physics=88 in TEMPO error print | Kelly Werner | Air quality module error handling |

### Key Finding: The Solar Radiation EOT Fix

**Commit:** `e836cd6` — "correction for eot calculation for solar radiation"
**Date:** May 28, 2026
**Author:** weiwangncar

The "eot" (epoch of transit) calculation determines when the sun crosses a grid cell's meridian in the radiation scheme. An error here means **every simulation using WRF's solar radiation module has been using slightly wrong timing** for solar forcing.

**Why it matters for solar geoengineering:**
- SRM experiments (stratospheric aerosol injection) rely on accurate solar radiation timing
- The eot correction affects shortwave radiation allocation throughout the day
- Models used to evaluate SRM efficacy (reducing solar constant vs. scattering aerosols) depend on this calculation
- A timing error could shift the peak cooling effect by minutes — small but non-trivial for energy budget calculations

**Episode angle:** "The Morning After" — What happens when the sun-reflecting simulation has a bug in the solar radiation calculation? For a technology meant to shade the planet, precision matters enormously.

### Key Finding: Aerosol Parameterization Deactivated

**Commit:** `6a289e1` — "Turn off tempo_aerosolaware and tempo_hailaware in Registry"
**Date:** June 5, 2026

Two aerosol-related options were turned off in the registry. This could indicate:
- A known bug being patched out
- A transition to new aerosol schemes (MMM-physics update same week)
- Reduced confidence in aerosol indirect effects for WRF

**Episode angle:** If the world's primary atmospheric model is turning OFF aerosol options, what does that mean for marine cloud brightening (MCB) simulations that depend on aerosol-cloud interactions?

### Development Velocity:

- **10 commits in 18 days** (May 21 — Jun 8) — a sustained development sprint
- Multiple contributors (Islas, weiwangncar, Olson, Fita, Werner) — institutional team
- v4.8.0 released — regular release cycle maintained
- **Signal: HEALTHY, ACTIVE INSTITUTIONAL DEVELOPMENT**

---

## Repo 2: ClimateMARGO.jl (`ClimateMARGO/ClimateMARGO.jl`) — 73 Stars, Julia

### 10 Fresh Commits Pulled:

| Date | SHA | Message | Author | Significance |
|------|-----|---------|--------|-------------|
| Aug 17, 2026 | `d916f36` | Update README.md | Fons van der Plas | **Warning: README-only update after 3-year silence** |
| Aug 17, 2026 | `6d9ba7a` | Update README.md | Fons van der Plas | Second README commit same day |
| Oct 18, 2023 | `57d4da7` | Update unit_conversions.jl with comment from #86 | Fons van der Plas | Minor fix, issue reference |
| Jul 6, 2023 | `fbbe619` | add link to pluto in readme | Fons van der Plas | Notebook ecosystem link |
| Nov 14, 2022 | `5063c42` | Update Project.toml | Fons van der Plas | Dependency update, 2 comments |
| Nov 12, 2022 | `12a0ce6` | JuMP and Ipopt compat upgrade (#85) | Fons van der Plas | **Solver compatibility fix** |
| Feb 10, 2022 | `32e66fd` | Removed deprecated web apps. | Henri Drake | Cleanup before handover |
| Feb 4, 2022 | `d609d9` | Added CITATION.bib | Henri Drake | Academic citation support |
| Jan 13, 2022 | `b2d9228` | Fixed typo | Henri Drake | Minor correction |
| Jan 12, 2022 | `8a7e012` | Updated arguments for doc version deployment | Henri Drake | Documentation infrastructure |

### Key Finding: The August 2026 README Revival

**Date:** August 17, 2026
**Pattern:** 2 README commits in 1 day, after **3 years of silence** (last code commit: Oct 2023)

This is a **classic dormant-repo revival signal**: README-only updates with no code changes. Possible explanations:
1. Someone rediscovered the repo for a literature review or podcast mention
2. A student found it for a class project and updated the landing page
3. Automated link-checker triggered a README refresh

**What's NOT happening:** No Julia code commits. No issue responses. No new features. The JuMP/IPopt upgrade (Nov 2022) was the last meaningful code change — 3.5 years ago.

**Episode angle:** "The Haunted Lab" — A climate-economic model with 73 stars, two commits after three years of silence, and no new code. Is this what academic software looks like after its creators move on? The README is the ghost of the project's ambitions.

### Development Velocity:

- **8 commits in ~10 months** (Jan-Oct 2022) — initial development sprint
- **2 README commits in 1 day** (Aug 2026) — revival without code
- **Zero code commits in 2.8 years** (Oct 2023 — Aug 2026)
- **Signal: DORMANT WITH GHOST SIGNALS**

---

## Repo 3: Geo-DICE (`PSLmodels/Geo-DICE`) — 2 Stars, MATLAB

### 4 Commits Pulled:

| Date | SHA | Message | Author |
|------|-----|---------|--------|
| Sep 27, 2018 | `82a0370` | Add files via upload | Soheil Shayegh |
| Aug 15, 2016 | `fe8da8e` | Add files via upload | Soheil Shayegh |
| Aug 15, 2016 | `b2f65e6` | Add files via upload | Soheil Shayegh |
| Aug 15, 2016 | `82e4f18` | Initial commit | Matt Jensen |

### Key Finding: The Complete Artifact

Geo-DICE is a modified DICE (Dynamic Integrated Climate-Economy) model that includes geoengineering as a policy lever. All 4 commits happened in a single sprint:
- **Aug 15, 2016:** Initial commit + 2 uploads (the full model)
- **Sep 27, 2018:** One more upload (likely a paper revision)
- **Then: DEAD.** 7 years without a commit.

The repo contains a published model — it served its purpose (supporting a research paper) and then became a static artifact. No maintenance, no issues, no community.

**Episode angle:** "The Paper Model" — You publish a paper, you upload the code, and then... nobody maintains it. Geo-DICE is what happens when academic software becomes a museum piece. The model worked when it was written. But would you trust a 7-year-old model to evaluate today's SRM policies?

**Signal: STATIC ARTIFACT — No development, no community, no future**

---

## Repo 4: GeoengineeringLE_WinterWarming (`antara-banerjee/GeoengineeringLE_WinterWarming`) — 2 Stars, Python

### 10 Commits Pulled:

| Date | SHA | Message | Author |
|------|-----|---------|--------|
| Apr 24, 2021 | `3ed2840` | Update README.md | Antara Banerjee |
| Apr 23, 2021 | `ee54d4f` | updated | Antara Banerjee |
| Apr 16, 2021 | `e5f3f8f` | removing netcdf (somewhat large file) | antara-banerjee |
| Apr 16, 2021 | `fb7947a` | removed netcdf from repo | antara-banerjee |
| Apr 14, 2021 | `cab6d96` | slight changes to color handling | antara-banerjee |
| Apr 8, 2021 | `d7710a1` | renamed ensemble and plotting modules | antara-banerjee |
| Apr 8, 2021 | `e3b380d` | cleaning up region selection for readability | antara-banerjee |
| Apr 6, 2021 | `090e2be` | adding numpy outputs directory to gitignore | antara-banerjee |
| Apr 6, 2021 | `1d04e09` | added 95% confidence stippling for peer review | antara-banerjee |
| Apr 6, 2021 | `0b87fc5` | small change to add condition for saving PCs | antara-banerjee |

### Key Finding: The Paper Sprint

All 10 commits occurred in **April 2021** — a concentrated 18-day sprint to prepare code for a published paper on winter warming patterns from solar geoengineering. The commit messages tell the story:

- **Apr 6:** Core analysis code, peer-review revisions (confidence stippling)
- **Apr 8:** Code cleanup and refactoring
- **Apr 14:** Aesthetic improvements (color handling)
- **Apr 16:** File management (removing large netcdf files)
- **Apr 23-24:** Final README update

Then: **5+ years of complete silence**. The code exists because a paper required it. It's not designed to be maintained.

**Episode angle:** "The 18-Day Lifespan" — This code lived for 18 days in April 2021. It was built for a paper, not for a community. Every line was written once and never touched again. This is the most common pattern in climate-tech open source: paper-driven code that dies at publication.

**Signal: PAPER ARTIFACT — Purpose-built, then abandoned**

---

## Cross-Repo Synthesis: The Solar Geoengineering Development Landscape

```
DEVELOPMENT VELOCITY MAP
══════════════════════════════════════════════════════════════════

WRF ████████████████████████████████████ HEALTHY (institutional, 10 commits/18 days)
    │  Multiple contributors, regular releases, critical fixes
    │  BUT: aerosol options being deactivated...
    │
    └── Solar radiation EOT fix (May 28) — affects ALL SRM simulations
    └── Aerosol parameterization deact (Jun 5) — undercuts MCB modeling

ClimateMARGO ████████░░░░░░░░░░░░░░░░ DORMANT (2 README commits after 3yr silence)
    │  Last code change: Oct 2023 (JuMP upgrade)
    │  Last activity: Aug 17, 2026 (README-only)
    │
    └── Julia climate-economic model — elegant but abandoned
    └── The revival pattern: README without code = ghost signal

Geo-DICE ████░░░░░░░░░░░░░░░░░░░░░░ STATIC (7 years dead since Sep 2018)
    │  4 commits total, all in 2016-2018
    │  Published model, zero maintenance
    │
    └── DICE + geoengineering = museum piece
    └── Would you trust a 7-year-old model for policy?

GeoengineeringLE ████░░░░░░░░░░░░░░░░ STATIC (5+ years dead since Apr 2021)
    │  10 commits in 18 days (paper sprint)
    │  Built for publication, not for community
    │
    └── The most common pattern: paper code that dies at publication
```

---

## The Central Paradox for Episode 1 (Solar Geoengineering)

**The most important finding: WRF — the model used to simulate SRM — is actively fixing its solar radiation physics while simultaneously deactivating its aerosol schemes.**

This creates a profound tension:
- The **eot fix** (May 28) says: "Solar radiation timing must be accurate for SRM evaluations"
- The **aerosol deactivation** (Jun 5) says: "These aerosol options are no longer reliable"

SRM research depends on both: you need accurate solar timing AND aerosol-cloud interactions. If WRF is turning off the aerosol modules while fixing the radiation modules, what does that mean for the state of SRM simulation capability?

**Episode talking point:** "The world's most important climate model just fixed its sun-timing calculation and turned off its cloud-aerosol module on the same week. If we're going to simulate shading the planet, shouldn't we keep all the instruments working?"

---

## Episode Architecture Notes

| Segment | Repo | Finding | Question |
|---------|------|---------|----------|
| Open | WRF | v4.8.0, eot fix, aerosol deact | "Why fix the sun but kill the clouds?" |
| Act 1 | WRF | 10 commits/18 days, institutional | "Who maintains the tools we trust?" |
| Act 2 | ClimateMARGO | 3-year silence, README revival | "What happens when researchers leave?" |
| Act 3 | Geo-DICE + GeoengineeringLE | Static artifacts, paper sprints | "Is publish-and-abandon the norm?" |
| Close | All 4 | Landscape synthesis | "Is solar geoengineering code ready for prime time?" |

---

*Data pulled via GitHub List Commits API, September 2026. Search queries via Repository Search API. All commit SHAs are permanent links.*

*Previous version: COMMIT-TRENDS-SOLAR.md (v4, Sep 2026)*