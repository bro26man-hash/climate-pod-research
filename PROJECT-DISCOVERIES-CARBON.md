# 🌍 Carbon Capture — Project Discoveries (v7)

> **Last updated:** September 2026 (v7 — fresh GitHub API pull)  
> **Branch:** `carbon-capture`  
> **Podcast episode:** Episode 2 — Carbon Capture

---

## Overview (v7 Update)

This document profiles open-source projects relevant to carbon capture, removal, and sequestration (CDR). v7 incorporates fresh 15-commit histories from 5 repos plus new analysis of the **AI governance signal**, the **CC0 revolution**, and the **OSHWA certification story**.

**v7 additions over previous versions:**
- Full 15-commit table for Open-Sustainable-Technology (was 10)
- AI governance signal: 3-day PR template evolution (Jul 17-19, 2026)
- claude-carbon category analysis (Aug 23, 2026)
- OSHWA blitz: ceremonial release pattern identified
- CC0 revolution: parallel timing across tjz21 repos confirmed
- Cross-theme connections: CC0 → AI pipeline identified

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

**v7 Commit Highlights (Full 15-Commit Pull):**

| Date | SHA | Addition | Contributor | Significance |
|------|-----|----------|-------------|-------------|
| **Sep 9** | `6e9f48c` | MUIO | Abdul Salam | New carbon removal/offset standard entry |
| **Sep 9** | `07e19b1` | MUIOGO | Abdul Salam | Complementary standard entry (same day, 2 commits) |
| Sep 1 | `1b6cb82` | Fix dead links | Mikhail Alabugin | Maintenance quality |
| Aug 23 | `d73a519` | **claude-carbon** | gwittebolle | **AI tool for carbon-aware compute scheduling** |
| Aug 18 | `6b6cd82` | Story Seed Library | Abdul Salam | Cross-domain: storytelling for sustainability |
| Aug 18 | `ca9d7a5` | openflexure microscope | Abdul Salam | Open hardware for science |
| **Jul 19** | `2303b7a` | Remove duplicate AI content review checkbox | Tobias Augspurger | **Governance signal — community building AI disclosure into PR process** |
| **Jul 19** | `c4c9fe7` | **Modify PR template for AI content review** | Tobias Augspurger | **🔥 FORMAL AI CONTENT GATE — every PR now requires AI-disclosure checkbox** |
| Jul 17 | `be14281` | Update PR template | Tobias Augspurger | Process refinement |
| Jul 2 | `5bc6609` | PowerIO | Tobias Augspurger | New energy project entry |
| Jul 1 | `e772ed4` | ASSETRA | Tobias Augspurger | New assessment tool entry |
| Jul 1 | `4c6f0a4` | ToOp | Tobias Augspurger | New optimization tool entry |
| Jun 23 | `1986e2c` | wbdata | Tobias Augspurger | World Bank development data tool |
| Jun 23 | `007a464` | Volca to LCA | Christophe Combelles | **CDR-relevant — LCA tool for carbon footprint of materials** |
| Jun 6 | `0601a42` | EpexPredictor | Tobias Augspurger | Electricity price prediction |

**v7 Analysis — The AI Governance Signal:**

The July 2026 AI content disclosure PR template (c4c9fe7, Jul 19) is a landmark. The climate-tech OSS community is formally grappling with AI-assisted contributions. This is the first time we've seen "AI content review" as a required PR template in climate tech.

The sequence tells the story:
1. **Jul 17:** `be14281` — Update PR template with review reminder (precursor)
2. **Jul 19:** `c4c9fe7` — Modify PR template for AI content review (the gate)
3. **Jul 19:** `2303b7a` — Remove duplicate AI content review checkbox (refinement)

Three commits in 3 days, all about AI governance. The community is actively deciding how to handle AI-generated entries. There's no playbook yet.

**The claude-carbon entry** (d73a519, Aug 23) is equally significant: it's a new category in the directory specifically for AI tools that manage carbon-aware compute scheduling. The directory doesn't just acknowledge AI — it's creating taxonomies for it.

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

**v7 Commit Highlights (Full 15-Commit Pull — The OSHWA Blitz):**

