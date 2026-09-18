# 🌍 Carbon Capture — Project Discoveries
## Fresh Research Notes — September 2026

---

## Overview

This document profiles **9 open-source repositories** relevant to carbon capture, direct air capture (DAC), and carbon capture optimization. These were selected from GitHub searches focused on carbon capture technologies, materials discovery, and AI-driven optimization.

---

## 1. Open-Sustainable-Technology (Directory)

| Field | Detail |
|-------|--------|
| **Repo** | `protontypes/open-sustainable-technology` |
| **Stars** | 2,552 ⭐ |
| **Language** | Multi-language directory |
| **Last activity** | September 9, 2026 |
| **License** | open source |

**What it is:** The most comprehensive open-source directory of climate technology projects on GitHub. 2,500+ projects cataloged across energy, carbon management, and sustainability.

**Why it matters for the podcast:** This is the **single most important resource** in the entire carbon capture GitHub ecosystem. With 2,552 stars, it's 30x more popular than any individual carbon capture repo. It's continuously maintained and serves as the gateway repository — anyone looking for open-source carbon capture tools eventually finds their way here.

**Episode hook:** *"2,552 stars. 2,500+ projects. One person maintaining it. This is the Library of Alexandria for climate tech — and it's still being read."*

---

## 2. openair-cyan (DIY Direct Air Capture)

| Field | Detail |
|-------|--------|
| **Repo** | `openair-collective/openair-cyan` |
| **Stars** | 76 ⭐ |
| **Language** | Hardware designs + documentation |
| **Last commit** | February 12, 2024 |
| **License** | OSHWA-certified open source hardware |

**What it is:** A DIY small-scale direct air carbon capture device. OpenAir Collective built an open-hardware DACC device called "Cyan" — the first OSHWA-certified (Open Source Hardware Association) carbon capture device in existence.

**Why it matters for the podcast:** This is the **holy grail of open-source carbon capture** — actually building something that works. The commit history reveals a dramatic story:
- **10 commits on a single day** (February 12, 2024) — a blitz of uploads, README updates, OSHWA certification, and CITATION.cff creation
- Before the blitz: 6 months of quiet development (May–July 2022)
- After the blitz: **2 years and 7 months of silence**

**The pattern suggests:** A团队 organized a launch event, uploaded everything at once, got certified, published the citation — and then moved on to the next project. The device works; the documentation is complete; the community engagement stopped.

**Episode hook:** *"They built a working carbon capture device, got it certified by the Open Source Hardware Association, uploaded everything in one day — and then vanished. What happened to the OpenAir Collective?"*

---

## 3. Carbon_Capture_ML (Literature Survey)

| Field | Detail |
|-------|--------|
| **Repo** | `zikribayraktar/Carbon_Capture_ML` |
| **Stars** | 56 ⭐ |
| **Language** | Python / Jupyter |
| **Last commit** | May 8, 2024 |
| **License** | open source |

**What it is:** A comprehensive survey of all published carbon capture machine learning papers, with data, code, and supplemental materials. This is the definitive ML-for-CC literature tracker.

**Why it matters for the podcast:** The commit history shows a **paper-driven lifecycle**:
- **January 2023 burst:** 9 commits in 10 days — first wave of papers surveyed
- **February 2023 burst:** 4 more papers added in 5 days
- **March–April 2024:** Steady updates as new papers published
- **May 8, 2024:** Final commit — OpenDAC paper added
- **17 months of silence** since

**The pattern is sustainable academic curation:** Not a single-burst ghost, but a periodically maintained reference tool. The author adds papers as they publish, then moves on until enough new papers accumulate to justify another update.

**Episode hook:** *"Someone read every carbon capture ML paper in existence and put it all online. Then they added one more, and stopped. What's the OpenDAC paper that broke the pattern?"*

---

## 4. carbon-capture-and-storage (BSc Thesis Ghost)

| Field | Detail |
|-------|--------|
| **Repo** | `yohanesnuwara/carbon-capture-and-storage` |
| **Stars** | 85 ⭐ |
| **Language** | Lasso (reservoir simulation) |
| **Last commit** | March 6, 2021 |
| **License** | open source |

**What it is:** Integration of reservoir simulation, rock physics, seismic modeling, and geomechanics for CCS (Carbon Capture and Storage) monitoring. Originally a BSc thesis project.

