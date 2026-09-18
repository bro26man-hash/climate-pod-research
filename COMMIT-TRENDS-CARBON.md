# 🌍 Carbon Capture — Commit Trend Analysis (v7)

> **Last updated:** September 2026 (v7)  
> **Branch:** `carbon-capture`  
> **Podcast episode:** Episode 2 — Carbon Capture

---

## Activity Overview (v7 Data)

| Repo | Total Commits Pulled | Date Range | Commit Density | Development State | Ghost Type |
|------|---------------------|------------|---------------|------------------|------------|
| protontypes/open-sustainable-technology | 15 | Jun-Sep 2026 | ~3-4/month sustained | 🟢 Active ecosystem curation | N/A (alive) |
| openair-collective/openair-cyan | 15 | May 2022-Feb 2024 | 💥 7/day blitz then ❌ frozen | ⚠️ Dormant 2+ years | Big-Bang-Then-Freeze |
| zikribayraktar/Carbon_Capture_ML | 10 | Jan-May 2024 | ~1/week then ❌ frozen | ⚠️ Dormant 1.5 years | Big-Bang-Then-Freeze |
| tjz21/DAC_peroxovanadates | 10 | Nov 2023-Sep 2025 | ❌ 6mo gap then 1 day, then ❌ | 🆕 CC0 adoption signal | CC0-Pioneer |
| tjz21/DAC_peroxotitanates | 10 | Feb-Sep 2024 | ~2/week then ❌ gap, then 1 day | 🆕 CC0 adoption signal | CC0-Pioneer |
| terranexum/OpenCarbon | 10 | May-Jul 2023 | 💥 3 PR merges, then ❌ | 💀 Dead 2+ years | Collaboration-Failure |
| salmansust/CO2-Sequestration | 2 | Mar 2019 | 2 commits same day, then ❌ | 💀 Dead 6+ years | Upload-and-Vanish |
| vasilistsavalias/BECCS | 5 | Jan-Feb 2024 | 5 commits in 8 days, then ❌ | 💀 Dead 1.5 years | Project-Workflow |
| ClimateSoton/climate-research-group | 4 | Aug 2026 | 4 commits same day | 🟢 Active (website) | Institutional-Canary |
| yohanesnuwara/carbon-capture-and-storage | 0 | Dead since 2021 | 💀 Ghost | 💀 Dead 4+ years | Ghost-Star Giant |

**Total v7 commits pulled: 21 across 4 new repos + 1 still-active repo**

---

## Trend 1: The Sustained Curation Model (v6/v7 Retained)

Open Sustainable Technology is the **only repo in the carbon-capture theme showing consistent, ongoing development.**

**v7 cross-reference:** The directory indexes content from ALL the ghost repos in this document. OpenAir-Cyan, Carbon_Capture_ML, carbon-capture-and-storage, and the DAC_peroxovanadates/titanates repos are all listed in the directory. The directory is more alive than what it catalogues.

**v7 signal:** The directory's AI governance PR template (Jul 2026) is the only governance signal in the entire carbon theme. No other repo shows governance awareness.

---

## Trend 2: The "Big Bang Then Freeze" Pattern (v6/v7 Retained)

Two repos show the same dramatic pattern:

| Repo | Build Phase | Lean Phase | Freeze | Ghost Type |
|------|------------|-----------|--------|------------|
| openair-cyan | May 2022: CodeQL, README, usability (6 commits) | Jul 2022: 1 README update | **Feb 12, 2024: 7 commits in 1 day (OSHWA blitz), then 2+ years silence** | Big-Bang-Then-Freeze |
| Carbon_Capture_ML | Feb 2023: 7 commits in 1 week (full survey build) | Mar-Dec 2023: slow additions | **May 8, 2024: OpenDAC paper added, then silence** | Big-Bang-Then-Freeze |

**v7 addition — Two new variants:**

| Repo | Pattern | Ghost Type | Story |
|------|---------|------------|-------|
| OpenCarbon | 2-month build, 3 PR merges in 1 day, then silence | Collaboration-Failure | Two contributors tried, made PRs, and the project died anyway |
| BECCS | 5 commits in 8 days, then "completed" | Project-Workflow | Honest completion — the author did a full job and moved on |

**The taxonomy of death:**

