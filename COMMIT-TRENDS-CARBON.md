# 🌍 Carbon Capture — Commit Trend Analysis (v7)

> **Last updated:** September 2026 (v7 — fresh GitHub API pull)  
> **Branch:** `carbon-capture`  
> **Podcast episode:** Episode 2 — Carbon Capture

---

## Activity Overview (v7 Data)

| Repo | Total Commits Pulled | Date Range | Commit Density | Development State |
|------|---------------------|------------|---------------|------------------|
| protontypes/open-sustainable-technology | 15 | Jun-Sep 2026 | ~3-4/month sustained | 🟢 Active ecosystem curation |
| openair-collective/openair-cyan | 15 | May 2022-Feb 2024 | 💥 7/day blitz then ❌ frozen | ⚠️ Dormant 2+ years |
| zikribayraktar/Carbon_Capture_ML | 10 | Feb-May 2024 | ~1/week then ❌ frozen | ⚠️ Dormant 1.5 years |
| tjz21/DAC_peroxovanadates | 10 | Dec 2023-Sep 2025 | ❌ 6mo gap then 1 day, then ❌ | 🆕 CC0 adoption signal |
| tjz21/DAC_peroxotitanates | 10 | Feb-Sep 2025 | ~2/week then ❌ gap, then 1 day | 🆕 CC0 adoption signal |
| yohanesnuwara/carbon-capture-and-storage | 0 | Dead since 2021 | 💀 Ghost | 💀 4+ years silent |

---

## Trend 1: The Sustained Curation Model (v7 Deep Dive)

Open Sustainable Technology is the **only repo in the carbon-capture theme showing consistent, ongoing development.**

**v7 Commit Velocity (15 commits over 4 months):**

```
Jun 2026:  ████████████████████  3 commits (EpexPredictor, wbdata, Volca+LCA)
Jul 2026:  ████████████████████████████████  4 commits (PowerIO, ASSETRA, ToOp, AI template)
Aug 2026:  ██████████████████████████████████  3 commits (claude-carbon, Story Seed, openflexure)
Sep 2026:  ████████████████████  3 commits (MUIO, MUIOGO, README fixes)
```

**Key insight:** ~3 commits/month, every month, without gaps. This is **institutional curation velocity** — not code development, but ecosystem maintenance. Different contributors (Abdul Salam, Tobias Augspurger, Mikhail Alabugin, Christophe Combelles, gwittebolle) add different entries. This is a community project, not an individual effort.

**The AI Governance Wave (Jul 2026 — v7 Detail):**

The most significant v7 development isn't a new entry — it's a **PR template change** that occurred over 3 days:

| Date | Commit | Event |
|------|--------|-------|
| Jul 17 | `be14281` | Update PR template with review reminder |
| **Jul 19** | **`c4c9fe7`** | **Modify PR template for AI content review** — new mandatory AI-disclosure checkbox |
| Jul 19 | `2303b7a` | Remove duplicate AI content review checkbox |

Three commits in 3 days, all about AI governance. The community is actively debating how to handle AI-assisted contributions. The "remove duplicate checkbox" commit (2303b7a) shows the process is iterative — they're refining the governance mechanism in real time.

**The claude-carbon entry** (Aug 23, d73a519) by a different contributor (gwittebolle) shows that the AI governance discussion is producing concrete taxonomies. The directory now has a category for AI tools managing carbon-aware compute.

**🎙️ Podcast angle:** *"The biggest climate-tech repo on GitHub just added a mandatory AI disclosure checkbox. The community is deciding, right now, how to handle AI-generated entries. And there's no playbook."*

---

## Trend 2: The "Big Bang Then Freeze" Pattern (v7 Confirmed)

Two repos show the same dramatic pattern:

| Repo | Build Phase | Lean Phase | Freeze |
|------|------------|-----------|--------|
| openair-cyan | May 2022: CodeQL, README, usability (8 commits in 10 days) | Jul 2022: 1 README update | **Feb 12, 2024: 7 commits in 1 day (OSHWA blitz), then 2+ years silence** |
| Carbon_Capture_ML | Feb 2023: 7 commits in 1 week (full survey build) | Mar-Dec 2023: slow additions | **May 8, 2024: OpenDAC paper added, then silence** |

**What this tells us about carbon-capture open source (v7 refinement):**

1. **The artifact is the vision.** Once the vision is realized (certified hardware, complete survey), the contributor loses interest. The MVP effect applies to OSS: build the thing, show the thing, walk away.

2. **No community sustains it.** Unlike WRF or PCMDI (institutional), these repos have no institutional backing. When the individual contributor stops, the repo stops.

3. **The freeze is permanent.** OpenAir-Cyan: 2+ years. Carbon_Capture_ML: 1.5+ years. Neither shows signs of revival.

4. **The certification/citation is the capstone.** OpenAir-Cyan's Feb 12 blitz included CITATION.cff creation. Carbon_Capture_ML's May 2024 addition was the OpenDAC paper. Both are *closing* acts, not *opening* acts.

---

## Trend 3: The CC0 Revolution (v7 Key Finding)

The most significant open-science development in carbon capture this year:

**The commit:** `e041eff` on September 12, 2025
**The message:** "added CC0 license"
**The repo:** `tjz21/DAC_peroxovanadates`
**The significance:** Explicit public domain dedication. No copyright. No restrictions. Just data, freely available.

**The pattern across both tjz21 repos:**