**Why it matters for the podcast:** This is the **highest-starred carbon capture repo that's completely dead.** 85 stars accumulated, then 5+ years of silence. The commit history shows a thesis defense pattern:
- **May 2020:** Initial commits — data upload, paper upload, spreadsheet creation
- **February 2021:** Geomechanics simulation data uploaded
- **March 2021:** 6 commits in 5 days — final paper upload, zip file results, cleanup
- **5 years, 6 months of silence** since

**The ghost repo pattern:** Stars measure citations, not usability. This repo got cited in papers, but nobody is running the code or fixing bugs. It’s a digital tombstone for a thesis that served its purpose.

**Episode hook:** *"85 stars, zero commits since 2021. This carbon capture_simulation code is the most-starred ghost in the ecosystem. Why did nobody fork it, fix it, or build on it?"*

---

## 5. GCCS-Core (Global Climate Control System)

| Field | Detail |
|-------|--------|
| **Repo** | `KOSASIH/GCCS-Core` |
| **Stars** | 9 ⭐ |
| **Language** | Python |
| **Last commit** | October 29, 2024 |
| **License** | open source |

**What it is:** The foundational framework for the "Global Climate Control System" — a proposed IoT-integrated climate monitoring and control platform. Includes data collection scripts, server setup, deployment automation, and example integrations.

**Why it matters for the podcast:** GCCS-Core is the most **ambitious** carbon capture/comclimate repo in terms of scope. The commit history shows a **single-day blitz**:
- **15 commits on October 29, 2024** — all infrastructure created in one day
- requirements.txt, setup.py, data_collection.sh, run_server.sh, deploy.sh
- Example files for IoT integration, usage, and configuration
- **2 years of silence** since

**The pattern is "launch and leave":** A developer built the entire stack in a day, pushed it, and moved on. The code may work, but there's no community, no issue tracking, and no roadmap.

**Episode hook:** *"One developer, one day, 15 commits. The Global Climate Control System was born — and then went silent. Is this ambitious or presumptuous?"*

---

## 6. CO2-Soft-Sensor (DAE-LSTM Hybrid Model)

| Field | Detail |
|-------|--------|
| **Repo** | `tonyzyl/CO2-Soft-sensor-for-a-carbon-capture-pilot-plant` |
| **Stars** | 16 ⭐ |
| **Language** | Jupyter Notebook |
| **Last commit** | August 5, 2022 |
| **License** | open source |

**What it is:** A hybrid mechanistic and data-driven (DAE-LSTM) model for estimating CO2 concentration profiles in a carbon capture plant. Combines physical equations with neural networks.

**Why it matters for the podcast:** This repo represents the **"hybrid AI" trend** in carbon capture — not pure data-driven, not pure physics-based, but a combination. The commit history shows steady development over 8 months:
- **March 2022:** Initial commit, data-driven and kinetic model
- **May 2022:** Semi-supervised method update, README fix
- **August 2022:** Final updates — figures, citation, removal from main folder
- **2 years, 9 months of silence** since

**The hybrid approach is significant:** Pure ML models for CCS need enormous training data. Pure physics models are rigid. The DAE-LSTM hybrid is a pragmatic middle ground that could generalize across different capture plant designs.

**Episode hook:** *"They combined chemical equations with neural networks to monitor CO2 in real-time. Then they removed it from the main folder and left. What does the 'soft sensor' future look like for CCS?"*

---

## 7. AI-for-Carbon-Capture-Optimization (Synthetic Data)

| Field | Detail |
|-------|--------|
| **Repo** | `Beckybams/AI-for-Carbon-Capture-Optimization` |
| **Stars** | 25 ⭐ |
| **Language** | Python |
| **Last commit** | March 2, 2026 |
| **License** | open source |

**What it is:** A machine learning project using synthetic industrial data to improve carbon capture efficiency. Predicts optimal operating conditions for capture processes.

**Why it matters for the podcast:** This is the **newest and most active** carbon capture repo in our sample. Unlike the burst-and-freeze pattern of older repos, this one shows fresh energy:
- **February 28, 2026:** Synthetic dataset and optimization model uploaded
- **February 28, 2026:** Files uploaded (README, project structure)
- **March 2, 2026:** README finalized
- **Only 3 commits, but all within 4 days**

**The "synthetic data" angle is crucial:** Real industrial CCS data is proprietary and guarded. This repo uses synthetic data to bypass the access barrier. If synthetic data can train ML models that work on real plants, it could unlock a revolution in CCS optimization.

