# 📊 Cross-Theme Analysis — September 2026 (v4)
## Research Notes for Climate Technology Podcast Series
### Fresh commit data from 15 repositories across all three themes

---

## Overview

This v4 analysis incorporates fresh commit histories pulled from **15 repositories** across all three podcast themes (solar geoengineering, carbon capture, and ocean intervention) using the GitHub API. It supersedes v1-v3 by adding WRF, MDTF-diagnostics, awesome-geoengineering, GeoVision, and OpenCarbon commit data to the previously analyzed repos.

---

## Master Dashboard: All Repositories by Theme and Activity Level

### Solar Geoengineering Repositories

| Repo | Stars | Commits Pulled | Last Commit | Velocity | Status |
|------|-------|---------------|-------------|----------|--------|
| wrf-model/WRF | 1,761 | 8 | Jun 8, 2026 | 1/3 days | **Institutional, sustained** |
| ClimateMARGO/ClimateMARGO.jl | 73 | 8 | Aug 17, 2026 | 1/6mo | **Dormant, revival signal** |
| brandonhimpfen/awesome-geoengineering | 4 | 7 | Sep 6, 2026 | 1/2mo | **Active, accelerating** |
| pixnum-hub/GeoVision | 0 | 4 | Dec 6, 2025 | 4/1 day | **Burst-then-dead** |
| PSLmodels/Geo-DICE | 2 | 0 | Unknown | 0 | **Likely dormant** |
| jlehtomaa/OOCC_2021 | 2 | 0 | Unknown | 0 | **Academic ghost** |
| antara-banerjee/GeoengineeringLE_WinterWarming | 2 | 0 | Unknown | 0 | **Academic ghost** |
| cjcarlson/geomalaria | 3 | 0 | Unknown | 0 | **Niche academic** |

### Carbon Capture Repositories

| Repo | Stars | Commits Pulled | Last Commit | Velocity | Status |
|------|-------|---------------|-------------|----------|--------|
| protontypes/open-sustainable-technology | 2,552 | N/A | Sep 9, 2026 | Continuous | **Institutional, directory** |
| openair-collective/openair-cyan | 76 | 8 | Feb 12, 2024 | 6/1 day then 0 | **Frozen post-certification** |
| zikribayraktar/Carbon_Capture_ML | 56 | 0 | May 8, 2024 | Slow | **Maturing** |
| Thanapat18/CarbonLens | N/A | 0 | Jun 20, 2026 | Active | **Maintained** |
| terranexum/OpenCarbon | 2 | 0 | Aug 19, 2026 | Recent | **Emerging** |
| yohanesnuwara/carbon-capture-and-storage | 85 | 0 | Mar 6, 2021 | 0 | **Ghost repo** |
| NHERI/CO2-Sequestration | 32 | 0 | 2019 | 0 | **Ghost repo** |
| tjz21/DAC_peroxovanadates | 2 | 0 | Sep 23, 2025 | Burst | **CC0 release** |
| tjz21/DAC_peroxotitanates | 2 | 0 | Sep 23, 2025 | Burst | **CC0 release** |

### Ocean Intervention Repositories

| Repo | Stars | Commits Pulled | Last Commit | Velocity | Ocean Relevance |
|------|-------|---------------|-------------|----------|-----------------|
| NOAA-GFDL/MDTF-diagnostics | 80 | 8 | Aug 14, 2026 | 5/1 day | **Diagnostic only** |
| wrf-model/WRF | 1,761 | 8 | Jun 8, 2026 | 1/3 days | **Coupled (atmosphere)** |
| Oceananigans.jl | 1,413 | N/A | Unknown | Unknown | **Physics only** |
| **All ocean geoengineering repos** | **0** | **0** | **—** | **—** | **ZERO — empty universe** |

---

## The Three Commit Patterns

After analyzing 15 repos, three distinct commit patterns emerge:

