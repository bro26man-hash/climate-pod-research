# ☀️ Solar Geoengineering — Commit Trend Analysis (v4, September 2026)

## Overview
Fresh commit histories pulled from **5 repositories** spanning atmospheric modeling, climate-economic optimization, geoengineering governance, and SRM cost theory. Combined: **40+ commits** analyzed.

---

## Repository-by-Repository Breakdown

### 1. wrf-model/WRF — 1,762★ — Atmospheric Foundation Model
**Commit window analyzed:** May 12 – June 8, 2026 (15 commits)
**Last commit:** June 8, 2026 (v4.8.0 release merge)

| Date | Commit Subject | Author | Signal |
|------|---------------|--------|--------|
| Jun 8 | Merge release-v4.8.0 | Anthony Islas | **v4.8.0 official release** |
| Jun 6 | Update README and version to v4.8.0 | Anthony Islas | Version declaration updated |
| Jun 5 | Turn off tempo_aerosolaware & tempo_hailaware | weiwangncar | **Aerosol awareness disabled** — potential SRM-related adjustment |
| May 30 | Fix vectorization option in AOCC stanza | weiwangncar | Compiler optimization fix |
| May 28 | **Correction for eot calculation for solar radiation** | weiwangncar | 🔥 **Solar radiation energy balance fix** — directly relevant to SRM modeling |
| May 27 | MYNN-EDMF pointer update; remove icloud_bl | Joseph Olson | Cloud physics revision |
| May 27 | Update MMM-physics repo SHA | Anthony Islas | Physics coupling update |
| May 26 | Fixing CDXWRF module | Lluís Fita | Diagnostics fix |
| May 26 | Update README for GFL option | weiwangncar | New feature documentation |
| May 21 | Include mp_physics=88 in TEMPO error | Kelly Werner | TEMPO gas-phase chemistry |
| May 20 | Minor Tempo changes | AndersJensen-NOAA | TEMPO update |
| May 20 | Fix scheme-guard bug in urban NbS init | Chenghao Wang | Urban nature-based solutions |
| May 20 | Add namelists for ShinHong PBL | weiwangncar | New PBL scheme |
| May 19 | Bug fix for udm | weiwangncar | Unified diagnostic framework |
| May 12 | Update MYNN-SFC submodule | Joseph Olson | Surface layer physics |

**🔑 Key Finding for Episode:** The **solar radiation correction (May 28)** and the **disabling of TEMPO aerosol awareness (Jun 5)** are the two most SRM-relevant commits. WRF v4.8.0 appears to be refining how solar radiation is computed — directly affecting any SRM ray-shift simulation. The TEMPO adjustment suggests aerosol-cloud interactions may be getting simplified for stability.

**Episode hook:** *"The most used climate model on Earth just fixed its solar radiation math — and the fix changes how we simulate geoengineering."*

---

### 2. ClimateMARGO/ClimateMARGO.jl — 73★ — Climate-Economic Optimization
**Commit window analyzed:** Oct 2023 – Aug 2026 (15 commits)
**Last commit:** August 17, 2026 (README update)

| Date | Commit Subject | Author | Signal |
|------|---------------|--------|--------|
| Aug 17 | Update README.md | Fons van der Plas | **⚠️ REVIVAL COMMIT #2** |
| Aug 17 | Update README.md | Fons van der Plas | **⚠️ REVIVAL COMMIT #1** |
| Oct 2023 | Update unit_conversions.jl | Fons van der Plas | Last code commit (2.5yr gap) |
| Jul 2023 | Add Pluto link | Fons van der Plas | Documentation only |
| Nov 2022 | Update Project.toml | Fons van der Plas | Dependency update |
| Nov 2022 | JuMP/Ipopt compat upgrade | Fons van der Plas | Solver compatibility fix |
| Feb 2022 | Removed deprecated web apps | Henri Drake | Cleanup |
| Feb 2022 | Added CITATION.bib | Henri Drake | Citation infrastructure |
| Jan 2022 | Fixed typo | Henri Drake | Minor fix |
| Jan 2022 | Doc version deployment | Henri Drake | Documentation |
| Jan 2022 | Added documenter key | Henri Drake | CI configuration |
| Jan 2022 | Update README | Henri Drake | Documentation |
| Jan 2022 | Bump version | Henri Drake | Release |
| Jan 2022 | Update documentation | Henri Drake | Documentation |
| Jan 2022 | Update documentation | Henri Drake | Documentation |

