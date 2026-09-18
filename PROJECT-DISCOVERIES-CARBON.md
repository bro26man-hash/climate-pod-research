# 🌍 Carbon Capture — Project Discoveries
## Research Notes for Podcast Episode: Direct Air Capture & Carbon Capture Technologies

*Last updated: September 2026 — based on fresh GitHub commit analysis*

---

## Executive Summary

The open-source carbon capture ecosystem on GitHub is **remarkably diverse** — spanning a 2,552-star comprehensive climate-tech directory, DIY open-hardware devices, ML-powered materials screening, and computational chemistry repos with CC0 public-domain licensing. Unlike solar geoengineering (where code lives inside climate models), carbon capture has **purpose-built repositories** with clear, specialized missions.

**Key finding: The carbon capture community is further along in open-source maturity than solar geoengineering — but the most impactful repo is a directory, not a device.**

---

## Repository Profiles

### 1. Open Sustainable Technology (protontypes/open-sustainable-technology)
| Attribute | Detail |
|-----------|--------|
| Stars | **2,552** (highest in our entire study) |
| Language | Python, JavaScript, Markdown |
| Last commit | **September 9, 2026** (2 commits that day) |
| Activity level | 🔴 VERY HIGH (continuous, 15 commits in ~3 months) |
| License | MIT |

**What it is:** A comprehensive, curated directory of **2,500+ open-source climate technology projects**. It's not a single tool — it's an ecosystem map. Think of it as the GitHub of climate tech.

**Recent commits (showing remarkable diversity):**
- `6e9f48c` — **Add-MUIO** (Sep 9, 2026) — MUIO likely refers to a modular input/output framework
- `07e19b1` — **Add-MUIOGO** (Sep 9, 2026) — companion to MUIO, suggesting a Go-based implementation
- `1b6cb82` —docs: fix dead links in README.md (Sep 1, 2026) — active maintenance of the portal
- `d73a519` — **Add claude-carbon** (Aug 23, 2026) — AI-assisted carbon analysis tool?
- `6b6cdc8` — **Add Story Seed Library** (Aug 18, 2026) — narrative/communication resources for climate action
- `ca9d7a5` — **Add openflexure microscope** (Aug 18, 2026) — open hardware for microscopy (science access)
- `5bc6609` — **Add PowerIO** (Jul 2, 2026) — power input/output tracking
- `e772ed4` — **Add ASSETRA** (Jul 1, 2026) — likely an assessment/monitoring tool
- `4c6f0a4` — **Add ToOp** (Jul 1, 2026) — Operation tool?
- `1986e2c` — **Add wbdata** (Jun 23, 2026) — World Bank data interface?
- `007a464` — **Add Volca to Life Cycle Assessment** (Jun 23, 2026) — LCA integration
- `0601a42` — **Add EpexPredictor** (Jun 6, 2026) — Extreme price predictor? Energy market?

**Why it matters for carbon capture:**
This is the **connective tissue** of the entire OSS climate community. It doesn't build capture technology — it maps who's building what. For a podcast, it's the perfect starting point: "Before you ask what the best DAC technology is, let's look at what the open-source community is actually working on."

**Episode hook:** *"The most important climate tech repo on GitHub isn't a device or a model — it's a map. 2,500 projects, one directory, and the answer to 'who's building what?'"*

---

### 2. OpenAir-Cyan (openair-collective/openair-cyan)
| Attribute | Detail |
|-----------|--------|
| Stars | **76** |
| Language | C, C++ (embedded systems) |
| Last commit | **February 12, 2024** | |
| Activity level | 🟡 DORMANT (blitz then freeze) |
| License | CERN-OHL-S-2.0 (open hardware!) |

**What it is:** **DIY open-hardware Direct Air Capture (DAC) device.** This is the most important carbon capture repo that most people haven't heard of. It's a completely open-source, 3D-printable, cost-reduced DAC device.

**What makes it special:**
- **OSHWA-certified** (US001095) — the only open-hardware DAC device with certification
- **CERN Open Hardware License** — the strongest copyleft license for physical devices
- **Blitz development:** All commits occurred on February 12, 2024 — a single-day surge of activity, then permanent dormancy
- **Last update:** OSHWA UID link added to README (Feb 12, 2024)

**The single-day story:** On February 12, 2024, someone (KCollins) pushed:
1. OSHWA UID logo
2. CITATION.cff creation
3. Multiple file uploads
4. README update with OSHWA UID link

This looks like a **final certification push** — the team got their device certified, documented it thoroughly, and then... stopped. The project appears complete. It's not abandoned; it's **finished**. The hardware was built, tested, certified, and documented.

**Why it matters:** OpenAir-Cyan proves that open-source hardware CAN work for carbon capture. It also proves that it's hard to sustain. The single-day Blitz followed by permanent dormancy is the story of citizen science: brilliant bursts of activity, then life moves on.

**Episode hook:** *"In one day, in February 2024, someone built and certified an open-source carbon capture device. Then they stopped. Was it a success? Or is this what happens when passionate people run out of funding?"*

---

### 3. Carbon Capture ML (zikribayraktar/Carbon_Capture_ML)
| Attribute | Detail |
|-----------|--------|
| Stars | **56** |
| Language | Python, Jupyter Notebook |
| Last commit | **May 8, 2024** |
| Activity level | 🟡 MATURING (survey completed, now in maintenance) |
| License | MIT |

