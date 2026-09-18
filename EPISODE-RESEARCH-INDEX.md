# 📋 Episode Research Index (v6)

> **Last updated:** September 2026 (v6)  
> **Branch:** `main`  
> **Podcast:** Climate Tech & Geoengineering

---

## Episode 1: Solar Geoengineering

**Branch:** `solar-geoengineering`  
**Files:** [PROJECT-DISCOVERIES-SOLAR.md](https://github.com/bro26man-hash/climate-pod-research/tree/solar-geoengineering/PROJECT-DISCOVERIES-SOLAR.md) | [COMMIT-TRENDS-SOLAR.md](https://github.com/bro26man-hash/climate-pod-research/tree/solar-geoengineering/COMMIT-TRENDS-SOLAR.md)

### Key Questions
Why is SRM code so scarce? Can interactive models democratize the discourse? What does the solar radiation bug fix mean for SRM trustworthiness?

### v6 Commit Evidence
| Repo | Stars | Commits | Key Finding |
|------|-------|---------|-------------|
| **wrf-model/WRF** | 1,762 | 15 (May-Jun 2026) | **Solar radiation EOT bug fix** (e836cd6, May 28) — every past SRM simulation using this scheme may have had systematic energy budget error. Also: TEMPO aerosol-aware/hailaware disabled for stratospheric stability (6a289e1, Jun 5). |
| **PCMDI/pcmdi_metrics** | 133 | 15 (Sep 3-17, 2026) | **10 commits in 2 days** for v4.2.1. **Roundoff bugfix** (90cbc50) — values clipping at 1.00 in mean_climate figures, corrupting normalized metrics. **numpy SVD fallback** (1fca2ec) — ensuring PCA reproducibility. |
| **ClimateMARGO** | 73 | 2 (Aug 17, 2026) | **Ambiguous revival** — 2 README updates after 2+ year dormancy, zero code changes. Pattern: heavy dev → 9mo gap → 2 README updates → 2+ year gap → 2 README updates. |
| **srm-forever** | 0 | 4 (Aug 2026) | **Weitzman discounting** — interactive model showing SRM economics flip based on discount rate. At defaults, SRM is cheaper (~$42T vs ~$55T) but TCRE range straddles the verdict. |

### Narrative Arcs
- **Arc A: "The Invisible Model"** — WRF is the engine behind every SRM claim. The solar radiation bug fix is the entry point.
- **Arc B: "The QA Lab"** — PCMDI is the model evaluation infrastructure. The roundoff bug story is "how science self-corrects."
- **Arc C: "The Economics Question"** — ClimateMARGO + srm-forever = policy and economics layer. The Weitzman twist makes the answer hinge on philosophy, not physics.
- **Arc D: "The Ghost Ship"** — ClimateMARGO's dormancy and revival. What does it mean when a climate model goes quiet?

---

## Episode 2: Carbon Capture

**Branch:** `carbon-capture`  
**Files:** [PROJECT-DISCOVERIES-CARBON.md](https://github.com/bro26man-hash/climate-pod-research/tree/carbon-capture/PROJECT-DISCOVERIES-CARBON.md) | [COMMIT-TRENDS-CARBON.md](https://github.com/bro26man-hash/climate-pod-research/tree/carbon-capture/COMMIT-TRENDS-CARBON.md)

### Key Questions
Can open source break the $1000/ton DAC cost barrier? What makes OSHWA certification special? The CC0 revolution — should all climate research data be public domain?

### v6 Commit Evidence
| Repo | Stars | Commits | Key Finding |
|------|-------|---------|-------------|
| **open-sustainable-technology** | 2,552 | 15 (Jun-Sep 2026) | **Only actively growing repo** — 2-3 commits/month. AI content disclosure PR template (Jul 19). New entries: MUIO, MUIOGO, claude-carbon, PowerIO, ASSETRA, ToOp. |
| **openair-cyan** | 76 | 15 (May 2022-Feb 2024) | **7-commits-in-1-day blitz** (Feb 12, 2024) for OSHWA certification (UID US001095). Then 2+ years silence. The certification was a peak, not a plateau. |
| **Carbon_Capture_ML** | 56 | 10 (Jan-May 2024) | **OpenDAC paper added** (May 8, 2024) — largest open dataset of DFT calculations for CO2 capture materials. Then silence. Earlier burst: 5 papers in 3 months (Feb-May 2023). |
| **DAC_peroxovanadates** | 2 | 10 (Nov 2023-Sep 2025) | **CC0 license added** (Sep 12, 2025, commit e041eff) — public domain dedication. The most significant open-science event in carbon capture this year. |
| **DAC_peroxotitanates** | 2 | 10 (Feb-Sep 2024) | **Same pattern** — CC0 dedication, companion repo to peroxovanadates. Two parallel screening pipelines, both public domain. |
| **carbon-capture-and-storage** | 85 | 0 (since 2021) | **Ghost repo** — 85 stars, dead since March 2021. Stars measure citations, not usability. |

### Narrative Arcs
- **Arc A: "The Catalogue"** — Open-Sustainable-Technology is the universe of climate tech. 2,552 stars, 2,500+ projects, constantly growing.
- **Arc B: "The Demo"** — OpenAir-Cyan's OSHWA certification was a landmark, but the silence since is the twist.
- **Arc C: "The Data Revolution"** — CC0 licensing in the DAC materials community. Two repos, both public domain. This is how open science is supposed to work.
- **Arc D: "The Ghosts"** — 85-star dead repos and citation inflation. What do stars actually measure?

---

## Episode 3: Ocean Intervention

**Branch:** `ocean-intervention`  
**Files:** [PROJECT-DISCOVERIES-OCEAN.md](https://github.com/bro26man-hash/climate-pod-research/tree/ocean-intervention/PROJECT-DISCOVERIES-OCEAN.md) | [COMMIT-TRENDS-OCEAN.md](https://github.com/bro26man-hash/climate-pod-research/tree/ocean-intervention/COMMIT-TRENDS-OCEAN.md)

### Key Questions
Why is ocean geoengineering the empty quadrant? What would open-source OAE look like? Is the silence itself a governance signal?

### v6 Commit Evidence
| Repo | Stars | Commits | Key Finding |
|------|-------|---------|-------------|
| **MDTF-diagnostics** | 80 | 5 (Jun 19, 2026) | **Precipitation-buoyancy POD** — 5 commits in 1 day, all touching same file. The most ocean-relevant diagnostic in open source, but for evaluation, not intervention. |
| **WRF (coupled)** | 1,762 | Indirect | Air-sea coupling physics in v4.8.0, but no one is using WRF for ocean intervention scenarios. |
| **Ocean geoengineering** | 0 | ZERO | **12 search queries, zero results** — no OAE, MCB, artificial upwelling, ocean fertilization, or ocean sensor repos exist. |

### The Ocean Gap — 12 Queries, Zero Results

| # | Search | Results |
|---|--------|---------|
| 1 | geoengineering simulation climate | 0 |
| 2 | climate technology carbon capture ocean | 0 dedicated |
| 3 | geoengineering stars:>50 | 1 (not ocean) |
| 4 | climate simulation modeling stars:>100 | 1 (atmosphere only) |
| 5 | carbon capture removal stars:>100 | 0 |
| 6 | ocean climate intervention stars:>50 | 0 |
| 7 | climate model atmospheric ocean stars:>200 | 0 |
| 8 | direct air capture DAC stars:>50 | 0 (not ocean) |
| 9 | ocean alkalinity enhancement | 0 |
| 10 | marine cloud brightening | 0 |
| 11 | artificial upwelling ocean model | 0 |
| 12 | ocean fertilization iron model | 0 |

### Narrative Arcs
- **Arc A: "The Empty Quadrant"** — We searched 12 ways. We found nothing. The silence is the signal.
- **Arc B: "The Three Hypotheses"** — Complexity barrier? Governance chill? Funding gap? All three plausible.
- **Arc C: "The Architecture"** — What would the first open-source OAE model look like? Here's a concrete sketch.
- **Arc D: "The Call to Action"** — The quadrant is empty. What are you going to do about it?

---

## Cross-Theme Patterns (v6 Update)

| Pattern | Solar | Carbon | Ocean |
|---------|-------|--------|-------|
| **Active institutional repos** | WRF (1,762★), PCMDI (133★) | Open-Sustainable-Tech (2,552★) | None |
| **Bug-fix stories** | WRF solar radiation (e836cd6), PCMDI roundoff (90cbc50) | — | — |
| **Dormant individual repos** | ClimateMARGO (73★) | OpenAir-Cyan (76★), Carbon_Capture_ML (56★) | None (there are none) |
| **Zero-star but critical** | srm-forever (0★) | tjz21 repos (2★ each) | The entire ocean quadrant |
| **CC0 / open-science** | srm-forever (MIT, open tool) | tjz21 (CC0-1.0), Open-Sustainable-Tech (CC0-1.0) | Zero data |
| **"Big bang then freeze"** | — | OpenAir-Cyan (7/day then 2yr silence), Carbon_Capture_ML (5 papers then silence) | The entire domain is a "big freeze" |

---

## Quick Links

| Resource | Location |
|----------|----------|
| 🏠 Repository | https://github.com/bro26man-hash/climate-pod-research |
| ☀️ Solar branch | https://github.com/bro26man-hash/climate-pod-research/tree/solar-geoengineering |
| 🌍 Carbon branch | https://github.com/bro26man-hash/climate-pod-research/tree/carbon-capture |
| 🌊 Ocean branch | https://github.com/bro26man-hash/climate-pod-research/tree/ocean-intervention |
| 📊 Cross-theme v6 | [CROSS-THEME-ANALYSIS-SEP2026-v6.md](https://github.com/bro26man-hash/climate-pod-research/blob/main/CROSS-THEME-ANALYSIS-SEP2026-v6.md) |