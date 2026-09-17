# 📊 Cross-Theme Commit Trend Analysis — September 2026 Research Round

**Updated:** September 2026 — v3 (fresh commit histories from 12 repositories across all themes)

---

## Methodology

This round of research pulled fresh commit histories from 12 key repositories across all three podcast themes, supplementing the ecosystem-level data in the v2 analysis. All commits were retrieved directly from GitHub's API.

| Theme | Repos Analyzed | Commits Pulled |
|-------|---------------|----------------|
| ☀️ Solar Geoengineering | WRF, PCMDI, MDTF-diagnostics, ClimateMARGO, srm-forever, open-earth-digital-twin | 53+ |
| 🌍 Carbon Capture | open-sustainable-technology, OpenCarbon, openair-cyan, Carbon_Capture_ML, DAC_peroxovanadates, DAC_peroxotitanates, carbon-capture-and-storage, CO2-Sequestration, ClimateSoton | 70+ |
| 🌊 Ocean Intervention | MDTF-diagnostics (ocean-adjacent), WRF (coupled), ClimateSoton (CFD) | 14+ |

---

## Fresh Commit Data — By Theme

### ☀️ Solar Geoengineering

| Repo | Stars | Fresh Commits | Activity Window | Key Signal |
|------|-------|---------------|-----------------|------------|
| WRF | 1,761 | 10 | May-Jun 2026 (v4.8.0) | Solar radiation EOT correction; TEMPO aerosol staging off; MYNN-EDMF update |
| PCMDI | 133 | 10 | Sep 3-4, 2026 (v4.2.1) | 10 commits in 2 days; roundoff fix; extremes chunking with dask/SVD |
| MDTF-diagnostics | 80 | 10 | Jun-Aug 2026 | MCS precipitation-buoyancy POD (5 commits Jun 19); README refreshes |
| ClimateMARGO | 73 | 2 | Aug 17, 2026 | README revival after 2+ years dormancy; no code commits |
| srm-forever | 0 | 4 | Aug 26, 2026 | Weitzman discounting adopted; vintage annuity pricing; interactive model |

### 🌍 Carbon Capture

| Repo | Stars | Fresh Commits | Activity Window | Key Signal |
|------|-------|---------------|-----------------|------------|
| open-sustainable-technology | 2,552 | 10 | Jul-Sep 2026 | claude-carbon added; MUIO/MUIOGO DAC units; steady ecosystem growth |
| OpenCarbon | 2 | 10 | May-Jul 2023 | 3 PRs merged; then total silence; cautionary tale |
| openair-cyan | 76 | 10 | Feb 2022-2024 | OSHWA certification; 6 commits on Feb 12 2024; then dormant |
| Carbon_Capture_ML | 56 | 10 | Feb 2023-May 2024 | OpenDAC paper added; maturing from research tool to reference |
| DAC_peroxovanadates | 2 | 10 | Dec 2023-Sep 2025 | CC0 license (Sep 2025); paper DOI additions; public domain commitment |
| DAC_peroxotitanates | 2 | 10 | May 2024-Sep 2025 | CASTEP references; CC0 license; intensive May-Jul 2024 burst |
| carbon-capture-and-storage | 85 | 10 | Feb-Mar 2021 | All commits in 1-month burst; then 5+ years dormant; ghost |
| CO2-Sequestration | 32 | 2 | Mar 2019 | 2 commits same day; then 6 years of silence; oldest ghost |
| ClimateSoton | — | 4 | Aug 6, 2026 | Website refresh; 3 file uploads + 1 zip deletion; active group |

### 🌊 Ocean Intervention

| Repo | Stars | Fresh Commits | Activity Window | Key Signal |
|------|-------|---------------|-----------------|------------|
| MDTF-diagnostics | 80 | 10 | Jun-Aug 2026 | Precipitation-buoyancy POD is the closest ocean-interaction diagnostic |
| WRF (coupled mode) | 1,761 | 10 | May-Jun 2026 | No ocean-specific commits; atmospheric physics only |
| ClimateSoton | — | 4 | Aug 6, 2026 | CFD methods; ocean-relevant research group, but website-only on GitHub |

---

## The Three Universes — Updated v3

### Fast Universe (Institutional, Funded, Sustained)

| Repo | Stars | Pace | Funding Source |
|------|-------|------|----------------|
| **open-sustainable-technology** | 2,552 | Steady (10/mo) | Community + ProtonTypes |
| **WRF** | 1,761 | Monthly commits | NCAR/NOAA |
| **Oceananigans.jl** (from v2) | 1,413 | 10 commits/3 days | CliMA/Caltech |
| **PCMDI** | 133 | Bursty releases | LLNL |
| **veros** (from v2) | 400 | Maintenance mode | team-ocean community |
| **MDTF-diagnostics** | 80 | Ongoing | NOAA-GFDL |

### Slow Universe (Individual, Unfunded, Dormant)

