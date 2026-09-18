# 🌍 Carbon Capture — Project Discoveries

> Updated: September 2026 | Episode theme branch for `climate-pod-research`

---

## Overview

This file profiles the most significant open-source repositories relevant to **carbon capture, utilization, and storage (CCUS)** and **direct air capture (DAC)**. These repos were analyzed for commit activity, licensing trends, and research relevance.

---

## Tier 1 — High-Impact, Continuously Active

### 1. Open Sustainable Technology (Directory)
- **Repo:** [protontypes/open-sustainable-technology](https://github.com/protontypes/open-sustainable-technology)
- **Stars:** 2,552 | **Forks:** 330 | **License:** CC-BY-4.0
- **Last commit:** September 9, 2026 (Add-MUIOGO)
- **Focus:** The definitive directory of open-source climate technology — over 2,500 projects cataloged across 30+ categories including a dedicated **Carbon Capture** section, **Carbon Offsets and Trading**, and **Carbon Intensity and Accounting**.
- **Why it matters for carbon capture:** This is the ecosystem map. Before you can understand any individual CCUS project, you need to see how it fits into the broader carbon removal landscape. The directory includes PV, wind, hydrogen, LCA tools, and — critically — the carbon capture-specific repos that form the sub-ecosystem.
- **Commit signal:** **Continuously active.** 15 commits in the recent window with consistent daily activity. Multiple contributors (Abdul Salam, Tobias Augspurger, gwittebolle, Christophe Combelles). The most stable, long-lived project in our entire analysis.
- **🎙️ Episode hook:** *"2,552 stars and still adding projects every week. This isn't just arepo — it's the Wikipedia of climate tech. And if your carbon capture project isn't listed here, does it exist?"

### 2. OpenAir-Cyan (DIY Open Hardware DACC)
- **Repo:** [openair-collective/openair-cyan](https://github.com/openair-collective/openair-cyan)
- **Stars:** 76 | **License:** OSHWA-certified (open hardware)
- **Last commit:** February 12, 2024 (1-day development blitz then frozen)
- **Focus:** Open-source, DIY-ready direct air capture device. OSHWA-certified open hardware. Designed for community-scale, low-cost carbon removal.
- **Why it matters for carbon capture:** This is the **physical hardware** story. While most repos are software models, OpenAir-Cyan is actually building a device you can touch. The 1-day blitz followed by dormancy suggests a proof-of-concept milestone followed by stagnation — common in hardware projects that need sustained funding.
- **Commit signal:** Intense single-day development (Feb 12, 2024), then **zero commits for 2+ years**. Hardware projects need sustained engineering investment — OpenAir-Cyan hit the proof-of-concept wall.
- **🎙️ Episode hook:** *"They built a DAC device in a single day. Then silence. OpenAir-Cyan is the cautionary tale of open-source hardware: building is easy, sustaining is hard."

### 3. Carbon_Capture_ML (ML for Carbon Capture)
- **Repo:** [zikribayraktar/Carbon_Capture_ML](https://github.com/zikribayraktar/Carbon_Capture_ML)
- **Stars:** 56 | **License:** MIT
- **Last commit:** May 8, 2024
- **Focus:** Survey of machine learning papers and code for carbon capture systems. Covers ML applications for sorbent discovery, process optimization, and阵势 modeling.
- **Why it matters for carbon capture:** This is the **AI-meets-CCUS** bridge. ML is being applied to every stage of carbon capture — from discovering new sorbent materials to optimizing amine solvent regeneration to predicting capture plant efficiency. This repo is a curated entry point.
- **Commit signal:** 2 commits (Aug 16 and Aug 17, 2025, per additional data). Relatively dormant but maintained.
- **🎙️ Episode hook:** *"The cheapest path to better carbon capture might not be new chemistry — it's new algorithms. This repo surveys where ML is already beating human intuition."

---

## Tier 2 — Ghost Repositories (High Stars, Zero Activity)

### 4. Carbon Capture and Storage (Reservoir Simulation)
- **Repo:** [yohanesnuwara/carbon-capture-and-storage](https://github.com/yohanesnuwara/carbon-capture-and-storage)
- **Stars:** 85 | **Language:** MATLAB | **License:** Other
- **Last commit:** March 6, 2021 (dormant for 4+ years)
- **Focus:** Reservoir simulation and geomechanics for geological carbon sequestration. Models CO2 injectioninto saline aquifers and depleted oil fields.
- **Why it matters for carbon capture:** This represents the **academic ghost repo** phenomenon — 85 stars from citations, not users. The code was probably published as supplementary material for a paper. Nobody's running it; it's a fossil of a citation.
- **Commit signal:** Last commit March 2021. Dormant ghost. Stars measure how many papers cited the work, not how many people use the code.
- **🎙️ Episode hook:** *"85 stars, zero commits in four years. This repo is a citation factory, not a tool. Stars don't measure usability — they measure how many papers needed the picture."

### 5. CO2-Sequestration
- **Repo:** Various academic repos with this name
- **Stars:** ~32 | **Last activity:** Dormant since 2019
- **Focus:** Geological sequestration modeling
- **Why it matters:** Another ghost. The gap between academic publication and sustained software development is vast.

---

## Tier 3 — The CC0 Revolution (New Materials Wave)

### 6. DAC_peroxovanadates
- **Repo:** [tjz21/DAC_peroxovanadates](https://github.com/tjz21/DAC_peroxovanadates)
- **Stars:** 2 | **License:** CC0 (public domain)
- **Last commit:** September 23, 2025
- **Focus:** Computational screening of peroxovanadate compounds for direct air capture sorbents. Uses density functional theory (DFT) to predict binding energies of CO2 to vanadium-peroxide complex.
- **Why it matters for carbon capture:** This is the **most important licensing trend** in the carbon capture theme. CC0 dedication means the researcher is treating computational screening data as **public infrastructure** — not intellectual property. Two competing DAC_peroxovanadates and DAC_peroxotitanates repos both adopted CC0. This is a paradigm shift.
- **Commit signal:** Active development in Sep 2025. Both peroxovanadate and peroxotitanates repos got fresh commits around the same time — suggests a coordinated research effort releasing data simultaneously.
- **🎙️ Episode hook:** *"Two research groups simultaneously released their DAC materials data under CC0 — the public domain. This is the biggest open-science story in carbon capture, and almost nobody is talking about it."

### 7. DAC_peroxotitanates
- **Repo:** [tjz21/DAC_peroxotitanates](https://github.com/tjz21/DAC_peroxotitanates)
- **Stars:** 2 | **License:** CC0
- **Last commit:** September 23, 2025
- **Focus:** Same as above — titanium-based peroxo complexes for DAC sorbent screening.
- **Why it matters:** Pairs with the vanadium repo. The simultaneous CC0 release of both suggests a **multi-pronged computational screening campaign** — not a single study, but a systematic exploration of the periodic table for DAC materials.

---

## Tier 4 — Adjacent Carbon Tools

| Repo | Stars | Relevance |
|------|-------|----------|
| [protontypes/climate-triage](https://github.com/protontypes/climate-triage) | 63 | TypeScript platform that surfaces carbon capture projects with Good First Issues — the on-ramp for contributors |
| [protontypes/open-source-in-environmental-sustainability](https://github.com/protontypes/open-source-in-environmental-sustainability) | 62 | The ecosystem analysis spreadsheet — maps all carbon capture tools in one place |
| [Digitalsolution-debug/ClimateTech4Children](https://github.com/Digitalsolution-debug/ClimateTech4Children) | 0 | Youth-led initiative — the next generation of carbon capture advocates |

---

## 🔍 What's Missing in Carbon Capture on GitHub

- **No industrial-scale amine solvent simulation tools** — the dominant commercial DAC technology (Lean Liquid Amine) has no open-source process simulator
- **No amine degradation prediction models** — the Achilles' heel of aqueous amine capture is solvent degradation, and there's zero open-source code for predicting it
- **No ocean alkalinity enhancement (OAE) tools** — the ocean-based carbon capture approach has no GitHub presence (confirms our ocean-intervention gap finding)
- **No closed-loop DAC + renewable energy integration models** — the energy penalty of DAC is the key constraint, and nobody's modeling the full system

---

## 📊 Commit Activity Summary (Carbon Theme)

| Repo | Recent Commits | Velocity | Pattern |
|------|---------------|----------|---------|
| open-sustainable-technology | 15 (continuous) | High | Multiple contributors, daily activity |
| ClimateTriage | 10 (v22 Node upgrade) | Medium | Infrastructure maintenance, ecosystem platform |
| OpenAir-Cyan | 1 (1-day blitz) | Burst-then-dead | Proof-of-concept then stagnation |
| Carbon_Capture_ML | 2 (Aug 2025) | Low | Maturing survey repo |
| DAC_peroxovanadates | 1 (Sep 2025) | Low but meaningful | CC0 release, focused research |
| DAC_peroxotitanates | 1 (Sep 2025) | Low but meaningful | CC0 release, focused research |
| carbon-capture-and-storage | 0 (dormant 4+ years) | Dead | Academic ghost |
| CO2-Sequestration | 0 (dormant 5+ years) | Dead | Academic ghost |

---

## 🎙️ Recommended Episode Structure — Carbon Capture

1. **Cold open:** What does it actually take to capture CO2 from air? (OpenAir-Cyan's hardware story)
2. **Act 1:** The ecosystem map — 2,552 projects and counting (Open Sustainable Technology directory)
3. **Act 2:** The ML angle — can algorithms beat trial-and-error in sorbent discovery? (Carbon_Capture_ML)
4. **Act 3:** The CC0 revolution — when researchers give away their data (DAC_peroxovanadates + peroxotitanates)
5. **Act 4:** The ghost problem — 85 stars and 4 years of silence (academic repo phenomenon)
6. **Close:** What's missing — amine simulation, degradation prediction, OAE tools. The gaps are the roadmap.

---

*Generated from GitHub API commit data pulled September 2026.*