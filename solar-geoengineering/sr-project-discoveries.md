# ☀️ Solar Geoengineering — Open-Source Project Discoveries

*Research pulled from GitHub: September 2026*

---

## Top Repositories

### 1. ClimateMARGO/ClimateMARGO.jl
| Field | Detail |
|---|---|
| **Language** | Julia |
| **Stars / Forks** | 73 ⭐ / 13 🍴 |
| **License** | MIT |
| **Last Updated** | 17 Aug 2026 |
| **URL** | https://github.com/ClimateMARGO/ClimateMARGO.jl |

**What it does:** A Julia implementation of MARGO — an idealized climate-economic optimization framework that balances emissions mitigation, adaptation, carbon dioxide removal, **and solar geoengineering**. The model is described in a peer-reviewed paper in *Environmental Research Letters* (open access).

**Why it matters for the podcast:** MARGO is one of the few open-source tools that explicitly models SRM as a climate-control lever alongside mitigation and CDR. The interactive Pluto notebook (runner link in README) lets users drag emissions curves and see warming outcomes in real-time — superb for a podcast demo segment. The repo is in beta; structural changes may occur before v1.0.0, so the landscape is still shifting.

---

### 2. FMS-ESM/AM3
| Field | Detail |
|---|---|
| **Language** | FORTRAN |
| **Stars / Forks** | 4 ⭐ / 5 🍴 |
| **License** | None (GFDL) |
| **Last Updated** | 1 Mar 2015 (master branch) |
| **URL** | https://github.com/FMS-ESM/AM3 |

**What it does:** AM3 is the atmospheric component of NOAA's GFDL CM3 coupled climate model. It was the **first GFDL global atmospheric model to include cloud-aerosol interactions** — directly relevant to how stratospheric aerosols (SAI) would interact with clouds. It has 20 interactive aerosol species, interactive tropospheric and stratospheric chemistry (85 species), and a cubed-sphere dynamical core.

**Why it matters for the podcast:** AM3 is a **legacy giant** — released March 2012, code on GitHub 2015, last commit 2015. It represents the closed-academic-model problem: the foundational simulation tools for SRM effects live in institutions (GFDL, NCAR, LASG) but aren't being actively developed in the open. The 4 stars but 5 forks suggest people star it for reference but don't necessarily contribute back. The cubed-sphere core and aerosol activations are exactly the physics we'd want to see open-sourced for SAI research.

---

### 3. srm-ecology/climate_analogs
| Field | Detail |
|---|---|
| **Language** | Jupyter Notebook (Python & R) |
| **Stars / Forks** | 0 ⭐ / 1 🍴 |
| **License** | MIT |
| **Last Updated** | 21 Jul 2026 |
| **URL** | https://github.com/srm-ecology/climate_analogs |

**What it does:** Generates **climate analogs** — i.e., current-day locations whose future climate (under SAI scenarios) matches the projected climate of a focal ecosystem. This is a powerful conceptual tool: instead of simulating SRM globally, you find places today that already *live* under the climate we'd create with SAI, and study their ecosystems as proxies.

**Why it matters for the podcast:** This is **emerging open-source SRM research** — a creative, ethically grounded alternative to running full GCMs. The workflow (raw data → monthly merge → geodiversity stats) is transparent and reproducible. Active commits from June–July 2026 show this is a living project. The MIT license means anyone can use it. The small star/fork count suggests it's early-stage but methodologically interesting.

---

### 4. ChinmayaSaran/sai-climate-tradeoffs
| Field | Detail |
|---|---|
| **Language** | TypeScript (Next.js + Recharts) |
| **Stars / Forks** | 0 ⭐ / 0 🍴 |
| **License** | MIT |
| **Last Updated** | 19 May 2026 |
| **URL** | https://github.com/ChinmayaSaran/sai-climate-tradeoffs |

**What it does:** An **interactive web tool** that visualizes peer-reviewed findings on stratospheric aerosol injection — latency effects, drought response, forcing curves, deployment feasibility, costs, and seasonality. Every number in the tool traces directly to a figure in one of **seven peer-reviewed papers**, each with DOI links.

