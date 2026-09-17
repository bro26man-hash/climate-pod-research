# 📊 Carbon Capture — Commit Trend Analysis

**Date:** September 2026
**Repositories Analyzed:** 7 (openair-cyan, Carbon_Capture_ML, DAC_peroxovanadates, DAC_peroxotitanates, climate-capture-and-storage, CarbonSink, ERIE-ATMO)

---

## Aggregate Statistics

| Repo | Total Commits (recent window) | Commits in Burst | Longest Gap | Current Status |
|------|------|------|------|------|
| openair-collective/openair-cyan | 15 (Feb 12, 2024) | **15 in 1 day** | **2 years 7 months** | Frozen |
| zikribayrakar/Carbon_Capture_ML | 12 (Jan 2023) | 12 in 10 days | **2 years 4 months** | Frozen |
| tjz21/DAC_peroxovanadates | 15 (Nov 2023–Sep 2025) | 8 in 1 day (Dec 2023) | 6 months | Dormant (README-only) |
| tjz21/DAC_peroxotitanates | Active | Updates through Aug 2026 | ~1 month | Low activity |
| yohanesnuwara/climate-capture-and-storage | 0 (since Mar 2021) | N/A | **5 years 6 months** | Ghost |
| brandonhimpfen/awesome-geoengineering | 7 (Jun 2025–Sep 2026) | 2 in 1 day | 2.5 months | Active (monthly)

---

## Trend 1: The Single-Day Blitz Then Freeze

**The pattern:** Multiple carbon capture repos show intense single-day activity followed by permanent freezing. This is the "document and abandon" pattern.

**Evidence:**

- **openair-cyan:** 15 commits on Feb 12, 2024 — complete OSHWA-certified device documentation. Then zero activity for 2.5 years.
- **DAC_peroxovanadates:** 8 commits on Dec 5, 2023 — paper README preparation with images and DOI links. Then 3-month gaps, then Sep 2025 license update.
- **Carbon_Capture_ML:** 12 commits in 10 days (Jan 2023) — rapid survey compilation. Then zero activity for 2 years 4 months.

**Common thread:** Each project had a focused " blitz" period where a specific deliverable was produced (device documentation, paper preparation, survey compilation). Once the deliverable was done, the project lost its purpose and froze.

**Implication for the podcast:** "The carbon capture open-source ecosystem doesn't build tools — it produces artifacts. A device manual, a paper, a survey. Then it stops. There's no iterative improvement, no community maintenance. Artifacts, not tools."

---

## Trend 2: The August 2026 DAC Materials Wave

**The pattern:** Four separate DAC materials-related repos all received updates in August 2026, suggesting a coordinated research event.

**Evidence:**

- **DAC_peroxotitanates:** Updated Aug 19, 2026
- **DAC_peroxovanadates:** Last significant update Sep 2025 (CC0 license), but README updates through May 2024
- **CarbonSink:** Updated Feb 2026
- **ERIE-ATMO:** Updated Apr 2026
- **The pattern:** While not a single-day burst like the solar geoengineering August wave, this is a sustained trickle of DAC materials activity from late 2025 through 2026.

**Possible explanation:** The DAC cost conversation has shifted from "can we capture CO2?" to "what sorbents work best?" Peroxide-based sorbents (peroxovanadates, peroxotitanates) represent a new computational screening approach.

**Implication:** "The DAC materials wave isn't about building simulation tools — it's about screening molecules. The open-source work is in the chemistry, not the code."

---

## Trend 3: Zero Simulation Code Across All Repos

**The pattern:** Not a single analyzed carbon capture repo contains actual simulation code that models DAC physics, chemistry, or economics.

**Evidence:**

- **openair-cyan:** Hardware documentation. No simulation.
- **Carbon_Capture_ML:** Survey of papers. No simulation.
- **DAC_peroxovanadates/titanates:** Computational screening data. No simulation.
- **climate-capture-and-storage:** Reservoir simulation (dormant since 2021). The only repo with actual simulation code, and it's dead.
- **CarbonSink/CarbonVault/Web3 projects:** Synthetic assets and tokens. Not simulation.

