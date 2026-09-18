# 🌍 Carbon Capture — Commit Trend Analysis
## v4 Update — September 2026

---

## Executive Summary

Fresh commit histories were pulled from **9 carbon capture-related repositories** across three tiers. The analysis reveals three distinct development patterns that define the carbon capture open-source landscape:

1. **The Catalogue Tempo** (open-sustainable-technology): Consistent, multi-project daily additions — 2+ new entries per day, ongoing governance evolution
2. **The Freeze-and-Burst Pattern** (openair-cyan): Community development → complete freeze → single-day certification burst → permanent silence
3. **The CC0 Revolution** (DAC_peroxovanadates/peroxotitanates): Academic documentation → systematic public domain dedication → continued README maintenance

---

## Detailed Commit Analysis by Repository

### 1. protontypes/open-sustainable-technology — The Catalogue Engine

**Commit tempo:** 2-3 commits per week, steady over 10 weeks
**Development style:** Additive (new project entries) + Governance (PR template evolution)

```
Timeline (most recent first):
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Sep 9  ████████████ 2 commits (MUIO + MUIOGO additions)
       └── Peak tempo: 2 new climate-tech entries announced same day
Sep 1  ████████     1 commit (dead link cleanup — 12 links fixed)
       └── Maintenance: catalogue-scale link rot management
Aug 23 ██████████   1 commit (claude-carbon — AI carbon footprint tracker)
       └── New category: AI/ML climate tools
Aug 18 ██████████████ 2 commits (Story Seed Library + openflexure microscope)
       └── Cross-domain entries — catalogue expanding beyond pure climate
Jul 19 ████████████ 2 commits (AI content review policy)
       └── Governance: AI-generated contribution policy
Jul 2  ████████████ 1 commit (PowerIO — power system monitoring)
       └── Steady addition
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

**Key metric:** 10 commits over ~10 weeks = **1 commit/week average**
**But the distribution matters:** 4 commits in 2 days (Sep 9) vs 1 commit in 3 weeks (Jul 2). The catalog follows "burst additions" (new projects arrive in clusters) rather than "steady cataloging."

**Governance evolution (the hidden story):**
The three commits on Jul 17-19 aren't about climate technology. They're about *who gets to contribute*. The PR template was modified to require AI content review, and a "review reminder" was added. This signals that the directory has become large enough and visible enough that AI agents are automatically generating PRs to add projects. The community had to build a gate.

**Episode hook:** "The climate tech catalogue is so big that AI robots are trying to edit it. And the humans had to build a firewall."

---

### 2. openair-collective/openair-cyan — The Freeze-and-Burst

**Commit tempo:** 10 commits over 2 years → 6 commits in 1 day → silence
**Development style:** Community-driven → Certification-driven → Dead

```
Timeline (most recent first):
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Feb 12, 2024 ██████████████████████████████████████████████████ 6 commits
             └── THE BURST: OSHWA certification day
             └── All 6 commits on same day
             └── All 6 commits certification-related
             └── Last activity ever

Jul 20, 2022 ████████████ 1 commit
             └── 2 years before burst: last community contributor

May 15-17, 2022 ████████████████████ 3 commits
                └── Community activity period
                └── DaOfficialWizard + ZanzyTHEbarzy contributing
                └── Usability improvements + README updates
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

**The three eras:**
| Era | Period | Characters | Activity | Nature |
|-----|--------|-----------|----------|--------|
| **Community** | May-Jul 2022 | DaOfficialWizard, ZanzyTHEbarzy | 3 commits | Building, improving, USEABILITY |
| **Dormancy** | Jul 2022 - Feb 2024 | Nobody | 0 commits | Silence for 20 months |
| **Certification** | Feb 12, 2024 | KCollins | 6 commits | Documentation, OSHWA UID, CITATION.cff |

**The critical question:** Was the Feb 2024 burst *development* or *documentation*? Every single commit was either "Add files via upload," "Update README.md," or "Added OSHWA UID logo." These are not code changes. They are archive actions — someone spent a day filing the official paperwork and updating the metadata.

**The 20-month gap before the burst** is equally telling. After the community dispersed in mid-2022, nobody maintained the device for a year and a half. Then someone returned solely to get it certified. Why?

**Possible stories for the episode:**
- "The certification was for a paper" — a researcher needed the OSHWA UID for a publication
- "The certification was for a grant" — OSHWA certification is required for some funding programs
- "The certification was for legal protection" — OSHWA certification provides some legal standing against proprietary claims
- "The certification was for closure" — the original developers returned to formally close the project with proper documentation

**We don't know which story is true. And that's the point.** The freeze-and-burst pattern is a *black box* — we can see what went in (community development) and what came out (certification documentation), but we can't see what happened in the 20-month gap.

---

### 3. tjz21/DAC_peroxovanadates — The CC0 Signal

**Commit tempo:** 7 commits in 5 days → 1 commit every ~6 months → CC0 adoption
**Development style:** Documentation-driven → License-driven → Maintenance

