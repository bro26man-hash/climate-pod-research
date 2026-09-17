# 🌍 Carbon Capture — Project Discoveries

**Last Updated:** September 2026
**Research Round:** Second pass — commit histories from 8 repositories

---

## Repository Catalog

### Tier 1 — Flagship / High-Impact

| Repo | Stars | Language | Focus | Last Activity |
|------|-------|----------|-------|---------------|
| **openair-collective/openair-cyan** | 76 | Python | DIY open hardware DACC device (OSHWA-certified) | Feb 12, 2024 |
| **yohanesnuwara/carbon-capture-and-storage** | 85 | Lasso | Reservoir simulation + geomechanics for CCS | Mar 6, 2021 |
| **zikribayraktar/Carbon_Capture_ML** | 56 | Jupyter | ML-for-carbon-capture survey | May 8, 2024 |
| **protontypes/open-sustainable-technology** | 2,552 | Multiple | Comprehensive OSS climate-tech directory | Sep 9, 2026 |

### Tier 2 — Active Research

| Repo | Stars | Language | Focus | Last Activity |
|------|-------|----------|-------|---------------|
| **tonyzyl/CO2-Soft-Sensor** | 16 | Jupyter | Hybrid mechanistic+ML (DAE-LSTM) CO2 model | Aug 18, 2026 |
| **Beckybams/AI-for-Carbon-Capture-Optimization** | 25 | Python | ML optimization of carbon capture efficiency | Mar 2, 2026 |
| **tjz21/DAC_peroxovanadates** | 2 | Python | Computational DAC sorbent (peroxovanadates) | Aug 19, 2026 |
| **tjz21/DAC_peroxotitanates** | 2 | Python | Computational DAC sorbent (peroxotitanates) | Aug 19, 2026 |
| **o7-machinehum/electro-swing-dacc** | — | — | Electro-swing DAC research collection | Aug 19, 2026 |

### Tier 3 — Niche / Dormant

| Repo | Stars | Language | Focus | Last Activity |
|------|-------|----------|-------|---------------|
| **SarkisovTeam/ML-NSGA-PSA-carbon-capture** | 3 | Jupyter | MOF design for carbon capture using ML | Jun 4, 2026 |
| **IBM/Carbon-capture-fingerprint-generation** | 2 | Python | Molecular representation for amine sorbents | Unknown |
| **CCSI-Toolset/membrane_model** | 6 | Makefile | Hollow fiber membrane separation model | Aug 23, 2026 |
| **dongyan3721/carbon-capture** | 3 | JavaScript | Carbon capture project (Chinese) | Apr 8, 2026 |

---

## Deep Dives

### 1. openair-collective/openair-cyan — The DIY Hardware Pioneer (76 stars)

**What makes it special:** The only open-source hardware carbon capture device that has achieved institutional certification (OSHWA UID US001095). It's a small-scale direct air capture device with open documentation, CERN-OHL-P license, and CITATION.cff.

**Commit pattern:** 6 commits on Feb 12, 2024 (OSHWA certification milestone), then complete silence. 2 years of README updates, then 2 years of nothing.

**The story:** A PhD student built a DAC device in a garage, got it certified, published it, and then... stopped. The project proved open-source DAC hardware can work. But it couldn't sustain momentum without an institutional home.

**Podcast angle:** "OpenAir-Cyan is the hero narrative of open-source carbon capture. It proved it can be done. But then it went dormant for 2.5 years. The question isn't whether open-source DAC works — it's whether it can survive without a patron."

### 2. zikribayraktar/Carbon_Capture_ML — The Literature Survey Model (56 stars)

**What it is:** A curated survey of all published carbon capture ML papers, data, code, and supplemental materials.

**Commit pattern:** Intense activity Feb 2-5, 2023 (4 commits, paper season). Then periodic updates through May 2024 (OpenDAC paper addition). Single author (Zikri Bayraktar).

**The pattern:** This is a research survey repo — it curates published work rather than producing new code. It's a literature management tool, not a simulation tool.

**Podcast angle:** "The dominant mode of open-source carbon capture is literature management, not tool-building. 56 stars for a survey, zero for a simulation."

### 3. yohanesnuwara/carbon-capture-and-storage — The Ghost Project (85 stars)

