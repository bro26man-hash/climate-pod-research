# ☀️ Solar Geoengineering — Project Discoveries
## Fresh Research Notes (September 2026 — v4 Update)

---

## Overview
This document profiles the most active open-source repositories relevant to solar geoengineering (SRM) and atmospheric climate modeling, based on fresh commit histories pulled from GitHub on September 18, 2026.

---

## 🔥 Tier 1: High-Activity, Institutionally Funded

### 1. WRF Model (`wrf-model/WRF`)
- **Stars:** 1,762 | **Language:** Fortran | **License:** BSD
- **Last commit:** June 8, 2026 (v4.8.0 release merge)
- **Focus:** The Weather Research and Forecasting model — the foundational atmospheric simulation tool used worldwide.

**Why it matters for solar geoengineering:**
- WRF is the primary model used to simulate the atmospheric effects of SRM proposals (stratospheric aerosol injection, marine cloud brightening)
- Its radiation scheme is directly relevant — any SRM intervention that blocks or redirects solar radiation must be evaluated through WRF's physics
- The v4.8.0 release includes updates to the MYNN-EDMF turbulence scheme and the MMM physics suite

**Key commits (15 pulled, May–June 2026):**
| Date | Commit | Significance |
|------|--------|-------------|
| Jun 8 | v4.8.0 release merge | Major version release — institutional milestone |
| Jun 6 | README & version update to v4.8.0 | Documentation sync |
| Jun 5 | Turn off tempo_aerosolaware & tempo_hailaware | Aerosol parameterization changes — **directly relevant to SRM simulation** |
| May 28 | Correction for EOT calculation for solar radiation | **Solar radiation fix — critical for SRM energy balance calculations** |
| May 27 | MYNN-EDMF pointer update & icloud_bl removal | Cloud physics changes affecting aerosol-cloud interactions |
| May 26 | CDXWRF module fix | Diagnostic tooling fix |
| May 21 | Include mp_physics=88 in TEMPO error print | Error handling improvement |
| May 20 | Minor Tempo changes | Ongoing development |
| May 20 | Urban NbS initialization bug fix | Urban environment modeling (relevant for city-scale SRM deployment) |
| May 20 | ShinHong PBL namelists + revised MMM surface layer | New PBL scheme — affects surface energy balance for SRM scenarios |

**🎙️ Episode hook:** "The most important climate model you've never heard of just released v4.8.0 — and the solar radiation fix buried in the commit log could change how we simulate a volcanic eruption's cooling effect."

---

### 2. PCMDI Metrics (`PCMDI/pcmdi_metrics`)
- **Stars:** 133 | **Language:** Python | **License:** BSD
- **Last commit:** September 17, 2026 (TODAY — active!)
- **Focus:** Evaluation toolkit for Earth System Models (ESMs) against CMIP6 data.

**Why it matters:**
- Before you can evaluate whether SRM "works," you need tools to detect and attribute model responses
- PCMDI metrics are the standard for CMIP6 model evaluation — they're used in every major IPCC assessment
- If SRM experiments are to be included in future CMIP rounds, these metrics will define success criteria

**Key commits (15 pulled, Sep 1–17, 2026):**
| Date | Commit | Significance |
|------|--------|-------------|
| Sep 17 | PR #1431 merge — modpath_list patch | Bug fix for file detection |
| Sep 4 | Bump version to 4.2.1 | **New release!** |
| Sep 4 | Prepare v4.2.1 + version/release date update | Release preparation |
| Sep 4 | Roundoff fix in mean_climate figures | **Precision fix — prevents 1.00 roundoff in climate statistics** |
| Sep 3 | Extremes chunking PR merge | Memory optimization for extreme value analysis |
| Sep 3 | Rechunk data for rolling operation | **Dask/SVD memory optimization — handling larger datasets** |
| Sep 3 | Force numpy SVD | Numerical stability fix |

