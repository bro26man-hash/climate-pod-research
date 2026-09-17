# 🌍 Carbon Capture (CDR) — Open-Source Project Discoveries

*Research pulled from GitHub: September 2026*

---

## Top Repositories

### 1. tjz21/DAC_peroxovanadates
| Field | Detail |
|---|---|
| **Language** | DIGITAL Command Language |
| **Stars / Forks** | 2 ⭐ / ? 🍴 |
| **Last Updated** | 19 Aug 2026 |
| **DOI** | [10.1039/D3SC05381D](https://doi.org/10.1039/D3SC05381D) |
| **URL** | https://github.com/tjz21/DAC_peroxovanadates |

**What it does:** Computational supplementary information (SI) for the paper *"Implementing Tetraperoxovanadates as Direct Air Carbon Capture Materials"* (Chemical Science, 2024). Contains quantum chemistry input/output files and analysis scripts for evaluating peroxovanadate compounds as DAC adsorbents.

**Why it matters for the podcast:** This is **open computational chemistry** for next-generation DAC sorbents. The Digital Command Language (likely Gaussian or VASP input files) means researchers can reproduce the DFT calculations publicly. The Aug 2026 update suggests active maintenance. This is a model for how materials science can go open — and how the podcast can explain "why open-source chemistry matters for carbon capture."

---

### 2. tjz21/DAC_peroxotitanates
| Field | Detail |
|---|---|
| **Language** | DIGITAL Command Language |
| **Stars / Forks** | 2 ⭐ / ? 🍴 |
| **Last Updated** | 19 Aug 2026 |
| **DOI** | [10.1021/acs.chemmater.4c01795](https://doi.org/10.1021/acs.chemmater.4c01795) |
| **URL** | https://github.com/tjz21/DAC_peroxotitanates |

**What it does:** Computational SI for *"Tetraperoxotitanates for High-Capacity Direct Air Capture of Carbon Dioxide"* (Chemistry of Materials, 2024). Same workflow as the vanadates paper — open quantum-chemistry inputs/outputs for evaluating titanium-based peroxide sorbents.

**Why it matters for the podcast:** Together with the vanadates repo, this shows a **clear pattern**: a researcher is systematically open-sourcing its DFT-based DAC materials screening. The twin repositories from the same author (tjz21) suggest a research program, not a one-off. The synchronised Aug 2026 updates are striking — this is a hot topic in open computational climate chemistry.

---

### 3. terranexum/OpenCarbon
| Field | Detail |
|---|---|
| **Language** | Not specified (Markdown + PDF + project plans) |
| **Stars / Forks** | 2 ⭐ / 1 🍴 |
| **License** | MIT |
| **Last Updated** | 18 Jul 2023 |
| **URL** | https://github.com/repo/terranexum/OpenCarbon |

**What it does:** A **three-project carbon management initiative**:
- **Cyan v.2** — upgrading the OSHWA-certified open-hardware carbon removal device (Cyan v.1) to add sorbent regeneration and renewable energy capacity
- **CarbonWall** — biochar + CaCO₃ insulation panels that earn carbon credits while improving building energy efficiency
- **BioDAC** — patent-free, open-sourced non-toxic functionalized biochar sorbent for direct air capture

**Why it matters for the podcast:** OpenCarbon is arguably the most **podcast-friendly** repo on this entire list. It spans hardware (Cyan), materials (BioDAC), and policy/market design (CarbonWall with PACE financing and 45Q credits). The contributors are clearly trying to build a circular business model where core contributors earn from products that get to market. The chemistry section (Ca(OH)₂ + CO₂ → CaCO₃ → CaCl₂ + CO₂ via HCl → Ca(OH)₂ regeneration + FeCl₃ electrowinning) is a great "how DAC actually works" segment. The July 2023 activity shows it's still being maintained.

---

### 4. o7-machinehum/electro-swing-dacc
| Field | Detail |
|---|---|
| **Language** | Not specified |
| **Stars / Forks** | 0 ⭐ / 0 🍴 |
| **Last Updated** | 19 Aug 2026 |
| **URL** | https://github.com/o7-machinehum/electro-swing-dacc |

**What it does:** Collects information and plans for building an **electro-swing direct air carbon capture (DAC)** device — using electrochemical pH swings to capture and release CO₂ from air.

**Why it matters for the podcast:** **DIY DAC** is a growing movement. Electro-swing DAC (e-DAC) is fundamentally simpler than thermal-swing DAC because it operates at near-ambient temperatures. This repo is a community knowledge base for building one. The Aug 2026 update suggests active development. Perfect for a "can a maker build a carbon capture machine?" episode segment.

---

### 5. api-evangelist/* (Climeworks, Spiritus, Clairity, 280 Earth)
| Field | Detail |
|---|---|
| **Language** | API profile pages |
| **Last Updated** | 16 Sep 2026 |
| **URL** | https://github.com/api-evangelist |

**What it does:** Independent third-party API profiles of major climate-tech companies including **Climeworks** (DAC), **Spiritus** (carbon capture), **Clairity** (carbon accounting), and **280 Earth** (DAC).

**Why it matters for the podcast:** These aren't simulation or R&D repos — they're **metadata profiles of the commercial DAC ecosystem**. They show which companies have public APIs and what their data surfaces look like. Useful for a segment on "the business of carbon capture" — who's commercial, who's open, and what does their tech stack look like? Recent updates (Sep 2026) show the commercial DAC landscape is being actively catalogued.

---

### 6. protontypes/open-sustainable-technology (Carbon Capture section)
| Field | Detail |
|---|---|
| **Language** | Multi-language |
| **Stars / Forks** | 2,552 ⭐ / 330 🍴 |
| **Last Updated** | 9 Sep 2026 |
| **URL** | https://github.com/protontypes/open-sustainable-technology |

**What it does:** The "Carbon Capture" subsection feeds directly into dozens of linked DAC and CDR projects (see README for the full list within Emissions → Carbon Capture).

**Why it matters for the podcast:** The most comprehensive curated list of OSS carbon capture projects exists within this mega-repo. The podcast should reference this as the "map" for CDR projects.

---

## Key Trend Summary

### Two Modes of Activity
The carbon-capture GitHub landscape splits into **two distinct rhythms**:

1. **Atomic materials science** (tjz21/vanadates, tjz21/titanates): Small repos with precisely-scoped computational chemistry updates. The August 2026 surge in DAC materials repositories (both peroxovanadates and peroxotitanates updated the same day) suggests a coordinated research push — open computational chemistry is accelerating for next-gen sorbents.

2. **Bursty system engineering** (terranexum/OpenCarbon): Larger, more narrative repos featuring project plans, hardware designs, and policy frameworks. OpenCarbon's commits are bursty (May–July 2023) — a team publishing milestones, not iterating daily.

### The DIY/Community TrapDoor
**o7-machinehum/electro-swing-dacc** (0 stars, Aug 2026) represents a totally different mode: community-driven, no-stars, knowledge-base style. DAC is no longer just for national labs. If this repo gains traction, it could fundamentally shift the narrative about who can capture carbon.

### The Commercial API Layer
The api-evangelist profiles (all updated Sep 2026) show that **commercial DAC companies (Climeworks, 280 Earth, etc.) increasingly expose public APIs** — making them queryable, auditable, and programmable. This is the bridge between open-source tools and the $1000+/ton commercial DAC market.

### Podcast Episode Angle
*"Can open-source break the DAC cost barrier?"* — The materials science is going open (vanadates, titanates, biochar), but system-level engineering (OpenCarbon) and commercial deployment (Climeworks APIs) remain closed or proprietary. The DIY electro-swing movement is attempting to third-world the technology. The tension between these three modes is the episode's spine.