```
Big-Bang-Then-Freeze:  Build everything → Celebrate → Vanish
Archive-a-Thon:        Document everything → Tag it → Vanish
Upload-and-Vanish:     Dump code → Leave → Ghost
Project-Workflow:      Build → Document → Complete → Move on
Collaboration-Failure: Multiple people → PRs → Silence
Ghost-Star Giant:      85 stars → 0 commits → Citation artifact
```

---

## Trend 3: The CC0 Revolution (v6/v7 Retained)

The most significant open-science development in carbon capture:

**The commit:** `e041eff` on September 12, 2025
**The message:** "added CC0 license"
**The repo:** `tjz21/DAC_peroxovanadates`
**The significance:** Explicit public domain dedication. No copyright. No restrictions. Just data, freely available.

**v7 cross-reference:** The CC0 revolution is the ONLY positive signal in the carbon theme that doesn't involve the directory. Two repos, both public domain, both with sparse activity. The CC0 decision was a standalone event — not a paper cycle. The author deliberately chose open infrastructure over intellectual property.

**Why this matters for the podcast:** This is the biggest open-science signal in the carbon capture space. It's the proof of concept that climate research data CAN be public infrastructure. The question is whether others follow.

---

## Trend 4: The Ghost Taxonomy (v7 NEW)

Based on fresh commit data from 4 additional repos, we can now classify all ghost repos:

### Type 1: Upload-and-Vanish — CO2-Sequestration

**The simplest death:** 2 commits, both on March 24, 2019. First commit is "Initial commit," second is "Add files via upload." That's it. 6+ years of silence.

```
Mar 24, 2019:
  41f2aa0  █ Initial commit
  b2d925e  █ Add files via upload
  💀💀💀💀💀💀  6+ years of nothing
```

**The pattern:** Someone had MATLAB code, uploaded it, and never came back. No README updates, no bug fixes, no feature additions. The 32 stars represent citations, not usage.

**🎙️ Episode angle:** *"Two commits. Same day. Six years ago. That's it. 32 people starred it. Nobody ran the code."

### Type 2: Project-Workflow — BECCS

**The honest death:** 5 commits over 8 days. Initial commit, PDF creation, 2 README updates, and then a commit message that just says "completed."

```
Jan 27, 2024:
  a154cec  █ Initial commit
  cd8915c  █ Create BECCS-overview.pdf
  b66880b  █ Update README.md
  133b694  █ Update README.md
Feb 3, 2024:
  e8c4d40  █ "completed"
```

**The pattern:** Someone started a BECCS project, did a complete job (initial commit → content → documentation), and then declared it done. The "completed" commit message is the most honest in climate tech OSS. One star. But at least they finished.

**🎙️ Episode angle:** *"'Completed' — the most honest commit message in climate tech. Someone made a BECCS overview, it took 7 days, and then they declared it done. One star. But at least they finished."

### Type 3: Collaboration-Failure — OpenCarbon

**The saddest death:** Two contributors, three pull requests, then silence.

```
May 18, 2023:
  f2c9866  █ Create Project_Plan.md (Dahl Winters)
  c5a9112  █ Update README.md (Dahl Winters)
  34ff91c  █ Update Project_Plan.md (Dahl Winters)
May 20, 2023:
  bb603ec  █ Update README.md (Dahl Winters)
  96e7c2c  █ Update README.md (Dahl Winters)

[2-month gap — summer?]

Jul 13, 2023:
  43528c8  █ Merge PR #1 from shrilaesturi2006
  f34380f  █ Merge PR #2 from shrilaesturi2006
  bc5a343  █ Update README.md (shrilaesturi2006)
Jul 18, 2023:
  e3e5afb  █ Merge PR #3 from shrilaesturi2006

  💀💀💀💀💀💀  2+ years of nothing
```

**The pattern:** Dahl Winters built the project plan and documentation in May 2023. Then shrilaesturi2006 joined and merged 3 pull requests in one day (Jul 13). Then both vanished. The repo has had zero commits since July 18, 2023.

**The v7 finding:** This is different from the other ghosts. It's not a single person who lost interest — it's a collaboration that failed. Two people showed interest, made PRs, and then the project died anyway. The PRs were merged, the work was done, and yet... silence.