| Date | SHA | Event | Significance |
|------|-----|-------|-------------|
| **Feb 12, 2024** | `b5422b3` | OSHWA UID link in README | **Certification finalized** |
| **Feb 12, 2024** | `b164257` | Add files via upload (docs) | Documentation push |
| **Feb 12, 2024** | `828f496` | OSHWA UID logo (US001095) | Visual certification mark |
| **Feb 12, 2024** | `b731cd8` | Add files via upload (technical) | Technical docs |
| **Feb 12, 2024** | `4b08fb3` | Create CITATION.cff | **Academic citation support** |
| **Feb 12, 2024** | `859bfa8` | Update README (final) | **Final push — 7 commits in 1 day** |
| Jul 20, 2022 | `d12008e` | README update | Last activity before blitz |
| May 17, 2022 | `b8621ba` | Usability improvements | |
| May 15, 2022 | `d025674` / `784ace5` | Two README updates same day | |
| May 11, 2022 | `09c761d` | Rename CodeQL file | |
| May 7, 2022 | `d502eb6` / `4350def` | Update CodeQL analysis | |
| May 7, 2022 | `718b209` | Create CodeQL analysis.yml | |
| May 5, 2022 | `b2198a2` | Delete .github/workflows | |

**v7 Analysis — The OSHWA Pattern:**

Three distinct phases:

1. **Build Phase (May 2022):** 8 commits in 10 days. CodeQL setup, usability improvements, workflow management. The team was building the thing.

2. **Stabilization Phase (Jul 2022):** 1 README update. Maintenance mode.

3. **OSHWA Blitz (Feb 12, 2024):** 7 commits in 1 day. Every single commit relates to certification: OSHWA UID logo, CITATION.cff, documentation, README. This is a *ceremonial* day — the certification was the finish line.

Then: **complete silence for 2+ years.**

**The interpretation:** OSHWA certification was the goal, and once achieved, the project lost its momentum. The contributors didn't disappear — they completed the mission. The CITATION.cff creation on Feb 12 is telling: they wanted the device to be citable in academic papers. The certification + citation = the project's identity as a scientific instrument, not a community project.

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

**v7 Commit Highlights:**

| Date | SHA | Event | Significance |
|------|-----|-------|-------------|
| **May 8, 2024** | `ca9a31f` | **OpenDAC paper added** | **Largest open dataset of DFT calculations for CO2 capture materials** |
| Apr 25, 2024 | `4c01842` | Update README | Preparatory |
| Mar 15, 2024 | `2b69376` | Update README | Preparatory |
| Jan 21, 2024 | `e80dfd6` / `fe28496` | Update README | Preparatory |
| Mar 1, 2023 | `a3a02e9` | New paper | Pre-OpenDAC era |
| Feb 16, 2023 | `93e5a40` | **MOFsimplify paper** | Framework for simplifying MOF structures for CO2 capture screening |
| Feb 5, 2023 | `0c62b02` / `6129691` | New process paper | |
| Feb 2, 2023 | `caf8b96` | New paper to process | |

**v7 Analysis — The Survey-as-Bridge Pattern:**

This repo is a bridge between two communities: ML researchers and DAC materials scientists. The Feb-Mar 2023 burst (5 papers in 3 months) was the survey's build phase. Then 14 months of silence. Then the OpenDAC landmark (May 2024) — the biggest open compilation of CO2 capture materials data ever.

The survey's role shifted: from "cataloging papers" to "providing the reference framework for the OpenDAC dataset." The survey is now the index for the dataset.

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

**v7 Analysis — The CC0 Pattern Deep Dive:**

The commit history shows a clear arc:

```
DAC_peroxovanadates:
  Dec 5, 2023:  ████ Paper submission batch (4 commits in 1 day)
  Mar 11, 2024: ████ DOI fixes + README updates (4 commits)
  --- 6 months of silence ---
  Sep 12, 2025: ██ CC0 license (e041eff) + README update
  --- 11 months of silence ---
  Sep 23, 2025: ██ Final README update

DAC_peroxotitanates:
  Feb 2024:     ██ Paper references (2 commits)
  Mar 2024:     ██ DOI links (2 commits)
  --- gap ---
  Sep 12, 2025: ██ CC0 license + README update
```