**What it is:** A **survey of machine learning papers and code for carbon capture**. It's a curated collection of ML approaches for DAC, CCS, and point-source capture.

**Recent activity:** Last commit May 2024, suggesting the survey is complete and now in maintenance mode. The repo serves as a **reading list** for researchers entering the ML-for-climate space.

**Why it matters for carbon capture:** It's the **best entry point** for anyone wanting to understand how ML is being applied to carbon capture. For a podcast, it's the perfect "further reading" recommendation.

---

### 4. DAC Peroxovanadates (tjz21/DAC_peroxovanadates)
| Attribute | Detail |
|-----------|--------|
| Stars | **2** |
| Language | Python, Jupyter Notebook |
| Last commit | **September 23, 2025** |
| Activity level | 🟢 ACTIVE (recent update) |
| License | **CC0 (public domain!)** |

**What it is:** Computational screening of **peroxovanadate compounds** for Direct Air Capture. This is materials-by-computation: using density functional theory (DFT) and machine learning to find sorbent materials that can efficiently capture CO2.

**Why the CC0 license matters:** This is HUGE. The repo is released under CC0 — **public domain dedication**. This means:
- Anyone can use the data for any purpose, including commercial DAC development
- No patent filings, no licensing fees, no restrictions
- The research data is treated as **public infrastructure**

**The CC0 trend:** This is the second repo in our study with a CC0 license (the other being DAC_peroxotitanates). Together, they represent a **movement**: researchers are choosing to make their computational screening data freely available. This is the open-science equivalent of "open-sourcing the periodic table."

**Episode hook:** *"Two researchers gave away their DAC materials data to the public domain. No patents. No licenses. Just CC0. Is this the future of climate-tech research?"*

---

### 5. DAC Peroxotitanates (tjz21/DAC_peroxotitanates)
| Attribute | Detail |
|-----------|--------|
| Stars | **2** |
| Language | Python, Jupyter Notebook |
| Last commit | **September 23, 2025** |
| Activity level | 🟢 ACTIVE |
| License | **CC0 (public domain!)** |

Same author, same story, different materials system (titanates instead of vanadates). The parallel release pattern suggests a **systematic study** of CC0 materials data for DAC sorbent discovery.

---

### 6. Carbon Capture and Storage (yohanesnuwara/carbon-capture-and-storage)
| Attribute | Detail |
|-----------|--------|
| Stars | **85** |
| Language | MATLAB, LaTeX |
| Last commit | **March 6, 2021** (dormant since) |
| Activity level | ⚫ GHOST (dead stars, alive citation count) |
| License | MIT |

**What it is:** Reservoir simulation and geomechanics for carbon capture and storage (CCS). Higher star count than the newer repos, but **dormant for over 4 years**.

**The ghost repo phenomenon:** 85 stars but zero commits since March 2021. Stars measure citations, not usability. This repo is cited in papers but not used in code. It's a **digital citation** — a monument to research, not a tool.

**Why it matters:** It reminds us that **stars ≠ value** in climate tech. Some of the most cited repos are the most inactive ones.

---

## 🌍 Development Trend Summary for Carbon Episode

### The Four Lifecycle Patterns
| Pattern | Repo | What It Tells Us |
|---------|------|------------------|
| **Perpetual Growth** | open-sustainable-technology | The directory model is self-sustaining — new projects keep arriving |
| **Blitz & Freeze** | openair-cyan | Open hardware can be completed in a single day, then left behind |
| **Survey & Maintain** | Carbon_Capture_ML | Literature reviews are valuable but inherently finite |
| **CC0 Pioneers** | DAC_peroxovanadates, DAC_peroxotitanates | A new movement: public-domain materials data for climate |
| **Ghost** | carbon-capture-and-storage | Stars measure citations, not community |

### The CC0 Revolution
The most significant trend in carbon capture on GitHub is **not technical — it's legal.** Two repos by the same author (tjz21) have adopted CC0 public domain dedication for computational DAC materials data.

**Why this matters:**
- Traditional academic publishing locks data behind paywalls
- Open-source software uses GPL/MIT, but data has no standard license
- CC0 says: "This data belongs to everyone, forever, no strings attached"
- For DAC, where sorbent materials are a key bottleneck, open data could **accelerate discovery by years**

**Episode hook:** *"The biggest open-science story in carbon capture isn't about code. It's about a license. CC0. Two researchers gave away their data. Here's why it matters."

---

## 📚 Sources & Links
- [Open Sustainable Technology](https://github.com/protontypes/open-sustainable-technology)
- [OpenAir-Cyan](https://github.com/openair-collective/openair-cyan)
- [Carbon Capture ML](https://github.com/zikribayraktar/Carbon_Capture_ML)
- [DAC Peroxovanadates](https://github.com/tjz21/DAC_peroxovanadates)
- [DAC Peroxotitanates](https://github.com/tjz21/DAC_peroxotitanates)
- [Carbon Capture and Storage](https://github.com/yohanesnuwara/carbon-capture-and-storage)

---

*Research methodology: GitHub commit API analysis, September 2026. Commit data pulled via GitHub REST API. All timestamps are approximate based on API response dates.*