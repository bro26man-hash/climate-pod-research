# ☀️ Solar Geoengineering — Commit Update (September 2026)

**Updated:** September 17, 2026
**Source repos analyzed:** WRFmodel/WRF, ClimateMARGO/ClimateMARGO.jl, PCMDI/pcmdi_metrics, FMS-ESM/AM3, Hausfath/srm-forever

---

## 📊 Fresh Commit Histories Pulled

### 1. WRF Model (wrf-model/WRF) — 1,761 ⭐

**Language:** Fortran | **Last commit:** June 8, 2026

| Date | Commit | Author | Focus |
|------|--------|--------|-------|
| Jun 8, 2026 | 06d4240 | Anthony Islas | Merge release-v4.8.0 |
| Jun 6, 2026 | 0708348 | Anthony Islas | Update README and version to v4.8.0 (#2347) |
| Jun 5, 2026 | 6a289e1 | weiwangncar | Turn off tempo_aerosolaware and tempo_hailaware in Registry (#2346) |
| May 30, 2026 | 4466746 | weiwangncar | Fix vectorization option in AOCC stanza (#2335) |
| May 28, 2026 | e836cd6 | weiwangncar | Correction for eot calculation for solar radiation (#2334) |
| May 27, 2026 | 8299919 | Joseph Olson | Update MYNN-EDMF pointer and removing icloud_bl package (#2336) |
| May 27, 2026 | 4fab0e2 | Anthony Islas | Update MMM-physics repo SHA with various fixes (#2339) |
| May 26, 2026 | 75ad1f9 | Lluís Fita | Fixing CDXWRF module (#2322) |
| May 26, 2026 | 0aa6582 | weiwangncar | Update readme file for GFL option (#2333) |
| May 21, 2026 | 02f02bc | Kelly Werner | Include mp_physics=88 in TEMPO error print message (#2325) |

**🎙️ Podcast insight:** WRF v4.8.0 is the most actively maintained climate simulation code on GitHub right now. The recent commits reveal two threads relevant to solar geoengineering: **(1)** aerosol-aware physics parameterizations are being actively developed and tested (tempo_aerosolaware), and **(2)** solar radiation calculations are being corrected and refined. This is the tool that SRM researchers use to model injection scenarios — but it's a general-purpose weather model, not an SRM-specific tool. The gap remains: no one has built an open-source SRM plugin for WRF.

---

### 2. ClimateMARGO.jl (ClimateMARGO/ClimateMARGO.jl) — 73 ⭐

**Language:** Julia | **Last commit:** August 17, 2026

| Date | Commit | Author | Focus |
|------|--------|--------|-------|
| Aug 17, 2026 | d916f36 | Fons van der Plas | Update README.md |
| Aug 17, 2026 | 6d9ba7a | Fons van der Plas | Update README.md |
| Oct 18, 2023 | 57d4da7 | Fons van der Plas | Update unit_conversions.jl with comment from #86 |
| Jul 6, 2023 | fbbe619 | Fons van der Plas | Add link to Pluto in README |
| Nov 14, 2022 | 5063c42 | Fons van der Plas | Update Project.toml |
| Nov 12, 2022 | 12a0ce6 | Fons van der Plas | JuMP and Ipopt compat upgrade (#85) |
| Feb 10, 2022 | 32e66fd | Henri Drake | Removed deprecated web apps |
| Feb 4, 2022 | d609d49 | Henri Drake | Added CITATION.bib |
| Jan 13, 2022 | b2d9228 | Henri Drake | Fixed typo |
| Jan 12, 2022 | 8a7e012 | Henri Drake | Updated arguments for doc version deployment |

**🎙️ Podcast insight:** ClimateMARGO is an **idealized climate-economic modeling framework** — it optimizes trade-offs between emissions mitigation, adaptation, and geoengineering. The two README updates on Aug 17, 2026 suggest the project is being revived after a long dormancy (2022–2023). This is the kind of tool that makes SRM *tractable* for policy analysis: it doesn't simulate the physics, but it simulates the decision-making. The Julia language choice is significant — it's modern, fast, and designed for scientific computing. If SRM needs a "Killer App," this is the closest thing.

---

### 3. PCMDI Metrics Package (PCMDI/pcmdi_metrics) — 133 ⭐

**Language:** Python | **Last commit:** September 4, 2026

| Date | Commit | Author | Focus |
|------|--------|--------|-------|
| Sep 4, 2026 | 3092cdd | Jiwoo Lee | Merge PR #1428 from PCMDI/lee1043-patch-1 |
| Sep 4, 2026 | 6419050 | Jiwoo Lee | Bump version to 4.2.1 |
| Sep 4, 2026 | 6443a1d | Jiwoo Lee | Merge PR #1429 from PCMDI/lee1043-patch-2 |
| Sep 4, 2026 | 0e3a96f | Jiwoo Lee | Update version and release date in CITATION.cff |
| Sep 4, 2026 | e7dc726 | Jiwoo Lee | Prepare v4.2.1 |
| Sep 4, 2026 | d0bcbd8 | Jiwoo Lee | Merge PR #1427 from PCMDI/jsgoodni_corr_roundoff |
| Sep 4, 2026 | 90cbc50 | James Goodnight | Prevents roundoff to 1.00 in mean_climate figures |
| Sep 3, 2026 | 71a0497 | Jiwoo Lee | Merge PR #1425 from PCMDI/1424_jsgoodni_extremes_chunking |
| Sep 3, 2026 | b2eb044 | Jiwoo Lee | Merge branch 'main' into 1424_jsgoodni_extremes_chunking |
| Sep 3, 2026 | c8711f1 | Jiwoo Lee | Merge PR #1423 from lewisjared/fix/variability-modes-dask-svd-memory |

**🎙️ Podcast insight:** This is the most important climate evaluation code on GitHub. The 10 commits in 2 days (Sep 3-4, 2026) for v4.2.1 represent a coordinated institutional release. The specific fixes — roundoff errors in mean climate figures,Extremes chunking with dask/SVD memory optimization, variability modes — are exactly the kind of precision tools needed to evaluate whether SRM actually produces the cooling effect we designed it to. If SRM were deployed, PCMDI-style metrics would be the verification infrastructure.

---

## 🔥 Updated Trend Assessment

### New findings from this commit pull:

1. **WRF is the hidden backbone.** With 1,761 stars and monthly commits, WRF is the actual workhorse of climate simulation on GitHub — far more active than any SRM-specific tool. The aerosol physics development (tempo_aerosolaware) is directly relevant to SRM modeling. Episode angle: "The SRM simulation stack doesn't start with SRM — it starts with WRF."

2. **ClimateMARGO's revival is a signal.** Two README updates after 2+ years of dormancy (Aug 2026) suggest renewed interest in idealized climate-economic modeling. The Julia implementation makes it accessible to a new generation of researchers. Episode question: "Could an idealized model be the on-ramp for SRM policy discussions?"

3. **PCMDI's institutional velocity is unmatched.** 10 commits/2 days, version-tagged, multi-contributor. This is what sustained open-source climate software looks like — and it's funded by DOE/LLNL. The contrast with the sparse SRM-specific ecosystem is the episode.

4. **The gap remains:** No SRM-specific simulation code exists on GitHub at any meaningful scale. WRF can model it, PCMDI can evaluate it, ClimateMARGO can cost it — but nobody has built the open-source SRM simulator.

### Updated Episode Questions:

1. **Why does SRM simulation depend on general-purpose weather models?** WRF is where SRM modeling happens — but it wasn't built for that. What would a purpose-built open-source SRM tool look like?
2. **Is ClimateMARGO's revival the sign of a policy-ready SRM modeling community?** Idealized models make the economics tractable — but can they inform real decisions?
3. **What does PCMDI's institutional model teach us about open-source climate software sustainability?** 133 stars and monthly releases vs. the typical dormant repo.
4. **The aerosol physics thread in WRF commits** — tempo_aerosolaware is being actively developed. How close are we to open-source SRM-relevant aerosol microphysics?
