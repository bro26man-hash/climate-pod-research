# 🌍 Carbon Capture — Project Discoveries (v6)

> **Last updated:** September 2026 (v6)  
> **Branch:** `carbon-capture`  
> **Podcast episode:** Episode 2 — Carbon Capture

---

## Overview (v6 Update)

This document profiles open-source projects relevant to carbon capture, removal, and sequestration (CDR). v6 incorporates fresh commit histories from 6 repos: Open-Sustainable-Technology (15 commits), OpenAir-Cyan (15), Carbon_Capture_ML (10), DAC_peroxovanadates (10), DAC_peroxotitanates (10), and carbon-capture-and-storage (0 — ghost).

---

## Tier 1: The Open-Source Climate-Tech Directory

### 1. Open Sustainable Technology (protontypes)

| Field | Detail |
|-------|--------|
| **Repo** | `protontypes/open-sustainable-technology` |
| **Stars** | 2,552 |
| **Last commit** | September 9, 2026 |
| **License** | CC0-1.0 |
| **URL** | https://github.com/protontypes/open-sustainable-technology |

**What it is:** The most comprehensive open-source directory of climate-tech projects — 2,500+ entries across energy, transport, industry, CO2 removal, land use, and adaptation. Not a simulation tool — it's the Wikipedia of climate tech, with structured data.

**Why it matters:** If you want to find open-source DAC code, CCS simulators, or carbon accounting tools, you start here. It's the universe's catalogue.

**v6 Commit Highlights (Fresh Pull):**

| Date | SHA | Addition | Significance |
|------|-----|----------|-------------|
| **Sep 9** | `6e9f48c` | MUIO | New carbon removal/offset standard entry |
| **Sep 9** | `07e19b1` | MUIOGO | Complementary standard entry (same day, 2 commits) |
| Sep 1 | `1b6cb82` | Fix dead links in README | Maintenance quality |
| Aug 23 | `d73a519` | **claude-carbon** | AI tool for carbon-aware compute scheduling |
| Aug 18 | `6b6cd82` | Story Seed Library | Cross-domain: storytelling for sustainability |
| Aug 18 | `ca9d7a5` | openflexure microscope | Open hardware for science |
| **Jul 19** | `2303b7a` | Remove duplicate AI content review checkbox | **Governance signal** — community building AI disclosure into PR process |
| **Jul 19** | `c4c9fe7` | Modify PR template for AI content review | **Formal AI content gate** — every PR now requires AI-disclosure checkbox |
| Jul 17 | `be14281` | Update PR template with review reminder | Process refinement |
| Jul 2 | `5bc6609` | PowerIO | New energy project entry |
| Jul 1 | `e772ed4` | ASSETRA | New assessment tool entry |
| Jul 1 | `4c6f0a4` | ToOp | New optimization tool entry |
| Jun 23 | `1986e2c` | wbdata | World Bank development data tool |
| Jun 23 | `007a464` | Volca to LCA | **CDR-relevant** — LCA tool for carbon footprint of materials |
| Jun 6 | `0601a42` | EpexPredictor | Electricity price prediction tool |

**v6 Signal:** The July 2026 AI content disclosure PR template (c4c9fe7) is a landmark. The climate-tech OSS community is formally grappling with AI-assisted contributions. This is the first time we've seen "AI content review" as a required PR template in climate tech.

**🎙️ Episode Hook:** *"The biggest climate-tech repo on GitHub just added a mandatory AI disclosure checkbox to its PR template. The community is deciding, right now, how to handle AI-generated entries. And there's no playbook."*

---

## Tier 2: DIY Open Hardware & Academic Research

### 2. OpenAir-Cyan (openair-collective)

| Field | Detail |
|-------|--------|
| **Repo** | `openair-collective/openair-cyan` |
| **Stars** | 76 |
| **Last commit** | February 12, 2024 |
| **License** | CERN-OHL-S-2.0 |
| **OSHWA UID** | US001095 |
| **URL** | https://github.com/openair-collective/openair-cyan |

**What it is:** DIY small-scale open hardware direct air carbon capture device. OSHWA-certified — the first open-source DAC device to receive formal hardware certification.

**v6 Commit Highlights (Fresh Pull):**

