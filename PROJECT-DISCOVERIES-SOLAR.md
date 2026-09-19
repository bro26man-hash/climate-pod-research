# ☀️ Solar Geoengineering — Project Discoveries

**Last updated:** September 2026
**Research cycle:** v5 — GitHub API dive, 8 repos surveyed, 40+ commits analyzed

---

## Summary

Solar geoengineering (SRM) code on GitHub lives **inside climate models**, not in SRM-specific repositories. The 4 repos below span the full spectrum from institutional powerhouse (PCMDI, 133★) to governance-fresh-startup (Zereo0317, 2 commits). The key insight for Episode 1: **SRM is modeled as a perturbation within general circulation models, not built as a standalone tool.**

---

## 1. PCMDI/pcmdi_metrics ⭐133

**URL:** https://github.com/PCMDI/pcmdi_metrics
**Language:** Python
**Maintainer:** Jiwoo Lee (lead), James Goodnight, Sarah Michalak

### What it is
The definitive open-source Python package for evaluating and comparing climate and Earth system models. PCMDI (Program for Climate Model Diagnosis and Intercomparison) is the analytical engine behind CMIP (Coupled Model Intercomparison Project) — the framework that IPCC reports rely on.

### Why it matters for solar geoengineering
PCMDI metrics are how scientists **detect and attribute** solar radiation modification effects across model ensembles. When a researcher runs a WRF-Chem simulation with sulfate aerosol injection, PCMDI's tools quantify whether the temperature response is realistic, spatially coherent, and statistically significant.

### Recent commit snapshot (Sep 2026 — very active)
| Date | Commit | Author |
|------|--------|--------|
| Sep 17 | Merge PR #1431 — mov_patch | Jiwoo Lee |
| Sep 17 | Patch for single-file modpath case | Jiwoo Lee |
| Sep 4 | Merge PR #1428 | Jiwoo Lee |
| Sep 4 | Bump version to 4.2.1 | Jiwoo Lee |
| Sep 4 | Merge PR #1429 — lee1043-patch-2 | Jiwoo Lee |
| Sep 4 | Prepare v4.2.1 release | Jiwoo Lee |
| Sep 4 | Fix roundoff to 1.00 in mean_climate figures | James Goodnight |
| Sep 3 | Merge PR #1425 — extremes chunking | Jiwoo Lee |

**Verdict:** 🔴 **Fast Universe** — institutional, funded, continuous. 10 commits in 2 weeks. Multiple contributors pushing version releases and bug fixes on a tightly managed schedule.

---

## 2. Sustainable-Solutions-Lab/regional-geo

**URL:** https://github.com/Sustainable-Solutions-Lab/regional-geo
**Language:** Python
**Maintainer:** Ken Caldeira (co-founder, Carnegie Science)

### What it is
Analysis of WRF-Chem regional climate model simulations exploring the effects of **stratospheric sulfate aerosol injection** on regional climate. This is the most directly SRM-focused codebase found on GitHub.

### Experimental design
- 2 seasonal episodes (May 2024 dry season, July 2024 wet season)
- 3 ensemble members per episode
- 4 SO₂ injection rates: 0 (control), 1,000, 10,000, 100,000 t/h
- 5×5 grid cell injection region
- 24 total simulation cases

### Key analysis modules
- `src/data_loader.py` — xarray-based NetCDF loader for WRF output
- `src/ratio_analysis.py` — gridded ratio fields with error propagation, showing how each grid cell contributes to domain-wide change

### Recent commit snapshot (Feb 2026 — burst pattern)
| Date | Commit | Author |
|------|--------|--------|
| Feb 15 | Gaussian smoothing | Ken Caldeira |
| Feb 14 | Improved maps and analysis | Ken Caldeira |
| Feb 14 | Show individual cases | Ken Caldeira |
| Feb 14 | Fixing figures | Ken Caldeira |
| Feb 13 | Start analysis | Ken Caldeira |
| Feb 13 | Read RDS files | Ken Caldeira |
| Feb 13 | Area calculation | Ken Caldeira |
| Feb 13 | Add data loader documentation | Ken Caldeira |
| Feb 13 | Remove defensive checks from data loader | Ken Caldeira |
| Feb 13 | Add data loader utility | Ken Caldeira |