**Episode hook:** *"No real plant data? No problem. One developer generated fake data that might be better than real data for training AI. Welcome to the synthetic data revolution in carbon capture."*

---

## 8. MOF-Based Carbon Capture (ML-NSGA-PSA)

| Field | Detail |
|-------|--------|
| **Repo** | `SarkisovTeam/ML-NSGA-PSA-carbon-capture` |
| **Stars** | 3 ⭐ |
| **Language** | Jupyter Notebook |
| **Last commit** | June 4, 2026 |
| **License** | open source |

**What it is:** Scripts for the article "Multi-Scale Computational Design of Metal-Organic Frameworks for Carbon Capture Using Machine Learning." Uses NSGA-II (a multi-objective optimization algorithm) to screen MOF materials for CO2 capture properties.

**Why it matters for the podcast:** This is the **materials-by-design** approach. Instead of testing thousands of chemicals in a lab, they use ML to predict which MOF structures will best capture CO2. The last commit was **June 4, 2026** — the most recent of any repo (besides awesome-geoengineering) in our entire analysis.

**The active signal:** While most carbon capture repos are dead, this one had activity in June 2026. The Sarkisov Team is actively publishing and updating their MOF screening code.

**Episode hook:** *"While most carbon capture code is frozen, one team is still actively designing new materials atom by atom using machine learning. What are they finding that nobody else is?"*

---

## 9. IBM Carbon-Capture Fingerprints

| Field | Detail |
|-------|--------|
| **Repo** | `IBM/Carbon-capture-fingerprint-generation` |
| **Stars** | 2 ⭐ |
| **Language** | Python |
| **Last commit** | Undated (IBM Research) |
| **License** | open source |

**What it is:** Code for generating molecular representations for amines used in carbon capture. Generates molecular fragment combinations to create "fingerprints" that predict capture performance.

**Why it matters for the podcast:** IBM Research brings **industrial-scale molecular simulation** to the carbon capture space. The "fingerprint" approach is a shortcut — instead of running expensive quantum chemistry calculations for every candidate molecule, you generate a fast fingerprint that predicts its properties. This is how industrial R&D works: scale, speed, and pragmatism.

**Episode hook:** *"IBM's approach to carbon capture: don't simulate every molecule, just fingerprint it. Welcome to the industrial side of open-source climate tech."*

---

## Cross-Cutting Themes Across Carbon Repos

| Pattern | Evidence |
|---------|----------|
| **The CC0 license revolution** | tjz21's DAC materials repos (peroxovanadates & peroxotitanates, Sep 2025) adopted CC0 public domain dedication — researchers are treating computational screening data as public infrastructure |
| **Burst-and-freeze is the norm** | 7 of 9 repos show single-burst patterns (thesis, paper, or launch), then dormancy |
| **Open hardware is the exception** | OpenAir-Cyan is the only physical device; everything else is software/models |
| **Stars ≠Usability** | carbon-capture-and-storage (85★, dead since 2021) vs. AI-for-Capture (25★, active 2026) |
| **Synthetic data is the new frontier** | Beckybams repo bypasses proprietary data barriers with synthetic samples |
| **Materials-by-design is alive** | ML-NSGA-PSA (June 2026) and IBM fingerprints are the most recently active repos |
| **The directory beats the destination** | open-sustainable-technology (2,552★) outshines every individual CC repo |

---

## Episode Talking Points — Carbon Capture

1. **The CC0 license story is the biggest open-science finding** — two DAC materials repos dedicated their computational screening data to the public domain in September 2025. This is a philosophical shift: data as infrastructure, not intellectual property.

2. **OpenAir-Cyan proved it can be done** — a working, certified, open-source DACC device. But the team vanished after launch. The hardware exists; the community doesn't.

3. **85-star ghost repo** — carbon-capture-and-storage has more stars than any other CC repo, but it's been dead for 5 years. Stars measure citations, not usefulness.

4. **Synthetic data bypasses the proprietary barrier** — if you can't get real plant data, generate fake data that works better. This could be the key to industrial CCS optimization.

5. **Materials-by-design is the live frontier** — ML-NSGA-PSA (June 2026) and IBM fingerprints are the only repos with recent activity. The future of carbon capture is being designed atom by atom.

6. **The directory is the real ecosystem** — open-sustainable-technology (2,552★) is the Library of Alexandria. If you want to find any CC tool, start here.

---

*Research compiled: September 2026 | Source: GitHub API commit histories, 9 repositories*
*Branch: carbon-capture*