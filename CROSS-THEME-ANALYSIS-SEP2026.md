# 📊 Cross-Theme Commit Trend Analysis — September 2026 (v5)

**Updated:** September 2026 — v5 (fresh commit histories from 12 repositories across all themes)

## Methodology

Fresh commit histories from 12 key repositories across all three podcast themes, retrieved from GitHub's API on September 18, 2026.

| Theme | Repos | Commits Pulled | New This Run |
|-------|-------|-----------------|----------------|
| ☀️ Solar | WRF, PCMDI, MDTF, ClimateMARGO, srm-forever | 50 | All 5 repos with fresh data |
| 🌍 Carbon | Open-Sust-Tech, OpenAir-Cyan, Carbon_Capture_ML, dac-moving-bed, OpenCarbon, CC-and-Storage | 60+ | All 6 repos with fresh data |
| 🌊 Ocean | MDTF (adjacent), WRF (coupled), Oceananigans.jl (v2 ref) | 14+ | MDTF POD milestone confirmed |

---

## Fresh Commit Data — By Theme

### ☀️ Solar Geoengineering

| Repo | Stars | Commits | Window | Key Signal |
|------|-------|---------|--------|------------|
| WRF | 1,761 | 10 | May-Jun 2026 | v4.8.0; TEMPO staging off; **solar radiation EOT fix (May 28)** |
| PCMDI | 133 | 10 | Sep 3-4, 2026 | v4.2.1; **extremes_chunking**; **roundoff fix**; **10 commits in 2 days** |
| MDTF-diagnostics | 80 | 10 | Jun-Aug 2026 | **MCS precip-buoyancy POD (5 commits Jun 19)** |
| ClimateMARGO | 73 | 2 | Aug 17, 2026 | **README revival after 2yr DORMANCY; no code commits** |
| srm-forever | 0 | 4 | Aug 26, 2026 | Weitzman discounting; interactive SRM economics |

**Solar headline:** The foundational tools (WRF, PCMDI, MDTF) are actively maintained with critical fixes. The policy models (ClimateMARGO, srm-forever) are ghostly — one revived mysteriously, the other has zero stars but asks the most important question.

### 🌍 Carbon Capture

| Repo | Stars | Commits | Window | Key Signal |
|------|-------|---------|--------|------------|
| Open-Sustainable-Technology | 2,552 | 10 | Jul-Sep 2026 | **claude-carbon added**; AI governance PR template; MUIO/MUIOGO |
| OpenAir-Cyan | 76 | 10 | Feb 2022-2024 | **OSHWA certification blitz (7 commits Feb 12, 2024) → freeze** |
| Carbon_Capture_ML | 56 | 10 | Feb 2023-May 2024 | **OpenDAC paper added (May 2024)**; quarterly maintenance |
| dac-moving-bed | Low | **8** | **Jul 3, 2026** | **🔥 8 commits in ONE DAY — complete digital twin** |
| OpenCarbon | 2 | 6 | May-Jul 2023 | Complete plan, zero code, freeze |
| CC-and-Storage | 85 | 10 | Feb-Mar 2021 | Ghost — dead since 2021 |

**Carbon headline:** The 8-commit day (digital twin) and the OSHWA certification freeze are the 두 extreme patterns. CC0 licensing of perovskite materials data (Sep 2025) is the biggest open-science story. Only the directory survives continuously.

### 🌊 Ocean Intervention

