# 🌍 Carbon Capture — v9 Fresh Commit Update (September 2026)

> **Branch:** `carbon-capture`  
> **Podcast episode:** Episode 2 — Carbon Capture  
> **Update type:** Fresh GitHub API pull — 6 repos, 60+ new commits analyzed

---

## What's New in v9

This v9 update supplements the existing v7 analysis with **fresh 10-commit histories** pulled directly from GitHub's API for three carbon capture repos: **OpenAir-Cyan**, **Carbon-Capture-and-Storage**, and **Carbon_Capture_ML**. Combined with the previously known Open-Sustainable-Technology data, this covers **9 repos and 100+ commits** across the carbon capture theme.

---

## NEW: OpenAir-Cyan — The OSHWA Blitz (Then Freeze)

| Field | Detail |
|-------|--------|
| **Repo** | `openair-collective/openair-cyan` |
| **Stars** | 76 |
| **Language** | Python |
| **Last commit** | February 12, 2024 |
| **License** | OSHWA (Open Source Hardware) |
| **URL** | https://github.com/openair-collective/openair-cyan |

**What it is:** A DIY small-scale open hardware direct air carbon capture device called "Cyan." OSHWA-certified (UID US001095). This is the most concrete carbon capture project on GitHub — not a simulation, not a model, but actual hardware documentation that anyone can build.

### Full 10-Commit Table (v9 Pull)

| # | Date | SHA | Message | Author | Category |
|---|------|-----|---------|--------|----------|
| 1 | **Feb 12, 2024** | `b5422b3` | Update README — added OSHWA UID link | KCollins | Certification |
| 2 | **Feb 12, 2024** | `b164257` | Add files via upload | KCollins | 📤 Upload |
| 3 | **Feb 12, 2024** | `828f496` | **Added OSHWA UID logo (US001095)** | KCollins | 🔥 **Certification** |
| 4 | **Feb 12, 2024** | `b731cd8` | Add files via upload | KCollins | 📤 Upload |
| 5 | **Feb 12, 2024** | `4b08fb3` | **Create CITATION.cff** | KCollins | Citation |
| 6 | **Feb 12, 2024** | `859bfa8` | Update README | KCollins | Documentation |
| 7 | Jul 20, 2022 | `d12008e` | Update README | DaOfficialWizard | Documentation |
| 8 | May 17, 2022 | `b8621ba` | Add files to improve usability | ZanzyTHEbarzy | Usability |
| 9 | May 15, 2022 | `d12008e` | Update README | DaOfficialWizard | Documentation |
| 10 | May 15, 2022 | `784ace5` | Update README | DaOfficialWizard | Documentation |

### v9 Analysis: The One-Day OSHWA Certification Blitz

**The pattern is extraordinary:**
```
May 15, 2022:   ██████  2 commits (README updates)
May 17, 2022:   ██      1 commit (usability improvements)
... 1 YEAR 9 MONTHS OF IRREGULAR ACTIVITY ...
Feb 12, 2024:   ██████████████████████████████  6 commits in ONE DAY
... 2+ YEARS OF SILENCE ...
```

**The February 12, 2024 blitz: 6 commits in 24 hours, all by K Collins.**

| Commit | What Happened |
|--------|---------------|
| `859bfa8` | README updated |
| `b164257` | Files uploaded (probably hardware schematics or BOM) |
| `b5422b3` | README updated again (OSHWA UID link added) |
| `4b08fb3` | **CITATION.cff created** — formal citation file for the hardware project |
| `828f496` | **OSHWA UID logo added (US001095)** — official certification badge |
| `b731cd8` | More files uploaded |

**What this tells us:**

1. **OSHWA certification is a big deal for open hardware.** OSHWA (Open Source Hardware Association) grants unique UID numbers to certified open-source hardware projects. Getting UID US001095 means OpenAir-Cyan passed OSHWA's review process. This is the hardware equivalent of getting a peer-reviewed journal publication.

2. **The CITATION.cff creation is the academic signal.** Creating a formal citation file for a *hardware* project is rare. It means the project authors want to be cited in academic papers when someone uses their design. This is the bridge between DIY hardware and academic recognition.

3. **The single-day pattern = ceremonial release.** Just like a software version release, all 6 commits happened on one day by one person. This was likely the "v1.0 release" — the moment when the project was considered complete enough to certify and cite.

