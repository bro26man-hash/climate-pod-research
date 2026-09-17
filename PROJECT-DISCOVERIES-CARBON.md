# 🌍 Carbon Capture — Project Discovery Catalog

**Last Updated:** September 2026 (v4 — fresh commit histories from 15 repositories including differentiable-flowsheets)
**Research Method:** GitHub repository search ("carbon capture", "DAC", "direct air capture", "CCS", "carbon capture ML", "differentiable simulation") + cross-reference with "open-sustainable-technology" directory

---

## Tier 1: Major Projects (50+ Stars, Active or Landmark Activity)

### Open Sustainable Technology — 2,552 Stars (ProtonTypes)
- **URL:** https://github.com/protontypes/open-sustainable-technology
- **Language:** Multi-language directory
- **Focus:** Comprehensive directory of 2,500+ open-source climate tech projects
- **Latest:** Sep 9, 2026 (MUIO and MUIOGO DAC hardware control units added)
- **Carbon Relevance:** Tracks the entire carbon capture ecosystem. New entries added regularly (MUIO, claude-carbon, PowerIO — Aug-Sep 2026).
- **Why It Matters:** The ecosystem infrastructure. This is the "github.com/awesome-climate-tech" that makes everything else discoverable.
- **v4 Update:** The "claude-carbon" entry (Aug 23, 2026) signals that AI-assisted carbon capture is now a recognized category in the directory.

### OpenAir-Cyan — 76 Stars (OpenAir Collective)
- **URL:** https://github.com/openair-collective/openair-cyan
- **Language:** HTML/CSS (hardware documentation)
- **Focus:** DIY small-scale direct air capture device. OSHWA-certified (UID US001095). CERN-OHL-P licensed.
- **Latest:** Feb 12, 2024 (OSHWA certification milestone) — dormant since
- **Why It Matters:** The only open-source DAC hardware project that reached institutional certification. Proved it can be done. Also failed to sustain momentum.

### Carbon_Capture_ML — 56 Stars (Zikri Bayraktar)
- **URL:** https://github.com/zikribayraktar/Carbon_Capture_ML
- **Language:** Python (survey/data)
- **Focus:** Survey of all published carbon capture ML papers, data, code, and supplemental materials
- **Latest:** May 8, 2024 (OpenDAC paper added) — periodic updates
- **Why It Matters:** The dominant open-source mode for carbon capture is literature curation, not code production. This repo IS the field's knowledge base.

### carbon-capture-and-storage — 85 Stars (yohanesnuwara)
- **URL:** https://github.com/yohanesnuwara/carbon-capture-and-storage
- **Language:** Lasso (reservoir simulation)
- **Focus:** Integration of reservoir simulation, rock physics, seismic modeling, and geomechanics for CCS monitoring
- **Latest:** Mar 6, 2021 (BSc thesis complete) — dormant for 5+ years
- **Why It Matters:** The ghost project. 85 stars, zero maintenance. Proves that academic incentive structures don't reward long-term code stewardship.

