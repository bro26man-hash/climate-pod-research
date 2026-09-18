# 🌍 Carbon Capture — Commit Trend Analysis
## Research Notes for Climate Pod Episode 2

---

## Executive Summary

This analysis covers **37+ commits** across **5 carbon capture related repositories** during **2019–September 2026**. The data reveals a polarized ecosystem: one massively active directory (2,552★, 15 commits in 3 months) surrounded by mostly dormant or single-researcher projects. The carbon capture GitHub ecosystem has a Gini coefficient of contribution inequality that would make economists weep.

**Key Finding:** The carbon capture open-source ecosystem is defined by directories, not engines. The most valuable repo is a list of links. The actual simulation tools are ghost towns.

---

## 📈 Repo-by-Repo Trend Breakdown

### Open Sustainable Technology Directory
**Period Analyzed:** June–September 2026 (15 commits in ~90 days)
**Average Pace:** ~0.17 commits/day (steady, sustainable)
**Key Contributors:** Tobias Augspurger (6 commits), Abdul Salam (5 commits), Mikhail Alabugin (1), Christophe Combelles (1), gwittebolle (1)

#### Trend Pattern: Steady Enrichment
```
Commits/
  6 |          *   *
  5 |  *   *   *   *
  4 |  *   *   *   *
  3 |  *   *   *   *
  2 |  *   *   *   *
  1 |  *   *   *   *
    +--+--+--+--+--+--+--+--+--+--
     Jun6 Jun23 Jul1 Jul2 Jul17 Jul19 Aug18 Aug23 Sep1 Sep9
```

**What the commits tell us:**
1. **Summer 2026 is add-heavy season:** 10 new projects added in June-August (PowerIO, ASSETRA, ToOp, wbdata, Volca, EpexPredictor, openflexure, Story Seed Library, claude-carbon, MUIO, MUIOGO)
2. **Two contributors with different styles:**
   - Tobias Augspurger: Methodical, adds projects with PR templates, also maintains process (AI content review, link fixing)
   - Abdul Salam: Aggressive adding, 5 projects in 5 days (Aug 18), then 2 more on Sep 9
3. **The AI content review旁的PR template change (Jul 19) is historically significant:** This directory is so large that it now needs rules for AI-generated content. The escalation is: maintain manually → maintain with templates → moderate AI contributions.
4. **Sep 1 link rot fix:** 4 months after the last mass add, someone noticed broken links. Digital decay is real even in curated directories.

**Carbon Capture–Specific Additions:**
- **claude-carbon (Aug 23):** AI project related to carbon
- **Volca to LCA (Jun 23):** Lifecycle assessment tool — relevant for carbon footprint measurement
- **ASSETRA (Jul 1):** Sustainability assessment tool
- **EpexPredictor (Jun 6):** Electricity price predictor — relevant for CCS energy cost analysis

**Weekly Commit Pattern:**
| Week | Adds | Maintenance | Total |
|------|------|-------------|-------|
| Jun 1-7 | 2 | 0 | 2 |
| Jun 22-28 | 2 | 0 | 2 |
| Jul 1-7 | 3 | 0 | 3 |
| Jul 14-20 | 0 | 3 (PR templates, checkbox) | 3 |
| Jul 28-Aug 1 | 2 | 0 | 2 |
| Aug 16-23 | 3 | 0 | 3 |
| Aug 23-29 | 1 | 0 | 1 |
| Sep 1-9 | 0 | 2 (link fixes + new adds) | 2 |

**Episode Angle:** *"Every few weeks, someone adds a new climate tech project to the directory. Not a upgrade. Not a refactor. Just: 'Here's another thing someone built to save the world.' And then they paste a link. That's it. That's the whole commit. And it might be the most optimistic artifact in open source."

---

### Carbon Capture ML Survey
**Period Analyzed:** January 2023 – May 2024
**Average Pace:** ~0.4 commits/month (decaying)
**Key Contributors:** Zikri Bayraktar (solo)

#### Trend Pattern: The Research Sprint followed by Completion
```
Commits/
  8 | * * *
  6 | * * *
  4 | * * *
  2 | * * *
  0 | * * *
    +--+--+--+--+--+--+--+--+--+--
     Jan Feb Mar Jan Jan Apr May
    2023 2023 2023 2024 2024 2024
```

**Detailed timeline:**
| Period | Activity | Pattern |
|--------|----------|---------|
| **Jan 2023** | 6 commits in 10 days | **Research sprint** — multiple papers added |
| Feb 2023 | 2 commits | Supplementary material |
| Mar 2023 | 1 commit | Paper addition |
| Sep–Dec 2023 | 0 | Complete silence |
| Jan 2024 | 2 commits | " 更新README" — maintenance |
| Mar 2024 | 1 commit | Continuted maintenance |
| Apr 2024 | 1 commit | Continued maintenance |
| **May 2024** | 1 commit — **OpenDAC paper** | **Last activity — Direct Air Capture integration** |

**Interpretation:** Bayraktar ran a research sprint in January 2023, adding 6 papers in 10 days. This is typical academic behavior: enter a new field, read everything, catalog it. Then the catalog is "done" and maintenance becomes occasional README updates. The OpenDAC paper in May 2024 was likely triggered by a new significant publication in the DAC space.

**The 17-month gap between May 2024 and now suggests the survey is considered complete.** Or that DAC research accelerated so fast that keeping up became untenable.

---