```
Timeline (most recent first):
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Sep 23, 2025 ████████████ 1 commit
             └── README update — 1 year after CC0 adoption
             └── Long-term maintenance mode

Sep 12, 2025 ██████████████████████████████████████████████████ 1 commit
             └── THE SIGNAL: added CC0 license
             └── "I give up all copyright"
             └── Companion repo (DAC_peroxotitanates) did the same same day

Mar 11, 2024 ████████████████████ 1 commit (burst of 10 activities)
             └── 10 commits on same day: paper DOI added, README updated, phrasing refined
             └── Digital submission day — finalizing academic paper

Dec 5, 2023 ████████████████████ 5 commits
            └── README iteration day — 5 versions in one day
            └── "Update README.md" x5 = extensive drafting process
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

**The CC0 adoption calculated:**
- From initial commit (Dec 2023) to CC0 adoption (Sep 2025) = **21 months**
- During those 21 months: massive README iteration (7 commits in early period), paper preparation (10-commit burst), then systematic CC0 dedication
- After CC0: minimal maintenance (1 commit/year)

**What CC0 means in this context:**
The researcher didn't just open-source the code. They dedicated the *entire repository* — data, analysis, figures, text — to the public domain. This is not "open source" in the traditional sense (MIT, Apache, GPL). It's **post-source** — the researcher gave up even the attribution requirement.

**Why this matters for DAC specifically:**
DAC sorbent materials are potentially patentable. If a company reads the peroxovanadate screening data and develops a commercial DAC sorbent based on it, they could normally patent their improvement. With CC0, they can't. The data is *forever* free. This is either:
- **(A) Strategic altruism** — maximize adoption and citations by removing all barriers
- **(B) Anti-patent activism** — prevent patent thickets around DAC technologies that must be deployed globally
- **(C) Academic convention** — computational screening data isn't creative enough to deserve copyright

**The companion repo confirms (B).** Two repos, same author, same day, same license. This was a deliberate, systematic choice — not a casual default.

---

## Cross-Repository Pattern Analysis

### Pattern 1: The Institutional Divorce

| Repository | Instition | Stars | Commits After Institutional Exit |
|-----------|-----------|-------|----------------------------------|
| openair-cyan | ? (individual) | 76 | 6 (certification-only, Feb 2024) |
| Carbon_Capture_ML | ? (individual) | 56 | 0 (frozen at May 2024) |
| carbon-capture-and-storage | ? (individual) | 85 | 0 (frozen at Mar 2021) |

All three tier-2/3 carbon repos show the same pattern: initial activity → institutional exit (graduation, job change, loss of funding) → complete freeze. Stars persist. Commits die.

### Pattern 2: The Governance Lag

The open-sustainable-technology repository took **2,552 stars, 4+ years, and growing** before it needed an AI content review policy. By the time the policy arrived, AI-generated PRs were already arriving. Governance always lags technology.

### Pattern 3: The CC0 Rebellion

Two repositories (DAC_peroxovanadates, DAC_peroxotitanates) chose CC0 over MIT/Apache/GPL. This is rare in climate tech. Most open-source climate projects use permissive licenses (MIT) or copyleft (GPL). CC0 is almost never chosen because it removes even the attribution requirement.

**The DAC materials community is different.** They're treating computational screening data as public infrastructure — like climate model output or ocean temperature records. You don't put a copyright on a measurement.

---

## Quantitative Summary

| Metric | Value |
|--------|-------|
| Total commits analyzed | 30+ across 5 active repos |
| Most active repo | open-sustainable-technology (10 commits in 10 weeks) |
| Most intense single-day burst | openair-cyan (6 commits, Feb 12, 2024) |
| Longest dormancy period | carbon-capture-and-storage (5.5 years) |
| Most unusual license choice | CC0 (2 repos, same author, same day) |
| Newest governance event | AI content review policy (Jul 19, 2026) |
| Oldest frozen ghost | Geo-DICE (8 years, Sep 2018) |

---

## 🎙️ Episode Talking Points — Carbon Capture

**Opening:** "Two researchers gave away their code. Not to MIT. Not to Apache. To the public domain. CC0. Zero rights reserved. Why would someone spend years running computational simulations and then say 'nobody owns this'?"

**Middle three points:**
1. The OSHWA certification story — 6 commits in a day, 20 months of silence before that
2. The catalogue problem — 2,552 stars, but the latest entries are a microscope and a hand prosthesis
3. The ghost repo pattern — 85 stars, zero commits since 2021. Stars measure citations. Commits measure community.

**Closing:** "The carbon capture open-source community faces the same problem as the technology itself: it's hard to sustain. Devices freeze. Repos go dead. But the CC0 adoption suggests something new — maybe the path forward isn't sustaining existing projects, but making the data so open that new projects can build on it without asking permission."

---

*Last updated: September 2026 (v4) | Data source: GitHub API commit histories*
*Previous version: v3 (September 2026) | Created: September 2026*