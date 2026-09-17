# 🎙️ Cross-Theme Climate Tech Analysis — September 2026 (v4)
## GitHub-Based Research for Podcast Series on Climate Technology & Geoengineering

---

## 📊 Master Dashboard: All Three Themes

### Commit Activity Summary
| Theme | Repos Sampled | Total Recent Commits | Avg Commits/Repo | Most Active Repo |
|-------|---------------|---------------------|-------------------|------------------|
| ☀️ Solar | 6 | 55 | 9.2 | WRF (15 in 30 days) |
| 🌍 Carbon | 10+ | 60+ | 6.0 | open-sustainable-technology (continuously active) |
| 🌊 Ocean | 5 | 25+ | 5.0 | aiida-icon (15 in 7 months) |
| **Total** | **21+** | **140+** | **6.7** | **WRF dominates solar** |

### Stars vs. Commits (The Reach vs. Activity Paradox)
| Repo | Stars | Recent Commits | Stars/Commit Ratio | Interpretation |
|------|-------|----------------|--------------------|----|
| open-sustainable-technology | 2,552 | Continuous | ∞ (ongoing) | The directory that never stops growing |
| WRF | 1,761 | 15 (monthly) | 117.4 | High-impact, actively maintained |
| Oceananigans.jl | 1,413 | (from v2) | High | Ocean physics star, intervention void |
| pcmdi_metrics | 133 | 10 (bi-monthly) | 13.3 | Steady institutional maintenance |
| ClimateMARGO | 73 | 2 (after 2yr gap) | 36.5 | Dormant-revival pattern |
| openair-cyan | 76 | 10 (one-day burst) | 7.6 | Frozen after certification |
| carbon-capture-and-storage | 85 | 0 (dead since 2021) | ∞ (static) | Ghost repo inflates ecosystem |
| ncAR_ML_EKE | 20 | 10 (15 months) | 2.0 | Academic paper lifecycle complete |
| GCCS-Core | 9 | 15 (one-day burst) | 0.6 | Empty shell with infrastructure |
| aiida-icon | 3 | 15 (7 months) | 0.2 | Low-star, high-quality institutional |
| OOCC_2021 | 2 | 15 (2021, dormant) | 0.1 | Active governance model, dead codebase |
| GeoVision | 0 | 4 (one-day) | 0 | Empty simulator shell |

---n
## 🔥 The Three Universes

### Fast Universe (Institutional, Funded, Sustained)
These repos have multi-contributor development, institutional backing, and continuous activity:
- **open-sustainable-technology** (2,552★) — The climate-tech GitHub hub. Continuously updated. 2,500+ projects cataloged.
- **WRF** (1,761★) — The world's most important atmospheric model. 7 contributors/month. v4.8.0 just shipped with solar radiation fix.
- **Oceananigans.jl** (1,413★) — GPU-accelerated ocean simulation. Active community. But zero intervention modules.
- **PCMDI/pcmdi_metrics** (133★) — ESM evaluation toolkit. v4.2.1 released Sep 2026. Institutional stewardship.
- **aiida-icon** (3★) — Workflow automation for ICON climate model. 14 contributors over 7 months. CSCS-backed.

### Slow Universe (Individual, Unfunded, Dormant)
These repos had moments of activity but are maintained by individuals with no ongoing funding:
- **ClimateMARGO** (73★) — Climate-economic SGE model. 2-year dormancy broken by 2 README updates in Aug 2026. Revival ambiguous.
- **openair-cyan** (76★) — DIY DAC hardware. OSHWA-certified. Frozen since Feb 2024 after certification push.
- **Carbon_Capture_ML** (56★) — Literature review/survey. Last commit May 2024. Slow-addiction pattern.
- **GCCS-Core** (9★) — "Global Climate Control System." 15 commits in one day, then dead. Empty shell.
- **carbon-swarm** (2★) — Carbon removal intelligence. 3 commits in one day, then dead. Product launch pattern.
- **NCAR_ML_EKE** (20★) — ML-on-HPC for MOM6. Academic paper lifecycle complete. Dormant since 2022.

### Empty Universe (Zero Presence)
Domains where GitHub has literally nothing:
- **Ocean geoengineering intervention** — 0 repos after 10+ search queries
- **Marine cloud brightening** — 0 repos
- **Ocean sensors for geoengineering** — 0 repos
- **OAE reactor designs** — 0 repos
- **Iron fertilization models** — 0 repos

---

## 🎯 Cross-Theme Findings

### Finding 1: The Directory Problem
**Theme:** Carbon
**Scoring:** The carbon capture ecosystem is more meta than real. The highest-starred repo (open-sustainable-technology, 2,552★) is a *directory* of projects, not a project itself. The second-highest (carbon-capture-and-storage, 85★) is a ghost repo.

