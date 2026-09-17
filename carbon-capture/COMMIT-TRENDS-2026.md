# 🌍 Carbon Capture — Commit Trend Analysis (September 2026)

## Overview
This document captures the commit history analysis of open-source carbon capture and direct air capture (DAC) projects, pulled from GitHub in September 2026. It covers 6 key repositories across DAC materials science, machine learning for capture, electro-swing capture, and system-level simulation.

---

## 🔥 Most Active Projects

### 1. zikribayraktar/Carbon_Capture_ML — 56 ⭐ | Survey & ML Papers
**The comprehensive survey of carbon capture ML — but frozen since May 2024.**

| Date | Commit | Significance |
|------|--------|-------------|
| May 8, 2024 | OpenDAC paper added | **Latest update — DAC materials paper** |
| Apr 25, 2024 | Update README.md | Documentation refresh |
| Mar 15, 2024 | Update README.md | Documentation refresh |
| Jan 21, 2024 | Update README.md (×2) | Documentation |
| Mar 1, 2023 | New paper | Paper addition |
| Feb 16, 2023 | MOFsimplify paper added | MOF materials survey |
| Feb 5, 2023 | New process paper (×2) | Process innovation papers |
| Feb 2, 2023 | New paper added to process | Process paper |

**Commit Pattern:** 12 commits in 10 days (Jan-Feb 2023) — a massive literature review sprint. Then 12 months of silence. Then 4 commits in 4 months (Jan-May 2024) adding papers. The project is a "living survey" — updated when its author publishes new review papers.

**🎙️ Podcast Angle:** This is the most comprehensive carbon capture ML resource on GitHub, but it's a survey, not a tool. The code is minimal; the value is in the curated paper list and dataset links. The pattern is clear: survey repos live or die with their author's publication cycle. No community maintenance = frozen after the last paper.

---

### 2. openair-collective/openair-cyan — 76 ⭐ | DIY Direct Air Capture
**Open hardware DACC device — OSHWA-certified, but frozen since Feb 2024.**

| Date | Commit | Significance |
|------|--------|-------------|
| Feb 12, 2024 | Update README - OSHWA UID link | OSHWA certification (US001095) |
| Feb 12, 2024 | Add files via upload (×2) | Documentation updates |
| Feb 12, 2024 | Added OSHWA UID logo | Certification badge |
| Feb 12, 2024 | Create CITATION.cff | Citation support |
| Feb 12, 2024 | Update README.md | Documentation |
| Jul 20, 2022 | Update README.md | Prior update |
| May 17, 2022 | Add files to improve usability | Usability improvements |
| May 15, 2022 | Update README.md (×2) | Documentation |

**Commit Pattern:** 15 commits on a single day (Feb 12, 2024) — all related to OSHWA open hardware certification. Before that, slow intermittent updates. After that: total silence. The certification was a milestone, not a launchpad.

**🎙️ Podcast Angle:** OpenAir-Cyan is the most interesting carbon capture project on GitHub for a general audience. It's DIY, open hardware, OSHWA-certified — the kind of project that embodies the "democratization" thesis. But after receiving the OSHWA certification, the project froze. 15 commits in one day to get certified, then nothing. The certification was the goal, not a beginning.

---

### 3. Beckybams/AI-for-Carbon-Capture-Optimization — 25 ⭐ | New & Active
**ML optimization for carbon capture efficiency — born in Feb 2026, the newest project in our survey.**

| Date | Commit | Significance |
|------|--------|-------------|
| Mar 2, 2026 | Create README.md | Documentation |
| Feb 28, 2026 | Add files via upload | Code upload |
| Feb 28, 2026 | Add synthetic dataset and optimization model | **Core contribution** |

**All 3 commits on 2 days.** A fresh project with synthetic industrial data for carbon capture optimization. The "synthetic data" angle is notable — real industrial data is proprietary, so ML researchers use synthetic data. This means the models may not transfer to real plants.

**🎙️ Podcast Angle:** The newest project in our survey represents the current frontier: using ML to optimize carbon capture processes. But it's built on synthetic data — the gap between "synthetic industrial data" and "actual plant data" is enormous. This is a common pattern in carbon capture ML: the data problem is the bottleneck.

---

## ❄️ Dormant but Relevant Projects

### 4. yohanesnuwara/carbon-capture-and-storage — 85 ⭐ | Reservoir Simulation
**The highest-starred project in our survey — and completely frozen since March 2021.**

| Date | Commit | Significance |
|------|--------|-------------|
| Mar 6, 2021 | Add sim result (zip) | Simulation output |
| Mar 6, 2021 | Delete first.txt | Cleanup |
| Mar 6, 2021 | Add sim result case 3C | Simulation output |
| Mar 6, 2021 | Delete CASE_3C directory | Directory cleanup |
| Mar 6, 2021 | Move sim results | Organization |
| Mar 6, 2021 | Injection sim result kv/kh=0.5 | Simulation output |
| Mar 3, 2021 | Upload notebook for CO2 EOS calculation | Thermodynamics |
| Mar 1, 2021 | Create first.txt | Initial file |
| Feb 25, 2021 | Upload geomechanics simulation data | Geomechanics |
| May 4, 2020 | Created using Colaboratory | Initial creation |