**Verdict:** 🟡 **Slow Universe** — single maintainer, 10 commits in 3 days (Feb 2026 analysis sprint), then dormant. Classic academic burst pattern: code ships with papers, then goes quiet until the next publication cycle.

---

## 3. eabarnes1010/actm-sai-csu

**URL:** https://github.com/eabarnes1010/actm-sai-csu
**Language:** Python
**Stars:** 6
**Maintainer:** Zachary Labe, Daniel Hueholt, Antonios Mamalakis

### What it is
**AI to detect, attribute, and quantify solar radiation management (SRM) effects and risks** under a range of geopolitical scenarios. Funded by DARPA (Defense Advanced Research Projects Agency).

### Why it matters
This is the **governance-adjacent** side of SRM code: not simulating the geoengineering itself, but building machine-learning tools to **detect whether SRM has been deployed** and attribute its effects. This is the intelligence-community angle — if SRM is deployed somewhere, how would you know?

### Recent commit snapshot (Jan–Mar 2023 — paper-driven)
| Date | Commit | Author |
|------|--------|--------|
| Mar 28 | New paper | Zachary Labe |
| Mar 28 | New paper! | Zachary Labe |
| Feb 9 | Add preprint link to README | Daniel Hueholt |
| Feb 8 | Add Jim's link | Daniel Hueholt |
| Feb 8 | Standardize capitalization | Daniel Hueholt |
| Feb 8 | Add code from Hueholt et al. 2023 | Daniel Hueholt |
| Jan 22 | Update README | Antonios Mamalakis |
| Jan 22 | Create README | Antonios Mamalakis |
| Jan 11 | New preprint | Zachary Labe |
| Jan 11 | New preprint | Zachary Labe |

**Verdict:** 🟡 **Slow Universe** — paper-driven lifecycle. 10 commits all tied to paper submissions (Jan–Mar 2023). No commits since. Code exists to support publications, not to be a living tool.

---

## 4. Zereo0317/climate-intervention-governance

**URL:** https://github.com/Zereo0317/climate-intervention-governance
**Language:** Shell
**Stars:** 0
**Created:** August 23, 2026

### What it is
Neutral regulatory and governance-intelligence tracking for solar radiation management (SRM) and climate-intervention technologies — covering the CBD moratorium, UNFCCC processes, and other international governance frameworks.

### Recent commit snapshot (Aug 2026 — brand new)
| Date | Commit | Author |
|------|--------|--------|
| Aug 23 | Fact-check and update MCP server wiring | Zereo0317 |
| Aug 23 | Initial public release | Zereo0317 |

**Verdict:** ⚫ **Empty Universe (adjacent)** — only 2 commits, both on day one. But it's the **first SRM governance codebase** found. The question for the episode: is this a signal that governance is finally being treated as a software problem, or is it vaporware?

---

##Cross-theme insight

**The SRM code paradox:** The most scientifically important SRM code (regional-geo) is buried inside a climate modeling lab with 0 stars. The most-starved SRM code (actm-sai-csu, 6★) is about detection, not simulation. Meanwhile, PCMDI — the tool that makes all of this quantifiable — has 133 stars and corporate-level development velocity.

**Episode 1 angle:** *Who controls the metrics?* If PCMDI defines how we measure solar geoengineering's effects, and PCMDI is run by a small institutional team, then the governance question isn't just about SRM deployment — it's about who writes the evaluation code that determines whether SRM "works."

---

## Quick reference

| Repo | Stars | Commits (recent) | Velocity | Theme |
|------|-------|-------------------|----------|-------|
| PCMDI/pcmdi_metrics | 133 | 10 in 2 weeks (Sep 2026) | 🔴 Fast | Model evaluation |
| regional-geo | 0 | 10 in 3 days (Feb 2026) | 🟡 Slow (burst) | WRF SRM simulation |
| actm-sai-csu | 6 | 10 in 3 months (2023) | 🟡 Slow (burst) | AI SRM detection |
| climate-intervention-governance | 0 | 2 (Aug 2026) | ⚫ Newborn | Governance tracking |
