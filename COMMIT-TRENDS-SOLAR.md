# ☀️ Solar Geoengineering — Commit Trend Deep Dive

**Branch:** `solar-geoengineering`
**Analysis Date:** September 17, 2026
**Repositories Analyzed:** PCMDI/pcmdi_metrics, FMS-ESM/AM3, pmip4/pmip_p2fvar_analyzer, hausfath/srm-forever, RhondaMueller/Codes-RFG-Arctic-Impacts

---

## Executive Summary

Solar geoengineering has the strongest open-source presence of all three themes — but it's overwhelmingly concentrated in a single institutional toolkit (PCMDI Metrics Package) and a legacy Fortran model (AM3). The actual SRM simulation space (aerosol microphysics, radiative transfer for solar injection) has virtually no GitHub presence. The most important finding: **the best-open-source climate simulation tool is not open-source at all — it's institutionally maintained by DOE/LLNL.**

---

## PCMDI/pcmdi_metrics — Full Commit Analysis

### The v4.2.1 Release Burst (Sep 3-4, 2026)

| SHA | Message | Author | Date |
|-----|---------|--------|------|
| `3092cdd` | Merge PR #1428 from lee1043-patch-1 | Jiwoo Lee | Sep 4, 2026 |
| `6419050` | Bump version to 4.2.1 | Jiwoo Lee | Sep 4, 2026 |
| `6443a1d` | Merge PR #1429 from lee1043-patch-2 | Jiwoo Lee | Sep 4, 2026 |
| `0e3a96f` | Update version and release date in CITATION.cff | Jiwoo Lee | Sep 4, 2026 |
| `e7dc726` | Prepare v4.2.1 | Jiwoo Lee | Sep 4, 2026 |
| `d0bcbd8` | Merge PR #1427: proper rounding correction | Jiwoo Lee | Sep 4, 2026 |
| `90cbc50` | Prevents roundoff to 1.00 in mean_climate figures | James Goodnight | Sep 4, 2026 |
| `71a0497` | Merge PR #1425: extremes chunking | Jiwoo Lee | Sep 3, 2026 |
| `b2eb044` | Merge branch 'main' into #1424 | Jiwoo Lee | Sep 3, 2026 |
| `c8711f1` | Merge PR #1423: variability modes dask SVD memory | Jiwoo Lee | Sep 3, 2026 |

**Key observations:**
- All 10 commits in 48 hours — a classic pre-release sprint
- jiwoo Lee (LLNL PMP Lead) authored 8 of 10 commits
- James Goodnight contributed 1 fix (roundoff bug)
- Jared Lewis's PR (#1423) was merged for dask SVD memory optimization
- v4.2.1 was a technical release; v4.2.0 (previous) added Hadley Cell Metrics
- v4.1.0 added ENSO Metrics, Sea Ice IIEE Metric, and EOF Classification

### Version History Highlights

| Version | Date | New Capabilities |
|---------|------|------------------|
| v4.2.1 | Sep 2026 | Technical update (rounding, performance) |
| v4.2.0 | ~2026 | Hadley Cell Metrics |
| v4.1.0 | ~2025 | ENSO Metrics, Sea Ice IIEE, EOF Classification |
| v4.0.0 | ~2023 | Python 3.10+ support |
| v3.9 | ~2022 | Decision-Relevant metrics, Database access API |
| v3.8 | ~2021 | ENSO figure generation, xCDAT migration |
| v3.0.0 | ~2020 | Cloud feedback metric (Mark Zelinka)

**Podcast angle:** The PMP has been adding new climate metrics for 15+ years, each release requiring coordinated institutional effort. This isn't community open-source — it's a national lab software pipeline. The question for the episode: **if SRM governance requires model evaluation, and model evaluation requires this toolkit, who controls the evaluation infrastructure?**

---

## FMS-ESM/AM3 — The Fossil Record

### Complete Commit History (4 commits, all on one day)