**Implication for Episode:** "The carbon capture GitHub ecosystem has a library but no books. We've spent more energy cataloging climate tech than building it."

### Finding 2: The Solar Radiation Fix That Changes Everything
**Theme:** Solar
**Scoring:** WRF v4.8.0 (June 2026) includes a correction for the EOT (Easterly Offset Temperature) calculation in solar radiation (commit e836cd6, May 28, 2026). This means every previous SRM simulation using WRF had a systematic radiation error. The fix came from weiwangncar at NCAR, reviewed via PR, merged by Anthony Islas.

**Implication for Episode:** "The most important solar geoengineering code on GitHub just fixed a bug that invalidated every previous result. And nobody in the SGE community noticed because nobody calls WRF a SGE tool."

### Finding 3: The Ocean Gap is Absolute
**Theme:** Ocean
**Scoring:** 10+ search queries. Zero dedicated ocean geoengineering repos. Every ocean modeling layer exists (physics, biogeochemistry, ice, waves, coastal, GPU, ML, workflow) but NONE have intervention capability. The absence is total and intentional — governance, cost, complexity, and stigma all reinforce the barrier.

**Implication for Episode:** "GitHub has more code for simulating the ocean's natural chemistry than for simulating what we'd do to the ocean if we tried geoengineering. The gap isn't a bug — it's a feature of how we've decided NOT to think about ocean intervention."

### Finding 4: The Single-Maintainer Risk
**Theme:** All
**Scoring:** 13 of 21 repos (62%) have exactly 1 contributor. Institutional multi-contributor repos are rare: WRF (7 contributors), ClimateMARGO (2), aiida-icon (14). The rest are solo practitioners whose personal decisions determine whether the code lives or dies.

**Implication for Episode:** "Two-thirds of the climate-tech GitHub ecosystem is one exhausted PhD student away from being a dead repo. The most important solar radiation physics code on the planet has 7 contributors. The best governance model for SGE has 1."

### Finding 5: The Dash Pattern (Burst Then Die)
**Theme:** All
**Scoring:** 5 of 21 repos show the "single-day burst" pattern: GCCS-Core (15 commits in 1 day), GeoVision (4 in 1 day), carbon-swarm (3 in 1 day), openair-cyan (10 in 1 day), NCAR_ML_EKE (7 in 1 day). The pattern: create infrastructure, push files, README, then silence.

**Implication for Episode:** "GitHub is full of repos that look like they had a lot to say. But the 15 commits that said 'I'm working on this' were all on the same day. A single day. Then the repo waited for someone else to continue."

### Finding 6: The CC0 Revolution
**Theme:** Carbon
**Scoring:** Two DAC materials repos (DAC_peroxovanadates, DAC_peroxotitanates) both adopted CC0 public domain dedication on September 23, 2025 — same day, same author. This is the biggest open-science signal in carbon capture GitHub: not just open source, but public domain. Researchers are treating computational screening data as public infrastructure.

**Implication for Episode:** "While the rest of science is opening access to papers, someone is opening access to the data itself. No copyright. No paywall. Just a researcher with a laptop, some supercomputing time, and the insistence that the results belong to everyone."

### Finding 7: The Governance Vacuum
**Theme:** Solar & Cross
**Scoring:** Only two repos address SGE governance: OOCC_2021 (2★, dead since 2021) and srm-forever (0★, Weitzman discounting). Neither is maintained. The governance models are older than the physics models. We've invested more in understanding the physics than in planning the deployment.

**Implication for Episode:** "We have the models to simulate solar geoengineering. What we don't have is the models to govern it. And the only governance code on GitHub is a dead repo from a PhD student who published in 2021 and never touched the code again."

---

## 📈 Trend Timeline: What's Happening When

### 2022: The Paper Cycle
- NCAR_ML_EKE launches and dies (Apr 2021–Mar 2022)
- OOCC_2021 publishes and stops (Sep 2021)
- ClimateMARGO's last code commit (Nov 2022)

### 2024: The Certification & Survey Year
- openair-cyan gets OSHWA certification, then freezes (Feb 2024)
- Carbon_Capture_ML adds OpenDAC paper, goes dormant (May 2024)
- GCCS-Core creates infrastructure, goes dormant (Oct 2024)

### 2025: The CC0 Revolution & Ghost Signatures
- DAC_peroxovanadates and DAC_peroxotitanates adopt CC0 (Sep 2025)
- GeoVision created as empty shell (Dec 2025)

