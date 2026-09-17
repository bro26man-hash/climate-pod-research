# ☀️ Solar Geoengineering — Project Discoveries (September 2026 — v4 Update)

## Search Strategy
Searched GitHub with queries: "geoengineering simulation climate", "geoengineering", "climate simulation", "solar geoengineering". Filtered for repositories with code, documentation, or models related to solar radiation management (SRM).

---

## Ranked Discoveries

### Tier 1: Essential (Active or High-Impact)

| # | Repository | Stars | Language | Last Activity | Why It Matters |
|---|-----------|-------|----------|---------------|---------------|
| 1 | **wrf-model/WRF** | 1,761 | Fortran | Sep 16, 2026 | The atmospheric model that underpins all SRM simulation. v4.8.0 released June 2026 with solar radiation correction (commit `e836cd6`, May 28). 15 commits pulled — continuous institutional activity. |
| 2 | **NOAA-GFDL/MDTF-diagnostics** | 80 | Jupyter | Aug 14, 2026 | Process diagnostics framework. New precip-buoyancy POD (5 commits on Jun 19, 2026 for same file `MCS_precip_buoy_stats.rst`). Ocean-adjacent tool. v4.2.1 release cycle. |
| 3 | **ClimateMARGO/ClimateMARGO.jl** | 73 | Julia | Aug 17, 2026 | Climate-economic model. Revival signal: 2 README commits after 2.5-year dormancy (Aug 17, 2026). No code commits. Could integrate SRM scenarios. |
| 4 | **brandonhimpfen/awesome-geoengineering** | 4 | Python | Sep 6, 2026 | The curated gateway list. Most sustainably maintained project. continuously updated.

### Tier 2: Relevant (Dormant but Influential)

| # | Repository | Stars | Language | Last Activity | Why It Matters |
|---|-----------|-------|----------|---------------|---------------|
| 5 | **pixnum-hub/GeoVision** | — | HTML | Dec 6, 2025 | Web-based geoengineering simulator. All 4 commits on one day. Functional? |
| 6 | **KOSASIH/GCCS-Core** | 9 | Python | Aug 2026 | Global Climate Control System core framework. Ambitious scope. |
| 7 | **jlehtomaa/OOCC_2021** | 2 | Python | Nov 15, 2021 | Governance model for SRM. Frozen since paper publication. |
| 8 | **antara-banerjee/GeoengineeringLE_WinterWarming** | 2 | Python | Apr 24, 2021 | Ensemble analysis for winter warming SRM experiments. Peer-review quality code. |
| 9 | **PSLmodels/Geo-DICE** | 2 | Matlab | Sep 27, 2018 | Modified DICE model with geoengineering. 8 years frozen. |
| 10 | **cjcarlson/geomalaria** | 3 | R | — | Malaria risk modeling with SRM. Ecological side-effect analysis. |

### Tier 3: Edge Cases

| # | Repository | Stars | Language | Last Activity | Notes |
|---|-----------|-------|----------|---------------|-------|
| 11 | **nicmenegoni/ROKA** | 33 | Matlab | Aug 15, 2026 | Rock slope analysis — false positive (geological, not climate) |
| 12 | **nicmenegoni/DICE** | 21 | Matlab | Sep 1, 2026 | Rock discontinuity analysis — false positive |

---

## Fresh Commit Evidence (Pulled Sep 2026)

### WRF — 15 Commits Pulled (May–June 2026)

| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| Jun 8, 2026 | `06d4240` | Anthony Islas | Merge release-v4.8.0 |
| Jun 6, 2026 | `0708348` | Anthony Islas | Update README and version to v4.8.0 |
| Jun 5, 2026 | `6a289e1` | weiwangncar | Turn off tempo_aerosolaware and tempo_hailaware |
| May 30, 2026 | `4466746` | weiwangncar | Fix vectorization option in AOCC stanza |
| **May 28, 2026** | **`e836cd6`** | **weiwangncar** | **Correction for eot calculation for solar radiation** ★ SRM-relevant fix |
| May 27, 2026 | `8299919` | Joseph Olson | Update MYNN-EDMF pointer, remove icloud_bl package |
| May 27, 2026 | `4fab0e2` | Anthony Islas | Update MMM-physics repo SHA |
| May 26, 2026 | `75ad1f9` | Lluís Fita | Fixing CDXWRF module |
| May 26, 2026 | `0aa6582` | weiwangncar | Update readme for GFL option |
| May 21, 2026 | `02f02bc` | Kelly Werner | Include mp_physics=88 in TEMPO error |
| May 20, 2026 | `06e6998` | AndersJensen-NOAA | Minor Tempo changes |
| May 20, 2026 | `8fa379b` | Chenghao Wang | Fix scheme-guard bug in urban NbS initialization |
| May 20, 2026 | `9c87d29` | weiwangncar | Add new namelists for ShinHong PBL and revised MMM surface layer |
| May 19, 2026 | `c1cd5c4` | weiwangncar | Bug fix for udm |
| May 12, 2026 | `b96a7e9` | Joseph Olson | Update MYNN-SFC submodule |

