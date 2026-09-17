# ☀️ Solar Geoengineering — Commit Trend Analysis

## Detailed commit histories from key repositories

---

## WRF Model: Institutional Pulse (May–Jun 2026)

| Date | Commit | Author | Theme |
|------|--------|--------|-------|
| Jun 8 | Merge release-v4.8.0 | Anthony Islas | Release |
| Jun 6 | Update README and version to v4.8.0 | Anthony Islas | Release |
| Jun 5 | Turn off tempo_aerosolaware and tempo_hailaware | weiwangncar | Physics config |
| May 30 | Fix vectorization option in AOCC stanza | weiwangncar | Build system |
| May 28 | Correction for eot calculation for solar radiation | weiwangncar | **SRM-relevant physics fix** |
| May 27 | MYNN-EDMF pointer update, remove icloud_bl | Joseph Olson | Physics |
| May 27 | Update MMM-physics repo SHA | Anthony Islas | Submodule |
| May 26 | Fixing CDXWRF module | Lluís Fita | Bug fix |
| May 26 | Update readme for GFL option | weiwangncar | Docs |
| May 21 | Include mp_physics=88 in TEMPO error print | Kelly Werner | Error handling |
| May 20 | Minor Tempo changes | AndersJensen-NOAA | Physics |
| May 20 | Fix scheme-guard bug in urban NbS | Chenghao Wang | Bug fix |
| May 20 | Add namelists for ShinHong PBL | weiwangncar | Physics |
| May 19 | Bug fix for udm | weiwangncar | Bug fix |
| May 12 | Updating MYNN-SFC submodule | Joseph Olson | Physics |

**Pattern:** 15 commits in ~4 weeks. Overwhelmingly institutional (NCAR/NOAA). The May 28 solar radiation eot fix is directly relevant to SRM simulation accuracy. TEMPO (Tropospheric Emissions: Monitoring of Pollution) is being integrated — this is the air Quality monitoring side of the same atmospheric modeling coin.

---

## PCMDI Metrics: The 3-Day Blitz (Sep 2-4, 2026)

| Date | Commit | Author |
|------|--------|--------|
| Sep 4 | Merge PR #1428 (bump to 4.2.1) | Jiwoo Lee |
| Sep 4 | Bump version to 4.2.1 | Jiwoo Lee |
| Sep 4 | Merge PR #1429 (patch-2) | Jiwoo Lee |
| Sep 4 | Update version and release date in CITATION.cff | Jiwoo Lee |
| Sep 4 | Prepare v4.2.1 | Jiwoo Lee |
| Sep 4 | Merge PR #1427 (roundoff fix) | Jiwoo Lee |
| Sep 4 | prevents roundoff to 1.00 in mean_climate | James Goodnight |
| Sep 3 | Merge PR #1425 (extremes chunking) | Jiwoo Lee |
| Sep 3 | Merge branch 'main' into extremes_chunking | Jiwoo Lee |
| Sep 3 | Merge PR #1423 (dask SVD memory fix) | Jiwoo Lee |
| Sep 3 | rechunk data for rolling operation | James Goodnight |
| Sep 3 | chore: rename | Jared Lewis |
| Sep 3 | fix: force numpy svd | Jared Lewis |
| Sep 2 | Merge PR #1422 (AIMIP page) | Jiwoo Lee |
| Sep 2 | Update index.rst | Kristin Chang |

**Pattern:** 15 commits in 3 days. Entirely focused on v4.2.1 release. Quality of life and bug fixes (roundoff, memory, SVD). This is how institutional software ships: intense bursts, then quiet.

---

## ClimateMARGO: The 2.5-Year Nap (Oct 2023 → Aug 2026)

| Date | Commit | Author |
|------|--------|--------|
| Aug 17, 2026 | Update README.md | Fons van der Plas |
| Aug 17, 2026 | Update README.md | Fons van der Plas |
| Oct 18, 2023 | Update unit_conversions.jl | Fons van der Plas |
| Jul 6, 2023 | Add Pluto link | Fons van der Plas |
| Nov 14, 2022 | Update Project.toml | Fons van der Plas |
| Nov 12, 2022 | JuMP and Ipopt compat upgrade | Fons van der Plas |
| Feb 10, 2022 | Removed deprecated web apps | Henri Drake |
| Feb 4, 2022 | Added CITATION.bib | Henri Drake |
| Jan 13, 2022 | Fixed typo | Henri Drake |
| Jan 12, 2022 | Updated doc version deployment | Henri Drake |
| Jan 12, 2022 | Added documenter key | Henri Drake |
| Jan 12, 2022 | Updated README.md | Henri Drake |
| Jan 12, 2022 | Bump version | Henri Drake |
| Jan 12, 2022 | Update documentation | Henri Drake |
| Jan 12, 2022 | Update documentation | Henri Drake |

**Pattern:** Dense activity Jan-Feb 2022 (12 commits). Then silence until Oct 2023 (1 commit). Then **2 README updates on the same day in Aug 2026**. The revival is real but minimal — just documentation, no code changes.

---

## Awesome Geoengineering: Steady Curation (2025-2026)

| Date | Commit | Author |
|------|--------|--------|
| Sep 6, 2026 | Update README.md | Brandon Himpfen |
| Sep 5, 2026 | Update README.md | Brandon Himpfen |
| May 5, 2026 | Update to v2.0.0 | Brandon Himpfen |
| Mar 12, 2026 | Update README.md | Brandon Himpfen |
| Jan 16, 2026 | Update README.md | Brandon Himpfen |
| Jun 28, 2025 | Update README.md | Brandon Himpfen |
| Jun 28, 2025 | Initial commit | Brandon Himpfen |

**Pattern:** One person, steady curation. 7 commits over 14 months. This is the healthiest activity pattern of any repo in the solar geoengineering space — consistent, though small.

---

## Cross-Cutting Trend: The Governance Gap

| Repo | Stars | Last Code Commit | Last Activity | Gap |
|------|-------|-------------------|---------------|-----|
| OOCC_2021 | 2 | Unknown (low activity) | 2021 | Governance model from 2021, never updated |
| Geo-DICE | 2 | Unknown | Unknown | Modified DICE with geo, minimal maintenance |
| srm-forever | 0 | Unknown | Aug 2026 | Economics model, no code history visible |
| orbital-climate-simulator | 2 | Sep 2026 | Sep 2026 | **Newest and most active governance-adjacent tool** |

**The story:** The physics simulation tools (WRF, PCMDI) are well-funded and actively maintained. The governance tools are either frozen in 2021 or brand-new and untested. This asymmetry is the defining feature of solar geoengineering on GitHub.