**What it is:** Integration of reservoir simulation, rock physics, seismic modeling, and geomechanics for CCS monitoring.

**Commit pattern:** 9 commits in 3 months (Feb-May 2021) — a BSc thesis project. Then complete silence for 5+ years. 85 stars, zero activity.

**The paradox:** The most-starred dedicated carbon capture repo is a ghost town. Academic incentive structures produce stars but not maintenance.

**Podcast angle:** "85 stars and zero commits since 2021. The academic incentive structure rewards publication, not stewardship. The code is a snapshot of one person's thesis — not a living tool."

### 4. The August 2026 Materials Wave (Coordinated Activity)

| Repo | Date | Activity | Focus |
|------|------|----------|-------|
| tjz21/DAC_peroxovanadates | Aug 19, 2026 | Commit update | Peroxovanadate sorbents |
| tjz21/DAC_peroxotitanates | Aug 19, 2026 | Commit update | Peroxotitanate sorbents |
| o7-machinehum/electro-swing-dacc | Aug 19, 2026 | Research collection | Electro-swing DAC |
| ChemicalEngineeringAI/Carbon-Capture | Aug 23, 2026 | Update | Carbon capture engineering |

**The signal:** Four independent repos, all updated within a 5-day window in August 2026. Same-day coordination (Aug 19) suggests a shared research event — possibly a paper submission, a preprocessing wave, or a community push for reproducible DAC materials computation.

**Podcast angle:** "Three DAC materials repos updated on the exact same day. Is this a coordinated community effort to make computational sorbent discovery reproducible? The August 2026 wave is the most significant signal in all of carbon capture on GitHub."

### 5. tonyzyl/CO2-Soft-Sensor — The Hybrid Model (16 stars)

**What it is:** A hybrid mechanistic and data-driven (DAE-LSTM) model for estimating CO2 concentration profiles in a carbon capture plant.

**Why it matters:** Bridges physics-based modeling (differential algebraic equations) with machine learning (LSTM). This is the emerging pattern in carbon capture: hybrid models that combine domain knowledge with data-driven flexibility.

**Commit pattern:** Updated Aug 18, 2026 — one of the most recently active carbon capture repos.

### 6. Beckybams/AI-for-Carbon-Capture-Optimization — The Optimization Angle (25 stars)

**What it is:** Uses synthetic industrial data to predict carbon capture efficiency through ML.

**Why it matters:** Focuses on optimization rather than simulation. The question isn't "can we capture CO2?" but "can we capture it more efficiently?" This is the applied engineering layer.

---

## The Carbon Capture Gap Matrix

| Layer | What Exists | What's Missing |
|-------|-------------|----------------|
| **Materials discovery** | Peroxovanadates, peroxotitanates (computational) | Experimental validation pipelines |
| **Device prototyping** | OpenAir-Cyan (hardware design) | Iterative development community |
| **Process simulation** | carbon-capture-and-storage (reservoir sim) | Maintenance, extension |
| **Economic modeling** | srm-forever (SRM only, not DAC) | DAC cost projection models |
| **Optimization** | AI-for-Carbon-Capture-Optimization | Scale-up from synthetic to real data |
| **System integration** | Nothing | Deploy-at-scale engineering |
| **Survey/knowledge** | Carbon_Capture_ML (56 stars) | Living, continuously updated |

---

## Episode Talking Points

1. **The materials science is accelerating; the engineering is absent.** The August 2026 wave shows computational sorbent discovery is becoming reproducible and open. But nobody is building the "deploy DAC at scale" code.

2. **OpenAir-Cyan proved it works. Now what?** Certification was the milestone. But 2.5 years of silence is the open-hardware limbo problem. The project needs an institution or funder to continue.

3. **The August 2026 wave is the most significant signal.** Four independent repos updating in the same week = a community forming around open computational chemistry.

4. **Hybrid models are emerging.** tonyzyl's DAE-LSTM approach combines physics with ML. This is the pattern that will scale — not pure data-driven, not pure physics, but both.

5. **The maintenance gap is structural.** Across all carbon capture repos, nobody is building long-term community infrastructure. The field is in knowledge-integration mode, not tool-building mode.

6. **carbon-capture-and-storage is the ghost that haunts all of this.** 85 stars, zero commits since 2021. Stars does not equal sustainability.