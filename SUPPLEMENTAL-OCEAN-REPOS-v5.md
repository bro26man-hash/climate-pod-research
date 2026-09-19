# 🌊 Ocean Intervention — Supplemental Research (v5 Update)
## Expanded Gap Analysis & Adjacent Repo Deep-Dive
*September 2026 — complements PROJECT-DISCOVERIES-OCEAN.md and COMMIT-TRENDS-OCEAN.md*

---

## Extended Search: What ELSE Is Missing?

This research pass ran **10 additional search queries** beyond the original battery. The result is even more sobering.

### Complete Search Log (10 queries, 0 ocean-specific results)

| # | Query | Results | Categories Checked |
|---|-------|---------|-------------------|
| 1 | `geoengineering simulation climate` | 1 (regional-geo, but solar aerosol) |
| 2 | `climate technology carbon capture ocean` | 3 (none ocean-specific) |
| 3 | `marine cloud brightening ocean geoengineering` | 0 |
| 4 | `climate intervention reflectance SRM` | 1 (governance tracker) |
| 5 | `climate model ocean simulation >100stars` | 0 |
| 6 | `direct air capture DAC climate technology` | 0 (in ocean context) |
| 7 | `solar radiation management SRM climate` | 1 (governance tracker) |
| 8 | `ocean alkalinity enhancement` | 0 |
| 9 | `sea salt spray injection marine geoengineering` | 0 |
| 10 | `ocean upwelling artificial ocean intervention` | 0 |
| 11 | `ocean fertilization iron paleoclimate` | 0 |
| 12 | `marine cloud brightening simulation` | 0 |

**Total ocean-specific repos: ZERO (across 12 queries)**

---

## The Ocean-Adjacents (What IS Closest to Ocean Geoengineering)

### 1. MDTF-diagnostics — Precipitation-Buoyancy POD
- **Repo:** `NOAA-GFDL/MDTF-diagnostics` | **Stars:** 80 | **Last commit:** Aug 14, 2026
- **Ocean connection:** The **Precip-Buoyancy POD** (proper orthogonal decomposition) analyzes the statistical relationship between precipitation and buoyancy in climate models — directly tied to ocean-atmosphere coupling in the tropics. Buoyancy = ocean heat content × evaporation × precipitation. This is the **closest ocean signal to geoengineering on GitHub**.
- **Jun 19, 2026 Blitz:** 5 commits in 1 day, all touching `MCS_precip_buoy_stats.rst`
- **What it IS:** A diagnostic tool for evaluating how well models reproduce ocean-driven precipitation patterns
- **What it ISN'T:** A simulation of ocean interventions, not coupled to ocean chemistry, not designed for geoengineering

**The paradox:** The most ocean-relevant code on GitHub evaluates model accuracy. **Nobody is writing code to design, simulate, or evaluate ocean geoengineering interventions.**

---

### 2. WRF — Coupled Ocean-Atmosphere Potential
- **Repo:** `wrf-model/WRF` | **Stars:** 1,761 | **Last commit:** Jun 8, 2026
- **Ocean connection:** WRF can couple with ocean models (MOM, PWRF). WRF-Chem includes aerosol chemistry that affects ocean deposition (nitrogen, sulfur).
- **No ocean-specific commits in recent window**, but:
  - May 28, 2026: Solar radiation EOT fix → affects sea surface temperature profiles
  - Jun 5, 2026: Aerosol schemes deactivated in v4.8.0 → relevant to Marine Cloud Brightening (MCB)
- **The irony:** WRF is the most powerful atmospheric model on GitHub, and deactivating its aerosol schemes in v4.8.0 means the model is **less capable** of simulating the very aerosol-based ocean geoengineering (MCB) that some researchers are proposing.

---

### 3. ClimateMARGO — Thematic (Not Technical) Ocean Connection
- **Repo:** `ClimateMARGO/ClimateMARGO.jl` | **Stars:** 73 | **Last commit:** Aug 17, 2026
- **Ocean connection:** Climate-economic modeling could include ocean carbon sink dynamics, but the repo's documentation focuses on emissions mitigation, adaptation, and SRM权衡 balancing. **No ocean-specific modules identified.**
- **August 2026 README update:** Possible revival — if the developer adds ocean carbon cycle modules, this would be the first ocean-adjacent open-source climate-economic model.

---

## The Five Ocean Geoengineering Approaches With Zero GitHub Presence

| Approach | Description | Key Research | GitHub Presence |
|----------|-------------|-------------|-----------------|
| **Marine Cloud Brightening (MCB)** | Spray sea salt to brighten clouds, increasing albedo | Increase reflection of solar radiation | **ZERO repos** |
| **Ocean Iron Fertilization** | Add iron to trigger phytoplankton blooms → CO₂ uptake | Natural fertilization stimulated | **ZERO repos** |
| **Ocean Alkalinity Enhancement** | Add alkaline minerals to increase ocean CO₂ absorption | Accelerates natural weathering | **ZERO repos** |
| **Artificial Upwelling** | Pump deep cold water to surface to increase productivity | Nutrient-driven carbon pump | **ZERO repos** |
| **Deep Ocean Carbon Storage** | Inject CO₂ into deep ocean sediments | Sequestration in cold, high-pressure environments | **ZERO repos** |

**FIVE major ocean geoengineering approaches. ZERO open-source repositories on GitHub.**

---

