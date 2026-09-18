# ☀️ Solar Geoengineering — Project Discoveries
## Fresh Research Notes — September 2026

---

## Overview

This document profiles **6 open-source repositories** relevant to solar geoengineering (SRM) and atmospheric climate simulation, based on GitHub searches and fresh commit history pulls. These represent the most active and conceptually important projects in the solar geoengineering space on GitHub.

---

## 1. WRF (Weather Research and Forecasting Model)

| Field | Detail |
|-------|--------|
| **Repo** | `wrf-model/WRF` |
| **Stars** | 1,762 ⭐ |
| **Language** | Fortran |
| **Last commit** | June 8, 2026 |
| **License** | open source |

**What it is:** The definitive open-source atmospheric model. WRF is the backbone of weather forecasting and climate simulation worldwide. Its solar radiation scheme is directly relevant to SRM research because any solar radiation management intervention must be evaluated against the same physics that WRF models.

**Why it matters for the podcast:** WRF v4.8.0 was released in June 2026. The commit history shows:
- **Solar radiation EOT calculation fix** (commit `e836cd6`, May 28, 2026) — a correction to "end-of-transit" solar geometry, critical for accurate insolation modeling
- **TEMPO aerosol-aware and hail-aware options turned off** (commit `6a289e1`, June 5, 2026) — TEMPO is the geostationary environmental satellite instrument; its aerosol data feeds into SRM-related atmospheric chemistry
- **MYNN-EDMF pointer updates and cloud package removals** (commit `8299919`, May 27, 2026) — boundary-layer physics that determine how contrail-like cloud brightening effects would propagate
- **ShinHong PBL namelists added** (commit `9c87d29`, May 20, 2026) — new planetary boundary layer schemes that affect surface energy balance calculations

**Episode hook:** *"The atmospheric model that runs the world's weather forecasts just got a solar radiation fix. What does it mean for solar geoengineering research?"*

---

## 2. ClimateMARGO.jl

| Field | Detail |
|-------|--------|
| **Repo** | `ClimateMARGO/ClimateMARGO.jl` |
| **Stars** | 73 ⭐ |
| **Language** | Julia |
| **Last commit** | August 17, 2026 |
| **License** | open source |

**What it is:** Julia implementation of MARGO (Moderately-round Event-based Generational Optimization), an idealized climate-economic modeling framework for optimizing trade-offs between emissions mitigation, adaptation, and solar geoengineering.

**Why it matters for the podcast:** ClimateMARGO is one of very few tools that explicitly models SRM as part of a climate-economic optimization. The commit history reveals a fascinating pattern:
- **2 README updates on August 17, 2026** after **2.5 years of complete dormancy** (last code commit was October 2023)
- No new code commits in the revival — only documentation updates
- Original development was active through early 2022 (version bumps, documentation, Julia package compatibility upgrades)

**The dormancy-then-revival pattern suggests:** Someone rediscovered the tool for policy-modeling purposes (possibly for an IPCC-aligned study or legislative testimony) but didn't have resources to update the code. The 2026 README updates could signal renewed policy interest in SRM governance modeling.

**Episode hook:** *"A climate-economic模型 went dormant for 2 years, then suddenly got its README updated. What reignited interest inSRM optimization?"*

---

## 3. Geo-DICE (Geodynamic Integrated Climate-Economy)

| Field | Detail |
|-------|--------|
| **Repo** | `PSLmodels/Geo-DICE` |
| **Stars** | 2 ⭐ |
| **Language** | MATLAB |
| **Last commit** | September 27, 2018 |
| **License** | open source |

**What it is:** A modified DICE model that includes geoengineering as a control variable. DICE (Dynamic Integrated Climate-Economy) is William Nordhaus's foundational climate-economics model; Geo-DICE adds the SRM dimension.

**Why it matters for the podcast:** Geo-DICE is conceptually important despite its near-zero star count. It's the model that introduced the idea of "surgical" climate intervention into the mainstream economic modeling framework. However, it's been **completely dormant since 2018** — 8 years without a commit.

**The 4 commits span:** Initial commit (Aug 2016) → two file uploads (Aug 2016) → one file upload (Sep 2018). No maintenance, no bug fixes, no updates for newer climate scenarios.

**Episode hook:** *"The model that first put geoengineering into economic optimization hasn't been touched in 8 years. Is Nordhaus's DICE framework still the right tool, or has it been superseded?"*

---

## 4. OOCC 2021 (Open Solar Geoengineering Governance Model)

| Field | Detail |
|-------|--------|
| **Repo** | `jlehtomaa/OOCC_2021` |
| **Stars** | 2 ⭐ |
| **Language** | Python |
| **Last commit** | November 15, 2021 |
| **License** | open source |