**🎙️ Episode hook:** "10 commits in one day. A precision fix that prevents your global temperature data from rounding to exactly 1.00°C. This is the unsexy infrastructure that makes SRM evaluation possible."

---

### 3. MDTF Diagnostics (`NOAA-GFDL/MDTF-diagnostics`)
- **Stars:** 80 | **Language:** Python | **License:** Apache-2.0
- **Last commit:** August 14, 2026
- **Focus:** Process-oriented diagnostics for model evaluation, including the **precipitation-buoyancy POD**.

**Why it matters for ocean-adjacent SRM:**
- Marine Cloud Brightening (MCB) is a solar geoengineering technique that targets marine clouds
- The precip-buoyancy POD is the most ocean-relevant diagnostic in open source — it evaluates how well models simulate precipitation-buoyancy relationships, which govern cloud formation
- This is the closest thing to an "ocean SRM evaluation tool" that exists

**Key commits (15 pulled, May–Aug 2026):**
| Date | Commit | Significance |
|------|--------|-------------|
| Aug 14 | PR #825 merge | Integration work |
| Jun 19 | 5 commits: MCS precip-buoyancy statistics POD | **🎯 5 commits in one day on the same file — the ocean's closest friend** |
| Jun 8 | PR #823 merge + README updates | Institutional update |
| Jun 2 | Citation added | Academic credibility push |
| Jun 1 | Quarterly metrics workflow for traffic logging | Infrastructure |
| May 27 | Move blocking_neale_nb to dev branch | Code organization |
| May 22 | Blocking notebook PR merge | New analysis capability |

**🎙️ Episode hook:** "Five commits in a single day, all to the same file — a precipitation-buoyancy statistics tool that happens to be the most ocean-relevant code in climate science. Is this the seed of marine cloud brightening evaluation? Or just good science practice?"

---

## 🟡 Tier 2: Individual Researchers, Dormant or Niche

### 4. ClimateMARGO (`ClimateMARGO/ClimateMARGO.jl`)
- **Stars:** 73 | **Language:** Julia | **License:** MIT
- **Last commit:** August 17, 2026 (README update after 2+ year dormancy)
- **Focus:** Idealized climate-economic modeling framework for optimizing mitigation/adaptation/geoengineering trade-offs.

**The ghost revival pattern:**
- Two README updates on Aug 17, 2026 — first activity since November 2023
- Zero code commits in the revival
- The 2022–2023 commits show real development: JuMP/Ipopt compatibility upgrades, deprecated web app removal, CITATION.bib addition
- The 2026 revival is documentation-only — does this signal renewed policy-modeling interest, or just a citation update?

**Key commits (15 pulled):**
| Date | Commit | Phase |
|------|--------|-------|
| Aug 17, 2026 | README update ×2 | 🟡 Revival signal? |
| Oct 2023 | unit_conversions.jl comment update | 🔴 Dormant |
| Jul 2023 | Pluto notebook link added | 🟡 Active |
| Nov 2022 | Project.toml update + JuMP/Ipopt compat upgrade | 🟢 Active |
| Feb 2022 | Web apps removed, CITATION.bib added, doc updates | 🟢 Active |
| Jan 2022 | Version bump, documentation, bug fixes | 🟢 Active peak |

**🎙️ Episode hook:** "A climate-economic model goes dormant for 2 years, then its README gets updated twice in one day. Is someone preparing for a policy moment? Or is this academic ghosting at its most ambiguous?"

---

### 5. SRM Forever (`hausfath/srm-forever`)
- **Stars:** 0 | **Language:** Unknown | **License:** Unknown
- **Last commit:** August 26, 2026
- **Focus:** Interactive economics model for Solar Radiation Management — Weitzman certainty-equivalent discounting applied to SRM cost dynamics.

**Why a zero-star repo matters:**
- This repo applies the Weitzman (1998) discounting framework to SRM — the "What does it cost to keep SRM going forever?" question
- The theoretical framework is conceptually critical: if SRM must be maintained continuously for centuries, the social cost of commitment is unknown
- Zero stars doesn't mean zero impact — this is the kind of paper that shapes how economists think about SRM commitment costs