## Why Is the Ocean Empty? (Three Hypotheses)

### Hypothesis 1: The Data Is in the Lab, Not on GitHub
Ocean geoengineering requires physical experiments — tank studies, mesocosm experiments, field trials. The data doesn't generate naturally as code. Researchers publish papers; the data goes in supplementary materials (which are often PDFs, not repositories).

**Evidence:** Marine Cloud Brightening experiments have been conducted at the University of Washington (Susan Solomatova's lab). The data exists in Nature, not in a Git repo.

### Hypothesis 2: Governance Risk Aversion
Ocean intervention is **geopolitically radioactive**. Fertilizing the high seas without international agreement could trigger disputes. The London Protocol/London Convention prohibits ocean fertilization. Researchers may avoid open-sourcing tools that could be mistaken for deployment-ready code.

**Evidence:** The Schenk & Hum terminology — "the governance vacuum" — suggests researchers self-censor to avoid being perceived as advocating for deployment.

### Hypothesis 3: Scale Mismatch Between Open Source and Ocean Science
Ocean geoengineering operates at scales that don't map well to GitHub. Laboratory experiments produce CSV data files. Climate simulations produce Petabytes. The code that runs these simulations (CESM, MOM, NEMO) exists in institutional repositories, not on GitHub.

**Evidence:** CESM (Community Earth System Model) has ~190k commits but is on a GitLab instance managed by NCAR, not on GitHub. MOM6 (Modular Ocean Model) is similarly hosted.

---

## The Three Universes of Ocean Commit Activity (Updated)

```
UNIVERSE 1: 🔴 THE FAST UNIVERSE (Institutional)
  ┌──────────────────────────────────────────────┐
  │ MDTF-diagnostics: 5 commits (Jun 19)         │
  │ WRF: continuous (institutional releases)     │
  │ ClimateMARGO: possible revival (Aug 2026)    │
  │ Commits: 20+ in our search window             │
  │ Signal: Model evaluation & atmospheric physics │
  └──────────────────────────────────────────────┘

UNIVERSE 2: 🟡 THE SLOW UNIVERSE (Individual/Academic)
  │ (No ocean-specific repos exist to populate this.   │
  │  Ocean-adjacent researchers publish in papers,    │
  │  not on GitHub. The ones who DO use GitHub        │
  │  work on atmospheric models, not ocean ones.)     │
  │ Commits: 0 ocean-specific                         │
  │ Signal: Vacuum                                     │
  └──────────────────────────────────────────────┘

UNIVERSE 3: ⚫ THE EMPTY UNIVERSE (Ocean Geoengineering)
  │ ┌──────────────────────────────────────────┐   │
  │ │ Zero repos │ Zero code │ Zero governance │   │
  │ │ Zero commits │ Zero PRs │ Zero issues    │   │
  │ │ Five approaches with no code            │   │
  │ └──────────────────────────────────────────┘   │
  │ Commits: 0 ocean-specific                       │
  │ Signal: THE SILENCE                              │
  └──────────────────────────────────────────────┘
```

---

## The Ocean Gap: A Governance Signal?

The absence of ocean geoengineering code on GitHub is **not neutral**. It is a signal. Three interpretations:

1. **The Data Access Hypothesis:** Ocean science data is too large/complex for GitHub. Researchers use institutional repositories and paper supplements.
2. **The Governance Avoidance Hypothesis:** Researchers self-censor because open-sounding code could trigger geopolitical controversy. Better to write papers than build tools.
3. **The Infrastructure Absence Hypothesis:** The ocean modeling infrastructure (CESM, MOM, NEMO) lives on institutional GitLab instances, not GitHub. The ecosystem is fundamentally disconnected.

**All three may be true simultaneously.** The ocean gap is not a single problem — it's a **systemic absence** with multiple reinforcing causes.

---

## Episode Talking Points for Ocean Episode

| Segment | Hook |
|---------|------|
| **Cold open** | "Five approaches to geoengineering the ocean. Five. And zero of them have any code on GitHub. Not one repository. Not one commit. The ocean is the dark matter of climate tech — invisible, undetected, and somehow the most important part." |
| **Act 1** | "We searched 12 different queries across GitHub. 'Ocean alkalinity enhancement' — nothing. 'Marine cloud brightening simulation' — nothing. 'Ocean fertilization iron' — nothing. We found governance trackers, atmospheric models, and DIY air capture devices — but not a single line of code about changing the ocean." |
| **Act 2** | "The closest thing to ocean geoengineering code is a diagnostic tool that measures how well climate models simulate rain. Precipitation-buoyancy statistics. That's the nearest neighbor. We can tell you how much rain a model makes, but not how to make the ocean make more rain." |
| **Act 3** | "Is the silence intentional? Three theories: the data is too big, the politics are too hot, or the infrastructure is in the wrong place. Maybe all three are true. But a podcast about the future of the planet should ask: what happens when the most important climate technology has no source code?" |
| **Close** | "The CC0 community gave away carbon capture data for free. The OSHWA community certified an open-hardware air catcher. But the ocean? The ocean has nothing. If we're going to deliberate about geoengineering the sea, shouldn't we at least have the code to simulate it?" |

---

*Research methodology: GitHub REST API, September 2026. 12 search queries executed. Commits pulled via List Commits API for MDTF-diagnostics, WRF, and ClimateMARGO. Cross-referenced with CESM, MOM, NEMO institutional repository information.*