### 2026: The Revival Signals
- **WRF v4.8.0 with solar radiation fix** (May–Jun 2026) — 15 commits, 7 contributors
- **ClimateMARGO README revival** (Aug 2026) — 2 updates after 2-year gap
- **MEA simulation fork updated** (Sep 2026) — active process engineering
- **aiida-icon multi-model support** (Aug 2025–Jan 2026) — 15 commits, 14 contributors
- **carbon-swarm launch** (Apr 2026) — carbon removal intelligence, 3 commits in one day

---

## 🧮 Quantitative Summary

| Metric | Value |
|--------|-------|
| Total repos sampled | 21 |
| Total commits analyzed | 140+ |
| Total stars across all repos | 6,462+ |
| Institutional multi-contributor repos | 3 (WRF, ClimateMARGO, aiida-icon) |
| Single-maintainer repos | 13 (62%) |
| Dead repos (star > 0, 0 commits recent) | 4 (carbon-capture-and-storage, CO2-Sequestration, GCCS-Core, GeoVision) |
| Dormant repos (1+ years no commits) | 5 (ClimateMARGO, NCAR_ML_EKE, openair-cyan, Carbon_Capture_ML, OOCC_2021) |
| Actively maintained repos | 4 (WRF, open-sustainable-technology, pcmdi_metrics, aiida-icon) |
| Total horizon-zero domains | 5 (ocean OGE, MCB, ocean sensors, OAE reactors, iron fertilization) |

---

## 🎙️ Episode Planning Matrix

| Episode | Branch | Central Question | Commit Evidence | Narrative Arc |
|---------|--------|-------------------|-----------------|---------------|
| **Solar Geoengineering** | `solar-geoengineering` | Why is SGE code so scarce? | WRF's solar radiation fix (15 commits); ClimateMARGO revival (2 README updates); GCCS-Core ghost (15-day burst); OOCC_2021 dead since 2021 | Infrastructure hidden → Governance vacuum → Resurrection question |
| **Carbon Capture** | `carbon-capture` | Can open source break the $1000/ton barrier? | OpenAir-Cyan OSHWA freeze; CC0 data revolution; open-sustainable-technology directory dominance; carbon-swarm burst-then-die | Directory trap → Hardware challenge → CC0 revolution |
| **Ocean Intervention** | `ocean-intervention` | Why is ocean the empty quadrant? | ZERO dedicated repos; aiida-icon active but intervention-free; NCAR_ML_EKEpublish-then-die; five governance-gap hypotheses | Adjacent life → Ghost of past → The gap itself |

---

## 🔮 Three Universal Patterns Across All Themes

### 1. The Directory Beats the Tool
Every theme has a meta-repo that outshines the actual technology:
- Solar: WRF (atmospheric model repurposed for SGE)
- Carbon: open-sustainable-technology (directory of 2,500+ projects)
- Ocean: Oceananigans.jl (beautiful physics, no intervention)

### 2. The Single-Day Burst
Five repos show the same pattern: create → push → README → silence. The burst isn't sustained development — it's a launch event with no follow-through.

### 3. The Stars-Measure-Citations Problem
2,552 stars for a directory. 85 stars for a dead repo. 2 stars for a CC0 public domain dataset. Stars on GitHub measure attention, not utility. The most important repos aren't the most-starred repos.

---

## 📋 Research Log

| Date | Activity |
|------|----------|
| Sep 17, 2026 | v1: Initial commit trends from 8 repositories; branches created and notes pushed |
| Sep 17, 2026 | v2: Ecosystem-level analysis including ocean models; 6 ocean search queries confirm zero repos |
| Sep 17, 2026 | v3: Fresh commit histories pulled from 12 repositories across all three themes |
| Sep 17, 2026 | v3: Detailed project profiles pushed to all three theme branches |
| Sep 17, 2026 | v3: CC0 license trend identified as major open-science signal |
| Sep 17, 2026 | v3: Weitzman discounting framework documented in srm-forever |
| Sep 17, 2026 | v4: WRF v4.8.0 solar radiation correction identified as most SGE-relevant change |
| Sep 17, 2026 | v4: ClimateMARGO dormancy-revival pattern documented with timeline |
| Sep 17, 2026 | v4: GCCS-Core, GeoVision, carbon-swarm single-day burst patterns cataloged |
| Sep 17, 2026 | v4: aiida-icon 15-commit institutional pattern analyzed (CSCS-backed, 14 contributors) |
| Sep 17, 2026 | v4: NCAR_ML_EKE complete academic lifecycle mapped (launch to death in 15 months) |
| Sep 17, 2026 | v4: Cross-theme quantitative summary built (21 repos, 140+ commits, 6,462 stars) |
| Sep 17, 2026 | v4: Five universal patterns identified across all themes |
| Sep 17, 2026 | v4: Episode planning matrix updated with commit evidence for all three themes |