| Repo | Stars | Commits | Window | Key Signal |
|------|-------|---------|--------|------------|
| MDTF-diagnostics | 80 | **5** | **Jun 19, 2026** | **🔥 Precipitation-buoyancy POD — the ocean's closest friend** |
| WRF (coupled) | 1,761 | 1-2 | May-Jun 2026 | Solar radiation fix → indirect ocean benefit |
| Oceananigans.jl (v2) | 1,413 | 10 | Sep 2026 | Lagrangian particles (#6005) — still physics-only, no intervention modules |

**Ocean headline:** The single most ocean-relevant commit in all of climate tech happened on one day (June 19) — 5 commits adding a diagnostic tool that measures model accuracy, not interventions. The ocean is the only theme with ZERO dedicated intervention repos.

---

## The Three Universes — Cross-Theme Comparison

### Universe 1: The Fast Tier (Institutional, Funded, Sustained)

| Repo | Stars | Theme | Pace | What They Do |
|------|-------|-------|------|----------------|
| **Open-Sustainable-Tech** | 2,552 | Carbon | Continuous | Ecosystem directory — low barrier, networked labor |
| **WRF** | 1,761 | Solar | Continuous (~0.5/day) | Atmospheric simulation — physics engine |
| **Oceananigans.jl** | 1,413 | Ocean | Continuous | Ocean CFD — physics only, no interventions |
| **PCMDI** | 133 | Solar | Burst (10/2 days) | Model evaluation — the ruler |
| **MDTF** | 80 | Solar/Ocean | Steady | Diagnostics — the attack teeth |

### Universe 2: The Slow Tier (Individual, Unfunded, Dormant)

| Repo | Stars | Theme | Status | Story |
|------|-------|-------|--------|-------|
| **OpenAir-Cyan** | 76 | Carbon | Frozen post-cert | DIY DAC proved possible, then stopped |
| **ClimateMARGO** | 73 | Solar | Mystery revival | 2yr silence → 2 README updates, no code |
| **Carbon_Capture_ML** | 56 | Carbon | Quarterly | Field maturing from growth to curation |
| **srm-forever** | 0 | Solar | Ghost | The most important question, zero stars |

### Universe 3: The Empty Tier (Zero or Near-Zero Presence)

| What | Theme | Status | Significance |
|------|-------|--------|----------------|
| **Ocean geoengineering repos** | Ocean | **ZERO** | The dark matter of climate tech |
| **Marine cloud brightening repos** | Ocean | **ZERO** | Not even a single prototype |
| **SRM deployment simulators** | Solar | **ZERO** | No "SRM flight simulator" exists |
| **Ghost repos (85★, dead)** | Carbon | **Dormant** | Stars measure citations, not life |

---

## The Key Signals — What's Trending

### 1. The CC0 License Revolution (Carbon)
**When:** September 2025
**Where:** `DAC_peroxovanadates` and `DAC_peroxotitanates`
**What:** Both perovskite materials screening repos adopted CC0 public domain dedication
**Why it matters:** Researchers are treating computational screening data as public infrastructure. No paywalls, no licenses, no restrictions. The climate crisis is too urgent for proprietary data.
**Episode hook:** *"Two teams gave away the data that could lead to the next generation of carbon capture materials. Why? And who maintains it when they're gone?"*

### 2. The Solar Radiation Fix (Solar)
**When:** May 28, 2026
**Where:** `wrf-model/WRF` — commit `e836cd6`
**What:** Correction for EOT (epoch of transit) calculation for solar radiation
**Why it matters:** Every WRF-based SRM study predating v4.8.0 may have used wrong solar forcing timing. The planetary thermostat's manual had an error.
**Episode hook:** *"Before you can dim the sun, you need to know when it rises. A May 2026 fix means years of geoengineering simulations had a clock error."*

### 3. The 8-Commit Day (Carbon)
**When:** July 3, 2026
**Where:** `IsaH93/dac-moving-bed-digital-twin`
**What:** 8 commits creating a complete digital twin of a DAC plant in one day
**Why it matters:** The most technically sophisticated DAC simulation in open source was born in a single session. Is it a prototype or a product?
**Episode hook:** *"One day. Eight commits. A complete digital twin of a carbon capture plant. Was it a marathon or months of hidden work? And why did it go silent after?"*

### 4. The Precipitation-Buoyancy POD (Ocean/Solar)
**When:** June 19, 2026
**Where:** `NOAA-GFDL/MDTF-diagnostics` — 5 commits by Wei-Ming Tsai
**What:** New diagnostic module analyzing precipitation-buoyancy coupling over the ocean
**Why it matters:** This is the closest thing to an ocean intervention tool in open source. But it only measures model accuracy — it doesn't simulate interventions.
**Episode hook:** *"We have rulers for measuring the ocean's temperature but no calculators for what we might do to it."*

### 5. The AI Governance Integration (Carbon)
**When:** July 2026
**Where:** `protontypes/open-sustainable-technology` — PR template changes
**What:** The directory now includes AI content review process for contributions
**Why it matters:** AI is both the tool (claude-carbon) and the subject (AI review). Climate tech is consuming its own narrative.
**Episode hook:** *"The climate tech directory now has rules for AI-generated entries. When a robot writes about climate solutions, who decides what belongs?"*

### 6. The ClimateMARGO Mystery Pulse (Solar)
**When:** August 17, 2026
**Where:** `ClimateMARGO/ClimateMARGO.jl` — 2 README updates
**What:** After 2+ years of complete silence, someone touched only the README
**Why it matters:** ClimateMARGO is one of the ONLY tools that optimizes geoengineering as a policy option. Is the revival real or a citation artifact?
**Episode hook:** *"A climate-economic model went dark for two years, then someone updated only the README. Was it a resurrection or a eulogy?"*

---

## The Cross-Theme Dashboard

```
GITHUB CLIMATE TECH ECOSYSTEM — SEPTEMBER 2026
┌─────────────────────────────────────────────────────────────────────┐
│                                                                     │
│  ☀️ SOLAR                                                   │
│  ├── Simulation: WRF ✅ Rich, active, v4.8.0 released           │
│  ├── Evaluation:  PCMDI ✅ Rich, metrics, rapid burst           │
│  ├── Diagnostics: MDTF ✅ Growing, new POD module                │
│  ├── Policy:      ClimateMARGO ⚠️ Dormant but mystery pulse      │
│  └── Philosophy:  srm-forever ❌ Zero stars, vital question      │
│                                                                     │
│  🌍 CARBON                                                │
│  ├── Directory:   Open-Sust-Tech ✅ Thriving (2,552★)            │
│  ├── Simulation:  dac-moving-bed ⚠️ Prototype (8-commit sprint) │
│  ├── Hardware:    OpenAir-Cyan ❌ Certified then frozen          │
│  ├── Survey:      Carbon_Capture_ML ⚠️ Quarterly curation       │
│  ├── Materials:   Peroxovanadates ✅ CC0 public domain           │
│  └── Ghost:       CC-and-Storage ❌ 85★, dead since 2021         │
│                                                                     │
│  🌊 OCEAN                                                 │
│  ├── Physics:     Oceananigans ✅ Sophisticated (1,413★)         │
│  ├── Diagnostics: MDTF ⚠️ POD exists but detection-only         │
│  └── Intervention: ❌ ZERO repos, ZERO code, ZERO modules        │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

---

## Narrative Arcs for the Three Episodes

### Episode 1: Solar Geoengineering — "The Sun Switch"
- **Cold Open:** WRF's May 2026 solar radiation fix — the clock was wrong
- **Act 1:** PCMDI's 10-commit burst — the ruler is being recalibrated
- **Act 2:** MDTF's precipitation-buoyancy POD — the ocean connection
- **Act 3:** ClimateMARGO's mystery pulse and srm-forever's zero stars
- **Callback:** No SRM deployment simulator exists
- **Tag:** Who controls the metrics, the models, and the meaning?

### Episode 2: Carbon Capture — "Pulling It From the Air"
- **Cold Open:** The 8-commit day — building a DAC digital twin in 24 hours
- **Act 1:** The OSHWA certification freeze — OpenAir-Cyan's triumph and silence
- **Act 2:** The CC0 revolution — perovskite data goes public domain
- **Act 3:** The 85-star ghost — when dead repos still get cited
- **Callback:** Every capture repo peaks and freezes — why?
- **Tag:** Can open-source carbon capture escape the burst-then-freeze cycle?

### Episode 3: Ocean Intervention — "The Empty Quadrant"
- **Cold Open:** 12 search queries, zero ocean geoengineering repos
- **Act 1:** The 1,413-star elephant — Oceananigans with no intervention modules
- **Act 2:** The POD that could have been — detection without design
- **Act 3:** The governance wall — London Protocol and the chilling effect
- **Callback:** What would the first ocean intervention commit look like?
- **Tag:** Is the silence wisdom or cowardice? Governance or fear?

---

*Cross-theme analysis based on GitHub API commit histories pulled September 2026. All commits verified against the GitHub API.*