# 🌍 Carbon Capture — Commit Trend Analysis (v9, September 2026)

> **Branch:** `carbon-capture`
> **Podcast episode:** Episode 2 — Carbon Capture
> **Data pulled:** September 2026 via GitHub API
> **Repos analyzed:** 6 (OpenCarbon, CO2-Sequestration, openair-cyan, Carbon_Capture_ML, tjz21/DAC_peroxovanadates, tjz21/DAC_peroxotitanates)

---

## Executive Summary

The carbon capture ecosystem has **four distinct development patterns**:

| Pattern | Repos | Behavior | Episode Angle |
|---------|-------|----------|---------------|
| **Launch-and-Stop** | OpenCarbon | 10 commits in 3 days, then 2+ years silent | "Why do climate tools die after a good start?" |
| **Ghost with Star Power** | CO2-Sequestration | 2 commits total (2019), but 32 stars | "Citation invites = citations without code" |
| **One-Day Blitz** | openair-cyan | 6 commits in a single day (Feb 2024), then frozen | "The ceremonial release — OSHWA certification as a finish line" |
| **Paceful Manuscript** | Carbon_Capture_ML | Steady paper additions over 16 months | "The literature review that writes itself" |
| **Parallel CC0 Twins** | DAC_peroxovanadates, DAC_peroxotitanates | Simultaneous release, CC0 license | "Data as public infrastructure, not IP" |

---

## 1. terranexum/OpenCarbon — Carbon Management Technologies

**Repo:** `terranexum/OpenCarbon` | **Stars:** 2 | **License:** Not specified

### Complete History: 10 commits over 3 days (May 18 + Jul 13, 2023)

| Date | SHA | Message | Author | Pattern |
|------|-----|---------|--------|---------|
| Jul 18, 2023 | `e3e5afb` | Merge PR #3 | shrilaesturi2006 | Final merge |
| Jul 13, 2023 | `bb5c7b2` | Update README | shrilaesturi2006 | Doc polish |
| Jul 13, 2023 | `f34380f` | Merge PR #2 | shrilaesturi2006 | 3-way merge day |
| Jul 13, 2023 | `43528c8` | Merge PR #1 | shrilaesturi2006 | Multi-branch merge |
| Jul 13, 2023 | `bc5a343` | Update README | shrilaesturi2006 | README overhaul |
| May 20, 2023 | `bb603ec` | Update README | Dahl Winters | Earlier contribution |
| May 20, 2023 | `96e7c2c` | Update README | Dahl Winters | Same-day pair |
| May 18, 2023 | `34ff91c` | Update Project_Plan | Dahl Winters | Planning doc |
| May 18, 2023 | `c5a9112` | Update README | Dahl Winters | Initial setup |
| May 18, 2023 | `f2c9866` | Create Project_Plan | Dahl Winters | **First commit** |

### Episode Talking Points

1. **The 3-Day Launch (May 18 + Jul 13):** Two bursts. May: Dahl Winters creates the project. July: shrilaesturi2006 does a 5-commit push — 3 merges, README rewrite — restructuring everything. Then 2+ years silence.

2. **Two Contributors, Two Styles:** Dahl was the planner; shrilaesturi2006 was the refactorer. They never overlapped. The "passing the baton" pattern between teams or semesters.

3. **The 2-Star Reality Check:** Two stars means nobody's using it. But the commit pattern shows real intent — two people, structured releases, formal PRs. It's a ghost ship with a working engine.

---

## 2. salmansust/CO2-Sequestration — CCS Simulator

**Repo:** `salmansust/CO2-Sequestration` | **Stars:** 32 | **Language:** MATLAB

### Complete History: 2 commits, both March 24, 2019

| Date | SHA | Message | Author |
|------|-----|---------|--------|
| Mar 24, 2019 | `b2d925e` | Add files via upload | Salman Karim |
| Mar 24, 2019 | `41f2aa0` | Initial commit | Salman Karim |

