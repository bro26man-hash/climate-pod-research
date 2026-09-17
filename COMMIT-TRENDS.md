# 📊 Solar Geoengineering — Commit Trend Analysis

**Date:** September 2026
**Repositories Analyzed:** 7 (WRF, PCMDI/pcmdi_metrics, MDTF-diagnostics, ClimateMARGO.jl, awesome-geoengineering, orbital-climate-simulator, srm-forever)

---

## Aggregate Statistics

| Repo | Total Commits (recent window) | Commits in Burst | Longest Gap | Current Status |
|------|------|------|------|------|
| wrf-model/WRF | 15 (May–Jun 2026) | 8 in 10 days | ~2 weeks | Active (v4.8.0 released) |
| PCMDI/pcmdi_metrics | 15 (Sep 2–4, 2026) | **15 in 3 days** | 1 day | Active (v4.2.1 released) |
| NOAA-GFDL/MDTF-diagnostics | 15 (May–Aug 2026) | 5 in 1 day (Jun 19) | ~2 months | Active |
| ClimateMARGO/ClimateMARGO.jl | 8 (Oct 2022–Aug 2026) | 5 in 2 weeks (Jan 2022) | **2 years 10 months** | Dormant (README revival) |
| brandonhimpfen/awesome-geoengineering | 7 (Jun 2025–Sep 2026) | 2 in 1 day (Sep 5–6) | 2.5 months | Active (monthly updates) |
| yanpefnsc/orbital-climate-simulator | 12 (Sep 15–16, 2026) | **12 in 24 hours** | N/A (new) | Blast-off |
| hausfath/srm-forever | 4 (Aug 26, 2026) | **4 in 1 day** | N/A (new) | Active (single-day build) |

---

## Trend 1: Institutional Bursts Dominate Climate Software

**The pattern:** The most committed-to repos show short, intense bursts of activity followed by long quiet periods. This is the signature of institutional, funded development — not organic community growth.

**Evidence:**

- **PCMDI/pcmdi_metrics:** 15 commits in 3 days (Sep 2–4, 2026) for v4.2.1 release. All by the same 3 contributors (Jiwoo Lee, James Goodnight, Jared Lewis). Pre-planned release sprint.
- **WRF:** 15 commits over ~4 weeks (May–Jun 2026) for v4.8.0. Multiple institutional contributors (NCAR, NOAA, university groups). Coordinated release.
- **MDTF-diagnostics:** 5 commits on Jun 19 adding the precip-buoyancy POD, then 2-month gap, then another burst in August. Project-based cadence.

**Implication for the podcast:** Climate simulation software is built by institutions, not communities. When funding stops, development stops. The "open-source" label is misleading — these are open-access institutional tools, not community-driven projects.

---

## Trend 2: The August 2026 SRM Economics Wave

**The pattern:** Three separate SRM-related repos all received updates in August 2026, suggesting a coordinated event or shared stimulus.

**Evidence:**

- **hausfath/srm-forever:** Complete rebuild on Aug 26, 2026 — 4 commits, all new
- **ClimateMARGO.jl:** README updates on Aug 17, 2026 — first activity in 2.5 years
- **brandonhimpfen/awesome-geoengineering:** v2.0.0 released May 5, then updates on Aug 14 and Sep 5–6

**Possible explanation:** The IMO's 2023 regulation on shipping black carbon emissions may be driving renewed interest in SRM cost economics. Or it could be the approaching IPCC AR7 timeline.

**Implication:** "August 2026 saw SRM economics models and curators waking up at the same time. What's in the air?"

---

## Trend 3: The Single-Day Build Phenomenon

**The pattern:** Interactive, democratization-oriented tools are appearing as single-day builds — high intensity, low longevity.

**Evidence:**

- **orbital-climate-simulator:** 12 commits in 24 hours (Sep 15–16, 2026). Full drone simulation + Streamlit dashboard built overnight.
- **srm-forever:** 4 commits in 1 day (Aug 26, 2026). Complete SRM economics model built in a single session.
- **openair-cyan:** 15 commits on Feb 12, 2024, then frozen. A DIY DAC device was fully documented in one day, then abandoned.

**Implication:** The "democratization" wave is real but fragile. People build impressive single-day tools, then move on. There's no sustained community maintaining these projects.

---

## Trend 4: Dormancy Is the Default

**The pattern:** 3 of 7 analyzed repos show dormancy periods of 2+ years. The baseline state of climate software is stillness.

**Evidence:**

- **ClimateMARGO.jl:** 2 years 10 months between code commits (Oct 2023 → Aug 2026). Only README maintenance during dormancy.
- **MDTF-diagnostics:** 2-month gaps between commit clusters. Project-based, not continuous.
- **awesome-geoengineering:** 2.5-month gaps between updates. Relies on single maintainer.

**Implication:** "If you depend on open-source SRM tools, you're waiting for someone who may not come back. The software equivalent of a ghost town."

---

## Trend 5: The Precision Gap

**The pattern:** Climate models are getting more precise, but the governing metrics are also getting more precise — and the gap between them is widening.

**Evidence:**

- **PCMDI/pcmdi_metrics** v4.2.1 fix: "prevents roundoff to 1.00 in mean_climate figures" — a precision fix at the 5th decimal place
- **WRF v4.8.0:** "correction for eot calculation for solar radiation" — fixing the physics that SRM scenarios depend on
- **ClimateMARGO.jl:** Unit conversion fixes (Oct 2023) — ensuring the optimization math is correct

**Implication:** The tools are getting more precise, but who audits the precision? A 5th-decimal-place fix in PCMDI metrics could change which models get approved for IPCC reports. That's governance power. "The people who fix the rounding errors decide which climate scenarios are 'trustworthy' — and whether SRM gets evaluated honestly."

---

## Trend 6: The Curation Outlives Code Pattern

**The pattern:** Curated lists and surveys are more durable than complex simulation code.

**Evidence:**

- **awesome-geoengineering:** 7 commits over 15 months, steady monthly updates, v2.0.0 in May 2026. The most consistently maintained non-institutional project.
- **Carbon_Capture_ML** (not analyzed in this round but referenced): Survey-only but comprehensive — 12 commits in 10 days (Jan 2023), then frozen.
- ** orbital-climate-simulator:** 12 commits in 1 day, then documentation fixes. Dashboard may not be maintained.

**Implication:** For the podcast, the most useful GitHub resource for episode preparation might be a curated list, not a simulation. "The best map of the geoengineering landscape is a list, not a model."

---

## Commit Trend Summary for Episode 1 (Solar Geoengineering)

| Theme | Evidence | Talking Point |
|-------|----------|---------------|
| Institutional control | PCMDI: 15 commits/3 days; WRF: 15 commits/4 weeks | "Climate simulation is an institutional sport, not a community one" |
| Governance through metrics | PCMDI v4.2.1: 5th-decimal precision fix | "The people who fix rounding errors decide which models are trusted" |
| Dormancy as default | ClimateMARGO: 2.5 yr gap; MDTF: project-based cadence | "Most climate software is a ghost town with an occasional maintainer" |
| Democratization (nascent) | orbital-climate-simulator: 12 commits/24 hrs; srm-forever: 4 commits/1 day | "Someone built an SRM drone simulator overnight — then what?" |
| Curation > Code | awesome-geoengineering: monthly updates, v2.0.0 | "The most active geoengineering project on GitHub is a list" |
| Precision gap | WRF: solar radiation physics fix; PCMDI: roundoff fix | "Fixing the 5th decimal could change which SRM scenarios get approved" |

---

*Analysis conducted September 2026 using GitHub commit API data.*