### differentiable-flowsheets — 13 Stars (John Kitchin)
- **URL:** https://github.com/jkitchin/differentiable-flowsheets
- **Language:** Python (JAX-based)
- **Focus:** Differentiable chemical process simulation and optimization for capture/separation systems
- **Latest:** Sep 17, 2026 (10 commits in 5 days — most active carbon capture repo in the analysis)
- **v4 Discovery:** THIS IS THE MOST SIGNIFICANT NEW FINDING. Claude (Anthropic's AI) is authoring production code commits — "Drop the legacy loading correction," "Fix Kremser two-inlet boundary condition." This is AI-augmented scientific computing in active use.
- **Why It Matters:** This is the "deploy at scale" layer that's been missing. Differentiable simulation means you can compute gradients of the entire separation process, enabling gradient-based optimization. The JAX backend means GPU acceleration. And AI is writing the code.

---

## Tier 2: Emerging Projects (10-50 Stars)

### CO2-Soft-Sensor-for-a-Carbon-Capture-Pilot-Plant — 16 Stars (tonyzyl)
- **URL:** https://github.com/tonyzyl/CO2-Soft-sensor-for-a-carbon-capture-pilot-plant
- **Language:** Jupyter Notebook
- **Focus:** Hybrid mechanistic and data-driven (DAE-LSTM) model for CO2 concentration estimation in DAC plants
- **Latest:** Aug 18, 2026 (August 2026 wave)
- **Why It Matters:** The closest thing to "deploy at scale" code. A soft-sensor is a practical engineering tool for plant control — more immediately useful than materials discovery.

### Differentiable-Flowsheets — 13 Stars (John Kitchin)
- **URL:** https://github.com/jkitchin/differentiable-flowsheets
- **Language:** Python/JAX
- **Focus:** Differentiable process simulation for chemical separation (REE extraction, CO2 capture)
- **Latest:** Sep 17, 2026 (active Claude-assisted development)
- **Why It Matters:** Bridges the gap between materials science and system engineering. AI- augmented optimization of separation processes. REE extraction crossover suggests mineral separation applications.

---

## Tier 3: CC0 Pioneer Projects (2 Stars Each)

### tjz21/DAC_peroxovanadates — 2 Stars (Jacob Hirschi)
- **URL:** https://github.com/tjz21/DAC_peroxovanadates
- **Language:** Python (computational screening)
- **Focus:** DFT computational screening of peroxovanadate sorbents for DAC
- **Latest:** Sep 23, 2025 (CC0 license added Sep 12, 2025!) — periodic README updates
- **Why It Matters:** The CC0 license adoption is the most significant single-commit signal in carbon capture open source. This is public domain dedication — not MIT, not Apache — CC0. Making computational screening data public infrastructure.

### tjz21/DAC_peroxotitanates — 2 Stars (Jacob Hirschi)
- **URL:** https://github.com/tjz21/DAC_peroxotitanates
- **Language:** Python (computational screening)
- **Focus:** DFT computational screening of peroxotitanate sorbents for DAC
- **Latest:** Sep 23, 2025 (CC0 license added Sep 12, 2025!) — CASTEP references added Jul 2024
- **Why It Matters:** Twin of the peroxovanadates repo. Same author, same CC0 adoption. The Jul 2024 burst added CASTEP reference files, output files, and reactant files — the complete computational screening workflow designed for machine-parsable metadata.

---

## Tier 4: The August/September 2026 Coordination Wave

### What Happened

Multiple independent repositories across different research approaches were updated in coordinated time windows:

| Repo | Date | Activity | Focus | Significance |
|------|------|----------|-------|-------------|
| jkitchin/differentiable-flowsheets | Sep 13-17, 2026 | 10 commits | Differentiable process simulation | **Most active carbon repo; Claude writing code** |
| tjz21/DAC_peroxovanadates | Sep 12, 2025 | CC0 license | Public domain DAC materials | **Biggest open-science signal** |
| tjz21/DAC_peroxotitanates | Sep 12, 2025 | CC0 license | Public domain DAC materials | **Twin of peroxovanadates** |
| protontypes/open-sustainable-technology | Aug 23, 2026 | claude-carbon added | AI for carbon capture directory entry | **AI recognized as category** |
| protontypes/open-sustainable-technology | Aug 18, 2026 | MUIO/MUIOGO added | DAC hardware control units | **Hardware ecosystem growing** |
| protontypes/open-sustainable-technology | Jul 2, 2026 | PowerIO added | Power IO for sustainable tech | **Infrastructure expansion** |

### Possible Explanations

1. **AI-augmented simulation wave (Sep 2026):** The differentiable-flowsheets commits with Claude-authored code suggest AI-assisted process simulation is becoming mainstream in climate tech.

2. **Shared paper or preprint (Sep 2025):** Both tjz21 repos adopted CC0 on the same day (Sep 12, 2025), suggesting a shared reference frame — possibly a paper or community norm.

3. **Coordinated community challenge (Aug 2026):** Multiple entries added to the open-sustainable-technology directory in a 5-day window.

4. **Breakthrough event:** A discovery that triggered parallel independent implementation.

### Why It Matters

The September 2026 AI-augmented simulation wave is the most significant new signal in this update. Claude-authored commits in differentiable-flowsheets aren't noise — they're fixes to boundary conditions and loading corrections in production code. AI is moving from code review to code writing in climate tech.

The September 2025 CC0 adoption across both tjz21 repos is the biggest structural signal. Public domain dedication enables AI training data. If AI models are trained on CC0-licensed DAC materials data, the license choice becomes foundational infrastructure.

---

## The Discovery Gap: What's NOT on GitHub (Updated)

| Missing Category | Why It's Missing | Nearest Existing Tool |
|-----------------|------------------|----------------------|
| DAC system integration code | Materials science is active; system engineering is absent | differentiable-flowsheets (JAX-based, but focused on REE extraction, not DAC-specific) |
| DAC economic modeling | No open-source cost analysis for full DAC systems | None |
| Commercial DAC plant monitoring | Operators don't share control systems open-source | CO2-Soft-Sensor (lab-scale, not commercial) |
| Long-term sorbent degradation data | Industry keeps this proprietary; academic projects don't have the data | None |
| AI-augmented DAC design | AI writing climate tech code is very new (Sep 2026) | differentiable-flowsheets (Claude-authored commits) |
| Public-domain DAC materials data | CC0 is rare; most repos use MIT/Apache/no license | tjz21/DAC_peroxovanadates + DAC_peroxotitanates (CC0, Sep 2025) |

---

## 🎙️ Episode Hooks (Updated)

1. **AI is writing climate tech code.** differentiable-flowsheets has Claude-authored commits fixing production code. This is not a literature survey — it's live engineering with AI. The implications for accelerating DAC system design are profound.

2. **The CC0-to-AI pipeline.** tjz21's public domain dedication (Sep 2025) enables AI training data. If AI models are trained on CC0-licensed DAC materials data, the public-domain commitment becomes the foundation of the entire AI-mentioned materials discovery pipeline.

3. **OpenAir-Cyan proved it can be done — and then stopped.** The OSHWA certification was the milestone. But 2.5 years of silence is the open-hardware limbo problem.

4. **The August/September 2026 wave is the coordination signal.** Not just 6 repos, but now AI-augmented simulation joining the party. The CC0 materials data (Sep 2025) may become the training infrastructure for AI-driven DAC design.

5. **The field is in knowledge-integration mode.** The dominant repo (Carbon_Capture_ML, 56 stars) curates papers. But differentiable-flowsheets is producing new code with AI assistance. The field may be transitioning from knowledge-integration to AI-augmented design.

6. **The ghost project haunts us.** carbon-capture-and-storage (85 stars, dormant since 2021) is the prototype of the "stars without sustainability" problem.

7. **The soft-sensor and differentiable-flowsheets are the two deployable layers.** Soft-sensors for plant control (tonyzyl, 16★) and differentiable simulation for process optimization (kitchin, 13★) bridge the gap between materials discovery and deployment.

8. **The MUIO/MUIOGO hardware control units are the physical layer.** These DAC control units added to the open-sustainable-technology directory (Sep 2026) represent the hardware-software interface that's been missing. You need control hardware to run a DAC system, and now open-source designs exist.

---

## Updated Episode Questions (v4)

1. Can open source break the $1000/ton DAC cost barrier? The materials science is accelerating, AI-augmented simulation is here (differentiable-flowsheets, Claude writing code), but the engineering integration is absent.

2. What happens when AI writes the code? differentiable-flowsheets has Claude-authored commits fixing production code. Climate tech is the canary in the AI-coordinated-engineering coal mine.

3. Is CC0 the future of open climate science? tjz21's public domain dedication (Sep 2025) enables AI training data. If the AI materials discovery pipeline depends on CC0 data, the license choice becomes infrastructure.

4. Will differentiable simulation replace bench-scale experimentation? JAX-based differentiable flowsheets compute gradients of chemical separation processes, enabling gradient-based optimization. This is the computational equivalent of "test 10,000 configurations in silico before building one."

5. What kills open-source hardware projects? OpenAir-Cyan's story — certification to dormancy — is a case study in what happens when the researcher moves on.

6. Are peroxides the sorbent of the future? The CC0 commitment (Sep 2025) suggests the researcher views them as public infrastructure, not intellectual property.

7. Is the soft-sensor + differentiable-flowsheets combination the real deployable? Soft-sensors for plant control and differentiable simulation for process optimization together bridge the full gap from materials science to deployment.

8. Is MUIO/MUIOGO the hardware-software interface? Open-source DAC control units added to the directory (Sep 2026) represent the physical layer that's been missing. You need hardware to run a DAC system, and now open designs exist.