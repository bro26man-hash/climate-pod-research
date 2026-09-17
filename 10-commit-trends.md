# 📊 Solar Geoengineering — Commit Trend Deep-Dive

> **Branch:** `solar-geoengineering`  
> **Analysis Date:** 2026-09-16

---

## Summary Statement

> **The core narrative tension for solar geoengineering on GitHub is the gap between simulation ambition and open-source availability.** The most active climate simulation codebases (WRF) are maintained inside institutions, while open SRM-specific projects are either early-stage prototypes or single-author research tools that stall after release.

---

## Trend by Theme

### 1. Institutional Physics Models (WRF) — Active Maintenance
- **Pattern:** Version bumps, physics module fixes, aerosol physics toggles
- **Key Insight:** SRM-adjacent physics (aerosol-aware modules, solar radiation schemes) are being actively developed but inside closed/controlled codebases
- **Narrative Implication:** The code needed to answer SRM risks exists but is not publicly auditable

### 2. Climate-Economic Optimization (ClimateMARGO.jl) — Bursty Academic Activity
- **Pattern:** Long silences interrupted by refresh bursts (2022 → 2023 → Aug 2026)
- **Key Insight:** Julia is gaining traction for climate-economic optimization; the repo tracks the policy dimension of SRM deployment
- **Narrative Implication:** Open-source SRM research is moving up the stack — from physics to policy economics

### 3. Climate Data Operations (clisops) — Mature, Bot-Maintained
- **Pattern:** Exclusively dependency updates from CI bots
- **Key Insight:** The operations/post-processing layer for climate data is stable; the modeling layer is elsewhere
- **Narrative Implication:** Data plumbing is solved; scientific modeling is the open frontier

### 4. Hydrological Impact (Xanthos) — Silent Maintenance
- **Pattern:** Single burst of commits in 2023, then silence
- **Key Insight:** Global hydrology (the most sensitive SRM side-effect) has an open framework but no ongoing development
- **Narrative Implication:** Precipitation disruption from SRM is the ultimate under-researched open problem

### 5. Geoengineering Simulators (GeoVision) — Initial Push & Stall
- **Pattern:** All commits on one day, no follow-up
- **Key Insight:** Geoengineering-specific simulators appear as one-shot academic uploads without community building
- **Narrative Implication:** The open-source geoengineering simulator category has not yet found maintainers

---

## Cross-Repo Pattern: The SRM Open-Source Stack

| Layer | Open Source Status | Example Repos |
|-------|-------------------|---------------|
| **Radiation & aerosol physics** | ❌ Institutional only | WRF (closed), CAM (closed) |
| **Earth system modeling** | ⚠️ Early-stage open | LOD-Climate, Earth Digital Twin |
| **Climate-economic optimization** | ✅ Active open | ClimateMARGO.jl (73★) |
| **Hydrological impact** | ⚠️ Mature but silent | Xanthos (38★) |
| **Regional risk assessment** | ⚠️ Single-author | geomalaria, Arctic codes |
| **Governance modeling** | ⚠️ Conceptual only | OOCC_2021 |

---

## 🎙️ Talking Points for the Episode

- "The most important physics for SRM — aerosol microphysics, stratospheric chemistry, precipitation response — lives in models you can't download."
- "ClimateMARGO.jl shows that the policy layer can be open even when the physics layer isn't."
- "GeoVision's one-day push and stall is the cautionary tale: open-source needs maintainers, not just uploaders."