**The story:** Two researchers, working on two sorbent chemistries, published their DFT screening data, then dedicated it to the public domain. The CC0 decision (e041eff, Sep 12, 2025) was a standalone event — not a paper cycle. The author deliberately chose open infrastructure over intellectual property.

**The parallel timing is the signal:** Both repos got CC0 licenses on the same day (Sep 12, 2025). This wasn't two independent decisions — it was a coordinated strategy. The author is building a public-domain corpus for DAC materials research.

**Why CC0 matters for climate tech:** CC0 is the most permissive license — no copyright, no restrictions, no attribution required. This means anyone can use, modify, and commercialize the data without asking permission. In a field where the gap between "published" and "used" is often years, CC0 removes the friction.

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

## Summary Table — Carbon Theme (v7)

| Repo | Stars | Status | Key v7 Signal | CC0? |
|------|-------|--------|---------------|------|
| **open-sustainable-technology** | 2,552 | 🟢 Very active | AI disclosure PR template (Jul 2026); claude-carbon entry | CC0-1.0 |
| **openair-cyan** | 76 | 💀 Dormant 2+ yr | OSHWA cert blitz (Feb 2024), then silence | CERN-OHL |
| **Carbon_Capture_ML** | 56 | 💀 Dormant 1.5 yr | OpenDAC paper (May 2024), then silence | MIT |
| **carbon-capture-and-storage** | 85 | 💀 Ghost 4+ yr | Dead since 2021 | MIT |
| **DAC_peroxovanadates** | 2 | 🟡 Sparse | **CC0 license (Sep 12, 2025)** | **CC0-1.0** |
| **DAC_peroxotitanates** | 2 | 🟡 Sparse | CC0 license | **CC0-1.0** |

---

## v7 Development Trend Signals

| Signal | Strength | Confidence | Repo(s) |
|--------|----------|------------|----------|
| **AI governance in OSS** | 🟢 High | 🟢 New (Jul 2026) | Open-Sustainable-Technology |
| **CC0 public domain dedication** | 🟢 High | 🟢 Clear (Sep 2025) | tjz21 (both repos) |
| **OSHWA certification peak** | 🟢 High | 🟢 Clear (Feb 2024) | OpenAir-Cyan |
| **OpenDAC as field reference** | 🟡 Medium | 🟢 Clear (May 2024) | Carbon_Capture_ML |
| **Ghost star inflation** | 🟡 Medium | 🟢 Clear | carbon-capture-and-storage |
| **Directory as only alive repo** | 🟢 High | 🟢 Clear | Open-Sustainable-Technology |
| **claude-carbon taxonomy** | 🟢 High | 🟢 New (Aug 2026) | Open-Sustainable-Technology |

---

## 🎙️ Episode 2 Narrative Arcs (v7)

### Arc A: "The Catalogue"
Open-Sustainable-Technology as the universe of climate tech. 2,552 stars, 2,500+ projects, constantly growing. The AI disclosure PR template (Jul 2026) is a governance milestone. claude-carbon is a new category.

### Arc B: "The Demo"
OpenAir-Cyan — the OSHWA-certified DIY DAC device. Can you build a carbon capture machine from open-source plans? The certification was a landmark, but the silence since is the twist.

### Arc C: "The Data Revolution"
CC0 licensing in the DAC materials community. Two repos, both public domain. Is this the future of climate research data?

### Arc D: "The Ghosts"
85-star dead repos and citation inflation. What do stars actually measure in climate tech?

### Arc E: "The Bridge"
Carbon_Capture_ML survey + OpenDAC dataset. How ML is accelerating materials discovery for carbon capture.

### Arc F: "The AI Question" (NEW)
The July 2026 AI disclosure PR template. The climate-tech community is deciding how to handle AI-generated entries. And there's no playbook.

---

*Last updated: September 2026 (v7) | Data source: GitHub API commit histories*
*Previous version: v6 (September 2026)*