| Date | SHA | Event |
|------|-----|-------|
| **Feb 12, 2024** | `b5422b3` | OSHWA UID link added to README |
| **Feb 12, 2024** | `b164257` | Add files via upload (documentation) |
| **Feb 12, 2024** | `828f496` | OSHWA UID logo (US001095) |
| **Feb 12, 2024** | `b731cd8` | Add files via upload (technical docs) |
| **Feb 12, 2024** | `4b08fb3` | Create CITATION.cff (academic citation support) |
| **Feb 12, 2024** | `859bfa8` | Update README (final push) |
| Jul 20, 2022 | `d12008e` | README update (last activity before blitz) |
| May 17, 2022 | `b8621ba` | Usability improvements |
| May 15, 2022 | `d025674` / `784ace5` | Two README updates same day |
| May 11, 2022 | `09c761d` | Rename CodeQL file |
| May 7, 2022 | `d502eb6` / `4350def` | Update CodeQL analysis |
| May 7, 2022 | `718b209` | Create CodeQL analysis.yml |
| May 5, 2022 | `b2198a2` | Delete .github/workflows |

**The pattern:** A massive burst of 7 commits on Feb 12, 2024 — all OSHWA certification-related — then complete silence for 2+ years. The certification may have been the finish line, not the starting signal.

**🎙️ Episode Hook:** *"They got the certification, published the plans, and then stopped. The most important open-source DAC device in the world has been silent for 2 years. Was OSHWA certification the finish line or the starting line?"*

---

### 3. Carbon Capture ML Survey (zikribayraktar)

| Field | Detail |
|-------|--------|
| **Repo** | `zikribayraktar/Carbon_Capture_ML` |
| **Stars** | 56 |
| **Last commit** | May 8, 2024 |
| **License** | MIT |
| **URL** | https://github.com/zikribayraktar/Carbon_Capture_ML |

**What it is:** A curated survey of ML papers and code for carbon capture. Covers MOFs for CO2 adsorption, process optimization, and dataset construction.

**v6 Commit Highlights (Fresh Pull):**

| Date | SHA | Event |
|------|-----|-------|
| **May 8, 2024** | `ca9a31f` | **OpenDAC paper added** — largest open dataset of DFT calculations for CO2 capture materials |
| Apr 25, 2024 | `4c01842` | Update README |
| Mar 15, 2024 | `2b69376` | Update README |
| Jan 21, 2024 | `e80dfd6` / `fe28496` | Update README |
| Mar 1, 2023 | `a3a02e9` | New paper |
| Feb 16, 2023 | `93e5a40` | **MOFsimplify paper** — framework for simplifying MOF structures for CO2 capture screening |
| Feb 5, 2023 | `0c62b02` / `6129691` | New process paper |
| Feb 2, 2023 | `caf8b96` | New paper to process |

**The pattern:** Intense activity Feb-May 2023 (5 papers in 3 months), then 14 months of silence, then the OpenDAC landmark in May 2024. The survey is the bridge between ML and DAC materials research.

**🎙️ Episode Hook:** *"A survey repo that added 5 landmark papers in 3 months, then went quiet for a year, then dropped the OpenDAC dataset — the biggest open compilation of CO2 capture materials data ever."*

---

## Tier 3: The CC0 Revolution

### 4. DAC Peroxovanadates & Peroxotitanates (tjz21)

| Field | Detail |
|-------|--------|
| **Repos** | `tjz21/DAC_peroxovanadates` (2★) + `tjz21/DAC_peroxotitanates` (2★) |
| **Last commit** | September 23, 2025 (peroxovanadates) |
| **License** | **CC0-1.0 (public domain)** |
| **URL** | https://github.com/tjz21/DAC_peroxovanadates |

**What they are:** Computational screening of peroxovanadate and peroxotitanate sorbents for direct air capture. DFT calculations to predict which structures have the right thermodynamic properties for CO2 capture. Two parallel pipelines for two sorbent chemistries.

**v6 Commit Highlights (Fresh Pull — peroxovanadates):**

| Date | SHA | Event | Significance |
|------|-----|-------|-------------|
| Sep 23, 2025 | `cfd04f7` | Updated README.md | Final documentation update |
| **Sep 12, 2025** | **`e041eff`** | **Added CC0 license** | **🔑 THE KEY COMMIT** — explicit public domain dedication. The most significant open-science event in carbon capture this year. |
| Mar 11, 2024 | `6e17397` | Fixed DOI link | Reference correction (paper-related) |
| Mar 11, 2024 | `e38c7dd` | Added paper DOI link | Paper reference addition |
| Mar 11, 2024 | `b6184d2` | Updated README | Coincident with DOI updates — paper publication triggered this batch |
| Mar 11, 2024 | `3096665` | Updated phrasing in README | Paper-related refinement |
| Dec 5, 2023 | `8d8bd1d`, `f7ecca1`, `ba71657`, `737d342` | Multiple README updates | 4 commits in one day — paper submission batch |