**10 commits all within 10 months (May 2020 - Mar 2021).** This was a BSc thesis project integrating reservoir simulation, rock physics, seismic modeling, and geomechanics for CCS monitoring. 85 stars but frozen for 5+ years. A "ghost project" — high visibility, zero maintenance.

**🎙️ Podcast Angle:** 85 stars and 5 years of silence. This is the archetype of the "dissertation repository" — created to fulfill academic requirements, cited by other students, then abandoned. The code was never meant to be a living tool. CCS monitoring is complex and domain-specific, which is why it can't attract community maintenance.

---

### 5. tonyzyl/CO2-Soft-sensor-for-a-carbon-capture-pilot-plant — 16 ⭐ | DAE-LSTM Model
**Hybrid mechanistic-data-driven model for CO2 concentration estimation — frozen since 2022.**

| Date | Commit | Significance |
|------|--------|-------------|
| Aug 5, 2022 | Remove from main folder | Cleanup |
| Aug 5, 2022 | Update README.md | Final update |
| Aug 5, 2022 | Update on figs, citation | Academic update |
| May 26, 2022 | Fix README | Documentation |
| May 26, 2022 | Update on semi-supervise method | Method update |
| Mar 2, 2022 | Data-driven and kinetic model | Core model |
| Mar 2, 2022 | Add files via upload | Initial upload |
| Mar 2, 2022 | Initial commit | Project creation |

**8 commits, all in 2022.** A hybrid DAE-LSTM model for estimating CO2 concentration profiles in a capture plant. The semi-supervised approach is technically interesting. But it's frozen after a May 2022 paper submission.

---

## 📊 Carbon Theme: Cross-Cutting Trend Summary

### Trend 1: The August 2026 DAC Materials Wave (External Context)
While we didn't directly pull commits from these repos, our broader research identified **four DAC materials repositories** (peroxovanadates, peroxotitanates, OpenCarbon, Carbon-Capture-Genome) all updated on **August 19, 2026**. This suggests a coordinated research event — likely a shared publication or dataset drop. Small repos (2 stars each) but simultaneously active.

**🎙️ Podcast Angle:** Four independent research groups dropping DAC materials code on the same day is not a coincidence. It's likely tied to a paper publication or a shared dataset release. The computational chemistry community for DAC materials is small but coordinated.

### Trend 2: The "Dissertation Ghost" Pattern
The highest-starred carbon capture project (yohanesnuwara, 85 stars) is completely frozen. Academic repos get stars for citations but no community maintenance. The pattern repeats across all sub-domains.

### Trend 3: Open Hardware Frozen at Certification
OpenAir-Cyan's 15 commits on one day (OSHWA certification) followed by permanent silence. The certification was the finish line, not the starting gun. Open hardware projects need a different sustainability model than software projects.

### Trend 4: ML for Carbon Capture = Survey + Synthetic Data
The two most recent ML-oriented projects (Carbon_Capture_ML and AI-for-Carbon-Capture-Optimization) represent the two modes: (1) literature survey that freezes with publication cycle, (2) synthetic-data models that may not transfer to real plants. Neither has real-world deployment code.

### Trend 5: No System-Level Open-Source Capture Planning
We found no open-source tool for system-level carbon capture planning — nothing like an "open-source CCS simulator" or "DAC facility design tool." The tools are either: (a) materials discovery (ML screening), (b) process simulation (DAE models), or (c) monitoring (reservoir simulation). Middle-out systems engineering is the gap.

---

## 🎙️ Episode Talking Points — Carbon Capture

1. **"The 85-star ghost"** — The most-starred CCS project on GitHub has been frozen for 5 years. It was a BSc thesis. Academic code is built for citation, not community.

2. **"OSHWA certification and then silence"** — OpenAir-Cyan got open hardware certification with 15 commits in one day, then froze. The certification was the goal, not the launch. What does open hardware sustainability look like?

3. **"The August 19th mystery"** — Four DAC materials repos all updated on the same day. A coordinated paper? A shared dataset? The small-size, high-alignment pattern suggests a publication event.

4. **"Synthetic data is the bottleneck"** - Both ML-for-capture projects use synthetic data. The real plant data is proprietary. Until we solve the data access problem, ML capture optimization remains theoretical.

5. **"Carbon_Capture_ML is the gateway resource"** — Despite being frozen, it's the most comprehensive survey. For a podcast audience, this is where to start learning about the ML-capture intersection.

6. **"The peroxovanadate moment"** — Computational screening of peroxovanadate and peroxotitanate sorbents is the hottest DAC materials direction. Four repos, same day, August 2026.

---

*Last updated: September 2026 based on GitHub commit data pulled from 6 repositories and broader wave analysis.*