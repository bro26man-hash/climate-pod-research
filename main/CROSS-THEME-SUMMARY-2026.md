# 🎙️ Cross-Theme Research Summary (September 2026)

## Overview
This document synthesizes commit trend findings from three podcast theme branches: solar geoengineering (☀️), carbon capture (🌍), and ocean intervention (🌊). Together, we analyzed 18+ repositories across 6 search strategies.

---

## 📊 Grand Total: What We Found

| Theme | Repos Searched | Active Repos | Total Stars (top 5) | Governance Code | Open Hardware |
|-------|---------------|-------------|--------------------|-----------------|--------------|
| ☀️ Solar Geoengineering | 10 | 4 | 1,950+ | 2 (both frozen) | Some SRM experiments |
| 🌍 Carbon Capture | 10 | 5 | 254+ | Some policy tools | OpenAir-Cyan (OSHWA) |
| 🌊 Ocean Intervention | 8 | 0 | 0 | 0 | 0 |
| **Total** | **28** | **9** | **2,200+** | **2 working** | **1 project** |

---

## 🔥 Top 5 Commit Trend Stories (September 2026)

### 1. The Institutional Burst Pattern
**WRF:** 15 commits in 4 weeks (v4.8.0 release, May-Jun 2026)
**PCMDI:** 15 commits in 3 days (v4.2.1 release, Sep 2-4, 2026)
**MDTF-diagnostics:** 10 commits in 3 months (precip-buoyancy POD, Jun 2026)

**Pattern:** All institutional, all funded, all releasing on schedule. Community-driven climate software is the exception.

**Why it matters for the podcast:** Climate code is not a "lonely genius" story. It's institutional infrastructure. The big models are maintained by national labs and agencies.

### 2. The August 19th Mystery (Carbon Theme)
Four DAC materials repos (peroxovanadates, peroxotitanates, OpenCarbon, Carbon-Capture-Genome) all updated on **August 19, 2026**.

**Pattern:** Simultaneous activity across small, unconnected repos. Most likely a shared publication or dataset drop.

**Why it matters:** The smallest, most specialized research groups are moving fast on DAC materials. The peroxovanadate family is emerging as the hot direction. But it's paper-driven, not community-driven.

### 3. The ClimateMARGO Revival Signal (Solar Theme)
ClimateMARGO went dormant for 2.5 years (Apr 2023 - Aug 2026), then got 2 README updates in August 2026.

**Pattern:** Someone came back to the codebase. The question is: was it a student finding old references, a researcher updating for a new paper, or an automated bot?

**Why it matters:** ClimateMARGO is a climate-economic modeling framework in Julia. If someone is updating it, they might be incorporating SRM scenarios for the first time.

### 4. The OSHWA Certification Freeze (Carbon Theme)
OpenAir-Cyan got 15 commits on February 12, 2024 (OSHWA certification), then zero activity since.

**Pattern:** Certification as a one-time event, not a sustainable development model. The finish line became the endpoint.

**Why it matters:** Open hardware is hard. You can certify the hardware, but you can't certify the community. The project needs ongoing maintenance, not just a certification badge.

### 5. The Ocean Silence (Ocean Theme)
**Zero repositories found across 8 search queries.** Not one project.

**Pattern:** Systematic absence. The ocean is the untapped quadrant.

**Why it matters:** This is the podcast's defining finding. If we can't simulate ocean interventions, we can't evaluate them, and if we can't evaluate them, we can't govern them. The code gap is a governance gap.

---

## 🧹 Governance Gap: The Meta-Finding

Across all three themes, governance code is systematically absent:

| Type | Solar | Carbon | Ocean |
|------|-------|--------|-------|
| SRM/ERM governance tools | 2 (frozen) | 0 | 0 |
| Affordability/cost modeling | 0 | Some (CCS_article, frozen) |
| Verification/MRV tools | 0 | 0 | 0 |
| Lifecycle assessment code | 0 | 0 | 0 |
| Policy feasibility models | Geo-DICE (frozen) | Some (frozen) | 0 |
| Interactive decision tools | srm-forever (tiny) | 0 | 0 |

**One working governance tool in the entire climate tech GitHub ecosystem: 45Q tax credit modeling in CCS_article (also frozen).**

---

## 🧹 Dormancy is the Default