### Episode Talking Points — The 32-Star Ghost

1. **32 stars, 2 commits, one in 2019.** This is the "citation invite" effect — stars as academic acknowledgment, not software usage.

2. **MATLAB lock-in:** Proprietary, expensive language. You can't run it without a license. The 32 stars might represent citations to the concept, not usage of the code.

3. **The lesson:** Not all stars mean usage. Some stars mean "this paper reminded me of my own work."

---

## 3. openair-collective/openair-cyan — DIY Open Hardware DACC

**Repo:** `openair-collective/openair-cyan` | **Stars:** 76 | **License:** OSHWA-certified

### Recent History: 6 commits in a single day (Feb 12, 2024)

| Date | SHA | Message | Significance |
|------|-----|---------|-------------|
| **Feb 12, 2024** | `b5422b3` | Update README — added OSHWA UID link | **OSHWA CERTIFICATION** |
| **Feb 12, 2024** | `b164257` | Add files via upload | New hardware files |
| **Feb 12, 2024** | `828f496` | **Added OSHWA UID logo (US001095)** | **Official certification** |
| **Feb 12, 2024** | `b731cd8` | Add files via upload | Additional files |
| **Feb 12, 2024** | `4b08fb3` | **Create CITATION.cff** | Citation metadata |
| **Feb 12, 2024** | `859bfa8` | Update README | Final README update |
| Jul 20, 2022 | `d12008e` | Update README | Earlier (7-month gap before) |
| May 17, 2022 | `b8621ba` | add files to improve usability | Community contribution |
| May 15, 2022 | `d025674` | Update README | First wave |
| May 15, 2022 | `784ace5` | Update README | Same-day pair |

### Episode Talking Points — The OSHWA Blitz

1. **The OSHWA Blitz (Feb 12, 2024):** Six commits in a single day. Three file uploads, two README updates, and OSHWA UID creation (US001095). A DIY direct air capture device got official open-source hardware certification.

2. **What is OSHWA?** Open Source Hardware Association — certifies that hardware meets open-source definitions. UID US001095 = cert number 1095.

3. **The CITATION.cff:** A standardized metadata file telling researchers exactly how to cite this hardware. It's the academic "cite this" button for physical objects.

4. **The Pattern:** Activity → 21-month silence → OSHWA blitz → silence. This is a ceremonial completion, not an ongoing development cycle.

---

## 4. zikribayraktar/Carbon_Capture_ML — ML Literature Review

**Repo:** `zikribayraktar/Carbon_Capture_ML` | **Stars:** 56 | **Language:** Jupyter Notebook

### 10 commits over 16 months (all by Zikri Bayraktar)

| Date | SHA | Message | Pattern |
|------|-----|---------|---------|
| **May 8, 2024** | `ca9a31f` | **OpenDAC paper added** | **Flagship ML-for-DAC survey** |
| Apr 25, 2024 | `4c01842` | Update README | Sync with new paper |
| Mar 15, 2024 | `2b69376` | Update README | Maintenance |
| Jan 21, 2024 | `e80dfd6` | Update README | Pre-paper sync |
| Jan 21, 2024 | `fe28496` | Update README | Same-day pair |
| Mar 1, 2023 | `a3a02e9` | New paper | First paper |
| Feb 16, 2023 | `93e5a40` | MOFsimplify paper | MOF screening |
| Feb 5, 2023 | `0c62b02` | New process paper | Process-level review |
| Feb 5, 2023 | `6129691` | New process paper | Second paper same day |
| Feb 2, 2023 | `caf8b96` | New paper | Three-paper blitz kickoff |

### Episode Talking Points — The Lit Review Factory

1. **The 3-Paper Blitz (Feb 2–5, 2023):** Three papers in 4 days by one person. Not casual curation — a concentrated literature review.

2. **The 16-Month Marathon:** Roughly one paper per month, with README updates paired. This is the "lit review that writes itself" — the repo becomes a living bibliography.

