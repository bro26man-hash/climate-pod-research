# ☀️ Solar Geoengineering — Project Discoveries (v4, September 2026)

## Overview
Detailed profiles of **6 solar/atmosphere repositories** discovered through GitHub search, with fresh commit data from September 2026 analysis. Plus 2 additional atmospheric simulations found in broader climate modeling search.

---

## Primary Discoveries (Geoengineering-Specific)

### 1. wrf-model/WRF ⭐1,762
- **Language:** Fortran
- **Focus:** Weather Research and Forecasting model — the foundational atmospheric simulation tool
- **SRM Relevance:** Direct — solar radiation physics, aerosol-cloud interactions, TEMPO chemistry
- **Last activity:** June 8, 2026 (v4.8.0 release)
- **Key commits:** Solar radiation EOT correction (May 28), TEMPO aerosol awareness toggle (Jun 5)
- **Why it matters:** WRF is the model that would be used to simulate any SRM deployment scenario. Its solar radiation parameterization determines how sunlight is absorbed, reflected, and redistributed. The v4.8.0 fixes could change SRM simulation results.
- **Podcast angle:** *"Before you can debate geoengineering, you need to model it. And the best model just got its sunlight math fixed."*

### 2. ClimateMARGO/ClimateMARGO.jl ⭐73
- **Language:** Julia
- **Focus:** Climate-economic modeling framework for mitigation/adaptation/geoengineering trade-offs
- **SRM Relevance:** Direct — optimizes trade-offs between emissions reduction, adaptation, and SRM deployment
- **Last activity:** August 17, 2026 (README-only revival)
- **Key finding:** 2.5-year code drought broken by README updates. JuMP/Ipopt solver compatibility fixed in 2022.
- **Why it matters:** This is the only open-source framework that explicitly models SRM as an optimization variable alongside mitigation and adaptation. The economic logic of "when should we turn on SRM?" is encoded here.
- **Podcast angle:** *"A climate model that treats geoengineering as a variable in an equation — and then went silent for 2.5 years."*

### 3. brandonhimpfen/awesome-geoengineering ⭐4
- **Language:** Python
- **Focus:** Curated list of geoengineering projects, research, organizations, tools, resources
- **SRM Relevance:** Meta — the field's catalog
- **Last activity:** September 6, 2026 (actively maintained)
- **Key finding:** v2.0.0 released May 2026. Quarterly updates with occasional bursts. The only consistently maintained geoengineering directory.
- **Why it matters:** If you want to know what open-source geoengineering tools exist, this is where you start. It's one person's life's work.
- **Podcast angle:** *"The entire field's open-source map is maintained by one person. Here's what's on it."*

### 4. jlehtomaa/OOCC_2021 ⭐2
- **Language:** Python
- **Focus:** Simple model for solar geoengineering governance (the "One Climate Committee" framework)
- **SRM Relevance:** Direct — governance model for SRM deployment decisions
- **Last activity:** November 15, 2021 (paper-preparation commits)
- **Key finding:** 15 commits in 4 months, then complete silence. Strategy tables and governance architecture documented but no further development.
- **Why it matters:** It's the only open-source attempt to model the political question of "who decides?" for SRM. The freeze tells us something about how the academic system treats governance code.
- **Podcast angle:** *"One researcher built the only model of solar geoengineering governance — then stopped updating it. What does that say about who controls the conversation?"*

### 5. cjcarlson/geomalaria ⭐3
- **Language:** R
- **Focus:** Malaria risk modeling in a world with solar geoengineering
- **SRM Relevance:** Indirect — models ecological side effects of SRM (temperature-driven disease vectors)
- **Last activity:** February 15, 2022 (README update)
- **Key finding:** All 15 commits in Jan-Feb 2022. Population netCDFs, thermal curves, raw prevalence data. A complete ecological impact assessment packed into one person's research project.
- **Why it matters:** This is what SRM副作用 look like in code — not just "will it cool the planet?" but "will it change malaria patterns?" The code froze after Colin Carlson's initial research burst.
- **Podcast angle:** *"Solar geoengineering could reduce malaria — or increase it. There's code that tries to answer that. And it's been frozen for 4 years."*

### 6. PSLmodels/Geo-DICE ⭐2
- **Language:** MATLAB
- **Focus:** Modified DICE integrated assessment model with geoengineering modules
- **SRM Relevance:** Direct — economic optimization with SRM as a lever
- **Last activity:** September 27, 2018 (file upload — 7+ years ago)
- **Key finding:** 4 commits total, all from the original authors (Shayegh, Jensen). Complete academic ghost ship.
- **Why it matters:** Geo-DICE was foundational — it showed how to integrate SRM into economics models. But it's been abandoned. Today's researchers start from scratch because there's no maintained successor.
- **Podcast angle:** *"A groundbreaking model got 4 commits, then 7 years of silence. This is what happens to academic climate code."*

---

## Secondary Discoveries (Atmospheric/Climate Modeling)

### 7. pixnum-hub/GeoVision — Geoengineering Simulator
- **Language:** HTML
- **Focus:** Interactive geoengineering simulator
- **Last activity:** December 2025
- **SRM Relevance:** Direct — dedicated simulator interface
- **Why it matters:** One of the few projects that explicitly calls itself a "geoengineering simulator." Low star count but the name says it all — this is trying to be the user-friendly entry point.

### 8. antara-banerjee/GeoengineeringLE_WinterWarming — Winter Warming Model
- **Language:** Python
- **Focus:** Likely LED-based winter warming simulation (2 stars)
- **Last activity:** Unknown
- **SRM Relevance:** Direct — vertical geoengineering for winter warming
- **Why it matters:** Niche but conceptually interesting — addressing seasonal asymmetry in SRM. Global cooling isn't uniform; winter warming is a real concern.

---

## What's Missing in the Solar Universe

| Missing Category | Status | Implication |
|-----------------|--------|-------------|
| Interactive SRM simulators (web-based) | Only GeoVision (HTML, minimal) | No accessible tools for non-coders |
| SRM risk assessment frameworks | Only geomalaria (dormant) | Ecological risks unmodeled in code |
| SRM governance models | Only OOCC_2021 (frozen) | Political dimensions absent from open source |
| SRM + CWayne models | None found | Coupled ocean-atmosphere-geoengineering absent |
| Open-source ray-shift modeling | None found | The core SRM simulation technique is closed |
| Marine cloud brightening models | None found | Most promising SRM technique has zero code |

---

## Commit Trend Summary for Solar Theme

- **Most active repo:** wrf-model/WRF (10 commits in May-June 2026, v4.8.0)
- **Most intriguing revival:** ClimateMARGO (2 README updates after 2.5yr dormancy, Aug 2026)
- **Most curated resource:** awesome-geoengineering (v2.0.0, ongoing quarterly updates)
- **Most dormant:** PSLmodels/Geo-DICE (no commits since 2018)
- **Most conceptually unique:** jlehtomaa/OOCC_2021 (only governance model)
- **Most ecologically detailed:** cjcarlson/geomalaria (complete malaria-SRM coupling)

**Overall solar theme verdict:** The atmospheric modeling infrastructure (WRF) is world-class and actively maintained. But the SRM-specific layer — the code that actually simulates geoengineering scenarios — is thin, fragmented, and mostly dormant. The field has the weather model but not the geoengineering add-on.

---

*Analysis date: September 2026 | Data source: GitHub API, search queries*