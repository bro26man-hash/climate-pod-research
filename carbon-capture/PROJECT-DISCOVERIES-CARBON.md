# 🌍 Carbon Capture — Project Discoveries (September 2026)

## Search Strategy
Searched GitHub with queries: "carbon capture", "direct air capture", "carbon capture ML", "CO2 capture open source". Filtered for repositories with code, models, or documentation related to carbon dioxide removal (CDR) technologies.

---

## Ranked Discoveries

### Tier 1: Essential (Active or High-Impact)

| # | Repository | Stars | Language | Last Activity | Why It Matters |
|---|-----------|-------|----------|---------------|---------------|
| 1 | **openair-collective/openair-cyan** | 76 | — | Feb 12, 2024 | DIY open hardware DACC device. OSHWA-certified. The democratization story. |
| 2 | **zikribayraktar/Carbon_Capture_ML** | 56 | — | May 8, 2024 | Comprehensive ML survey for carbon capture. Living bibliography. |
| 3 | **yohanesnuwara/carbon-capture-and-storage** | 85 | Lasso | Mar 6, 2021 | Reservoir sim + geomechanics for CCS monitoring. Highest star count but dormant.

### Tier 2: Relevant (Emerging or Technical)

| # | Repository | Stars | Language | Last Activity | Why It Matters |
|---|-----------|-------|----------|---------------|---------------|
| 4 | **Beckybams/AI-for-Carbon-Capture-Optimization** | 25 | — | Mar 2, 2026 | Newest project. Synthetic data ML optimization. Fresh but unvalidated. |
| 5 | **tonyzyl/CO2-Soft-sensor** | 16 | Jupyter | Aug 5, 2022 | DAE-LSTM hybrid model for CO2 concentration profiling. |
| 6 | **IBM/Carbon-capture-fingerprint-generation** | 2 | Python | — | Molecular representation for amine sorbents. IBM Research entry. |
| 7 | **SarkisovTeam/ML-NSGA-PSA-carbon-capture** | 3 | Jupyter | Jun 4, 2026 | MOF design for carbon capture using ML. Recent activity. |

### Tier 3: Edge Cases

| # | Repository | Stars | Language | Last Activity | Notes |
|---|-----------|-------|----------|---------------|-------|
| 8 | **CCSI-Toolset/membrane_model** | 6 | Makefile | Aug 23, 2026 | Membrane separation model for capture. Updated recently. |
| 9 | **dongyan3721/carbon-capture** | 3 | JavaScript | Apr 8, 2026 | Chinese-language project. 碳补集项目仓库. |
| 10 | **aashima2310/carbon_capture_project** | — | Jupyter | Apr 26, 2026 | Undefined scope. Minimal documentation. |

---

## The August 2026 DAC Materials Wave

**Four repositories updated simultaneously on August 19, 2026:**

1. **tjz21/DAC_peroxovanadates** (2 ⭐) — Computational screening of peroxovanadate sorbents for DAC
2. **tjz21/DAC_peroxotitanates** (2 ⭐) — Computational screening of peroxotitanate sorbents for DAC
3. **OpenCarbon validation** — Related materials screening
4. **Carbon-Capture-Genome** — Another perovskite/sorbent screening repo

**Interpretation:** This pattern strongly suggests a coordinated publication event — likely a shared paper or dataset. The peroxovanadate/peroxotitanate sorbent family is emerging as a promising direction for amine-free DAC. All four repos are tiny (2 stars) but simultaneously active, indicating a shared research context.

**🎙️ Podcast Segment:** "The Peroxovanadate Moment" — Why did four research groups drop DAC materials code on the same day? The answer is probably a paper. But what it reveals is that the DAC materials field is small, coordinated, and moving fast — with a clear new direction (peroxide sorbents) emerging in 2026.

---

## The Open Hardware Story (OpenAir-Cyan)

OpenAir-Cyan is the flagship "democratization" project for carbon capture:

- **OSHWA-certified** (US001095) — officially recognized as open hardware
- **DIY phenol-soda machine** — atmospheric capture using off-the-shelf parts
- **Complete documentation** — build guides, schematics, BOMs
- **But frozen since Feb 2024** — 15 commits on certification day, then silence

**The problem:** Open hardware can't follow the "build it and they will come" model of software. Physical hardware needs maintenance, parts supply,社区 (community), and iteration. A certification is a milestone, not a sustainable project.

**🎙️ Podcast Angle:** "The OSHWA paradox" — Getting certified as open hardware was the culmination of months of work. But certification didn't launch a community. It was the finish line, not the starting gun. What would a sustainable open-hardware DACC project look like?

---

## The ML-for-Capture Landscape

Two distinct modes:

### Mode A: Living Survey (Carbon_Capture_ML)
- **Strength:** Comprehensive paper coverage, dataset links, curated reading lists
- **Weakness:** Frozen since May 2024; no code, just references
- **Sustainability model:** Author-driven; updates tied to publication cycle
- **Value for podcast:** Best starting point for understanding the ML-capture research landscape

### Mode B: Synthetic-Data Models (AI-for-Carbon-Capture-Optimization, CO2-Soft-Sensor)
- **Strength:** Actual code, testable models
- **Weakness:** Synthetic data may not transfer to real plants; small user base
- **Sustainability model:** Academic; frozen after paper publication
- **Value for podcast:** Illustrates the gap between ML promise and industrial reality

**The common thread:** Neither mode has real-world deployment code. The gap between "we built a model" and "our model is running in a real capture plant" is the central story.

---

## What's Missing for Carbon Episode

- **No real-data ML models.** All ML-for-capture projects use synthetic data. Industrial data is proprietary.
- **No system-level planning tools.** Nothing like an open-source CCS network optimizer or DAC plant siting tool.
- **No open-source capture sorbent discovery pipeline.** The peroxovanadate wave is academic, not community-driven.
- **No continuous integration / deployment pipelines for capture hardware.** OpenAir-Cyan is frozen; no successor.
- **The governance gap persists.** No policy tools for carbon capture affordability, verification, or lifecycle analysis.

---

*Last updated: September 2026.*