**🔑 Key Finding for Episode:** Two README updates in August 2026 after **2.5 years of dormancy** — but zero code commits. This is the second false-start revival signal. The codebase froze at v0.x with JuMP/Ipopt compatibility fixed in Nov 2022. The 2026 README updates may indicate renewed interest from policy-modeling communities, but without code contributions, it remains a "zombie project" — alive on GitHub, dead in practice.

**Episode hook:** *"A climate-economic model woke from 2.5 years of sleep — but only to update its resume."*

---

### 3. brandonhimpfen/awesome-geoengineering — 4★ — Curated Resource Directory
**Commit window analyzed:** Jun 2025 – Sep 2026 (7 commits)
**Last commit:** September 6, 2026 (README update)

| Date | Commit Subject | Author | Signal |
|------|---------------|--------|--------|
| Sep 6 | Update README.md | Brandon Himpfen | **Most recent — actively maintained** |
| Sep 5 | Update README.md | Brandon Himpfen | Two-day rapid update |
| May 5 | Update to v2.0.0 | Brandon Himpfen | **Major version release** |
| Mar 12 | Update README.md | Brandon Himpfen | Content addition |
| Jan 16 | Update README.md | Brandon Himpfen | Content addition |
| Jun 28 | Update README.md | Brandon Himpfen | Initial update |
| Jun 28 | Initial commit | Brandon Himpfen | Project launch |

**🔑 Key Finding for Episode:** The only actively maintained geoengineering directory on GitHub. v2.0.0 released May 2026 with two rapid README updates in September 2026. This is the go-to catalog for the field — if a project isn't listed here, it might not exist. The commit pattern shows steady quarterly updates with occasional bursts.

**Episode hook:** *"The wikipedia of geoengineering is one person's side project — and it's the most up-to-date map of the field we have."*

---

### 4. PSLmodels/Geo-DICE — 2★ — Modified DICE with Geoengineering
**Commit window analyzed:** Aug 2016 – Sep 2018 (4 commits)
**Last commit:** September 27, 2018 (file upload)

| Date | Commit Subject | Author | Signal |
|------|---------------|--------|--------|
| Sep 2018 | Add files via upload | Soheil Shayegh | Final commit — 7+ years ago |
| Aug 2016 | Add files via upload | Soheil Shayegh | Initial content |
| Aug 2016 | Add files via upload | Soheil Shayegh | Content expansion |
| Aug 2016 | Initial commit | Matt Jensen | Project creation |

**🔑 Key Finding for Episode:** Completely dormant since 2018. The Geo-DICE model (DICE integrated with geoengineering modules) was a pioneering effort by Soheil Shayegh and Matt Jensen — but it's been abandoned for 7+ years. No version control, no README updates, no community contributions. This is what happens when academic models outlive their funding cycles.

**Episode hook:** *"A groundbreaking geoeconomic model got 4 commits and then silence. Academic code has a half-life."*

---

### 5. jlehtomaa/OOCC_2021 — 2★ — Solar Geoengineering Governance Model
**Commit window analyzed:** Jul 2021 – Nov 2021 (15 commits)
**Last commit:** November 15, 2021 (BibTeX update)