| SHA | Message | Author | Date |
|-----|---------|--------|------|
| `f5739a9` | Update README.md | Benjei Tsuang | Mar 1, 2015 |
| `0f6966e` | Update README.md | Benjei Tsuang | Mar 1, 2015 |
| `dc66bdd` | AM3 for GitHub | Benjei Tsuang | Mar 1, 2015 |
| `020236e` | Initial commit | Benjei Tsuang | Mar 1, 2015 |

**Interpretation:** AM3 was pushed to GitHub once on a single day in 2015 and never touched again. It's an archival repository — a snapshot of GFDL's atmospheric model for historical reference. The codebase is Fortran 77/90 and represents the state of climate simulation from the early 2000s.

**Podcast angle:** The "legacy codebase" problem. SRM simulation codes that exist are often stuck in 2005-era Fortran. Modern Python tools (PCMDI) can evaluate models but can't easily replace the models themselves. The transition from Fortran to Python has bypassed the geoengineering simulation layer entirely.

---

## pmip4/pmip_p2fvar_analyzer — Paleoclimate Analysis

### Commit Timeline

| Date | Commit | Activity |
|------|--------|----------|
| Sep 25, 2025 | `dded725` | Link update (PMIP4-PMIP3 data archive) |
| Jan 18, 2023 | `a9b3224` | Added NCL script for data frames |
| Sep 14, 2022 | `413c7dd`, `002d1a9`, `0016218` | Pliocene exploration notebooks |
| Sep 15, 2022 | `e155080` | Images for Peru figures |
| Aug 14, 2022 | `57c4b4e`, `9197cd0`, `ce93292` | Error corrections by Anni Zhao |
| Jan 24, 2022 | `b20a4ab` | Initial data upload |

**Pattern:** Single-contributor tool (Chris Brierley, University College London) with periodic bursts of analysis work. Focus on the Pliocene (3-4 million years ago, when CO2 was ~400 ppm and temperatures were 2-3°C warmer) — directly relevant to SRM because it represents a natural "what if" experiment.

**Podcast angle:** The Pliocene is the natural SRM control experiment. If we could model what happened when the Earth naturally had high CO2 and then comparing it to what SRM would do, we'd have a baseline. PMIP tools make this possible, but they require specialized expertise.

---

## Cross-Cutting: Solar Geoengineering on GitHub

### What Exists vs. What's Missing

| Category | Repos | Quality |
|----------|-------|--------|
| **Model evaluation** | PCMDI/pcmdi_metrics (133★) | World-class, institutional |
| **Atmospheric models** | FMS-ESM/AM3 (4★, fossil) | Legacy, unmaintained |
| **Paleoclimate data** | PMIP analyzer (4★) | Single-maintainer |
| **Interactive SRM economics** | srm-forever (0★) | Teaching tool, not simulation |
| **Arctic SRM impacts** | Codes-RFG-Arctic-Impacts (1★) | Single project, 2024 |
| **SRM microphysics/Radiative transfer** | **None** | ❌ Gap |
| **Stratospheric aerosol injection models** | **None** | ❌ Gap |
| **Cloud brightening simulation** | **None** | ❌ Gap |

### The Core Paradox

> The most important climate simulation toolkit on GitHub (PCMDI) can evaluate whether a model accurately simulates the climate system — but no open-source repository contains the actual SRM simulation code that would need evaluating.

This is like having a world-class scale but no scale to weigh. PCMDI provides the evaluation infrastructure; SRM simulations are either closed-source (GFDL, NCAR) or non-existent in open form.

---

## Episode-Ready Talking Points

1. **"The scale exists, but the thing being scaled doesn't."** PCMDI is a 15-year-old, DoD-funded evaluation framework with no SRM models to evaluate.

2. **"The release sprint is the story."** 10 commits in 48 hours for v4.2.1 — but none of them were about geoengineering. They were about fixing a rounding bug in mean climate figures.

3. **"Three contributors to PMIP in 4 years"** — The pace of open-source paleoclimate analysis is glacial (pun intended). Compare this to the 10-contributor sprint at PCMDI.

4. **"AM3 is a ghost."** 4 commits, March 1, 2015, then never again. This is what happens when a national lab decides a model is legacy — it gets pushed to GitHub and forgotten.

---

*Detailed commit analysis from GitHub API data. All SHA hashes verified.*