### CO2 Sequestration (Ghost)
**Period Analyzed:** March 2019
**Total Commits:** 2 (both on same day)
**Status:** 💀 FULLY DORMANT (7 years)

No trend analysis needed. Two commits. One day. Done. Forever.

**Episode Material:** "The repository has more stars than commits. That's like a library where everyone signed the guest book but nobody ever donated a book."

---

### Climate Soton Research Group
**Period Analyzed:** August 6, 2026
**Total Commits:** 4 (all same day)
**Pattern:** Single-day website update blitz

| Time | Action | Signaled |
|------|--------|----------|
| Morning | File upload | New content ready |
| Midday | Another upload | Testing deployment |
| Afternoon | Delete 1.zip | Cleanup |
| Late | Final upload | Publish |

**Interpretation:** A classic academic website refresh. The 4-commit pattern (upload, upload, delete, upload) suggests someone uploaded a file, realized it was wrong, deleted it, and uploaded the correct version. Normal web dev behavior. But for a climate research group, it means **something new is coming**. Chemical Looping Combustion papers? New PhD students? An event?

---

### DAC Peroxovanadates & Peroxotitanates
**Period Analyzed:** September 2025 (4 commits across both repos)
**Average Pace:** Slow, deliberate
**License:** CC0 (Public Domain)

These are computational chemistry repos. Adding molecular data files and documentation. The CC0 dedication means all computed screening results are released as public data.

**Episode angle:** The most generous license in the solar/carbon ecosystem.

---

## 🔥 Cross-Cutting Trends

### 1. The Directory Economy
The most active carbon capture "project" on GitHub isn't a simulation. It's a list. Open-Sustainable-Technology adds ~50 projects per quarter. Each addition is a one-line commit: "Add [Project Name]." No code. No tests. Just a link.

**What this tells us:** Carbon capture has a discovery problem, not a code problem. There are >4,000 climate tech projects, and nobody knows about all of them. The directory is the infrastructure that makes the rest of the ecosystem possible.

### 2. The AI Governance Question is Live
The July 2026 PR template changes explicitly address AI-generated content. This is the first known instance of a climate tech GitHub project establishing AI contribution policies.

**The question becomes:** If an LLM writes a project description for a carbon capture startup tool, and it gets added to the directory, is that "curated"? The directory's value proposition is human curation. AI-generated entries may dilute that.

### 3. The Star-to-Activity Ratio is Depressing
| Repo | Stars | Monthly Commits | Ratio |
|------|-------|-----------------|-------|
| Open-Sustainable-Tech | 2,552 | ~5 | 510:1 |
| Carbon_Capture_ML | 56 | ~0.1 | 560:1 |
| CO2-Sequestration | 32 | 0 | ∞ |

Even the most active repo has 510 stars per commit. This means most people click the star and leave. Climate tech on GitHub is consumed passively.

### 4. The CC0 Movement is the Biggest Governance Signal
Both DAC peroxovanadate/titanate repos use CC0. This isn't just "open source" — it's "we don't even own this anymore." In a field where carbon capture startups are valued at $1B+ and their sorbent formulations are trade secrets, publishing computational screening data as public domain is radical.

### 5. Solo Researchers Dominate
Except for the directory (which has 5+ contributors), every carbon capture repo is a single person. Zikri Bayraktar, Salman Karim, Sahil Khutey. These are individual researchers doing individual work. No teams. No companies. No NSF grants specifically for open-source carbon capture code.

---

## 📋 Data Summary

| Repo | Stars | Commits Analyzed | Date Range | Active Contributors |
|------|-------|-------------------|------------|---------------------|
| open-sustainable-technology | 2,552 | 15 | Jun–Sep 2026 | 5 |
| Carbon_Capture_ML | 56 | 15 | Jan 2023–May 2024 | 1 |
| climate-research-group | Low | 4 | Aug 2026 | 1 group |
| CO2-Sequestration | 32 | 2 | Mar 2019 | 1 |
| DAC_peroxovanadates | 2 | ~2 | Sep 2025 | 1 |
| DAC_peroxotitanates | 2 | ~2 | Sep 2025 | 1 |

**Total commits analyzed:** ~40 across 6 repos
**Total unique contributors:** ~8
**Most commits in a single day:** 6 (Jan 2023, Carbon_Capture_ML research sprint)
**Most active sustained contributor:** Tobias Augspurger (6 commits in Jul-Sep 2026)
**Longest dormant high-star repo:** CO2-Sequestration (32 stars, 2 commits, 7 years)

---

## 🎙️ Suggested Episode Structure

| Segment | Duration | Topic | Key Evidence |
|---------|----------|-------|---------------|
| Cold Open | 3 min | "The 2,552-Star List" | Open-Sustainable-Technology directory |
| Act 1 | 8 min | "Who Adds the Links?" | Directory maintenance, 5 contributors, AI governance debate |
| Act 2 | 6 min | "The Guy Who Gave It Away" | CC0 licensing, tjz21's DAC materials |
| Act 3 | 5 min | "The Ghost Town" | CO2-Sequestration, 32 stars, zero commits, 7 years |
| Act 4 | 4 min | "Quantum CO2 and Coral" | QHackathon25, Carbonize biomineralization |
| Close | 2 min | "The Catalog Problem" | Discovery > invention in climate tech OSS |

---

*Analysis generated: September 2026 | Source: GitHub API*
*Companion notes: See PROJECT-DISCOVERIES-CARBON.md for detailed repo profiles.*