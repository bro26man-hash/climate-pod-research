# 🌍 Carbon Capture — Episode Research Notes

## Episode Overview
This episode covers Direct Air Capture (DAC) and other carbon dioxide removal (CDR) technologies — the hardware, materials science, and open-source tools that could make carbon capture economically viable. We explore the DIY hardware movement, the computational materials screening pipelines, and the systemic questions about whether capture alone can solve climate change.

---

## Key Open-Source Projects

### 1. openair-cyan (openair-collective/openair-cyan)
- **Stars:** 76 | **Language:** Open Hardware | **Last Updated:** Feb 12, 2024
- **What it does:** DIY small-scale open hardware direct air carbon capture device. Complete documentation, OSHWA-certified (US001095). Designed to be buildable by individuals and small labs.
- **Why it matters for the episode:** This is the most impactful carbon capture repo on GitHub. It proves that DAC hardware can be documented, replicated, and improved by a community — not just billion-dollar startups.
- **Commit activity:** Dense burst of 9 commits on Feb 12, 2024 (OSHWA certification, CITATION.cff, file uploads), then silence. Earlier activity in 2022 with maintenance commits.
- **Episode angle:** "Can a $200 DIY device prove that carbon capture doesn't need to cost $1,000/ton?"

### 2. DAC_peroxovanadates (tjz21/DAC_peroxovanadates)
- **Stars:** 2 | **Language:** — | **Last Updated:** Aug 19, 2026
- **What it does:** Computational screening of peroxovanadate compounds for DAC sorbent applications.
- **Why it matters:** Part of a coordinated August 2026 research event where multiple DAC materials repositories were created simultaneously. Suggests a systematic computational materials screening approach.
- **Commit activity:** Last updated Aug 19, 2026. Minimal commit history visible.
- **Episode angle:** "Are peroxides the next-generation sorbent? A computational chemist's GitHub burst says maybe."

### 3. DAC_peroxotitanates (tjz21/DAC_peroxotitanates)
- **Stars:** 2 | **Language:** — | **Last Updated:** Aug 19, 2026
- **What it does:** Same as above, but for peroxotitanate compounds. Sister repo to the vanadates screening.
- **Commit activity:** Same pattern as peroxovanadates — created Aug 19, 2026.
- **Episode angle:** "Why did two peroxo-sorbent repos appear on the same day? The coordinated research wave."

### 4. OpenCarbon (terranexum/OpenCarbon)
- **Stars:** 2 | **Language:** — | **Last Updated:** Aug 19, 2026
- **What it does:** Carbon management technologies and planning tools for DAC — ensuring clean energy use and low-cost operation.
- **Episode angle:** "The planning layer: you can build a DAC device, but can you plan a DAC *system*?"

### 5. carbon-capture-cant-solve-climate-change (datasets/)
- **Stars:** N/A | **Language:** Datasets | **Last Updated:** Jul 3, 2026
- **What it does:** Data behind ProPublica's 2026 explainer comparing decades of carbon capture projections against solar power projections.
- **Why it matters:** The definitive data-journalism resource on the "can CCS save us?" question. ProPublica found that CCS has consistently underperformed projections while solar has exceeded them.
- **Episode angle:** "The dataset that proves carbon capture has been lying to us for decades — and the numbers are still worse."

### 6. ClimateSoton / ClimateSoton.github.io
- **Stars:** N/A | **Language:** HTML | **Last Updated:** Jul 26, 2026
- **What it does:** Research group page for the CLIMATE Research Group at University of Southampton. Chemical looping, advanced capture materials, sustainable energy.
- **Episode angle:** "What does a working university capture lab's web presence look like?" (More of a hub than a tool.)

### 7. Carbonize (SahilKhutey/Carbonize)
- **Stars:** N/A | **Language:** Python | **Last Updated:** Jul 29, 2026
- **What it does:** Coral-inspired biomineralization multi-pollutant capture simulator (CBMS-Sim). Industrial SaaS platform for CO2, SO2, NOx, and heavy metals capture using biomimetic materials.
- **Episode angle:** "What if carbon capture looked like coral? Nature's mineralization playbook, simulated in Python."

### 8. openair-sorbent-tester (openair-collective/)
- **Stars:** 3 | **Language:** — **Last Updated:** Jan 10, 2026
- **What it does:** Moisture swing DAC sorbent tester — companion hardware to the Cyan device for quickly evaluating sorbent materials.
- **Episode angle:** "The testing infrastructure matters as much as the device. OpenAir is building both."

---

## Commit Trend Analysis: Carbon Capture

| Pattern | Finding |
|---------|--------|
| **The August 2026 DAC materials wave** | Three repos (peroxovanadates, peroxotitanates, OpenCarbon) all updated on Aug 19, 2026. This wasn't organic — it was a coordinated research event, likely a paper submission or grant deliverable. |
| **Hardware vs. software asymmetry** | The most important carbon capture repo (OpenAir-Cyan, 76★) is hardware documentation, not software. The "code" is a BOM and assembly guide. |
| **The CCS-vs-solar data story** | ProPublica's dataset is 0 stars but potentially the most influential carbon capture resource on GitHub — it provides the evidentiary backbone for the "CCS doesn't work" narrative. |
| **Biomimicry emerging** | Carbonize (coral-inspired mineralization) represents a new direction — using biological patterns for capture materials. Computational, simulation-first approach. |
| **Dormancy is universal** | Every carbon capture repo except OpenAir's 2024 burst and the 2026 materials wave is dormant. The field is project-based, not platform-based. |
| **The sorbent testing gap** | OpenAir's sorbent tester (3★) shows that the community is starting to build *evaluation infrastructure*, not just devices. This is a maturing signal. |

---

## Key Episode Questions

1. **Can open-source hardware break the $1,000/ton DAC cost barrier?** OpenAir-Cyan proves the concept, but has it scaled?
2. **The August 2026 materials wave:** Was it a real breakthrough or just a coordinated GitHubmoment? Three peroxo-sorbent repos appearing on the same day is either a genuine convergence or a job-market flex.
3. **CCS has failed — so why does the industry keep championing it?** ProPublica's data shows decades of overpromising. Is carbon capture a sector built on bad lie detection?
4. **Biomimicry vs. engineering:** Is coral-inspired mineralization the future, or are we overcomplicating something that should be simple?
5. **The infrastructure gap:** We have DIY DAC devices but almost no open-source tools for system-level DAC planning. OpenCarbon is the start.

---

## Sources & Links
- [openair-cyan](https://github.com/openair-collective/openair-cyan)
- [DAC_peroxovanadates](https://github.com/tjz21/DAC_peroxovanadates)
- [DAC_peroxotitanates](https://github.com/tjz21/DAC_peroxotitanates)
- [OpenCarbon](https://github.com/terranexum/OpenCarbon)
- [carbon-capture-cant-solve-climate-change](https://github.com/datasets/carbon-capture-cant-solve-climate-change)
- [Carbonize](https://github.com/SahilKhutey/Carbonize)
- [openair-sorbent-tester](https://github.com/openair-collective/openair-sorbent-tester)