3. **OpenDAC (May 8, 2024):** The crown jewel — likely the OpenDAC project using ML to screen materials for DAC. Added as the final entry before the repo goes quiet.

4. **Solo Contributor:** Every commit by Zikri Bayraktar. 56 stars for a solo-authored lit review in Jupyter Notebooks — strong signal of community value.

---

## 5. tjz21/DAC_peroxovanadates & DAC_peroxotitanates — CC0 Twins

**Repos:** `tjz21/DAC_peroxovanadates` | `tjz21/DAC_peroxotitanates` | **Stars:** 2 each | **License:** CC0-1.0

### Parallel Release: Sep 23, 2025

Both repos released simultaneously by tjz21, both about computational screening of peroxide-based sorbent materials for DAC, both dedicated to public domain.

### Episode Talking Points — The CC0 Revolution

1. **The Synchronized Release:** Two repositories, same day, same author, same focus. The parallelism is deliberate — a research strategy.

2. **CC0-1.0:** All rights waived to public domain. No copyright. No restrictions. In academic publishing, this is almost unheard of.

3. **The 2-Star Paradox:** Legally free, scientifically useful, zero community engagement on GitHub. Has the scientific community embraced computational screening data as a first-class scholarly object?

---

## Cross-Theme Carbon Patterns

### The Four Development Cultures

| Culture | Repos | Commit Pattern | Meaning |
|---------|-------|-----------------|---------|
| **Launch-and-Stop** | OpenCarbon | 10 commits in 3 days, then silence | Good start, life moved on |
| **Ghost-Star** | CO2-Sequestration | 2 commits, 32 stars forever | Stars are citations, not usage |
| **Ceremonial Certification** | openair-cyan | Activity → silence → OSHWA blitz | Finish line = starting gun |
| **Solo Lit Review** | Carbon_Capture_ML | Steady 16-month additions | One person, one mission |
| **CC0 Pioneer** |DAC_peroxovanadates/titanates | Parallel release, public domain | Data as infrastructure |

### Timeline (2022–2026)

```
May 2022  openair-cyan: two README updates (community starts)
Jul 2022  openair-cyan: one README update (solo maintenance)
Feb 2023  Carbon_Capture_ML: 3-paper blitz (starts)
Feb 2024  openair-cyan: OSHWA CERTIFICATION BLITZ (6 commits, 1 day)
Jan 2024  Carbon_Capture_ML: paper sync
Apr 2024  Carbon_Capture_ML: OpenDAC paper
May 2024  Carbon_Capture_ML: final README update
Sep 2025  DAC_peroxovanadates + DAC_peroxotitanates: CC0 parallel release
Sep 2026  This analysis pushed
```

---

## Episode 2 Production Notes

### Opening Hook
> "On February 12, 2024, someone spent an entire day pushing six commits to GitHub — certifying a DIY air capture device as official open-source hardware, creating a citation file, uploading design documents. The repository had been silent for twenty-one months before that day. And after that day... silence again."

### Three Narrative Arcs

1. **The Ghost-Star Arc (CO2-Sequestration):** 32 stars, 2 commits, MATLAB code that requires a $2,000 license. Stars as academic acknowledgment, not usage.

2. **The Blitz Arc (openair-cyan):** OSHWA certification day. Six commits in 24 hours. DIY DAC device goes from hobby project to officially certified hardware.

3. **The CC0 Revolution Arc (DAC twins):** Two repositories, released simultaneously, dedicated entirely to public domain. Zero copyright. Zero restrictions. Just data, free for anyone.

### Closing Question
> "If a DIY air capture device needs a single day of frantic activity to get certified, and a solo literature reviewer spends 16 months building a living bibliography, and two twin datasets are released into the public domain with only 2 stars each — is the problem that climate tech open-source is failing, or that it's succeeding in ways GitHub wasn't designed to measure?"

---

*Last updated: September 2026 (v9) | Next update: December 2026*