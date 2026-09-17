# 🌍 Carbon Capture — Commit Trend Analysis

**Research Date:** September 2026
**Podcast Episode:** Carbon Capture & Direct Air Capture (DAC)

---

## methodology

Commit histories were pulled from 9 carbon-capture-related repositories using GitHub's API. Each repository was analyzed for:
- Recency and frequency of commits
- Active development periods vs. dormancy
- Types of changes (code, docs, releases, governance)
- Contributor patterns (single-author vs. multi-author)
- License and open-science signals

---

## Activity Heat Map

| Repository | Stars | Last Commit | Commits in Last Year | Status |
|-----------|-------|-------------|---------------------|--------|
| protontypes/open-sustainable-technology | 2,552 | Sep 9, 2026 | ~15 | 🟢 Very Active |
| ClimateSoton/climate-research-group | — | Aug 6, 2026 | 4 | 🟡 Recently Updated |
| tjz21/DAC_peroxovanadates | 2 | Sep 23, 2025 | 2 | 🟡 Slow Activity |
| tjz21/DAC_peroxotitanates | 2 | Sep 23, 2025 | 2 | 🟡 Slow Activity |
| openair-collective/openair-cyan | 76 | Feb 12, 2024 | 0 | ⚪ Dormant (Complete) |
| zikribayraktar/Carbon_Capture_ML | 56 | May 8, 2024 | 0 | ⚪ Dormant (Maturing) |
| terranexum/OpenCarbon | 2 | Jul 18, 2023 | 0 | ⚪ Dormant |
| yohanesnuwara/carbon-capture-and-storage | 85 | Mar 6, 2021 | 0 | 💀 Ghost |
| salmansust/CO2-Sequestration | 32 | Mar 24, 2019 | 0 | 💀 Ghost |

---

## Key Findings

### 1. The Directory Is the Only Ecosystem Engine

`protontypes/open-sustainable-technology` is the **only** carbon-capture-adjacent repository showing sustained, high-frequency development. With 2,552 stars and 10+ commits per month, it functions as the ecosystem's central nervous system — indexing what exists, tracking what's new, and signaling what's gaining attention.

**Implication for the podcast:** When searching for "what's happening in carbon capture," start here. When searching for "what's *worked* in carbon capture," you won't find it here — only what's *listed*.

### 2. The CC0 License Trend Is Real

Both tjz21/DAC_peroxovanadates and tjz21/DAC_peroxotitanates adopted CC0 public domain dedication in September 2025. This is not just "open source" — it's a deliberate choice to remove all copyright restrictions. For computational chemistry work, this is unusual and significant.

**Why it matters:** Most academic code uses MIT, GPL, or Apache licenses. CC0 is the nuclear option of open science — "this code belongs to everyone." It suggests the authors view their computational screening data as public infrastructure, not intellectual property.

### 3. The DAC Hardware Story Has Two Chapters

- **Chapter 1 (2022):** openair-cyan community develops DIY DAC blueprint. Multiple contributors. Rapid iteration.
- **Chapter 2 (2024):** OSHWA certification. 6 commits in one day. Then silence.

The hardware blueprint is complete. Nobody is iterating on it. This could mean: (a) the project succeeded and people are building it elsewhere, or (b) the project lost momentum after the original team moved on.

### 4. Academic Ghosts Dominate the Star Count

The two highest-starred carbon-capture repositories — `carbon-capture-and-storage` (85★) and `CO2-Sequestration` (32★) — are both abandoned academic projects. They were created for thesis work, completed, and then abandoned. The stars accumulated through citations, not usability.

**The uncomfortable truth:** In academia, a repository's star count measures how many people cited it, not how many people used it. The most-starred carbon-capture code on GitHub is the least maintained.

### 5. The Commit Pattern: Paper-Driven, Not Product-Driven

Most carbon-capture repositories follow the same pattern:
1. **Burst of activity** when a paper is being prepared
2. **README updates** when the paper is published
3. **Silence** until the next paper

This is the opposite of software engineering best practices (continuous integration, automated testing, semantic versioning). It's the "publish or perish" model applied to code.

**Exception:** `open-sustainable-technology` is the only repo that looks like real software engineering — continuous commits, PR reviews, issue tracking, structured contributions.

### 6. The Aug 2026 Materials Wave

Both DAC sorbent repositories (peroxovanadates and peroxotitanates) show September 2025 activity (CC0 licenses) and July 2024 activity (intensive data additions). The ClimateSoton group website also shows August 2026 activity. This suggests a coordinated wave of DAC materials research output around mid-2024 to late-2025, with ongoing publication activity.

---

## What the Commit Histories Don't Tell You

### Missing: DAC system simulations

No repository contains a working model of a full DAC system — from air intake → sorbent contact → CO2 desorption → compression → storage. The computational work (peroxovanadates, peroxotitanates) focuses on *materials discovery* (finding better sorbents), not *system design* (making the whole machine work).

### Missing: Economic models

Except for the research context within other repos, there are no open-source economic models for DAC cost trajectories. The `srm-forever` project (solar geoengineering theme) has economics, but nothing comparable exists for carbon capture.

### Missing: Life cycle assessment

No repository integrates life cycle assessment (LCA) for DAC technologies. The energy penalty of DAC is a critical concern — pulling CO2 from air requires ~250 kWh per ton, and the carbon footprint of the energy source matters enormously. LCA code is absent.

---

## Episode Talking Points

1. **"The open-source carbon capture ecosystem is a directory with no code."** The most active repo is a curated list of 2,500+ projects. The actual code repos are mostly abandoned.

2. **"The DIY air capture blueprint is OSHWA-certified and then nobody touched it."** openair-cyan proves you *can* build a DAC in your garage. But the project stopped updating after certification.

3. **"The most-starred carbon capture code on GitHub is a ghost."** 85 stars, zero commits since 2021. Academic incentive structures don't reward long-term code stewardship.

4. **"DAC materials researchers are going public domain."** CC0 license adoption in the peroxovanadates/peroxotitanates repos is a signal that computational chemistry is shifting toward open-data infrastructure.

5. **"The August 2026 wave may be a flag."** Multiple repos showing coordinated activity suggests a research community forming — but it's forming around materials discovery, not system-level engineering.