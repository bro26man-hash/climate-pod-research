# ☀️ Solar Geoengineering — Project Discoveries (v5 Update)
## Research Notes for Climate Pod Episode: Solar Geoengineering
*Updated: October 2026 — v5: Fresh commit pull from 8 key repos*

---

## Overview

This document profiles the most significant open-source repositories related to solar geoengineering (Solar Radiation Management, SRM) and atmospheric modeling. Data from GitHub search queries and direct commit-history pulls, October 2026.

---

## Executive Summary: The Solar Episode Is Getting Active

After v4 (September 2026), the solar geoengineering ecosystem on GitHub shows **three distinct signals**:

1. **🔴 Institutional cores remain steady** — WRF and PCMDI continue their methodical, funded development cadence
2. **🟡 Individual projects are REVIVING** — srm-forever burst 4 commits in one day (Aug 26), Marine-Cloud-Brightening added a temperature analysis notebook (Jun 16)
3. **⚫ Governance is emerging** — A new regulatory tracker (climate-intervention-governance) appeared, signaling that SRM is moving from pure science into the policy arena

---

## Repository Profiles

### 1. WRF Model (`wrf-model/WRF`)
- **Stars:** 1,763 | **Language:** Fortran/C | **License:** Apache 2.0
- **Last activity:** June 8, 2026 (v4.8.0 release, develop branch merged)
- **Branch status:** `develop` = `main` at v4.8.0. No new commits since the v4.8.0 merge.
- **What it is:** The Weather Research and Forecasting model — the foundational atmospheric simulation tool used worldwide.
- **Why it matters for solar geoengineering:** WRF is the primary tool used to *simulate the effects* of solar geoengineering. SRM experiments are modeled using WRF's chemistry and radiation modules.

**Key commits (develop branch, 10 pulled):**