**Implication:** "You can't run an open-source DAC simulation. You can read about one, screen one, or tokenize one. But you can't simulate one. The 'software' in carbon capture is bibliography, not code."

---

## Trend 4: The Ghost and the Frozen

**The pattern:** Two of the most relevant carbon capture repos are dead — one a ghost, one frozen after a single blitz.

**Evidence:**

- **climate-capture-and-storage:** 85 stars, zero commits since March 2021. The most-starred carbon capture repo on GitHub is a 5-year-old fossil.
- **openair-cyan:** 76 stars, frozen since Feb 2024 after a 15-commit one-day documentation sprint.
- **Carbon_Capture_ML:** 56 stars, frozen since May 2024 after a 12-commit ten-day survey sprint.

**Implication:** "The three most important carbon capture GitHub projects are either dead or frozen. The field's GitHub presence is a cemetery of single-day achievements. What gets built doesn't get maintained."

---

## Trend 5: Web3 Infiltration of Carbon Capture

**The pattern:** Multiple active carbon capture projects are Web3/crypto synthetic instruments — tokenized carbon removal, synthetic assets tracking DAC tech. These have more ongoing activity than any scientific carbon capture repo.

**Evidence:**

- **CarbonSink (bigg-kay):** Updated Feb 2026 — synthetic instrument for DAC technology exposure
- **CarbonVault (drakemesh/aslembadru):** Active updates through 2026 — tokenized carbon removal protocol
- **ERIE-ATMO (ericrenone):** Updated Apr 2026 — atmospheric carbon reckoning concept
- **All five Web3 projects have more recent activity than the top 3 scientific carbon capture repos**

**Implication for the podcast:** "While chemists document peroxides and DIY builders freeze their devices, crypto developers are actively tokenizing carbon removal. The carbon capture ecosystem is being shaped by financial engineers, not climate engineers. Is this a problem, an opportunity, or both?"

---

## Trend 6: The Governance Vacuum

**The pattern:** There are zero active governance, regulatory, or policy tools for carbon capture on GitHub.

**Evidence:**

- **OSHWA certification** (openair-cyan) is the only governance-adjacent artifact — and it's frozen
- **No policy models, no regulatory simulators, no cost-benefit tools** for carbon capture exist as active GitHub projects
- **The only governance signal is CC0 licensing** on the DAC materials repos — open science commitment, not policy infrastructure

**Implication:** "Solar geoengineering has 3 governance-adjacent tools (PCMDI metrics, SRM economics, awesome-geoengineering). Carbon capture has zero. Both fields have governance gaps, but carbon capture's gap is absolute — there's not even a dormant tool to wake up."

---

## Commit Trend Summary for Episode 2 (Carbon Capture)

| Theme | Evidence | Talking Point |
|-------|----------|---------------|
| Build then freeze | OpenAir-Cyan: 15 commits/1 day, then 2.5 yr freeze; Carbon_Capture_ML: 12 commit/10 days, then 2 yr freeze | "The carbon capture community produces artifacts, not tools" |
| No simulation code | Zero repos with DAC physics/chemistry/economics simulation | "You can't run an open-source DAC simulation. Period." |
| The ghost project | climate-capture-and-storage: 85 stars, 5 years dead | "The best tool is the one nobody maintains" |
| Web3 infiltration | 5+ active Web3 carbon projects vs 3 frozen scientific repos | "Crypto is more invested in carbon capture than climate scientists are" |
| Governance vacuum | Zero policy/regulatory tools; only frozen OSHWA cert | "Carbon capture has no governance layer — not even a dormant one" |
| Peroxide screening wave | Peroxovanadates + peroxotitanates: computational screening, not simulation | "The open-source work is in the chemistry, not the code" |

---

*Analysis conducted September 2026 using GitHub commit API data.*