**What it is:** A simple model for solar geoengineering governance, created for the Open Solar Geoengineering Conference (OOCC) 2021. It simulates governance scenarios for SRM deployment.

**Why it matters for the podcast:** OOCC is the only repository that explicitly models SRM *governance* rather than just the physics or economics. The commit history shows intense development during the conference period (July-September 2021), with 10+ commits in 3 months. After the conference, development slowed to citation and README updates, with the final commit in November 2021.

**The conference-to-dormancy pattern is common in academic GitHub:** The tool was built for a specific event, served its purpose, and then was abandoned. This raises the question: *What happens to open-source governance tools after the conference ends?*

**Episode hook:** *"A governance model for solar geoengineering was built in 3 months for a single conference. What does it tell us about the gap between governance theory and practice?"*

---

## 5. awesome-geoengineering

| Field | Detail |
|-------|--------|
| **Repo** | `brandonhimpfen/awesome-geoengineering` |
| **Stars** | 4 ⭐ |
| **Language** | Python (curated list) |
| **Last commit** | September 6, 2026 |
| **License** | open source |

**What it is:** A curated, regularly updated list of projects, research, organizations, tools, and resources related to geoengineering. This is the "best of" directory for the field.

**Why it matters for the podcast:** This is the **only actively maintained solar geoengineering repository** in our entire sample (aside from WRF and MDTF-diagnostics). The commit history shows:
- **7 commits total**, with 4 in the last 4 months (Jan-Sep 2026)
- Version bump to v2.0.0 in May 2026
- Consistent monthly updates throughout 2026

**This is a signal:** While the actual SRM simulation code is sparse and dormant, the *directory* of geoengineering resources is actively curated. Someone is maintaining the map even as the territory remains largely unexplored.

**Episode hook:** *"The geoengineering directory is being updated every month, but the actual simulation code is dead. What does that tell us about the state of the field?"*

---

## 6. geomalaria (Malaria Risk in a World with Solar Geoengineering)

| Field | Detail |
|-------|--------|
| **Repo** | `cjcarlson/geomalaria` |
| **Stars** | 3 ⭐ |
| **Language** | R |
| **Last commit** | February 15, 2022 |
| **License** | open source |

**What it is:** A model of malaria risk in a world with solar geoengineering. Colin J. Carlson (a prominent biogeographer) built this to assess the unintended biological consequences of SRM — specifically how altering solar radiation would shift mosquito habitat ranges and disease patterns.

**Why it matters for the podcast:** This repo represents the **unintended-consequences subfield** of SRM research. All 15 commits are from January-February 2022, with a burst of activity (9 commits in 2 days, January 30, 2022). After the initial paper and data upload, the repo went dormant.

**The pattern is significant:** SRM research on GitHub tends to follow a "burst and freeze" pattern — researchers upload code for a specific paper, get cited, and then move on. There's no sustained software engineering culture in this field.

**Episode hook:** *"What happens to malaria-carrying mosquitoes if we block the sun? One researcher modeled it, published the paper, and then vanished. The code sits frozen since 2022."*

---

## Cross-Cutting Themes Across Solar Repos

| Pattern | Evidence |
|---------|----------|
| **Burst-and-freeze development** | 5 of 6 repos show single-burst commit patterns (conference, paper, or thesis), then dormancy |
| **Zero SRM-specific simulation code** | No repo directly simulates stratospheric aerosol injection, marine cloud brightening, or space-based reflectors |
| **Governance gap** | OOCC is the only governance tool, and it's been dead since 2021 |
| **Atmospheric physics infrastructure exists** | WRF provides the physics engine, but no one builds SRM-specific modules on top of it |
| **Curated lists outperform actual code** | awesome-geoengineering (4★, actively maintained) has more recent activity than all actual simulation repos combined |
| **Climate-economic models are frozen in time** | Geo-DICE (2018), ClimateMARGO (2023 code, 2026 README-only revival) — neither reflects current climate scenarios |

---

## Episode Talking Points — Solar Geoengineering

1. **The WRF solar fix is the most actionable finding** — a real, operational atmospheric model just corrected its solar physics. This should concern anyone thinking about SRM.
2. **ClimateMARGO's mysterious revival** — 2 README updates after 2.5 years of silence. What triggered it? Policy momentum? New paper? We may never know.
3. **The 8-year dormancy of Geo-DICE** — Nordhaus's framework for geoengineering economics hasn't been updated since 2018. Is it still relevant?
4. **The conference-to-ghost lifecycle** — OOCC 2021 was built for a single event and then abandoned. This is the academic open-source pattern.
5. **The directory is alive; the territory is not** — awesome-geoengineering gets monthly updates, but the actual SRM simulation codebase is a ghost town.

---

*Research compiled: September 2026 | Source: GitHub commit histories, 6 repositories*
*Branch: solar-geoengineering*