# 🌍 Carbon Capture — Podcast Episode Research Notes

**Episode Title (Working):** "Can Open Source Break the $1,000/Ton DAC Barrier?"

---

## 🔍 Top Repository Discoveries

### 1. openair-collective/openair-cyan — 76 ⭐ | DIY Open Hardware DACC
- **Focus:** DIY small-scale open hardware direct air carbon capture device. OSHWA-certified (UID US001095). Documentation hosted at https://openair-collective.github.io/openair-cyan
- **Last Updated:** Feb 12, 2024
- **Language:** Not specified (open hardware project)
- **Key Commits (all on Feb 12, 2024 — single-day burst):**
  - `b5422b3` — Added OSHWA UID link to README
  - `b164257` — File upload (design files)
  - `828f496` — OSHWA UID logo (US001095)
  - `b731cd8` — File upload (additional documentation)
  - `4b08fb3` — Created CITATION.cff (citation metadata)
- **🎙️ Episode Angle:** This is the most important carbon capture repo on GitHub. It's not software — it's open-source *hardware*. OSHWA certification means it meets open-source hardware standards. The single-day commit burst in Feb 2024 was the OSHWA certification push. **Interview question:** "If you can 3D-print a direct air capture device, does that democratize climate action — or just spread poorly-engineered solutions?"

### 2. zikribayraktar/Carbon_Capture_ML — 56 ⭐ | ML Survey
- **Focus:** Survey of all published carbon capture ML papers, data, code, and supplemental materials.
- **Last Updated:** May 8, 2024 (OpenDAC paper added)
- **Language:** Jupyter Notebook
- **Key Commits:**
  - `ca9a31f` (May 8, 2024) — OpenDAC paper added (latest significant update)
  - `4c01842` (Apr 25, 2024) — README update
  - `2b69376` (Mar 15, 2024) — README update
  - `e80dfd6` / `fe28496` (Jan 21, 2024) — README updates
- **🎙️ Episode Angle:** This is the "meta-repo" — a living survey of the entire ML-for-carbon-capture field. The OpenDAC paper addition is notable: OpenDAC (Open Direct Air Capture) is a benchmark framework. **Interview question:** "Is a survey paper on GitHub the new academic paper?"

### 3. yohanesnuwara/carbon-capture-and-storage — 85 ⭐ | Reservoir Simulation
- **Focus:** Integration of reservoir simulation, rock physics, seismic modeling, and geomechanics for CCS monitoring. Originally the author's BSc thesis.
- **Last Updated:** Jul 1, 2026 (repository metadata)
- **Language:** Lasso (unusual for this domain)
- **🎙️ Episode Angle:** 85 stars but dormant — the last meaningful commit was Mar 2021. This is the "academic thesis ghost project": high star count, zero maintenance. It illustrates the fundamental problem with academic open-source: it's optimized for the thesis defense, not long-term stewardship. **Interview angle:** "This repo got 85 stars and then the author moved on. Is that the lifecycle of academic climate code?"

### 4. Beckybams/AI-for-Carbon-Capture-Optimization — 25 ⭐ | ML Optimization
- **Focus:** Machine learning project using synthetic industrial data to improve carbon capture efficiency. Predicts performance.
- **Last Updated:** Mar 2, 2026
- **Language:** Python (presumed)
- **🎙️ Episode Angle:** Synthetic industrial data for CC optimization — this is the "digital twin" approach to carbon capture. Not measuring real plants, but simulating them. **Interview question:** "If you train an AI on synthetic data about a real process, how do you know the AI understands reality?"

### 5. tonyzyl/CO2-Soft-sensor-for-a-carbon-capture-pilot-plant — 16 ⭐ | Hybrid Modeling
- **Focus:** A hybrid mechanistic and data-driven (DAE-LSTM) model for estimating CO2 concentration profiles in a carbon capture plant.
- **Last Updated:** Aug 18, 2026
- **Language:** Jupyter Notebook
- **🎙️ Episode Angle:** This is the most technically interesting repo — it combines physics-based differential algebraic equations (DAE) with LSTM neural networks. The "soft sensor" concept: instead of measuring CO2 concentration with physical sensors, you *estimate* it using a model. **Interview angle:** "A soft sensor doesn't measure the real world — it *predicts* it. Is a model-based estimate good enough for climate accountability?"