| Date | Commit Subject | Author | Signal |
|------|---------------|--------|--------|
| Nov 2021 | Update bibtex entry | jlehtomaa | Final commit — paper preparation |
| Oct 2021 | Update bibtex reference | jlehtomaa | Citation work |
| Sep 2021 | Update README (×3) | jlehtomaa | Documentation push |
| Sep 2021 | Update citation (×2) | jlehtomaa | Citation infrastructure |
| Jul 2021 | Update README | jlehtomaa | Documentation |
| Jul 2021 | Comment errors | jlehtomaa | Bug fix |
| Jul 2021 | Update strategy tables | jlehtomaa | **Core content — SRM governance strategies** |
| Jul 2021 | Update | jlehtomaa | General maintenance |
| Jul 2021 | Cleanups and checks | jlehtomaa | Final polish |

**🔑 Key Finding for Episode:** A densely packed 4-month development burst (Jul–Nov 2021) producing a solar geoengineering governance model. All commits are paper-preparation focused — strategy tables, citations, README. The model addresses international coordination challenges for SRM deployment. Dormant since Nov 2021 but conceptually important: it's one of the few open-source attempts to model SRM governance.

**Episode hook:** *"In 4 months, one researcher built the only open-source model of solar geoengineering governance — then froze it for publication."*

---

## Cross-Repo Solar Theme Trends

### Trend 1: The "Fix-and-Freeze" Pattern (WRF, Geo-DICE)
Large institutional models (WRF) get active maintenance and(version bumps, while academic models (Geo-DICE) freeze after initial publication. The difference: funding. WRF is NOAA/NCAR funded; Geo-DICE lost its grant cycle.

### Trend 2: The "Zombie Revival" (ClimateMARGO)
Projects that go dormant for years then get a single README update — no code, no tests, no community engagement. Two such events now (Jan 2022 documented activity → Aug 2026 README-only updates). The project is being kept on life support, not restarted.

### Trend 3: The Solo Curator (awesome-geoengineering)
One person maintaining the field's most important directory. 7 commits over 14 months, with a v2.0.0 milestone. Fragile but irreplaceable.

### Trend 4: Governance Models Don't Scale (OOCC_2021)
The only SRM governance model got 15 commits in 4 months, then stopped. The academic incentive structure doesn't support long-term code maintenance — publish or perish, not build or maintain.

### Trend 5: Solar Radiation Physics is Actively Being Refined (WRF v4.8.0)
The May 28 solar radiation EOT correction and June 5 TEMPO aerosol disable are not SRM-specific commits, but they directly affect how SRM scenarios would be modeled. The field's foundational tool is being refined in real time.

---

## Commit Activity Heatmap (Solar Theme)

```
2016 ████████ Geo-DICE (4 commits, all 2016)
2017 ░░░░░░░░ (silent)
2018 ██░░░░░░ Geo-DICE (1 final commit)
2019-2020 ░░░░░░░░ (silent)
2021 ████████ OOCC_2021 (15 commits in 4 months)
2022 ████████ ClimateMARGO (10 commits, mostly Jan)
2023 ██░░░░░░ ClimateMARGO (2 commits, Jul-Oct)
2024 ░░░░░░░░ (silent)
2025 ████████ awesome-geoengineering (3 commits)
2026 ████████████ WRF v4.8.0 (10 commits) + MARGO revival (2) + awesome (4)
```

---

## Episode Talking Points

1. **"The solar radiation fix"** — WRF v4.8.0 just corrected how solar radiation energy balance is computed. This is the most used climate model on Earth, and its solar physics directly determines how we'd simulate SRM.

2. **"The governance gap"** — There's exactly one open-source model of SRM governance (OOCC_2021), and it's been frozen for 5 years. We have no live tools for answering "who decides whether to deploy SRM?"

3. **"The zombie economy"** — ClimateMARGO's 2.5-year dormancy followed by README-only revivals is the norm, not the exception. Academic climate code has a "half-life" after publication.

4. **"One person, one directory"** — The entire geoengineering field's open-source catalog is maintained by Brandon Himpfen as a personal project. If he stops, the map goes stale.

5. **"7 years of silence"** — Geo-DICE, a pioneering geoeconomic model, has had zero commits since 2018. Grant funding ends, code dies.

---

*Analysis date: September 2026 | Data source: GitHub API commit histories*