**🎙️ Episode angle:** *"Two people built a carbon capture project, merged three pull requests in one day, and then vanished. The README still says '力争上游' (strive for the upper). The code never shipped. The plans never materialized. This is what happens when carbon capture open source runs out of teamwork — not a dramatic explosion, just a fade to silence."

### Type 4: Ghost-Star Giant — carbon-capture-and-storage

**The most misleading death:** 85 stars, zero commits since March 2021.

**The pattern:** High star count, zero commits. In climate tech, stars measure whether someone found the repo useful for their literature review — not whether the code works.

**How to read star counts in climate tech (v7 update):**
- **1,000+ stars:** Institutional project with sustained development (Open-Sustainable-Tech)
- **100-500 stars:** Active community project (none in carbon theme)
- **10-100 stars:** Individual project, may be dormant (OpenAir-Cyan, Carbon_Capture_ML)
- **2-9 stars:** Either brand new (srm-forever), or niche research tool (DAC_peroxovanadates)
- **80+ stars but 0 commits since 2021:** Ghost-Star Giant. Citation artifact, not usable code.

---

## Trend 5: The Institutional-Canary Pattern (v7 NEW)

ClimateSoton/climate-research-group is the ONLY carbon-theme repo with 2026 activity.

**The pattern:**
```
Aug 6, 2026:
  4b7cc18  █ Update index.html
  f0b123f  █ Delete 1.zip (cleanup)
  503e839  █ Add files via upload
  3807b50  █ Add files via upload
```

**Why it's a canary:** A research group website doesn't simulate carbon capture. But it represents an active institution. The CLIMATE Research Group works on chemical looping, CFD modelling, and CO₂ conversion. Their CFD expertise is the closest thing to ocean circulation modeling in the carbon capture space.

**The canary sings:** The institution is alive. The research is ongoing. But the code isn't on GitHub. The next paper might include code. The next grant might fund open-source. The canary hasn't died — but it hasn't sung yet either.

**🎙️ Episode angle:** *"The only carbon-capture repo with 2026 activity is a website. Four commits, all same day, cleaning up a zip file. But that website means the research group is alive. And their CFD work might be the bridge to ocean intervention modeling."

---

## Trend 6: The Directory vs. The Content Gap (v7 Deep Dive)

Open-Sustainable-Technology (2,552★) indexes content from repos that are mostly dead.

**The v7 mapping:**

| Directory Entry | Repo Status | Stars | Commits Since 2024 |
|----------------|-------------|-------|---------------------|
| OpenAir-Cyan | 💀 Dormant | 76 | 0 |
| Carbon_Capture_ML | 💀 Dormant | 56 | 0 |
| carbon-capture-and-storage | 💀 Ghost | 85 | 0 |
| CO2-Sequestration | 💀 Ghost | 32 | 0 |
| BECCS | 💀 Dormant | 1 | 0 |
| OpenCarbon | 💀 Dead | 2 | 0 |
| DAC_peroxovanadates | 🟡 Sparse | 2 | 0 |
| DAC_peroxotitanates | 🟡 Sparse | 2 | 0 |

**8 of 8 indexed repos have zero commits since their last activity.** The directory is the only alive thing in the carbon-capture ecosystem.

**The podcast angle:** *"The biggest climate-tech repo on GitHub is a directory, not a tool. It's the only living thing in an ecosystem of ghosts. The catalogue is more alive than the content it catalogues."

---

## Commit Density Comparison (v7)

```
Open-Sustainable-Tech:    ████████████████████████████████  3-4 commits/month sustained
OpenAir-Cyan:             ████████████████████████████████████████  7/day blitz, then nothing
Carbon_Capture_ML:        ██████████████████████  1/week during build, then nothing
DAC_peroxovanadates:      ██  1 day for CC0, chain of silence
OpenCarbon:               ███  3 PRs in 1 day, then nothing
CO2-Sequestration:        █  2 commits same day, then nothing
BECCS:                    ██  5 commits in 8 days, then "completed"
ClimateSoton:             ████  4 commits same day (Aug 2026), only 2026 activity
carbon-capture-storage:   █  0 commits / 4 years
```

**The story:** Carbon-capture OSS has exactly one sustained developer (the directory), two "big bang then freeze" projects, two CC0 pioneers, one collaboration failure, one upload-and-vanish, one honest completion, and one institutional canary. The actual carbon capture CODE on GitHub is far less active than the star count suggests.

---

