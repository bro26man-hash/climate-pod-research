# 🌍 Carbon Capture — Open-Source Project Discoveries

## Branch: `carbon-capture`
*Last updated by podcast research, Sept 2026*

---

## 1. Overview

Direct Air Capture (DAC) and carbon-dioxide removal (CDR) have become the frontier of climate-tech open-source innovation. What makes this branch distinctive is the coexistence of two very different modes of development: **atomic material-science updates** (single-commit computational chemistry experiments on peroxovanadates and peroxotitanates) and **bursty system-engineering sprints** (OpenCarbon's coordinated multi-file push). This dual rhythm tells us something about the maturity of the field.

---

## 2. Project Catalog

### ⚗️ openair-collective/openair-cyan — **76 ⭐** — `C++ / Hardware`
**URL:** https://github.com/openair-collective/openair-cyan
**Last updated:** Aug 19, 2026
**Focus:** DIY small-scale open hardware Direct Air Capture device (OSHWA-certified)

The flagship open-hardware DAC project. Cyan is a tabletop direct air capture machine — several variants exist (v1, v2, Cyanide).

**Recent commits (Aug 19, 2026 — page 1):**
- `b5422b3`: Update README — added OSHWA UID link
- `828f496`: Added OSHWA UID logo (US001095)
- `4b08fb3`: Create CITATION.cff (academic citation support)

These are README/hardware-certification updates — the project is maturing from "DIY hack" to "certified open hardware with formal documentation."

**Podcast angle:** The first OSHWA-certified open-hardware carbon removal device. What does it mean when a DAC machine is open-sourced? Can peer review accelerate hardware iteration?

---

### 🏗️ terranexum/OpenCarbon — **2 ⭐** — `MIT`
**URL:** https://github.com/terranexum/OpenCarbon
**Last updated:** Jul 18, 2023
**Focus:** Carbon management technologies — DAC, biochar, insulation

Three products under one roof: **Cyan v.2 upgrade**, **CarbonWall** (biochar + CaCO₃ insulation panels), and **BioDAC** (functionalized biochar sorbent for DAC).

**Recent commits (Jul 13–18, 2023):**
- `e3e5afb`: Merge PR #3 (shrila-dev branch)
- `bb5c7b2` / `bc5a343`: README updates
- `96e7c2c` / `bb603ec`: README updates by Dahl Winters
- `34ff91c`: Update Project_Plan.md
- `f2c9866`: Create Project_Plan.md

**Podcast angle:** The multi-product carbon strategy. Biochar + DAC + building insulation = carbon removal that pays for itself. Interesting contrast with Cyan's pure-hardware approach.

**Chemistry highlights from README:**
- **Cyan v.2 capture:** Ca(OH)₂ + CO₂ → CaCO₃ + H₂O
- **Release:** 2 HCl + CaCO₃ → CaCl₂ + H₂O + CO₂
- **Regeneration:** CaCl₂ + Fe₂O₃ → Ca(OH)₂ + 2FeCl₃
- **Electrowinning:** 2FeCl₃ → 2Fe + 3Cl₂ (requires renewable electricity)

---

### 🧪 tjz21/DAC_peroxovanadates — **2 ⭐** — `Python`
**URL:** https://github.com/tjz21/DAC_peroxovanadates
**Last updated:** Aug 2026
**Focus:** Computational chemistry SI for DAC materials (peroxovanadate sorbents)

Single-commit push — a supplementary-information repo for computational DAC materials research.

**Commit:** `8faba53` (Aug 24, 2026) — Added supplementary information for a novel metal-oxide DAC sorbent paper.

---

### 🧪 tjz21/DAC_peroxotitanates — **2 ⭐** — `Python`
**URL:** https://github.com/tjz21/DAC_peroxotitanates
**Last updated:** Aug 2026
**Focus:** Computational chemistry SI for DAC materials (peroxotitanate sorbents)

Twin repo to peroxovanadates. Both pushed within days of each other in August 2026.

---

### ⚡ o7-machinehum/electro-swing-dacc — **unlisted stars** — `Python`
**URL:** https://github.com/o7-machinehum/electro-swing-dacc
**Last updated:** Aug 2026
**Focus:** DIY electro-swing DAC plans (open-source)

Electro-swing DAC is an emerging approach using electrochemical cycling to capture and release CO₂ — potentially much lower energy than thermal-swing DAC.

---

### 🌐 api-evangelist/280-earth — **unlisted stars**
**URL:** https://github.com/api-evangelist/280-earth
**Last updated:** Sep 16, 2026
**Focus:** API profile of 280 Earth (DAC company) — third-party public API surface catalog

Not a simulation tool, but a metadata profile — tracks how climate-tech companies expose their data.

---

## 3. Carbon Capture Commit Trends

| Signal | Observation |
|--------|-------------|
| **Bursty vs. steady** | Two patterns: (1) single-shot computational chemistry commits (tjz21), (2) coordinated multi-file pushes (OpenCarbon, Cyan) |
| **August 2026 surge** | 4 DAC materials repos updated in a single week — suggests rising interest in open computational chemistry for sorbent discovery |
| **Hardware certification** | Cyan's OSHWA certification move signals a shift from "hacker project" to "regulated device" |
| **($/ton conversation)** | No repo directly addresses the $1,000/ton cost barrier in code — the conversation is still in README narratives and Google Docs, not in deployed software |
| **Language trend** | Python dominates new DAC code; hardware repos use C++/KiCad; no Rust or Julia yet |

---

## 4. Cross-Project Comparison (Carbon)

| Project | Stars | Mode | Energy Question | Sorbent Type | Hardware? |
|---------|-------|------|-----------------|-------------|-----------|
| **openair-cyan** | 76 | Steady (certification) | Low-temp heat | Ca(OH)₂ | ✅ Open hardware |
| **OpenCarbon / BioDAC** | 2 | Bursty | Chemical regen | Biochar + QA | ❌ Material science |
| **DAC_peroxovanadates** | 2 | Single commit | N/A (computational) | Peroxovanadate | ❌ SI only |
| **electro-swing-dACC** | — | Unknown | Electrical swing | Electro-swing | 🔬 Plans |
| **CarbonWall** | — | Part of OpenCarbon | Low energy | Biochar + CaCO₃ | 🧱 Passive |

---

## 5. Key Questions for Episode

1. **Can open-source break the $1,000/ton DAC cost wall?** Current projects are material-science proofs-of-concept, not deployable systems.
2. **Does open hardware accelerate iteration?** Cyan's OSHWA certification is a test case.
3. **What's missing?** No open-source tool for system-level DAC plant optimization, no cost-modelling framework, no life-cycle assessment tool.
4. **Who's building?** Solo researchers and small collectives — no major institutional presence comparable to PCMDI in the modeling space.
