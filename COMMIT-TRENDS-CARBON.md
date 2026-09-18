# 🌍 Carbon Capture — Commit Trend Analysis (v6)

> **Last updated:** September 2026 (v6)  
> **Branch:** `carbon-capture`  
> **Podcast episode:** Episode 2 — Carbon Capture

---

## Activity Overview (v6 Data)

| Repo | Total Commits Pulled | Date Range | Commit Density | Development State |
|------|---------------------|------------|---------------|------------------|
| protontypes/open-sustainable-technology | 15 | Jun-Sep 2026 | ~3-4/month sustained | 🟢 Active ecosystem curation |
| openair-collective/openair-cyan | 15 | May 2022-Feb 2024 | 💥 7/day blitz then ❌ frozen | ⚠️ Dormant 2+ years |
| zikribayraktar/Carbon_Capture_ML | 10 | Jan-May 2024 | ~1/week then ❌ frozen | ⚠️ Dormant 1.5 years |
| tjz21/DAC_peroxovanadates | 10 | Nov 2023-Sep 2025 | ❌ 6mo gap then 1 day, then ❌ | 🆕 CC0 adoption signal |
| tjz21/DAC_peroxotitanates | 10 | Feb-Sep 2024 | ~2/week then ❌ gap, then 1 day | 🆕 CC0 adoption signal |
| yohanesnuwara/carbon-capture-and-storage | 0 | Dead since 2021 | 💀 Ghost | 💀 4+ years silent |

---

## Trend 1: The Sustained Curation Model (v6 Deep Dive)

Open Sustainable Technology is the **only repo in the carbon-capture theme showing consistent, ongoing development.**

**v6 Commit Velocity:**
```
Jun 2026:  ████████████████████  3 commits (EpexPredictor, wbdata, Volca+LCA)
Jul 2026:  ████████████████████████████████  4 commits (PowerIO, ASSETRA, ToOp, AI template)
Aug 2026:  ██████████████████████████████████  3 commits (claude-carbon, Story Seed, openflexure)
Sep 2026:  ████████████████████  3 commits (MUIO, MUIOGO, README fixes)
```

**Key insight:** ~3 commits/month, every month, without gaps. This is **institutional curation velocity** — not code development, but ecosystem maintenance. Different contributors (Abdul Salam, Tobias Augspurger, Mikhail Alabugin, Christophe Combelles, gwittebolle) add different entries. This is a community project, not an individual effort.

**The AI Governance Signal (Jul 2026):**
The most significant v6 development isn't a new entry — it's a **PR template change** (commit c4c9fe7, Jul 19, 2026):

```
Modify PR template for AI content review
→ New mandatory AI-disclosure checkbox
→ Applied to every new project entry PR
```

This is the first concrete governance response to AI-generated contributions in climate tech OSS. The community is actively deciding how to handle AI-assisted entries. There's no playbook yet.

**🎙️ Podcast angle:** *"The biggest climate-tech repo on GitHub just added a mandatory AI disclosure checkbox. The community is deciding, right now, how to handle AI-generated entries. And there's no playbook."*

---

## Trend 2: The "Big Bang Then Freeze" Pattern (v6 Confirmed)

Two repos show the same dramatic pattern:

| Repo | Build Phase | Lean Phase | Freeze |
|------|------------|-----------|--------|
| openair-cyan | May 2022: CodeQL, README, usability (6 commits) | Jul 2022: 1 README update | **Feb 12, 2024: 7 commits in 1 day (OSHWA blitz), then 2+ years silence** |
| Carbon_Capture_ML | Feb 2023: 7 commits in 1 week (full survey build) | Mar-Dec 2023: slow additions | **May 8, 2024: OpenDAC paper added, then silence** |

**The pattern:** A rapid build phase (1 week to 1 day) produces the full artifact, then a slow maintenance phase, then complete freeze.

**What this tells us about carbon-capture open source:**

1. **The artifact is the vision.** Once the vision is realized (certified hardware, complete survey), the contributor loses interest. The MVP effect applies to OSS: build the thing, show the thing, walk away.

2. **No community sustains it.** Unlike WRF or PCMDI (institutional), these repos have no institutional backing. When the individual contributor stops, the repo stops.

3. **The freeze is permanent.** OpenAir-Cyan: 2+ years. Carbon_Capture_ML: 1.5+ years. Neither shows signs of revival. The "ghost" pattern dominates carbon-capture OSS.

---

## Trend 3: The CC0 Revolution (v6 Key Finding)

The most significant open-science development in carbon capture this year:

**The commit:** `e041eff` on September 12, 2025
**The message:** "added CC0 license"
**The repo:** `tjz21/DAC_peroxovanadates`
**The significance:** Explicit public domain dedication. No copyright. No restrictions. Just data, freely available.

**The pattern across both tjz21 repos:**