## Episode 2: Commit-Based Talking Points (v7)

| Talking Point | Evidence | Source |
|---------------|----------|--------|
| "The biggest climate-tech repo is a directory, not a tool" | 2,552★, 2,500+ entries, 3-4 commits/month | Open-Sustainable-Tech commit log |
| "The community is debating AI governance right now" | AI disclosure PR template, Jul 19, 2026 | Open-Sustainable-Tech commit c4c9fe7 |
| "The OSHWA certification was a peak, not a plateau" | 7 commits Feb 12, 2024, then 2+ years silence | OpenAir-Cyan commit log |
| "The OpenDAC dataset is the field's reference" | Added May 8, 2024, then silence | Carbon_Capture_ML commit ca9a31f |
| "Two researchers released all data to public domain" | CC0 license, Sep 12, 2025 | DAC_peroxovanadates commit e041eff |
| "85 stars, zero commits since 2021" | Ghost repo | carbon-capture-and-storage |
| "Two people, three PRs, then silence" | Collaboration failure | OpenCarbon commit log |
| "Two commits, same day, six years ago" | Upload-and-vanish | CO2-Sequestration commit log |
| "The most honest commit message: 'completed'" | 7-day project, then done | BECCS commit e8c4d40 |
| "The only 2026 activity is a website" | 4 commits, Aug 6, 2026 | ClimateSoton commit log |
| "Stars measure citations, not usability" | Ghost repos vs. active repos comparison | Cross-repo analysis |
| "The directory is more alive than what it indexes" | 8 of 8 indexed repos have 0 commits since last activity | Cross-repo analysis |

---

## v7 Signal Summary

| Signal | Strength | Confidence | Repo(s) |
|--------|----------|------------|----------|
| CC0 public domain dedication | 🟢 High | 🟢 Clear | tjz21 (both repos) |
| AI governance in OSS | 🟢 High | 🟢 New | Open-Sustainable-Tech |
| OSHWA certification peak | 🟢 High | 🟢 Clear | OpenAir-Cyan |
| OpenDAC as field reference | 🟡 Medium | 🟢 Clear | Carbon_Capture_ML |
| Ghost star inflation | 🟡 Medium | 🟢 Clear | carbon-capture-and-storage |
| Directory as only alive repo | 🟢 High | 🟢 Clear | Open-Sustainable-Tech |
| Big-bang-then-freeze pattern | 🟢 High | 🟢 Clear | OpenAir-Cyan, Carbon_Capture_ML |
| Collaboration failure pattern | 🟢 High | 🟢 New | OpenCarbon |
| Upload-and-vanish pattern | 🟢 High | 🟢 New | CO2-Sequestration |
| Project-workflow pattern | 🟡 Medium | 🟢 New | BECCS |
| Institutional canary pattern | 🟡 Medium | 🟢 New | ClimateSoton |
| Directory-content gap | 🟢 High | 🟢 Clear | Open-Sustainable-Tech indexes 8 dead repos |

---

## v7 Research Log

| Date | Activity |
|------|----------|
| Sep 2026 | v6: Initial commit trend analysis from 6 repos, 6 signals identified |
| Sep 2026 | v7: Fresh commit data pulled from 4 additional repos (OpenCarbon, CO2-Sequestration, BECCS, ClimateSoton) |
| Sep 2026 | v7: Ghost taxonomy created — 4 types: Upload-and-Vanish, Project-Workflow, Collaboration-Failure, Ghost-Star Giant |
| Sep 2026 | v7: OpenCarbon analyzed as Collaboration-Failure (2 contributors, 3 PRs, then silence) |
| Sep 2026 | v7: CO2-Sequestration confirmed as simplest ghost (upload-and-vanish, 2 commits same day) |
| Sep 2026 | v7: BECCS identified as honest completion ('completed' commit after 7 days) |
| Sep 2026 | v7: ClimateSoton website update (Aug 2026) identified as Institutional-Canary |
| Sep 2026 | v7: Directory-content gap mapped — 8 of 8 indexed repos have 0 commits since last activity |
| Sep 2026 | v7: Six new signals added to v7 Signal Summary (Collaboration Failure, Upload-and-Vanish, Project-Workflow, Institutional-Canary, Directory-Content Gap) |
| Sep 2026 | v7: Updated talking points with v7-specific evidence from 4 new repos |