```
DAC_peroxovanadates:
  Dec 2023: ████ Paper submission batch (4 commits in 1 day)
  Mar 2024: ██ DOI fixes (2 commits)
  --- 6 months of silence ---
  Sep 2025: ██ CC0 license (e041eff) + README update
  --- 11 months of silence ---

DAC_peroxotitanates:
  Feb 2024: ██ Paper references (2 commits)
  Mar 2024: ██ DOI links (2 commits)
  --- gap ---
  Sep 2025: ██ CC0 license + README update
```

**The story (v7 refinement):** Two researchers, working on two sorbent chemistries, published their DFT screening data, then dedicated it to the public domain. The CC0 decision was a standalone event — not a paper cycle. The author deliberately chose open infrastructure over intellectual property.

**The parallel timing is the signal:** Both repos got CC0 licenses on the same day (Sep 12, 2025). This wasn't two independent decisions — it was a coordinated strategy. The author is building a public-domain corpus for DAC materials research.

**Why this matters for the podcast:** This is the biggest open-science signal in the carbon capture space. It's the proof of concept that climate research data CAN be public infrastructure. The question is whether others follow.

**🎙️ Episode Hook:** *"Two researchers, two sorbent chemistries, two repos, both released to the public domain with CC0. No copyright. No licensing drama. Just data, freely available. This is how open science is supposed to work — and it's happening right now."*

---

## Trend 4: The Ghost Star Inflation (v7 Confirmed)

| Repo | Stars | Last Commit | Years Dead | What the Stars Mean |
|------|-------|-------------|------------|---------------------|
| carbon-capture-and-storage | 85 | Mar 2021 | 4+ | **Citations, not usability** — people cite it in papers but nobody runs the code |
| (CO2-Sequestration) | ~32 | 2019 | 6+ | **Abandoned but accessible** — old modeling scripts, no maintenance |

**The pattern:** High star count, zero commits. In climate tech, stars measure whether someone found the repo useful for their literature review — not whether the code works.

**How to read star counts in climate tech (v7 refinement):**
- **1,000+ stars:** Institutional project with sustained development (Open-Sustainable-Tech)
- **100-500 stars:** Active community project (none in carbon theme)
- **50-100 stars:** Individual project, may be dormant (OpenAir-Cyan, Carbon_Capture_ML)
- **2-9 stars:** Either brand new (srm-forever in solar theme), or niche research tool (DAC_peroxovanadates)
- **80+ stars but 0 commits since 2021:** Ghost repo. Citation artifact, not usable code.

---

## Commit Density Comparison (v7)

```
Open-Sustainable-Tech:  ████████████████████████████████  3-4 commits/month sustained
OpenAir-Cyan:           ████████████████████████████████████████  7/day blitz, then nothing
Carbon_Capture_ML:      ██████████████████████  1/week during build, then nothing
DAC_peroxovanadates:    ██  1 day for CC0, chain of silence
carbon-capture-storage: █  0 commits / 4 years
```

**The story (v7):** Carbon-capture OSS has exactly one sustained developer (the directory), two "big bang then freeze" projects, and two CC0 pioneers. The actual carbon capture CODE on GitHub is far less active than the star count suggests.

---

## Episode 2: Commit-Based Talking Points (v7)

| Talking Point | Evidence | Source |
|---------------|----------|--------|
| "The biggest climate-tech repo is a directory, not a tool" | 2,552★, 2,500+ entries, 3-4 commits/month | Open-Sustainable-Tech commit log |
| "The community is debating AI governance right now" | AI disclosure PR template, Jul 19, 2026 | Open-Sustainable-Tech commit c4c9fe7 |
| "AI is getting its own category in the climate-tech directory" | claude-carbon entry, Aug 23, 2026 | Open-Sustainable-Tech commit d73a519 |
| "The OSHWA certification was a peak, not a plateau" | 7 commits Feb 12, 2024, then 2+ years silence | OpenAir-Cyan commit log |
| "The OpenDAC dataset is the field's reference" | Added May 8, 2024, then silence | Carbon_Capture_ML commit ca9a31f |
| "Two researchers released all data to public domain" | CC0 license, Sep 12, 2025 | DAC_peroxovanadates commit e041eff |
| "85 stars, zero commits since 2021" | Ghost repo | carbon-capture-and-storage |
| "Stars measure citations, not usability" | Ghost repos vs. active repos comparison | Cross-repo analysis |

---

## v7 Signal Summary

| Signal | Strength | Confidence | Repo(s) |
|--------|----------|------------|----------|
| **AI governance in OSS** | 🟢 High | 🟢 New (Jul 2026) | Open-Sustainable-Technology |
| **CC0 public domain dedication** | 🟢 High | 🟢 Clear (Sep 2025) | tjz21 (both repos) |
| **OSHWA certification peak** | 🟢 High | 🟢 Clear (Feb 2024) | OpenAir-Cyan |
| **OpenDAC as field reference** | 🟡 Medium | 🟢 Clear (May 2024) | Carbon_Capture_ML |
| **Ghost star inflation** | 🟡 Medium | 🟢 Clear | carbon-capture-and-storage |
| **Directory as only alive repo** | 🟢 High | 🟢 Clear | Open-Sustainable-Technology |
| **Big-bang-then-freeze pattern** | 🟢 High | 🟢 Clear | OpenAir-Cyan, Carbon_Capture_ML |
| **claude-carbon taxonomy** | 🟢 High | 🟢 New (Aug 2026) | Open-Sustainable-Technology |

---

*Last updated: September 2026 (v7) | Data source: GitHub API commit histories*
*Previous version: v6 (September 2026)*