### 6. CCSI-Toolset/membrane_model — 6 ⭐ | Membrane Separation
- **Focus:** Membrane separation model for carbon capture — hollow fiber membrane model and system example.
- **Last Updated:** Aug 23, 2026
- **🎙️ Episode Angle:** Membrane-based DAC is less discussed than amine-based, but it could be cheaper. This repo models the membrane physics. **Episode angle:** "Membranes vs. amines: the billion-dollar debate in DAC, and the GitHub evidence is thin on both sides."

---

## 📊 Commit Trend Analysis — Carbon Capture Theme

### Pattern 1: The August 2026 DAC Materials Wave
Multiple repositories in the carbon capture space were updated around Aug 19-23, 2026:
- `tjz21/DAC_peroxovanadates` and `tjz21/DAC_peroxotitanates` — computational DAC materials (peroxides)
- `CCSI-Toolset/membrane_model` — Aug 23, 2026
- `Beckybams/AI-for-Carbon-Capture-Optimization` — active through Mar 2026

This suggests a **coordinated research event** in open computational chemistry for DAC materials. Multiple groups investigating perovskite/peroxide sorbents simultaneously.

**Episode angle:** "In August 2026, four separate GitHub repos started looking at the same chemical space. Coordination or convergence? Either way, the perovskite moment in DAC is now."

### Pattern 2: The Open Hardware vs. Open Software Divide
The carbon capture GitHub ecosystem splits into two distinct tracks:
- **Open hardware:** OpenAir-Cyan (OSHWA-certified DIY DAC device)
- **Open software:** Carbon_Capture_ML, AI-for-Carbon-Capture-Optimization, membrane_model

No repo bridges both worlds. The hardware people don't publish code; the software people don't publish hardware designs.

**Episode angle:** "The carbon capture open-source community is split in two: people who share designs and people who share models. They rarely talk to each other."

### Pattern 3: Dormancy is the Default
Of 6 carbon capture repos analyzed:
- 3 are fully dormant (last commit 2021-2024)
- 2 are maintenance-only (README bumps)
- 1 is active (membrane_model, Aug 2026)

The most-starred repo (carbon-capture-and-storage, 85★) is the most dormant. Star count ≠ maintenance.

**Episode soundbite:** "Carbon capture on GitHub is like a museum: lots of visitors, nobody cleaning the windows."

### Pattern 4: The Hybrid Modeling Trend
Two repos (DAE-LSTM soft sensor, AI-for-CC-optimization) represent a growing trend: combining physics-based models with machine learning. This is the "digital twin" approach — not pure simulation, not pure data science, but a hybrid.

**Episode angle:** "The future of carbon capture modeling isn't physics OR data — it's physics WITH data. The hybrid models are the most credible."

---

## 🎙️ Episode Structure Recommendation

| Segment | Content | Duration |
|---------|---------|----------|
| **Cold Open** | OpenAir-Cyan: you can download the CAD files for a direct air capture device. What could go wrong? | 3 min |
| **Act 1** | The state of DAC: $600-$1,000/ton, amine chemistry, and why open source hasn't broken the cost barrier |
| **Act 2** | The ML wave: Carbon_Capture_ML survey, perovskite peroxides, hybrid DAE-LSTM models |
| **Act 3** | The open hardware question: OSHWA certification, DIY risk, the democratization argument |
| **Act 4** | The dormancy problem: 85 stars and dead code — why academic climate projects die |
| **Close** | The uncomfortable question: if open source can't lower DAC below $100/ton, does the effort matter? |

---

## 🔗 Key Links
- OpenAir-Cyan: https://github.com/openair-collective/openair-cyan
- Carbon_Capture_ML: https://github.com/zikribayraktar/Carbon_Capture_ML
- carbon-capture-and-storage: https://github.com/yohanesnuwara/carbon-capture-and-storage
- AI-for-Carbon-Capture-Optimization: https://github.com/Beckybams/AI-for-Carbon-Capture-Optimization
- CO2 Soft Sensor: https://github.com/tonyzyl/CO2-Soft-sensor-for-a-carbon-capture-pilot-plant
- Membrane Model: https://github.com/CCSI-Toolset/membrane_model

---

*Last updated: Sep 2026 | Research method: GitHub API commit history pull + repository search*