**Why it matters for the podcast:** This is a **transparency-first** approach to SRM communication. Instead of simulating SRM itself, it aggregates and visualizes the *published literature* in an accessible, citable format. The live demo (sai-climate-tradeoffs.vercel.app) is a great podcast reference. The tool's limitation disclaimer — "interpolated values carry additional uncertainty beyond the source data" — models the kind of scientific humility we want to hear on the show.

---

### 5. protontypes/open-sustainable-technology
| Field | Detail |
|---|---|
| **Language** | Multi-language |
| **Stars / Forks** | 2,552 ⭐ / 330 🍴 |
| **License** | CC-BY-4.0 |
| **Last Updated** | 9 Sep 2026 |
| **URL** | https://github.com/protontypes/open-sustainable-technology |

**What it does:** A **comprehensive directory** of open-source projects across climate change, sustainable energy, biodiversity, and natural resources. Their atmospheric section includes radiative transfer, atmospheric chemistry & aerosol, and Earth/climate modeling subcategories.

**Why it matters for the podcast:** With 2,552 stars and 330 forks, this is the **most active OSS climate-tech directory on GitHub**. It's a curated hub that links out to dozens of SRM-relevant projects (GeoMIP, EN-ROADS, FAIR climate model, etc.). The recent commit activity (Sep 2026) shows continuous curation. It's the "map" for exploring the rest of this list.

---

### 6. brandonhimpfen/awesome-geoengineering
| Field | Detail |
|---|---|
| **Language** | Python (markdown) |
| **Stars / Forks** | 4 ⭐ / 0 🍴 |
| **License** | CC-BY-SA 4.0 |
| **Last Updated** | 6 Sep 2026 |
| **URL** | https://github.com/brandonhimpfen/awesome-geoengineering |

**What it does:** A curated list of geoengineering projects, research, organizations, tools, and resources — explicitly covering both **Carbon Dioxide Removal (CDR)** and **Solar Radiation Management (SRM)**. Well-organized with policy/ethics, tool/model/data, and open-source project sections.

**Why it matters for the podcast:** Small but meticulously maintained. Updated as recently as September 2026 with active README edits. The "Open Source Projects" section links to EN-ROADS, FAIR, and GeoMIP — the core simulation infrastructure. A great starting point for listeners who want to dig deeper.

---

### 7. pmip4/pmip_p2fvar_analyzer
| Field | Detail |
|---|---|
| **Language** | Jupyter Notebook |
| **Stars / Forks** | 4 ⭐ / 0 🍴 |
| **Last Updated** | 19 Sep 2025 |
| **URL** | https://github.com/pmip4/pmip_p2fvar_analyzer |

**What it does:** Analyzes past-to-future (P2F) variable output from **CMIP6** — the Coupled Model Intercomparison Project that underpins all IPCC climate projections, including SRM sensitivity studies.

**Why it matters for the podcast:** CMIP6 includes GeoMIP and GeoMIP-like experiments (e.g., G4, G6). This analyzer is a lightweight tool for podcast listeners to explore CMIP6 data themselves. The four stars suggest it's a specialized tool, not a mainstream one.

---

## Key Trend Summary

### The Code Gap
- **Legacy Fortran models dominate** (AM3, last commit 2015). The foundational SRM simulation infrastructure is decades old and not actively maintained in the open.
- **New Jupyter/TypeScript tools are emerging** (climate_analogs, sai-climate-tradeoffs) but start small — 0–4 stars.
- The **real open-source activity** is in curation (open-sustainable-technology with 2,552 stars) and educational visualization rather than in running the actual GCMs.
- **ClimateMARGO.jl** is the standout exception — a modern, actively-developed (Julia/Python) optimization framework that includes SRM. 73 stars and recent commits.

### The Governance Story
Several repos (awesome-geoengineering, sai-climate-tradeoffs) come with explicit policy/ethics disclaimers. The open-source SRM community is acutely aware of the governance risks and builds transparency into their tools.

### Podcast Episode Angle
*"Why can't we simulate solar geoengineering in the open?"* — The answer is: we can, but the heavy compute and institutional funding barriers keep it closed. The emerging trend is lighter-weight tools (analog-based, data-visualization, optimization) that democratize access without requiring a supercomputer.