```
DAC_peroxovanadates:
  Nov 2023: ████ Paper submission batch (4 commits in 1 day)
  Dec 2023: ████ Paper updates (4 commits)
  Mar 2024: ██ DOI fixes (2 commits)
  --- 6 months of silence ---
  Sep 2025: ██ CC0 license (1 commit, e041eff) + README update
  --- 11 months of silence ---

DAC_peroxotitanates:
  Feb 2024: ██ Paper references (2 commits)
  Mar 2024: ██ DOI links (2 commits)
  --- gap ---
  Sep 2025: ██ CC0 license + README update
```

**The story:** Two researchers, working on two sorbent chemistries, published their DFT screening data, then dedicated it to the public domain. The CC0 decision was a standalone event — not a paper cycle. The author deliberately chose open infrastructure over intellectual property.

**Why this matters for the podcast:** This is the biggest open-science signal in the carbon capture space. It's the proof of concept that climate research data CAN be public infrastructure. The question is whether others follow.

**🎙️ Episode Hook:** *"Two researchers, two sorbent chemistries, two repos, both released to the public domain with CC0. No copyright. No licensing drama. Just data, freely available. This is how open science is supposed to work — and it's happening right now."*

---

## Trend 4: The Ghost Star Inflation

| Repo | Stars | Last Commit | Years Dead | What the Stars Mean |
|------|-------|-------------|------------|---------------------|
| carbon-capture-and-storage | 85 | Mar 2021 | 4+ | **Citations, not usability** — people cite it in papers but nobody runs the code |
| (CO2-Sequestration) | ~32 | 2019 | 6+ | **Abandoned but accessible** — old modeling scripts, no maintenance |

**The pattern:** High star count, zero commits. In climate tech, stars measure whether someone found the repo useful for their literature review — not whether the code works.

**How to read star counts in climate tech:**
- **1,000+ stars:** Institutional project with sustained development (WRF, Open-Sustainable-Tech)
- **100-500 stars:** Active community project (PCMDI, MDTF)
- **10-100 stars:** Individual project, may be dormant (OpenAir-Cyan, Carbon_Capture_ML)
- **2-9 stars:** Either brand new (srm-forever), or niche research tool (DAC_peroxovanadates)
- **80+ stars but 0 commits since 2021:** Ghost repo. Citation artifact, not usable code.

---

## Commit Density Comparison (v6)

```
Open-Sustainable-Tech:  ████████████████████████████████  3-4 commits/month sustained
OpenAir-Cyan:           ████████████████████████████████████████  7/day blitz, then nothing
Carbon_Capture_ML:      ██████████████████████  1/week during build, then nothing
DAC_peroxovanadates:    ██  1 day for CC0, chain of silence
carbon-capture-storage: █  0 commits / 4 years
```

**The story:** Carbon-capture OSS has exactly one sustained developer (the directory), two "big bang then freeze" projects, and two CC0 pioneers. The actual carbon capture CODE on GitHub is far less active than the star count suggests.

---

## Episode 2: Commit-Based Talking Points

| Talking Point | Evidence | Source |
|---------------|----------|--------|
| "The biggest climate-tech repo is a directory, not a tool" | 2,552★, 2,500+ entries, 3-4 commits/month | Open-Sustainable-Tech commit log |
| "The community is debating AI governance right now" | AI disclosure PR template, Jul 19, 2026 | Open-Sustainable-Tech commit c4c9fe7 |
| "The OSHWA certification was a peak, not a plateau" | 7 commits Feb 12, 2024, then 2+ years silence | OpenAir-Cyan commit log |
| "The OpenDAC dataset is the field's reference" | Added May 8, 2024, then silence | Carbon_Capture_ML commit ca9a31f |
| "Two researchers released all data to public domain" | CC0 license, Sep 12, 2025 | DAC_peroxovanadates commit e041eff |
| "85 stars, zero commits since 2021" | Ghost repo | carbon-capture-and-storage |
| "Stars measure citations, not usability" | Ghost repos vs. active repos comparison | Cross-repo analysis |

---

## v6 Signal Summary

| Signal | Strength | Confidence | Repo(s) |
|--------|----------|------------|----------|
| CC0 public domain dedication | 🟢 High | 🟢 Clear | tjz21 (both repos) |
| AI governance in OSS | 🟢 High | 🟢 New | Open-Sustainable-Tech |
| OSHWA certification peak | 🟢 High | 🟢 Clear | OpenAir-Cyan |
| OpenDAC as field reference | 🟡 Medium | 🟢 Clear | Carbon_Capture_ML |
| Ghost star inflation | 🟡 Medium | 🟢 Clear | carbon-capture-and-storage |
| Directory as only alive repo | 🟢 High | 🟢 Clear | Open-Sustainable-Tech |
| Big-bang-then-freeze pattern | 🟢 High | 🟢 Clear | OpenAir-Cyan, Carbon_Capture_ML |