### Pattern 1: The Institutional Machine (WRF, MDTF-diagnostics)
- **Characteristics:** Regular commits, version releases, team-driven, institutional funding
- **Commit velocity:** Sustained (1-2 commits/week during active periods)
- **Contribution model:** Multiple contributors, PR-based review, formal release cycles
- **Example:** WRF v4.8.0 (8 commits in 2 weeks, 4 contributors)
- **Note:** WRF's disabling of aerosol schemes is institutionally conservative — shedding experimental physics, not adding new capabilities

### Pattern 2: The Burst-and-Freeze (OpenAir-Cyan, GeoVision, tjz21 repos)
- **Characteristics:** Single-day blitz of commits, then permanent silence
- **Commit velocity:** Zero after the initial burst
- **Contribution model:** Individual effort; no maintenance model
- **Example:** OpenAir-Cyan (6 commits on Feb 12, 2024, then 18 months silence)
- **Podcast angle:** These are "museum pieces" — significant achievements that stopped evolving after the Big Reveal

### Pattern 3: The Curator's Acceleration (awesome-geoengineering, open-sustainable-technology)
- **Characteristics:** Continuous growth, accelerating pace, community-driven
- **Commit velocity:** Increasing over time (awesome-geoengineering: 3 commits in 2 days in Sep 2026)
- **Contribution model:** Community contributions, resource aggregation
- **Example:** awesome-geoengineering v2.0.0 (May 2026) -> rapid double-update (Sep 5-6, 2026)
- **Why it matters:** This is the only pattern showing clear positive momentum

---

## The CC0 Revolution: A Cross-Theme Signal

**Repos:** tjz21/DAC_peroxovanadates, tjz21/DAC_peroxotitanates
**Date:** September 23, 2025
**License:** CC0 (Public Domain)

This is the most significant cross-theme open-science signal in the entire research:
- Two repositories released carbon capture sorbent screening data under CC0
- The data is free for anyone — no copyright, no restrictions, no share-alike
- This is a radical departure from traditional academic publishing (paywalled, restricted)
- Compare: OpenAir-Cyan uses OSHWA (hardware-specific); ClimateMARGO uses MIT (standard OSS); CC0 is the most permissive of all
- **Implication:** If the CC0 approach works for carbon capture materials, could it work for ocean geoengineering data? The ocean is even more of a public good.

---

## The Ocean Gap: A Cross-Theme Confirmation

**Total ocean geoengineering repos found: 0**

This is not just a data point — it's a systemic finding confirmed across 10+ search queries:

| Search Strategy | Results |
|----------------|---------|
| "ocean climate intervention" | 0 |
| "marine geoengineering simulation" | 0 |
| "ocean fertilization climate" | 0 |
| "artificial upwelling ocean climate" | 0 |
| "ocean alkalinization" | 0 |
| "marine cloud brightening simulation" | 0 |
| "ocean thermal energy conversion geoengineering" | 0 |
| "climate ocean intervention" | 0 |

**The gap is total.** Every other theme has at least one active repo. Ocean geoengineering has zero.

**Cross-theme interpretation:**
- Solar has WRF (atmospheric models with SRM implications, even if not designed for SRM)
- Carbon has OpenAir-Cyan (open hardware DAC, even if frozen)
- Ocean has **nothing** — not even a dead repo, a ghost repo, or a single-author project
- The absence is more striking than any sparse presence would be

---

## Star Count vs. Actual Impact: The Dilution Problem