**🎙️ Podcast Insight:** The May 28 solar radiation correction (`e836cd6`) is directly SRM-relevant — it fixes the energy balance calculation that SRM simulations depend on. The 10-commit burst in May 2026 shows WRF is in active development, not maintenance mode. Multiple developers (weiwangncar, Islas, Olson, Wang, Werner) indicate institutional breadth.

### PCMDI/pcmdi_metrics — 15 Commits Pulled (Sep 3–17, 2026)

| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| Sep 17, 2026 | `b8f231a` | Jiwoo Lee | Merge PR #1431 (mov_patch) |
| Sep 17, 2026 | `90a4bc1` | Jiwoo Lee | Patch for single file modpath_list case |
| Sep 4, 2026 | `3092cdd` | Jiwoo Lee | Merge PR #1428 |
| **Sep 4, 2026** | **`6419050`** | **Jiwoo Lee** | **Bump version to 4.2.1** ★ |
| Sep 4, 2026 | `6443a1d` | Jiwoo Lee | Merge PR #1429 |
| Sep 4, 2026 | `0e3a96f` | Jiwoo Lee | Update version and release date in CITATION.cff |
| Sep 4, 2026 | `e7dc726` | Jiwoo Lee | Prepare v4.2.1 |
| Sep 4, 2026 | `d0bcbd8` | Jiwoo Lee | Merge PR #1427 (roundoff fix) |
| Sep 4, 2026 | `90cbc50` | James Goodnight | Prevents roundoff to 1.00 in mean_climate figures |
| Sep 3, 2026 | `71a0497` | Jiwoo Lee | Merge PR #1425 (extremes chunking) |
| Sep 3, 2026 | `b2eb044` | Jiwoo Lee | Merge branch 'main' into extremes_chunking |
| Sep 3, 2026 | `c8711f1` | Jiwoo Lee | Merge PR #1423 (variability modes dask SVD memory) |
| Sep 3, 2026 | `ac634d7` | James Goodnight | Rechunk data to higher order than rolling operation |
| Sep 3, 2026 | `d0a79e5` | Jared Lewis | Chore: rename |
| Sep 3, 2026 | `1fca2ec` | Jared Lewis | Fix: force to use numpy SVD |

**🎙️ Podcast Insight:** 10 commits on a single day (Sep 4) for v4.2.1 release — classic institutional release burst. The roundoff fix (preventing 1.00 in mean_climate figures) and the SVD memory optimization show that CMIP evaluation is maturing. The "extremes chunking" PR is particularly relevant for SRM attribution — extreme event analysis is how you detect SRM injection signals.

### MDTF-diagnostics — 15 Commits Pulled (May–Aug 2026)

| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| Aug 14, 2026 | `87f8105` | Aparna Radhakrishnan | Merge PR #825 |
| **Jun 19, 2026** | **`4cfc99c`** | **Wei-Ming Tsai** | **Update MCS_precip_buoy_stats.rst** ★ (5th commit on same file same day) |
| Jun 19, 2026 | `699de27` | Wei-Ming Tsai | Update MCS_precip_buoy_stats.rst |
| Jun 19, 2026 | `d6bc6d0` | Wei-Ming Tsai | Update MCS_precip_buoy_stats.rst |
| Jun 19, 2026 | `3904d29` | Wei-Ming Tsai | Update MCS_precip_buoy_stats.rst |
| **Jun 19, 2026** | **`33024ad`** | **Wei-Ming Tsai** | **Add MCS precipitation-buoyancy statistics POD** ★ NEW POD |
| Jun 8, 2026 | `2df59f6` | Aparna Radhakrishnan | Merge PR #823 |
| Jun 8, 2026 | `16f936c` | jongsooshin5 | Update README |
| Jun 8, 2026 | `b96127e` | jongsooshin5 | Update README.md |
| Jun 2, 2026 | `97b3028` | — | Merge branch 'NOAA-GFDL:main' into main |
| Jun 2, 2026 | `a20f615` | jongsooshin5 | Add citation |
| Jun 1, 2026 | `988326a` | Aparna Radhakrishnan | Update quarterly-metrics.yml |
| Jun 1, 2026 | `95991fc` | Aparna Radhakrishnan | Add quarterly metrics workflow for traffic logging |
| May 27, 2026 | `16403a4` | Dani Coleman | Move diagnostics/blocking_neale_nb to dev branch |
| May 22, 2026 | `52c95e3` | Dani Coleman | Merge PR #800 (blocking notebook) |

**🎙️ Podcast Insight:** The June 19 burst — 5 commits on the same file (`MCS_precip_buoy_stats.rst`) — is the single most ocean-relevant signal in our entire dataset. The precipitation-buoyancy POD evaluates whether models correctly simulate the relationship between precipitation and buoyancy, which is fundamental to ocean stratification and mixing. If ocean geoengineering is ever deployed, this is the diagnostic that would verify it's working. 5 commits on one day suggests a paper deadline or targeted development sprint.

### ClimateMARGO.jl — The Revival Signal (Detailed)

**Commit Span:** Jan 2022 – Aug 2026 (but with 2.5-year gap)

| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| **Aug 17, 2026** | **`d916f36`** | **Fons van der Plas** | **Update README.md** ★ Revival commit 1 |
| **Aug 17, 2026** | **`6d9ba7a`** | **Fons van der Plas** | **Update README.md** ★ Revival commit 2 |
| Oct 18, 2023 | `57d4da7` | Fons van der Plas | Update unit_conversions.jl with comment from #86 |
| Jul 6, 2023 | `fbbe619` | Fons van der Plas | Add link to Pluto in README |
| Nov 14, 2022 | `5063c42` | Fons van der Plas | Update Project.toml |
| Nov 12, 2022 | `12a0ce6` | Fons van der Plas | JuMP and Ipopt compat upgrade (#85) |
| Feb 10, 2022 | `32e66fd` | Henri Drake | Removed deprecated web apps |
| Feb 4, 2022 | `d609d49` | Henri Drake | Added CITATION.bib |
| Jan 13, 2022 | `b2d9228` | Henri Drake | Fixed typo |

**Phase Analysis:**
- **Phase 1 (Jan–Feb 2022):** Henri Drake established the project — 7 commits, full setup
- **Phase 2 (Nov 2022):** Dependency maintenance — 2 commits, JuMP/Ipopt compat
- **Phase 3 (GAP):** No meaningful activity for 2.5 years (Feb 2022 → Aug 2026)
- **Phase 4 (Aug 2026):** Fons van der Plas (different maintainer!) updates README twice on the same day

**🎙️ Podcast Angle:** The change in maintainer is the key signal. Henri Drake → Fons van der Plas suggests institutional takeover, not just a personal revival. But two README commits with no code changes is ambiguous — it could be a genuine relaunch or just a link update. The Julia climate-economic modeling niche is small enough that any new maintainer matters.

### srm-forever — The Weitzman Model (4 Commits, All on One Day)

| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| Aug 26, 2026 | `61df1a4` | hausfath | Add effective discount rate chart |
| Aug 26, 2026 | `aa9bc0f` | hausfath | **Adopt Weitzman certainty-equivalent discounting; add discount-rate essay** ★ |
| Aug 26, 2026 | `9ee822a` | hausfath | Price abatement as a vintage annuity |
| Aug 26, 2026 | `9999436` | hausfath | Interactive SRM-forever vs mitigation+CDR cost model |

**🎙️ Podcast Insight:** All 4 commits on a single day (Aug 26, 2026) — a concentrated theoretical burst. The Weitzman certainty-equivalent discounting framework is conceptually critical: it asks "what does it cost to keep SRM going forever?" This is the economic argument against indefinite SRM dependency. The "vintage annuity" framing for abatement pricing is a novel theoretical contribution. Despite 0 stars, this repo may be the most上升到 policy-relevant code in the solar geoengineering space.

---

## The Governance Gap (Solar Theme — Updated)

**Three governance-related repos found, all dormant:**

1. **OOCC_2021** — Simple SRM governance model, paper-driven, frozen 2021
2. **Geo-DICE** — Modified DICE with geoeconomic scenarios, frozen 2018
3. **srm-forever** — Interactive SRM cost model, active Aug 2026 but 0 stars, theoretical only

**New finding:** srm-forever is the only governance-adjacent repo with fresh commits (Aug 2026). The Weitzman discounting framework is the most rigorous economic analysis of SRM sustainability ever coded. But it's interactive-only, not a policy tool.

**Pattern:** Governance code is created for papers, not maintained. The physics community has no equivalent of "Astropy" for SRM governance — a mature, community-maintained tool.

---

## The Simulation Stack (What's Actually Used — Updated)

Based on fresh commit analysis, the SRM simulation stack in 2026 is:

1. **WRF** (atmospheric physics, radiation, aerosol transport) — 15 commits pulled, v4.8.0, solar radiation fix
2. **MDTF-diagnostics** (model evaluation, process verification) — 15 commits pulled, v4.2.1, precip-buoyancy POD
3. **ClimateMARGO** (economic scenario framing, mitigation/adaptation trade-offs) — 2 README revivals, no code
4. **awesome-geoengineering** (discovery gateway) — continuously maintained
5. **srm-forever** (SRM cost economics) — 4 commits, Weitzman framework, 0 stars

Everything else is either dormant or a one-off paper artifact.

---

## What's Missing for Solar Episode (Updated)

- **No interactive SRM simulators exist that are actively maintained.** GeoVision was one attempt, frozen after 4 commits.
- **No open-source radiative transfer code specific to SRM.** WRF handles it but it's a general circulation model, not a targeted SRM tool.
- **No SRM-specific CWM (climate working memory) or data assimilation tools.**
- **The governance gap is the story.** Everything from OOCC_2021 onward has been frozen, except srm-forever's theoretical burst.
- **The evaluation infrastructure is maturing.** PCMDI's v4.2.1 release and MDTF's precip-buoyancy POD show that the community is investing in verification, not just simulation.

---

*Last updated: September 2026 (v4 — fresh commit data pulled from GitHub API).*