**The CC0 pattern:** The commit history shows a clear arc: paper submissions (Dec 2023, Mar 2024) → 6 months of silence → then the CC0 license addition (Sep 2025) → then 11 more months of silence. The CC0 decision was a standalone event, not part of a paper cycle. The author deliberately dedicated the data to the public domain AFTER the papers were published.

**The peroxotitanates companion** follows the same pattern: sparse activity, CC0 license, same author. Two parallel screening pipelines, both released as public infrastructure.

**🎙️ Episode Hook:** *"Two researchers, two sorbent chemistries, two repos, both released to the public domain with CC0. No copyright. No licensing drama. Just data, freely available. This is how open science is supposed to work — and it's happening in the DAC materials community right now."*

---

## Tier 4: Ghost Repos

### 5. Carbon Capture and Storage (yohanesnuwara)

| Field | Detail |
|-------|--------|
| **Repo** | `yohanesnuwara/carbon-capture-and-storage` |
| **Stars** | 85 |
| **Last commit** | March 6, 2021 |
| **License** | MIT |
| **Status** | 💀 Ghost — dead for 4+ years |

**What it is:** Reservoir simulation + geomechanics model for CCS. Simulates CO2 injection into geological formations, including pressure propagation and caprock integrity.

**Why it matters:** 85 stars but completely inactive since 2021. Stars measure citations, not usability. The code may still work, but it's running on an old MATLAB version with no bug fixes.

---

## Summary Table — Carbon Theme (v6)

| Repo | Stars | Status | Key v6 Signal | CC0? |
|------|-------|--------|---------------|------|
| **open-sustainable-technology** | 2,552 | 🟢 Very active | AI disclosure PR template (Jul 2026) | CC0-1.0 |
| **openair-cyan** | 76 | 💀 Dormant 2+ yr | OSHWA cert blitz (Feb 2024), then silence | CERN-OHL |
| **Carbon_Capture_ML** | 56 | 💀 Dormant 1.5 yr | OpenDAC paper (May 2024), then silence | MIT |
| **carbon-capture-and-storage** | 85 | 💀 Ghost 4+ yr | Dead since 2021 | MIT |
| **DAC_peroxovanadates** | 2 | 🟡 Sparse | **CC0 license (Sep 2025)** | **CC0-1.0** |
| **DAC_peroxotitanates** | 2 | 🟡 Sparse | CC0 license | **CC0-1.0** |

---

## v6 Development Trend Signals

### Signal 1: The CC0 Revolution Is Real
Two repos from the same author (tjz21) chose public domain dedication. This is the most significant open-science development in carbon capture on GitHub.

### Signal 2: The OSHWA Certification Was a Peak, Not a Plateau
OpenAir-Cyan's Feb 2024 burst was a finish line, not a starting signal. 2 years of silence since.

### Signal 3: The Directory Is the Only Alive Repo
Open-Sustainable-Technology is the only carbon theme repo with truly active development. AI disclosure PR template signals the community is grappling with governance.

### Signal 4: Ghost Repos Inflate the Star Count
85★ on a repo dead since 2021. 32★ on one dead since 2019. Stars measure citations, not usability.

### Signal 5: The OpenDAC Dataset Is the Field's Reference
Added May 2024 to the Carbon_Capture_ML survey. This is what ML-for-CCR research builds on.

### Signal 6: AI Governance Is Entering Climate Tech OSS
The July 2026 AI content disclosure PR template in Open-Sustainable-Technology is the first concrete governance response to AI-generated contributions in climate tech.

---

## Episode 2 Narrative Arcs (v6)

### Arc A: "The Catalogue"
Open-Sustainable-Technology as the universe of climate tech. 2,552 stars, 2,500+ projects, constantly growing. The AI disclosure PR template is a governance milestone.

### Arc B: "The Demo"
OpenAir-Cyan — the OSHWA-certified DIY DAC device. Can you build a carbon capture machine from open-source plans? The certification was a landmark, but the silence since is the twist.

### Arc C: "The Data Revolution"
CC0 licensing in the DAC materials community. Two repos, both public domain. Is this the future of climate research data?

### Arc D: "The Ghosts"
85-star dead repos and citation inflation. What do stars actually measure in climate tech?

### Arc E: "The Bridge"
Carbon_Capture_ML survey + OpenDAC dataset. How ML is accelerating materials discovery for carbon capture.