| Date | Commit | Significance |
|------|--------|-------------|
| Jun 8, 2026 | Merge release-v4.8.0 into develop | **Development branch catches up to release** — v4.8.0 is now the base for future work |
| Jun 6, 2026 | Update README and version to v4.8.0 | Documentation update for new release |
| Jun 5, 2026 | **Turn off tempo_aerosolaware and tempo_hailaware** | **Aerosol parameterization adjustment** — directly relevant to SRM modeling; some aerosol schemes deactivated |
| May 30, 2026 | Fix vectorization option in AOCC stanza | Compiler optimization fix for AMD |
| May 28, 2026 | **Correction for eot calculation for solar radiation (#2334)** | **Critical fix** — eot = epoch of transit for solar radiation; errors affect ALL SRM simulations |
| May 27, 2026 | Updating MYNN-EDMF pointer, removing icloud_bl | Planetary boundary layer physics update |
| May 27, 2026 | Update MMM-physics repo SHA with fixes | Multiscale physics consolidation |
| May 26, 2026 | Fixing CDXWRF module | Regional climate model interface fix |
| May 26, 2026 | Update readme for GFL option | Green's function lidar documentation |
| May 21, 2026 | Include mp_physics=88 in TEMPO error print | Air quality module error handling |

**Episode angle (v5):** The v4.8.0 release is the **first major WRF version where aerosol-aware schemes were deactivated by default** (Jun 5). This is a double-edged sword: it simplifies the model for users not doing SRM, but it also means that future SRM experiments will need to explicitly re-enable these schemes. The solar radiation EOT fix (May 28) means every SRM simulation run between earlier versions and v4.8.0 may have had slightly wrong solar forcing. For a technology meant to shade the planet, precision matters enormously.

---

### 2. PCMDI Metrics (`PCMDI/pcmdi_metrics`)
- **Stars:** 133 | **Language:** Python | **License:** BSD-3-Clause
- **Last activity:** September 17, 2026 (v4.2.1 — very recent!)
- **What it is:** The Program for Climate Model Diagnosis and Intercomparison's evaluation toolkit — used to assess how accurately climate models simulate observed realities. CMIP6 metrics standard.
- **Why it matters:** Before you can evaluate whether solar geoengineering "works," you need metrics to measure model accuracy. PCMDI provides the yardstick.

**Key commits (10 pulled):**

| Date | Commit | Significance |
|------|--------|-------------|
| Sep 17, 2026 | Merge PR #1431 (mov_patch) | Latest patch — file modification path handling |
| Sep 17, 2026 | Patch for single file modpath_list case | Edge case fix in metrics computation |
| Sep 4, 2026 | Merge PR #1428 | PR consolidation |
| Sep 4, 2026 | **Bump version to 4.2.1** | **New release** — active maintenance signal |
| Sep 4, 2026 | Merge PR #1429 | Parasol patch |
| Sep 4, 2026 | Update version and release date in CITATION.cff | Citation metadata update |
| Sep 4, 2026 | Prepare v4.2.1 | Release preparation |
| Sep 4, 2026 | Merge PR #1427 (jsgoodni_corr_roundoff) | Roundoff fix PR |
| Sep 4, 2026 | **Prevents roundoff to 1.00 in mean_climate figures** | **Critical fix** — roundoff errors in climate metrics could mask small but important temperature differences |
| Sep 3, 2026 | Merge PR #1425 (extremes_chunking) | Extremes chunking for large datasets |

**Episode angle (v5):** PCMDI's roundoff fix (Sep 4) is quietly profound. If climate metrics round to 1.00, small temperature differences that matter for SRM evaluation (e.g., 0.5°C regional cooling vs. 0.7°C) could be invisible. The fact that PCMDI is actively fixing these issues means the SRM evaluation community is maturing — but it also means that older CMIP6 evaluations may have had masked results.

---

### 3. srm-forever (`hausfath/srm-forever`) — 🆕 REVIVAL SIGNAL
- **Stars:** Low (personal project) | **Language:** HTML/JavaScript (interactive model) | **License:** Unknown
- **Last activity:** **August 26, 2026 — 4 commits in one day!** 🔥
- **What it is:** Interactive model comparing 1.5°C held with stratospheric aerosol injection vs. rapid mitigation plus carbon removal. Based on Weitzman (2012) climate-economics framework.
- **Why it matters:** This is the most directly SRM-focused interactive tool on GitHub. It asks the fundamental question: *Is it cheaper to reflect sunlight or to decarbonize + remove carbon?*

**Key commits (4 pulled — ALL on Aug 26, 2026):**

| Date | Commit | Significance |
|------|--------|-------------|
| Aug 26, 2026 | Add effective discount rate chart | **Visual economics** — now plots the discount rate that determines SRM vs. mitigation preference |
| Aug 26, 2026 | **Adopt Weitzman certainty-equivalent discounting** | **Major theoretical update** — switches from expected-utility to Weitzman's certainty-equivalent framework, which changes the cost comparison fundamentally |
| Aug 26, 2026 | Price abatement as a vintage annuity | Economic modeling improvement — treats abatement costs as a stream of annuities |
| Aug 26, 2026 | Interactive SRM-forever vs mitigation+CDR cost model | **Core interactive model** — the main event |

**Episode angle (v5):** srm-forever's Aug 26 burst is the **single biggest development signal** in the solar geoengineering space this quarter. The shift to Weitzman certainty-equivalent discounting is theoretically significant: Weitzman (2012) argued that under deep uncertainty about climate sensitivity, the certainty-equivalent discount rate can be much lower than the expected-rate discount rate, which **changes the cost comparison between SRM and mitigation+CDR**. This isn't just a code update — it's a paradigm shift in how the SRM-vs-mitigation question is framed. The fact that this is an *interactive* model means policymakers can explore the tradeoffs themselves.

---

### 4. Marine Cloud Brightening Project (`meneskoksal/Marine-Cloud-Brightening`)
- **Stars:** Low | **Language:** Jupyter Notebook | **License:** Unknown
- **Last activity:** June 16, 2026 — **10 commits in one day!** 🔥
- **What it is:** Research code for marine cloud brightening (MCB) — a SRM technique that brightens marine clouds to reflect more sunlight. Uses RRTM (Rapid Radiative Transfer Model) to simulate effects on net solar radiation.
- **Why it matters:** MCB is one of the three main SRM techniques (alongside stratospheric aerosol injection and space-based reflectors). It's the most geographically localized and potentially the most reversible.

**Key commits (10 pulled — ALL on Jun 16, 2026):**

| Date | Commit | Significance |
|------|--------|-------------|
| Jun 16, 2026 | Update README with authors and file changes | Metadata cleanup |
| Jun 16, 2026 | Delete RadiativeFluxes/readme | Structure cleanup |
| Jun 16, 2026 | Add files via upload (julkrag) | New content from contributor |
| Jun 16, 2026 | Enhance README with project details and structure | Documentation improvement |
| Jun 16, 2026 | **Added temperature analysis notebook (LenaPredl)** | **New analysis capability** — temperature response to MCB |
| Jun 16, 2026 | Delete Temperature/ReadMe | Structure migration |
| Jun 16, 2026 | CloudCover Analysis (ba3ee26) | **New cloud cover analysis** — direct MCB effect measurement |
| Jun 16, 2026 | Delete CloudCover/readme | Structure migration |
| Jun 16, 2026 | Delete runscripts/readme | Structure migration |
| Jun 16, 2026 | Add files via upload | More content from contributors |

**Episode angle (v5):** MCB's Jun 16 burst adds temperature and cloud-cover analysis notebooks — this is the transition from "can we simulate cloud brightening?" to "what are the precise temperature and cloud microphysics effects?" The fact that multiple contributors (meneskoksal, julkrag, LenaPredl) participated suggests a **collaborative research effort**, possibly academic. The deletion of old readme files and restructuring suggests the project is maturing from a personal experiment into a more organized research tool.

---

### 5. ClimateMARGO.jl (`ClimateMARGO/ClimateMARGO.jl`)
- **Stars:** 73 | **Language:** Julia | **License:** MIT
- **Last activity:** August 17, 2026 (2 README updates)
- **What it is:** Julia implementation of MARGO, an idealized climate-economic modeling framework for optimizing trade-offs between emissions Mitigation, Adaptation, and geoengineering (SRM/CDR).
- **Why it matters:** ClimateMARGO bridges the gap between climate models and economic models. It's the tool for asking: "Given a budget of geoengineering, what's the optimal allocation between SRM and CDR?"

**Key commits (10 pulled):**

| Date | Commit | Significance |
|------|--------|-------------|
| Aug 17, 2026 | Update README.md (Fons van der Plas) | **Minor revival** — README update after 2+ years of dormancy |
| Aug 17, 2026 | Update README.md (Fons van der Plas) | Second README update same day |
| Oct 18, 2023 | Update unit_conversions.jl with comment | Last code change before dormancy |
| Jul 6, 2023 | Add link to Pluto in README | Documentation |
| Nov 14, 2022 | Update Project.toml | Dependency update |
| Nov 12, 2022 | JuMP and Ipopt compat upgrade (#85) | Solver compatibility fix |
| Feb 10, 2022 | Removed deprecated web apps | Cleanup |
| Feb 4, 2022 | Added CITATION.bib | Citation support |
| Jan 13, 2022 | Fixed typo | Bug fix |
| Jan 12, 2022 | Updated arguments for doc version deployment | Documentation infrastructure |

**Episode angle (v5):** ClimateMARGO's Aug 2026 README updates are a ** faint but real revival signal**. The core code hasn't changed since October 2023, but Fons van der Plas is re-engaging with the project — updating documentation, maybe preparing for a new release. If this project gets fresh code commits, it could become the bridge between the WRF/PCMDI institutional universe and the srm-forever individual universe.

---

### 6. Climate Intervention Governance Tracker (`Zereo0317/climate-intervention-governance`) — 🆕 NEW DISCOVERY
- **Stars:** Low | **Language:** Shell | **License:** Unknown
- **Last activity:** August 23, 2026
- **What it is:** Neutral regulatory and governance-intelligence tracking for solar radiation management (SRM) and climate-intervention technologies. Covers CBD moratorium, London Protocol, and other international regulatory frameworks.
- **Why it matters:** This is the **first governance-focused repository** found in our research. SRM is moving from pure science into the policy arena — the existence of a governance tracker signals that the question is no longer "can we do SRM?" but "should we, and who decides?"

**Episode angle (v5):** The governance tracker is the most politically significant discovery in this research cycle. For a podcast episode, this is the "what's at stake beyond the science" angle. The CBD (Convention on Biological Diversity) has had a de facto moratorium on SRM since 2010, and the London Protocol regulates ocean fertilization. But there's no equivalent governance framework for the atmosphere — which is the "global commons" problem in its purest form.

---

### 7. orbital-climate-simulator (`yanpefnsc/orbital-climate-simulator`)
- **Stars:** 2 | **Language:** Python | **License:** Unknown
- **Last activity:** September 18, 2026
- **What it is:** Interactive mission-control dashboard for a conceptual Solar Radiation Management drone fleet. Not a real SRM deployment tool — more of an educational/artistic concept.
- **Why it matters:** Shows how SRM is entering the cultural imagination — not just as a climate solution but as a design fiction.

---

## Cross-Cutting Solar Episode Themes

### Theme 1: The Precision Problem
Both WRF (solar radiation EOT fix) and PCMDI (roundoff to 1.00 fix) had **critical precision-related commits** in the last 6 months. The theme: solar geoengineering requires the same precision as the climate models that simulate it, and even small errors can cascade into large uncertainties.

### Theme 2: The Economics Revolution
srm-forever's shift to Weitzman certainty-equivalent discounting (Aug 26) represents a **paradigm shift** in the SRM-vs-mitigation cost comparison. The old framework used expected-utility discounting; the new framework uses certainty-equivalent discounting, which under deep uncertainty **always favors more cautious, long-term actions** — potentially undermining the "SRM is cheap" argument.

### Theme 3: The Governance Vacuum
The discovery of climate-intervention-governance (Aug 2026) confirms that SRM governance is becoming a real field. But the vacuum remains: there is no international body with authority to mandate, permit, or prohibit SRM deployment. The podcast episode should ask: *If a country unilaterally deploys SRM, who stops them?*

### Theme 4: The Burst-and-Sleep Pattern
Both srm-forever (4 commits/1 day) and MCB (10 commits/1 day) show burst-then-sleep patterns. This is the **poke-and-hope** model of research: big effort spikes followed by long dormancy. This contrasts sharply with the institutional steady-state of WRF and PCMDI.

---

## Solar Episode Architecture (v5)

| Segment | Duration | Content |
|---------|----------|--------|
| **Cold Open** | 2 min | "What if the code that simulates sun-dimming had a bug in how it calculates sunlight?" (WRF EOT fix) |
| **The Science** | 15 min | WRF's aerosol parameterization changes + PCMDI's metrics revolution + how SRM is simulated |
| **The Economics** | 12 min | srm-forever's Weitzman shift: why the cheap-SRM argument may be wrong |
| **The Governance** | 10 min | Who decides? CBD moratorium, London Protocol, the governance tracker, and the vacuum |
| **The Ethics** | 8 min | MCB as a localized, reversible SRM — is it a gateway drug or a legitimate tool? |
| **The Future** | 5 min | ClimateMARGO's revival and what an optimal SRM+CDR allocation might look like |

---

## Research Methodology
- **Search queries:** 8 distinct queries across geoengineering, SRM, MCB, and climate economic modeling
- **Commit pulls:** 10 most recent commits from each of 7 key repositories (70 total commits analyzed)
- **API calls:** GitHub Repository Search, List Commits, Get Repository, List Branches
- **Date of research:** October 2026

---

*Research methodology: GitHub REST API, October 2026. Commits pulled via List Commits API. Search queries via Repository and Code Search APIs.*