| Repo | Stars | Last Activity | Status |
|------|-------|---------------|--------|
| yohanesnuwara/carbon-capture-and-storage | 85 | Mar 2021 | 5-year ghost |
| jlehtomaa/OOCC_2021 | 2 | Nov 2021 | 5-year ghost |
| antara-banerjee/GeoengineeringLE_WinterWarming | 2 | Apr 2021 | 5-year ghost |
| PSLmodels/Geo-DICE | 2 | Sep 2018 | 8-year ghost |
| openair-collective/openair-cyan | 76 | Feb 2024 | 2.5-year ghost |
| zikribayraktar/Carbon_Capture_ML | 56 | May 2024 | 2-year ghost |
| tonyzyl/CO2-Soft-Sensor | 16 | Aug 2022 | 4-year ghost |
| pixnum-hub/GeoVision | - | Dec 2025 | 10-month flash |

**15 of 18 repositories show no meaningful activity in the last year.**

---

## 🧹 Curation Outlives Code

| Project | Type | Activity | Sustainability |
|---------|------|----------|---------------|
| awesome-geoengineering | Curated list | 7 commits / 14 months | ✅ Healthy |
| Carbon_Capture_ML | Survey + links | 12 / 10 days, then seasonal | ⚠️ Moderate |
| ClimateMARGO | Economic model | Revival signal | ❓ Unknown |
| WRF | GCM | 15 / 4 weeks | ✅ Very Healthy |
| MDTF-diagnostics | Diagnostics | 10 / 3 months | ✅ Healthy |
| GeoVision | Simulator | 4 / 1 day | ❌ Dormant |
| GeoengineeringLE_WinterWarming | Analysis code | 10 / 1 month | ❌ Dormant |
| Geo-DICE | Economic model | 4 / 2 years | ❌ Dormant |
| OpenAir-Cyan | Open hardware | 15 / 1 day | ❌ Frozen |

**The pattern: Curation and infrastructure survive. Complex simulations don't.**

---

## 🔮 What's Trending (Where Development is Headed)

### Solar Geoengineering
- **Direction:** Better atmospheric physics (aerosol-cloud interactions, solar radiation accuracy)
- **Signal:** WRF's May-Jun 2026 commits fix solar radiation — the core SRM quantity
- **Gap:** No interactive SRM simulators; governance code frozen since 2018
- **Opportunity:** ClimateMARGO revival could bring economic modeling into the Julia ecosystem with SRM scenarios

### Carbon Capture
- **Direction:** LDA materials screening (peroxovanadates, peroxotitanates)
- **Signal:** August 19, 2026 wave — 4 repos simultaneously updated
- **Gap:** No real-data ML models; no system-level planning tools; open hardware frozen at certification
- **Opportunity:** The "peroxovanadate moment" could be the breakthrough that makes amine-free DAC economically viable

### Ocean Intervention
- **Direction:** Nothing. Literally zero.
- **Signal:** The absence itself is the signal
- **Gap:** No simulation tools, no governance code, no open hardware, no community
- **Opportunity:** The first committed open-source OAE simulator could change everything — and the podcast could be the catalyst

---

## 🎙️ Episode Planning (Final)

| Episode | Branch | Core Question | Key Evidence |
|---------|--------|---------------|-------------|
| **Solar Geoengineering** | solar-geoengineering | "Why is the code for fixing the climate's thermostat so much better than the code for governing it?" | WRF v4.8.0 (15 commits, solar radiation fix); governance tools frozen since 2018; awesome-geoengineering is the only healthy project |
| **Carbon Capture** | carbon-capture | "Is open-source carbon capture stuck between frozen academic code and a materials wave we can't see coming?" | 85-star ghost project; OSHWA certification freeze; August 19th wave; synthetic data bottleneck |
| **Ocean Intervention** | ocean-intervention | "What happens when the most important climate technology on GitHub has zero repositories?" | 8 searches, 0 results; MDTF as only ocean-adjacent tool; no governance, no community, no code |

---

## 📋 Updated Research Log

| Date | Activity |
|------|----------|
| 2026-09-03 | Repository created; initial research notes pushed to all branches |
| 2026-09-17 | Full commit trend analysis from 8 repositories; all branch notes updated with detailed commit data |
| 2026-09-17 | Second research round: additional commit histories pulled from 7 more repositories across all themes |
| 2026-09-17 | Ocean gap analysis: 8 search queries confirm zero ocean geoengineering repos; pushed to ocean-intervention branch |
| 2026-09-17 | Cross-theme synthesis: identified 5 headline trends, governance gap analysis, and periodic table of climate tech sustainability |
| 2026-09-17 | **This update:** Comprehensive commit trend analysis from 15+ repositories; all branch files updated; cross-theme summary pushed to main |

---

*Last updated: September 2026 based on GitHub commit data from 15+ repositories across all three themes.*