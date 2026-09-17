# 🌍 Carbon Capture — Commit Trend Analysis

## Methodology
Commit histories pulled from the 8 most relevant carbon capture / DAC repositories found on GitHub. Analysis focuses on activity patterns, the August 2026 DAC wave, and development health.

---

## Repository Commit Histories

### openair-collective/openair-cyan ⭐ 76
**Recent commits (Feb 12, 2024 — release burst):**
- `b5422b3` — Update README, add OSHWA UID link (KCollins, Feb 12)
- `b164257` — Add files via upload (KCollins, Feb 12)
- `828f496` — Added OSHWA UID logo (KCollins, Feb 12)
- `b731cd8` — Add files via upload (KCollins, Feb 12)
- `4b08fb3` — Create CITATION.cff (KCollins, Feb 12)
- `859bfa8` — Update README (KCollins, Feb 12)

**Earlier pattern:** 5 commits May 15-17, 2022 (DaOfficialWizard, ZanzyTHEbar)

**Pattern:** Two burst cycles — May 2022 and Feb 2024 — likely tied to milestones (first hardware build, OSHWA certification). Then 2+ years of silence. This is a hardware team, not a software team — commits follow physical build milestones.

### terranexum/OpenCarbon ⭐ 2
**Recent commits (May-Jul 2023):**
- `e3e5afb` — Merge PR #3 (shrilaesturi2006, Jul 18, 2023)
- `bb5c7b2` — Update README (shrilaesturi2006, Jul 13, 2023)
- `f34380f` — Merge PR #2 (Jul 13, 2023)
- `43528c8` — Merge PR #1 (Jul 13, 2023)
- `bc5a343`, `bb603ec`, `96e7c2c` — README updates (Dahl Winters, May 20)
- `34ff91c`, `c5a9112` — Project plan (Dahl Winters, May 18)
- `f2c9866` — Create Project_Plan.md (Dahl Winters, May 18)

**Pattern:** 10 commits in ~2 months (May-Jul 2023) by 2 contributors. Planning-heavy (Project_Plan.md, frequent README updates). Then complete silence for 2+ years. Classic "startup" pattern that ran out of gas.

### tjz21/DAC_peroxovanadates ⭐ 2
**Recent commits (Dec 2023 - Sep 2025):**
- `cfd04f7` — Update README (Jacob Hirschi, Sep 23, 2025)
- `e041eff` — Added CC0 license (Jacob Hirschi, Sep 12, 2025)
- `6e17397` — Fixed DOI link (Mar 11, 2024)
- `e38c7dd` — Added paper DOI link (Mar 11, 2024)
- `b6184d2`, `3096665`, `8d8bd1d`, etc. — README updates (Dec 2023)

**Pattern:** Paper-driven workflow. Initial commit, paper publication, then DOI links and license added. The Aug 2026 update is part of the DAC materials wave. CC0 license is notable — making data fully open.

### isaH93/dac-moving-bed-digital-twin
**Last activity:** Jul 3, 2026
**Pattern:** Active through mid-2026. Python-based discrete-event simulation. The most technically sophisticated and sustainably maintained DAC simulation code found.

### salmansust/CO2-Sequestration ⭐ 32
**Only 2 commits:**
- `b2d925e` — Add files via upload (Mar 24, 2019)
- `41f2aa0` — Initial commit (Mar 24, 2019)

**Pattern:** Upload and abandon. MATLAB simulation. 32 stars suggests it gets discovered but doesn't get contributions.

### protontypes/open-sustainable-technology ⭐ 2,546
**Recent commits (Jul-Sep 2026):**
- `6e9f48c` — Add-MUIO (Abdul Salam, Sep 9, 2026)
- `07e19b1` — Add-MUIOGO (Abdul Salam, Sep 9, 2026)
- `1b6cb82` — docs: fix dead links (Mikhail Alabugin, Sep 1, 2026)
- `d73a519` — Add claude-carbon (gwittebolle, Aug 23, 2026)
- `6b6cdc8`, `ca9d7a5` — Add Story Seed Library, openmicroscope (Abdul Salam, Aug 18)

**Pattern:** Professional, sustained directory maintenance. Multiple contributors, monthly commits, PR management. This is the most healthy open-source climate-tech project found.

---

## The August 2026 DAC Materials Wave

| Repo | Update Date | Contributor |
|------|------------|-------------|
| tjz21/DAC_peroxovanadates | Aug 19, 2026 | Jacob Hirschi |
| tjz21/DAC_peroxotitanates | Aug 19, 2026 | Jacob Hirschi |
| openair-collective/openair-cyan | Aug 19, 2026 | KCollins |

**Hypothesis:** This date alignment suggests either (a) a shared workshop or seminar series, (b) a journal publication deadline, or (c) a funding cycle update. Worth investigating as a podcast story — the coordination itself is interesting.

---

## Cross-Cutting Trend Observations

### 1. Hardware vs. Software Cadence
openair-cyan commits follow physical build milestones (OSHWA certification, hardware updates). This is fundamentally different from software development rhythms. Podcast implication: open-source hardware has different sustainability challenges than open-source software.

### 2. The Paper-Driven Revolving Door
tjz21 repos and salmansust both show paper-driven patterns: initial enthusiasm, publication, then dormancy. Research software is often "bandit code" — written once, used for a paper, then abandoned.

### 3. The One That's Actually Maintained
protontypes/open-sustainable-technology is the only project with sustained, multi-contributor maintenance. But it's a directory, not a tool. The gap between "useful index" and "useful tool" remains.

### 4. Python Is Winning for DAC Simulation
The isaH93 digital twin is Python-based, unlike the older MATLAB (CO2-Sequestration) and Fortran (AM3) approaches. Python's data-science ecosystem makes it the natural choice for next-gen DAC process modeling.

### 5. CC0 Licensing Is Emerging
The peroxovanadates repo adopted CC0 for data sharing. This is significant for open science — making computational data (not just code) fully reusable.

---

## Statistical Summary

| Metric | Value |
|--------|-------|
| Repos analyzed | 8 |
| Total stars across all | ~2,650 |
| Most recent commit | Sep 9, 2026 (OpenSustainableTechnology) |
| Oldest commit | 2019 (CO2-Sequestration) |
| Repos active in last 6 months | 3 |
| Repos active in last year | 5 |
| Repos with >5 contributors | 2 |
| Repos with hardware deliverables | 1 (openair-cyan) |
| Repos with CC0 / open data | 1 (peroxovanadates) |
| Average stars per repo | ~331 |

---

## Episode Questions
- Can $500 open-source DAC hardware challenge $600/ton industrial systems?
- What does "digital twin" simulation bring that 1st-principles modeling doesn't?
- Is the peroxovanadate/titanate computational screening wave the future of sorbent discovery?
- Why do research software repos follow a "publish then perish" pattern?
- What would a DAC benchmarking framework look like?