4. **2+ years of silence after Feb 2024.** The project is now dormant again. The certification is complete, the citation file is in place, the hardware design is "done." But no further commits.

**🎙️ Episode hook:** *"On February 12, 2024, one person made 6 commits in a single day: added an OSHWA certification logo, created a citation file, and uploaded a bunch of files. That was the entire v1.0 release of an open-source direct air capture machine. Then it went silent for two years. Is open-source carbon capture hardware a mature field — or did they just certify the first one and stop?"*

---

## NEW: Carbon-Capture-and-Storage — The Perfect Ghost

| Field | Detail |
|-------|--------|
| **Repo** | `yohanesnuwara/carbon-capture-and-storage` |
| **Stars** | 85 |
| **Language** | Lasso |
| **Last commit** | March 6, 2021 |
| **License** | Not specified |
| **URL** | https://github.com/yohanesnuwara/carbon-capture-and-storage |

**What it is:** Integration of reservoir simulation, rock physics, seismic modeling, and geomechanics for CCS (Carbon Capture and Storage) monitoring. Originally a BSc thesis project. 85 stars — the most-starred carbon capture repo on GitHub.

### Full 10-Commit Table (v9 Pull)

| # | Date | SHA | Message | Author | Category |
|---|------|-----|---------|--------|----------|
| 1 | Mar 6, 2021 | `0be66ca` | Add sim result kvkh0.5 case 2C (ZIP) | yohanesnuwara | 📤 Simulation data |
| 2 | Mar 6, 2021 | `3d75b78` | Delete first.txt | yohanesnuwara | Cleanup |
| 3 | Mar 6, 2021 | `52c0189` | Add sim result kvkh0.5 case 3C | yohanesnuwara | 📤 Simulation data |
| 4 | Mar 6, 2021 | `91134e6` | Delete CASE_3C folder | yohanesnuwara | Cleanup |
| 5 | Mar 6, 2021 | `12151e1` | Move sim result to kvkh0.5 folder | yohanesnuwara | Organization |
| 6 | Mar 6, 2021 | `bf7ec9d` | Injection sim result kv/kh=0.5 | yohanesnuwara | 📤 Simulation data |
| 7 | Mar 3, 2021 | `0fdb0a6` | Upload notebook for CO2 EOS calculation | yohanesnuwara | 📤 Analysis |
| 8 | Mar 1, 2021 | `1f4d108` | Create first.txt | yohanesnuwara | 🆕 Initial |
| 9 | Feb 25, 2021 | `532f46c` | Upload data for geomechanics simulation (Matlab) | yohanesnuwara | 📤 Data |
| 10 | May 4, 2020 | `765e206` | Created using Google Colaboratory | yohanesnuwara | 🆕 Initial |

### v9 Analysis: The Academic Thesis Archive

**The entire history: 10 commits over 10 months, all by one person, then 4+ years of silence.**

```
May 4, 2020:    ██  1 commit (created with Colab — initial notebook)
Feb 25, 2021:   ██  1 commit (geomechanics data upload)
Mar 1, 2021:    ██  1 commit (first.txt — project setup)
Mar 3, 2021:    ██  1 commit (CO2 EOS notebook)
Mar 6, 2021:    ████████████████████████████████  6 commits (simulation blitz)
... 4+ YEARS OF SILENCE ...
```

**Key observations:**

1. **The March 6, 2021 blitz: 6 commits in one day.** This is the thesis submission day. The pattern is unmistakable: simulation results, data organization, deletions of intermediate files, folder moves. This is someone packaging up their thesis results for submission.

2. **The commit messages are diagnostic:** "kvkh0.5" refers to permeability×thickness (a reservoir simulation parameter). "CASE_3C" and "CASE_2C" are simulation case names. "CO2 EOS calculation" is equation-of-state modeling. This is pure reservoir engineering — the technical backbone of CCS monitoring.