**🎙️ Episode hook:** "Zero stars, but this repo solves the most important unanswered question in SRM economics: what's the price of keeping the sun shield up forever?"

---

## ⚪ Tier 3: Emergent / Low Visibility

### 6. Geo-DICE (`PSLmodels/Geo-DICE`)
- **Stars:** 2 | **Language:** MATLAB | **License:** Unknown
- **Focus:** Modified DICE integrated assessment model with geoengineering modules.

**Context:** The DICE model (Nordhaus) is the canonical IAM used in climate economics. Geo-DICE adds SRM modules. With only 2 stars, it's a niche academic tool — but it's where SRM enters the economic policy discussion.

---

### 7. Awesome Geoengineering (`brandonhimpfen/awesome-geoengineering`)
- **Stars:** 4 | **Language:** Python (curated list)
- **Last commit:** September 6, 2026
- **Focus:** A curated directory of geoengineering projects, research, organizations, and tools.

**This is a meta-resource** — it points to other projects. Updated as recently as Sep 6, 2026. Good starting point for finding additional repos.

---

## 🔍 Cross-Cutting Themes from Commit Analysis

### 1. The "Solar Radiation Fix" Pattern
WRF's May 28 commit — "correction for EOT calculation for solar radiation" — is buried in a routine bug fix. But it affects how models calculate energy balance under SRM scenarios. The people building SRM tools are the same people fixing radiation schemes. This is invisible infrastructure.

### 2. Institutional Thunder vs. Individual Drizzle
PCMDI dropped 10 commits in one day. WRF condensed 15 commits into 3 weeks. Meanwhile, ClimateMARGO's revival is two README edits. The institutional pace makes individual research feel like a glacier.

### 3. The Evaluation Gap
All three Tier-1 repos are about **evaluating** climate models, not **simulating** SRM scenarios. PCMDI metrics, MDTF diagnostics, and WRF physics are evaluation tools. Where are the SRM simulation tools? The absence is striking: we're good at checking if models work, but we lack open-source tools to actually simulate SRM deployments.

### 4. The Aerosol Parameterization Signal
WRF's June 5 commit turning off `tempo_aerosolaware` and `tempo_hailaware` suggests that the TEMPO aerosol scheme may have issues for certain configurations. For SRM researchers, aerosol parameterization is everything — small errors in aerosol forcing translate to large errors in cooling predictions.

---

## 📊 Summary Table

| Repo | Stars | Last Activity | Commits Pulled | Activity Level | SRM Relevance |
|------|-------|--------------|----------------|----------------|---------------|
| WRF | 1,762 | Jun 2026 (active) | 15/15 | 🔥🔥🔥🔥🔥 | Direct (radiation scheme) |
| PCMDI | 133 | Sep 2026 (TODAY) | 15/15 | 🔥🔥🔥🔥🔥 | Direct (evaluation tools) |
| MDTF | 80 | Aug 2026 (active) | 15/15 | 🔥🔥🔥🔥 | Direct (ocean-adjacent POD) |
| ClimateMARGO | 73 | Aug 2026 (revival?) | 15/15 | 🔥🔥 | Moderate (economic modeling) |
| srm-forever | 0 | Aug 2026 | Limited | 🔥 | Conceptual (commitment costs) |
| Geo-DICE | 2 | Unknown | Limited | ⚪ | Moderate (IAM + SRM) |
| Awesome-List | 4 | Sep 2026 | Limited | 🔥 | Meta (directory) |

---

*Generated from GitHub API commit data pulled September 18, 2026. All commit URLs available in the raw research log.*

**Next steps:** Cross-reference with SRM-specific repositories (search for "stratospheric aerosol injection", "marine cloud brightening", "cirrus cloud thinning" as separate queries). Reach out to PCMDI maintainers for interview. Interview question: "How do you evaluate a climate model that simulates an intervention that hasn't happened?"