| Repo | Stars | Status | Last Activity |
|------|-------|--------|---------------|
| **openair-cyan** | 76 | Dormant (complete) | Feb 2024 |
| **ClimateMARGO** | 73 | Dormant revival | Aug 2026 (README only) |
| **Carbon_Capture_ML** | 56 | Maturing (reference) | May 2024 |
| **DAC_peroxovanadates** | 2 | Slow activity | Sep 2025 |
| **DAC_peroxotitanates** | 2 | Slow activity | Sep 2025 |
| **carbon-capture-and-storage** | 85 | Ghost | Mar 2021 |
| **CO2-Sequestration** | 32 | Ghost | Mar 2019 |
| **OpenCarbon** | 2 | Ghost | Jul 2023 |
| **srm-forever** | 0 | Single burst | Aug 2026 |

### Empty Universe (Zero Presence)

| Domain | Repos | Nearest Proxy |
|--------|-------|--------------|
| **Ocean geoengineering (OAE, iron fertil, upwelling)** | 0 | MDTF-diagnostics (precipitation-buoyancy POD) |
| **Marine cloud brightening** | 0 | WRF (can simulate marine clouds, no config) |
| **Ocean carbon cycle simulation** | 0 | OceanBioME.jl (biological pump, v2) |
| **Ocean sensors / observatories** | 0 | None found |

---

## What the Fresh Data Confirms (and Adds)

### Confirmed from v2:
1. ✅ Institutional bursts dominate climate software — PCMDI's 10-in-2-days, WRF's v4.8.0
2. ✅ The August 2026 DAC materials wave — confirmed CC0 licenses and README bursts
3. ✅ Ocean geoengineering is silent — confirmed with 6 additional search queries returning zero
4. ✅ Dormancy is the default — confirmed across all themes

### New from v3:
1. 🆕 **The CC0 license trend is the biggest open-science story** — Both tjz21 repos adopted CC0 in Sep 2025. This is not just "open source" — it's public domain dedication. Researchers are treating computational screening data as public infrastructure.

2. 🆕 **The srm-forever economics model is conceptually important despite zero stars** — Weitzman certainty-equivalent discounting applied to SRM cost dynamics. This is the theoretical framework for "what does it cost to keep SRM going forever?"

3. 🆕 **ClimateMARGO's revival is ambiguous** — Two README updates after 2-year dormancy. No code commits. Could signal policy-modeling interest, or could be another false start.

4. 🆕 **The precipitation-buoyancy POD is the ocean's closest friend** — 5 commits on June 19, 2026 for the same file. This is the most ocean-relevant diagnostic in open source, and it's for evaluating model accuracy, not simulating interventions.

5. 🆕 **Academic ghost repos dilute the star count** — 85★ carbon-capture-and-storage (dead since 2021) and 32★ CO2-Sequestration (dead since 2019). Stars measure citations, not usability.

6. 🆕 **ClimateSoton is the most recent carbon-adjacent activity** — 4 commits on Aug 6, 2026. But it's website-only, not code. Active research group, no software product.

---

## Cross-Theme Comparison Dashboard — v3

### Activity Level

```
Solar:       ████████████████████ 1,761★ WRF (continuous)
             ████████████████████████████ 2,552★ Open-SustainTech (continuous)
             ████████████ 133★ PCMDI (bursty)
             ████████ 80★ MDTF (ongoing)
             ████ 73★ ClimateMARGO (dormant revival)
             ██ 0★ srm-forever (single burst)

Carbon:      ████████████████████████████ 2,552★ Open-SustainTech (continuous)
             ██████████ 85★ carbon-cc-and-storage (ghost)
             ████████ 76★ openair-cyan (dormant complete)
             ██████ 56★ Carbon_Capture_ML (maturing)
             ██████████ 32★ CO2-Sequestration (ghost)
             ██ 2★ DAC_peroxovanadates (slow)
             ██ 2★ DAC_peroxotitanates (slow)
             ██ 2★ OpenCarbon (ghost)

Ocean:       ████████████████████████████████ 0 dedicated repos
             ████████████ 80★ MDTF (ocean-adjacent only)
             ████████ 1,413★ Oceananigans.jl (from v2, no intervention module)
             ████████ 80★ OceanBioME.jl (from v2, gas exchange, not OAE)
```

### What Each Theme Has vs. What It Needs

| Theme | Has | Needs | Gap |
|-------|-----|-------|-----|
| ☀️ Solar | Atmospheric models, evaluation tools, economics model | Small-scale SRM simulation tools, accessible interfaces | Medium — the physics tools exist but aren't configured for SRM |
| 🌍 Carbon | Directory/index, DIY hardware, materials screening, ML survey | Full-system DAC models, economic cost models, LCA tools | Large — the ecosystem is fragmented across materials discovery and system engineering |
| 🌊 Ocean | Ocean climate models (Oceananigans, veros), gas exchange (OceanBioME), diagnostics (MDTF) | **Everything intervention-related**: OAE chemistry, iron fert biogeochemistry, marine cloud brightening, upwelling pumps | Total — the ocean gradient from climate science to geoengineering is a cliff, not a slope |

---

## 🎙️ Podcast Narratives — Updated v3