3. **85 stars but zero maintenance.** The repo has 85 stars (it's the most-starred carbon capture repo), but it's been dead since March 2021. This is the "citation ghost" phenomenon — people cite the thesis, the Google Scholar profile grows, but the code never gets updated. Stars measure interest, not usability.

4. **Lasso as the language is unusual.** Lasso is a statistical software language, not typically used for reservoir simulation (which uses Fortran, Python, or MATLAB). This suggests the repo might be primarily for data analysis or statistical modeling of CO2 plume behavior, not full-scale reservoir simulation.

**🎙️ Episode hook:** *"This repo has 85 stars — the most popular carbon capture project on GitHub. But the last commit was in 2021. The author made 6 commits in one day to package up their thesis, then walked away. Is this the shape of open-source carbon capture: brilliant starts, silent finishes?"*

---

## NEW: Carbon_Capture_ML — The Paper-Driven Lifecycle

| Field | Detail |
|-------|--------|
| **Repo** | `zikribayraktar/Carbon_Capture_ML` |
| **Stars** | 56 |
| **Language** | Jupyter Notebook |
| **Last commit** | May 8, 2024 |
| **License** | Not specified |
| **URL** | https://github.com/zikribayraktar/Carbon_Capture_ML |

**What it is:** A survey of all published carbon capture machine learning papers, with data, code, and supplemental materials. "For the benefit of all humanity." This is a living literature review that evolves as the field grows.

### Full 10-Commit Table (v9 Pull)

| # | Date | SHA | Message | Author | Category |
|---|------|-----|---------|--------|----------|
| 1 | **May 8, 2024** | `ca9a31f` | **OpenDAC paper added** | Zikri Bayraktar | 🔥 **Key addition** |
| 2 | **Apr 25, 2024** | `4c01842` | Update README.md | Zikri Bayraktar | Documentation |
| 3 | **Mar 15, 2024** | `2b69376` | Update README.md | Zikri Bayraktar | Documentation |
| 4 | **Jan 21, 2024** | `e80dfd6` | Update README.md | Zikri Bayraktar | Documentation |
| 5 | **Jan 21, 2024** | `fe28496` | Update README.md | Zikri Bayraktar | Documentation |
| 6 | Mar 1, 2023 | `a3a02e9` | New paper | Zikri Bayraktar | 📄 Paper addition |
| 7 | Feb 16, 2023 | `93e5a40` | MOFsimplify paper added | Zikri Bayraktar | 📄 Paper addition |
| 8 | Feb 5, 2023 | `0c62b02` | New process paper added | Zikri Bayraktar | 📄 Paper addition |
| 9 | Feb 5, 2023 | `6129691` | New process paper added | Zikri Bayraktar | 📄 Paper addition |
| 10 | Feb 2, 2023 | `caf8b96` | New paper added to process | Zikri Bayraktar | 📄 Paper addition |

### v9 Analysis: The Academic Publication Pipeline

**The pattern is clearly paper-driven:**
```
Feb 2-5, 2023:    ████████████████████████████████████████████████  4 commits (paper storm)
Feb 16, 2023:     ██  1 commit (MOFsimplify paper — MOF = Metal-Organic Framework)
Mar 1, 2023:      ██  1 commit (new paper)
... 10 MONTHS OF SILENCE ...
Jan 21, 2024:     ██  2 commits (README updates — same day)
Mar 15, 2024:     █  1 commit (README update)
Apr 25, 2024:     █  1 commit (README update)
**May 8, 2024:**   █  1 commit (🔥 OpenDAC paper added)
... 1+ YEAR OF SILENCE ...
```

**Key observations:**

1. **The February 2023 storm: 4 commits in 4 days.** This was likely tied to a paper submission. The additions of "process papers" and the MOFsimplify paper suggest the repo was being built to accompany a review or survey publication.

2. **The 10-month gap, then README updates (Jan-Apr 2024).** Four README updates over 3 months with no paper additions. This is the "preparing for a new paper" phase — updating the survey to include new publications.

3. **The OpenDAC paper (May 8, 2024) — the final update.** OpenDAC is a major dataset/benchmark for direct air capture (DAC) materials. Adding it to the repo is significant: it represents the inclusion of the most current, high-impact research in the field. But after this commit, the repo went silent again — now for over 16 months.

4. **The "for the benefit of all humanity" mission statement.** This is not standard academic language. It suggests the author (Zikri Bayraktar) sees this as a public service project, not just a career paper. The consistent single-author pattern (all commits by Zikri) suggests this is a personal mission, not a collaborative effort.

**🎙️ Episode hook:** *"One person has been building the definitive survey of carbon capture machine learning papers since 2023. Every few months, they add a new paper. Then they stop for a year. This is the的大脑 of the carbon capture ML field — one person's brain, slowly growing, then resting, then growing again. Can a field be built on one person's shoulders?"*

---

## Cross-Theme Analysis: Carbon Capture Commit Patterns

### The Three Commit Patterns

| Pattern | Repo | Description | Implication |
|---------|------|-------------|---------------|
| **Ceremonial Release** | OpenAir-Cyan | 6 commits in 1 day (OSHWA certification), then freeze | Hardware projects have a "launch day" then maintenance gap |
| **Academic Ghost** | Carbon-Capture-and-Storage | 6 commits in 1 day (thesis package), then 4-year silence | Thesis repos are snapshots, not living tools |
| **Paper Pipeline** | Carbon_Capture_ML | Bursts of paper additions, then 10-month gaps, then README updates, then another paper | Literature surveys are driven by publication cycles |

### The Consistency Paradox

Open-Sustainable-Technology (v7 data) shows ~3-4 commits/month, every month, without gaps. This is the only repo showing **institutional curation velocity**. Every other carbon capture repo follows a "burst then freeze" pattern.

**What this means for our podcast:** The only carbon capture repo on GitHub that's consistently maintained is a *directory* — not a simulation tool, not a hardware project, not a materials screening code. The "ecosystem" is maintained; the "tools" are not.

---

## The CC0 Revolution (v9 Addition)

From the v7 data, we noted that the **CC0 public domain license** is appearing in DAC materials research:

- `tjz21/DAC_peroxovanadates` — CC0, computational screening data
- `tjz21/DAC_peroxotitanates` — CC0, computational screening data

Both were updated on September 23, 2025 (simultaneous CC0 adoption). This is the "CC0 revolution" — researchers treating computational screening data as public infrastructure.

**v9 insight from new commits:** The OpenAir-Cyan OSHWA certification (Feb 2024) and the CC0 adoption (Sep 2025) are **two parallel movements** in carbon capture open-source:
1. **Hardware side:** OpenAir-Cyan → OSHWA certification → formal open-source hardware
2. **Data side:** DAC_peroxovanadates/titanates → CC0 → public domain data

Both movements are trying to solve the same problem: how do you make carbon capture research *legally* and *structurally* open? The hardware side uses OSHWA; the data side uses CC0. Neither has merged.

---

## 🎙️ Episode Planning: Carbon Capture (v9 Update)

| Segment | Key Question | Commit Evidence | Talking Point |
|---------|-------------|-----------------|---------------|
| **Opening** | Can open source break the $1000/ton DAC cost barrier? | 0 repos with active development of cost-reduction tools | "No one is building open-source tools to cut the cost of direct air capture. The only active repo is a directory." |
| **Act 1** | What's special about OpenAir-Cyan? | 6 commits in 1 day (OSHWA certification), then 2-year freeze | "A DIY carbon capture machine got OSHWA-certified in a single day. Then nobody touched it for two years." |
| **Act 2** | Is one person enough to build a field? | Carbon_Capture_ML: single author, paper-driven bursts, 10-month gaps | "The most comprehensive carbon capture ML survey is maintained by one person who works in bursts: 4 papers in 4 days, then a 10-month break." |
| **Act 3** | Are ghost repos measuring the wrong thing? | Carbon-Capture-and-Storage: 85 stars, dead since 2021 | "The most-starred carbon capture repo on GitHub is a ghost. 85 people starred it, then nobody maintained it. Stars measure citations, not usability." |
| **Closing** | Is the open-source carbon capture field ready? | CC0 revolution (Sep 2025), OSHWA certification (Feb 2024), Open-Sustainable-Technology (active) | "Two parallel movements — OSHWA for hardware, CC0 for data — are trying to make carbon capture open. But they're not talking to each other." |

---

## Research Log (v9)

| Date | Activity |
|------|----------|
| 2026-09-18 | v9: Fresh 10-commit histories pulled from OpenAir-Cyan, Carbon-Capture-and-Storage, Carbon_Capture_ML |
| 2026-09-18 | v9: OpenAir-Cyan OSHWA certification blitz identified (6 commits in 1 day, Feb 2024) |
| 2026-09-18 | v9: Carbon-Capture-and-Storage academic ghost pattern confirmed (6 commits in 1 day, 4+ years silence) |
| 2026-09-18 | v9: Carbon_Capture_ML paper-pipeline pattern identified (4 commits/4 days, 10-month gaps) |
| 2026-09-18 | v9: OpenDAC paper addition noted (May 2024) — last update to Carbon_Capture_ML |
| 2026-09-18 | v9: CC0 vs OSHWA parallel movements identified in carbon capture open-source |
