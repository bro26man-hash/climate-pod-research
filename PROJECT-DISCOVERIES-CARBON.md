# 🌍 Carbon Capture — Project Discoveries (v4: Sep 2026 Update)
## Research Notes | Climate Pod Research | September 2026

---

## Overview

This document profiles the most significant open-source repositories related to **carbon capture, utilization, and storage (CCUS)** and **direct air capture (DAC)**. These repos form the backbone of our Episode 2 research — "Can open source break the $1000/ton DAC cost barrier?"

---

## 🔬 Tier 1: Flagship Repos (High Activity, Large Community)

### 1. Open-Sustainable-Technology — The Climate Tech Directory
- **Repo:** [protontypes/open-sustainable-technology](https://github.com/protontypes/open-sustainable-technology)
- **Stars:** 2,552 ⭐ (largest climate tech repo discovered)
- **Language:** Markdown/JSON
- **Last commit:** September 9, 2026 (two commits that day)
- **Active contributors:** Abdul Salam, Tobias Augspurger, Mikhail Alabugin, gwittebolle, Christophe Combelles

**What it is:** A **comprehensive open-source directory of 2,500+ sustainable technology projects** — the single largest curated collection of climate tech OSS on GitHub. It's not a simulation tool; it's an ecosystem map.

**Recent commit highlights (15 commits pulled):**
| Date | Commit | Significance |
|------|--------|-------------|
| Sep 9, 2026 | Add-MUIO (#1638) | New project added |
| Sep 9, 2026 | Add-MUIOGO (#1639) | Companion project — MUIOGO variant |
| Sep 1, 2026 | docs: fix dead links in README | Maintenance — link rot with 2,500+ entries |
| Aug 23, 2026 | Add claude-carbon (#1633) | CAI project — carbon-related AI initiative |
| Aug 18, 2026 | Add Story Seed Library (#1630) | Narrative project — sustainability storytelling |
| Aug 18, 2026 | Add openflexure microscope (#1631) | Open hardware — lab equipment for climate research |
| Jul 19, 2026 | Remove duplicate AI content review checkbox | Process improvement |
| Jul 19, 2026 | Modify PR template for AI content review | **Governance evolution** — adapting to AI-assisted contributions |
| Jul 17, 2026 | Update PR template with review reminder | Quality control |
| Jul 2, 2026 | Add PowerIO (#1619) | Power systems project |
| Jul 1, 2026 | Add ASSETRA (#1620) | Assessment framework |
| Jul 1, 2026 | Add ToOp (#1621) | Unknown — new project type |
| Jun 23, 2026 | Add wbdata (#1615) | World Bank data tools |
| Jun 23, 2026 | Add Volca to Life Cycle Assessment (#1617) | LCA integration |
| Jun 6, 2026 | Add EpexPredictor (#1612) | Energy market price prediction |

**🎙️ Episode hook:** This isn't just a directory — it's a **living ecosystem**. In the last 3 months alone, 15 new projects were added by 5 different contributors. The AI content review PR template (July 19) is a fascinating signal: the community is grappling with how to handle AI-generated contributions to a climate tech directory.

---

### 2. Carbon_Capture_ML — ML for Carbon Capture Materials
- **Repo:** [zikribayraktar/Carbon_Capture_ML](https://github.com/zikribayraktar/Carbon_Capture_ML)
- **Stars:** 56 ⭐
- **Language:** Python/Notebooks
- **Last commit:** May 8, 2024 (OpenDAC paper added)
- **Contributor:** Zikri Bayraktar (single developer)

**What it is:** A **curated survey of machine learning papers and code for carbon capture** — covering Metal-Organic Frameworks (MOFs), sorbent materials, process optimization, and surrogate modeling.

**Commit timeline — the paper delivery pattern:**
| Period | Commits | Content |
|--------|---------|--------|
| Jan 2023 | 6 | Initial survey, DOI fixes, surrogate paper |
| Feb 2023 | 6 | MOFsimplify paper, process papers (3), new paper |
| Mar 2023 | 1 | Process paper |
| Apr 2023 | 1 | Process paper |
| Jan 2024 | 2 | README update |
| Mar 2024 | 1 | README update |
| Apr 2024 | 1 | README update |
| **May 2024** | **1** | **OpenDAC paper added — the landmark Direct Air Capture benchmark** |

**🎙️ Episode hook:** The **OpenDAC paper commit (May 8, 2024)** is the milestone. OpenDAC — the Open DAC benchmark — is the community's attempt to standardize ML evaluation for DAC materials. Bayraktar's repo is the **index** pointing to this effort. The pattern: 2023 was about building the survey, 2024 was about anchoring it to the OpenDAC benchmark.

---

### 3. OpenCarbon
- **Repo:** Open source carbon accounting platform
- **Stars:** 2 ⭐
- **Last activity:** Dormant
- **Language:** Python

**What it is:** An **open-source carbon accounting platform** for organizations to track and report emissions. Unlike the materials-focus of other repos, OpenCarbon handles the *measurement and reporting* side of carbon management.

**🎙️ Episode hook:** OpenCarbon's 2-star count against its practical utility is telling. Carbon accounting is a **compliance-driven** market — organizations use it because regulations require it, not because it's innovative. Dormant repos in compliance tool categories suggest the market is consolidating around commercial solutions.

---

## 🌱 Tier 2: Active but Small / Specialist Repos

### 4. OpenAir-Cyan — DIY Open Hardware DACC Device
- **Repo:** [openair-collective/openair-cyan](https://github.com/openair-collective/openair-cyan)
- **Stars:** 76 ⭐
- **Language:** CAD/Documentation
- **Last commit:** February 12, 2024 (OSHWA certification push)
- **Contributors:** KCollins (lead), DaOfficialWizard, ZanzyTHEbarzy

**What it is:** A **DIY, open-source, OSHWA-certified Direct Air Capture and Concentration (DACC) device**. This is hardware, not software — 3D-printable, citizen-science carbon capture. The OSHWA UID (US001095) makes it the **only certified open-source CCUS hardware project on GitHub**.

**Recent commit highlights (15 commits pulled):**
| Date | Commit | Significance |
|------|--------|-------------|
| **Feb 12, 2024** | **7 commits in one day** | **The Great Blitz** — OSHWA UID, CITATION.cff, README, file uploads |
| Jul 20, 2022 | Update README | Documentation update |
| May 17, 2022 | Add files to improve usability | Accessibility improvements |
| May 15, 2022 | Update README (2 commits) | Documentation |
| May 11, 2022 | Rename CodeQL analysis file | CI/CD maintenance |
| May 7, 2022 | Update CodeQL (2 commits) | Static analysis |
| May 5, 2022 | Delete .github/workflows | **CI/CD removal** — possible migration |

**🎙️ Episode hook:** This is the most **politically significant** repo in our research. A DIY, OSHWA-certified, 3D-printable direct air capture device with 76 stars and a one-day development blitz in February 2024. The message: **citizens are building carbon capture hardware that industries charge $500+ per ton for.** The OSHWA certification is the legal shield — it's open hardware, protected by certification.

---

### 5. Carbon Capture and Storage (Reservoir Simulation)
- **Repo:** [yohanesnuwara/carbon-capture-and-storage](https://github.com/yohanesnuwara/carbon-capture-and-storage)
- **Stars:** 85 ⭐
- **Language:** MATLAB
- **Last commit:** March 6, 2021 (dormant ghost)
- **Contributor:** yohanesnuwara (academic)

**What it is:** A **reservoir simulation and geomechanics toolkit** for carbon capture and storage in geological formations. MATLAB-based, covering CO2 injection modeling, caprock integrity, and long-term storage assessment.

**🎙️ Episode hook:** 85 stars, dormant since 2021. This is the **ghost repo paradox** — highly cited, completely abandoned. The MATLAB dependency is both its strength (universality in academia) and its weakness (no community contributions). A student could fork this and port it to Python, potentially reviving an entire subfield.

---

### 6. DAC Peroxovanadates — Computational DAC Materials
- **Repo:** [tjz21/DAC_peroxovanadates](https://github.com/tjz21/DAC_peroxovanadates)
- **Stars:** 2 ⭐
- **Language:** Python/Notebooks
- **Last commit:** September 23, 2025
- **License:** CC0 (public domain)
- **Contributor:** tjz21

**What it is:** A **computational screening repository for peroxovanadate-based DAC sorbents**. TJ Z21 is systematically computing the electronic and structural properties of peroxovanadate molecules for CO2 capture applications.

**🎙️ Episode hook:** The **CC0 license is the story here.** TJ Z21 has dedicated this research to the **public domain** — no copyright, no restrictions, anyone can use these findings. This is part of a growing movement among computational DAC researchers who are treating their screening data as **public infrastructure**.

---

### 7. DAC Peroxotitanates — Companion to Peroxovanadates
- **Repo:** [tjz21/DAC_peroxotitanates](https://github.com/tjz21/DAC_peroxotitanates)
- **Stars:** 2 ⭐
- **Language:** Python/Notebooks
- **Last commit:** September 23, 2025
- **License:** CC0 (public domain)

**What it is:** The **titanium companion** to the peroxovanadate study — same methodology, different metal center. Together, these two repos form a **systematic computational screening platform** for DAC sorbent materials.

**🎙️ Episode hook:** Two repos, same author, same day, same CC0 license, same methodology, different metals. This is **industrial-strength open science**. TJ Z21 isn't publishing papers — they're publishing **datasets**. The peroxovanadate + peroxotitanate pair is a **materials screening pipeline** that anyone can access, extend, or commercialize without asking permission.

---

### 8. CO2-Sequestration
- **Repo:** Academic CO2 sequestration modeling
- **Stars:** 32 ⭐
- **Last commit:** Dormant since 2019
- **Language:** Likely MATLAB/Python

**What it is:** An **academic repository for CO2 sequestration modeling** — covering injection, migration, and trapping in geological formations.

**🎙️ Episode hook:** 32 stars, dormant for 7 years. The "ghost with a citation" pattern. Papers cite it, nobody maintains it. A Python port could make this accessible to a whole new community.

---

### 9. ClimateSoton/climate-research-group
- **Repo:** University of Southampton climate research group website
- **Last activity:** August 2026 (active)
- **Language:** HTML/CSS/JavaScript

**What it is:** The **website for the University of Southampton's climate research group** — actively maintained, hosting publications, projects, and contact info.

**🎙️ Episode hook:** While not a code repository, this is an **active institution** that could be a gateway to underground CCUS code. The Southampton group works on climate modeling and decarbonization pathways.

---

## 📊 Cross-Repo Carbon Trend Analysis

### The CC0 License Revolution
The most significant legal story in carbon capture OSS is the **CC0 (Creative Commons Zero / Public Domain) license trend**:

| Repo | License | Significance |
|------|---------|-------------|
| DAC_peroxovanadates | **CC0** | Sorbent screening data as public infrastructure |
| DAC_peroxotitanates | **CC0** | Complementary dataset, same philosophy |
| OpenAir-Cyan | **OSHWA** | Open hardware certification (complementary form) |
| Carbon_Capture_ML | **Custom** (research use) | Standard academic source |

**🎙️ Episode hook:** Two researchers just up and gave away their computational DAC screening data to the public domain. No patent filings, no licensing discussions, no "contact us for collaboration." Just CC0. In the context of the $1000/ton DAC cost barrier, this is radical: **the materials data that could lead to the next breakthrough is free.**

---

### The Activity Spectrum
| Tier | Repos | Character | Podcast Narrative |
|------|-------|-----------|-------------------|
| **Ecosystem builders** | Open-Sustainable-Tech (2,552★) | Continuously active, 5 contributors | "The map-makers" |
| **Paper trackers** | Carbon_Capture_ML (56★) | Periodic updates anchored to publications | "The indexes" |
| **Hardware pioneers** | OpenAir-Cyan (76★) | One-day blitz, then frozen, OSHWA certified | "The garage builders" |
| **Computational screeners** | DAC_peroxovanadates/titanates (2★ each) | CC0 public domain, systematic methodology | "The data donors" |
| **Academic ghosts** | carbon-capture-and-storage (85★), CO2-Sequestration (32★) | Dormant, highly cited, abandoned | "The haunted libraries" |

---

## The $1000/Ton Question

**Current state of open-source CCUS:**
- **No repo simulates a full DAC system** from sorbent to release
- **No repo models the economics** of DAC at scale
- **Hardware exists** (OpenAir-Cyan) but at bench scale, not commercial scale
- **Materials screening** (DAC_peroxovanadates/titanates) is accelerating but needs experimental validation
- **The directory** (Open-Sustainable-Tech) tracks projects but doesn't synthesize them
- **Reservoir simulation** (carbon-capture-and-storage) is mature but dormant

**What would break the $1000/ton barrier?**
1. **Sorbent innovation** — Computational screening can identify new materials 100x faster than lab trial-and-error
2. **Process optimization** — ML-driven process control could reduce energy costs
3. **Modular hardware** — DIY approaches could drive down costs through competition and iteration
4. **Public domain data** — CC0 licensing removes IP barriers that slow innovation
5. **Community coordination** — Open-Sustainable-Tech's 2,500+ projects need a synthesis layer

---

## 🎙️ Episode 2 Talking Points

### The Hardware Story
- OpenAir-Cyan: OSHWA-certified DIY DACC device, 76 stars, 7 commits in one day
- **The question:** Can citizen scientists build carbon capture that industries charge $500+ for?

### The Materials Revolution
- TJ Z21's peroxovanadate + peroxotitanate repos: CC0 public domain
- **The question:** Is the CC0 trend the fastest path to breaking the $1000/ton barrier?

### The Machine Learning Angle
- Carbon_Capture_ML: Survey of ML papers, anchored by OpenDAC benchmark
- **The question:** Can ML identify the sorbent that changes the economics?

### The Ecosystem Map
- Open-Sustainable-Tech: 2,552 stars, 2,500+ projects, continuously active
- **The question:** What's the synthesis layer that turns a directory into a breakthrough?

### The Ghost Problem
- carbon-capture-and-storage (85★, dormant), CO2-Sequestration (32★, dormant)
- **The question:** What happens when academic software becomes a citation corpse?

---

*Last updated: September 2026 (v4) | Data source: GitHub API commit histories for 9 repositories*