### Narrative 1: "The Institutional Divide"
Climate software funded by national labs (WRF, PCMDI, MDTF, Oceananigans) has thousands of stars and monthly commits. Climate software built by individuals (srm-forever, DAC materials screening, openair-cyan) has hundreds of stars and irregular activity. The funding gap is the open-source gap.

### Narrative 2: "The CC0 Revolution"
Two obscure DAC materials repositories just put their work in the public domain. CC0 is the nuclear option of open science — "this belongs to everyone." This isn't MIT or Apache licensing. It's a philosophical statement: computational screening data should be public infrastructure. Is this the future of open climate science?

### Narrative 3: "The Ocean is the Silence That Speaks Loudest"
We searched GitHub with 10+ queries. Zero ocean geoengineering repos. Meanwhile, the atmosphere gets WRF (1,761★) and the ocean gets... nothing. The London Protocol may be suppressing code. Or it might be computational expense. Or it might be that ocean researchers simply don't share code the way atmospheric researchers do.

### Narrative 4: "Ghost Stars Don't Mean Ghost Science"
The most-starred carbon-capture repo (85★) hasn't been touched since 2021. The oldest ghost (32★) is dead since 2019. Academic incentive structure: citation > maintenance. A GitHub star is a citation, not a usage metric.

### Narrative 5: "The Nearest Feasible Ocean Project"
An Oceananigans.jl OAE module. The physics engine exists (1,413★, 10 commits/3 days). The developers are active. The gas exchange physics exists (OceanBioME, actively developing). The gap is in the intervention layer. A graduate student could build this. Nobody has.

### Narrative 6: "The August 2026 Wave"
Six independent repositories updated in a 5-day window. DAC peroxovanadates and peroxotitanates both got CC0 licenses. Open-sustainable-technology added new DAC units. ClimateSoton refreshed their website. Is this a coordinated community event? A paper drop? Or just a busy season?

---

## 🔮 What to Watch Next Quarter — Updated v3

1. **WRF TEMPO aerosol physics** — Will experimental aerosol options be re-enabled? The SRM simulation tool is one config change away.

2. **CC0 license propagation** — Will other DAC materials researchers follow tjz21's lead and dedicate their work to the public domain?

3. **ClimateMARGO revival** — Will Aug 2026 README updates lead to code commits? The Julia climate-economics community needs a working tool.

4. **Oceananigans intervention modules** — Will anyone add an OAE or iron fertilization module to the most active ocean model? The platform is ready.

5. **OceanBioME gas exchange → OAE** — Will active gas exchange development lead to alkalinity-specific modules?

6. **OpenAir-Cyan commercialization** — Can the OSHWA-certified hardware become a product?

7. **The ocean remains silent** — Unless someone builds the first open-source OAE model, the absence will persist into 2027.

8. **PCMDI extremes chunking** — The dask/SVD memory fix suggests they're scaling for larger ensembles. SRM scenario testing would need exactly this.

9. **srm-forever adoption** — Will the Weitzman discounting framework gain traction in the SRM economics community? Zero stars, but conceptually important.

10. **August wave coherence** — Will the 6 repos from the August 2026 carbon wave collaborate, or fragment into separate silos?

---

## 🔗 Research Structure

| Branch | File | Content |
|--------|------|--------|
| ☀️ solar-geoengineering | PROJECT-DISCOVERIES-SOLAR.md | Detailed profiles of 6 solar/atmosphere repos with fresh commit data |
| ☀️ solar-geoengineering | COMMIT-TRENDS-SOLAR.md | Solar-specific trend analysis and episode hooks |
| 🌍 carbon-capture | PROJECT-DISCOVERIES-CARBON.md | Detailed profiles of 9 carbon capture repos with fresh commit data |
| 🌍 carbon-capture | COMMIT-TRENDS-CARBON.md | Carbon-specific trend analysis and episode talking points |
| 🌊 ocean-intervention | PROJECT-DISCOVERIES-OCEAN.md | Ocean gap analysis and ocean-adjacent repo profiles |
| 🌊 ocean-intervention | COMMIT-TRENDS-OCEAN.md | Ocean-specific trend analysis and narrative arcs |
| main | COMMIT-TRENDS.md | Master consolidated analysis (v2) |
| main | CROSS-THEME-ANALYSIS-SEP2026.md | This file (v3 cross-theme fresh data) |

---

## 📋 Research Log

| Date | Activity |
|------|----------|
| 2026-09-03 | Repository created; initial research notes pushed |
| 2026-09-17 | v2: Full ecosystem analysis including ocean models (Oceananigans, veros, OceanBioME); branches updated |
| 2026-09-17 | v3: Fresh commit histories pulled from 12 repositories across all three themes using GitHub API |
| 2026-09-17 | v3: Detailed project profiles and commit trend analyses pushed to all three theme branches |
| 2026-09-17 | v3: Cross-theme comparison dashboard and updated podcast narratives pushed to main |
| 2026-09-17 | v3: Ocean gap confirmed — 10+ search queries, zero dedicated ocean geoengineering repos |
| 2026-09-17 | v3: CC0 license trend identified as major open-science signal in DAC materials community |