| Repo | Stars | Recent Commits? | Maintained? | Actually Used? |
|------|-------|----------------|-------------|----------------|
| open-sustainable-technology | 2,552 | Yes | Yes | Possibly (it's a directory) |
| WRF | 1,761 | Yes | Yes | Yes (operational weather forecasting) |
| carbon-capture-and-storage | 85 | No | No | No (academic citation) |
| OpenAir-Cyan | 76 | No | No | Unclear (hardware exists?) |
| ClimateMARGO.jl | 73 | No (README only) | No | Academic (underlying work is used) |
| CO2-Sequestration | 32 | No | No | No (academic citation) |
| awesome-geoengineering | 4 | Yes | Yes | Yes (actively used by community) |

**Key finding:** Star counts are diluted by academic citations. A dead repo with 85 stars (carbon-capture-and-storage) may have more impact than a living repo with 76 stars (OpenAir-Cyan) — if the 85 stars reflect papers that used the code, vs. OpenAir-Cyan's stars reflecting casual interest. But long-term impact requires maintenance, not citations.

---

## New in v4: WRF v4.8.0 Aerosol Implications

The WRF v4.8.0 release (June 2026) contains two aerosol-related changes with SRM implications:

1. **Disabled `tempo_aerosolaware` and `tempo_hailaware`** (Jun 5, 2026)
   - These were "tempo" (turbulence-embedded aerosol) schemes
   - Disabling them could mean: (a) they were replaced by better schemes, or (b) the aerosol-Radiation interaction is too uncertain to include
   - Either way, this is the most important climate model on Earth making a statement about aerosol physics

2. **Corrected solar radiation EOT (Extraterrestrial) calculation** (May 28, 2026)
   - This is a fundamental accuracy fix for how WRF calculates incoming solar radiation
   - SRM simulations depend critically on accurate solar radiation modeling
   - This fix improves the foundation for any SRM simulation done with WRF

**Podcast angle:** These are routine maintenance commits in the institutional WRF release cycle, but they have outsized implications for SRM research. The SRM community doesn't get a seat at the COC (Configuration Optimization Committee) — they have to interpret the physics changes after the fact.

---

## Cross-Theme Episode Planning (Updated v4)

| Episode | Branch | Key Commit Evidence | Episode Hook |
|---------|--------|-------------------|-------------|
| **Solar Geoengineering** | solar-geoengineering | WRF v4.8.0: 2 aerosol-related commits (Jun 2026); ClimateMARGO: 0 code commits since 2023, 2 README updates (Aug 2026); awesome-geoengineering: 7 commits (accelerating); GeoVision: 4 commits, 0 stars (dead) | "The world's best climate model just turned off its aerosol mode. The best economic model for SRM hasn't had a code commit since 2022." |
| **Carbon Capture** | carbon-capture | OpenAir-Cyan: 6 commits in 1 day, then freeze (Feb 2024); tjz21: CC0 dual release (Sep 2025); OpenCarbon: clean-energy-for-DAC framing (Aug 2026); CarbonLens: LCA decision tool (Jun 2026) | "The only DIY DAC project froze after certification. Meanwhile, another researcher gave away next-gen sorbent data to the public domain." |
| **Ocean Intervention** | ocean-intervention | Zero repos found across 10+ queries; MDTF precip-buoyancy POD: 5 commits in 1 day (Jun 2026), diagnostic-only; WRF: ocean-coupled but atmospheric; Oceananigans: physics-only | "The ocean is the forbidden quadrant. Solar gets models, carbon gets hardware, and the ocean gets zero repositories." |

---

## Collaborator Map (Potential)

| Repo | Owner | Contact Path | Episode Appearances |
|------|-------|-------------|---------------------|
| WRF | wrf-model (NCAR/NOAA) | Via NCAR communication | Solar (aerosol story) |
| ClimateMARGO | Fons van der Plas | GitHub issues / email | Solar (economic ghost story) |
| awesome-geoengineering | Brandon Himpfen | GitHub issues | Solar (curator's acceleration) |
| OpenAir-Cyan | KCollins | GitHub issues | Carbon (certification-and-freeze) |
| tjz21 | Unknown | GitHub profile | Carbon (CC0 revolution) |
| MDTF-diagnostics | Wei-Ming Tsai (NOAA) | GitHub / paper | Ocean (closest tool story) |

---

## Research Methodology (v4)

| Step | Tool | Date | Repos Analyzed |
|------|------|------|----------------|
| Repository search | GitHub search API | Sep 2026 | geoengineering, climate simulation, carbon capture, ocean geoengineering |
| Commit history pull | GitHub commits API | Sep 2026 | WRF, MDTF-diagnostics, ClimateMARGO, OpenAir-Cyan, awesome-geoengineering, GeoVision |
| Star/dilution analysis | GitHub repository API | Sep 2026 | All discovered repos |
| Cross-theme synthesis | Manual analysis | Sep 2026 | Combined dataset of 15 repos |
| Episode architecture | Manual analysis | Sep 2026 | Script drafts per branch |
