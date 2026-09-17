# ☀️ Solar Geoengineering — Project Discoveries

**Date:** September 2026
**Research Method:** GitHub repository search across 5 query strategies + targeted commit history analysis

---

## Top Repositories by Activity and Relevance

| Repo | Stars | Language | Last Active | Focus Area |
|------|-------|----------|-------------|------------|
| **wrf-model/WRF** | 1,761 | Fortran/C | Jun 2026 | Foundational atmospheric model (v4.8.0) — solar radiation physics |
| **PCMDI/pcmdi_metrics** | 133 | Python | Sep 2026 | ESM evaluation toolkit — CMIP6 metrics, v4.2.1 |
| **NOAA-GFDL/MDTF-diagnostics** | 80 | Jupyter/Python | Aug 2026 | Process-oriented diagnostics — precip-buoyancy POD (ocean-adjacent) |
| **ClimateMARGO/ClimateMARGO.jl** | 73 | Julia | Aug 2026 | Climate-economic modeling framework — SRM optimization |
| **brandonhimpfen/awesome-geoengineering** | 4 | Markdown | Sep 2026 | Curated geoengineering resource list — v2.0.0 |
| **yanpefnsc/orbital-climate-simulator** | 2 | Python | Sep 2026 | Interactive SRM drone fleet dashboard |
| **hausfath/srm-forever** | 0 | Python | Aug 2026 | Interactive single-page SRM economics model |

---

## Detailed Profiles

### 1. wrf-model/WRF — The Bedrock
- **Why it matters:** WRF is the most widely used regional atmospheric model in the world. Its solar radiation parameterization schemes are directly relevant to SRM simulation — any solar geoengineering scenario must be evaluated against realistic atmospheric dynamics.
- **Key commits (May–Jun 2026):** 15 commits leading to v4.8.0 release, including:
  - `e836cd6`: **Correction for eot calculation for solar radiation** — directly fixes SRM-relevant physics
  - `9c87d29`: New namelists for ShinHong PBL and revised MMM surface layer
  - `8299919`: MYNN-EDMF pointer update (boundary layer physics for aerosol effects)
  - `6a289e1`: Turned off tempo_aerosolaware and tempo_hailaware in Registry (aerosol-aware physics adjustments)
- **Episode angle:** "The model that simulates our atmosphere just fixed its solar radiation code. What does that mean for SRM simulations?"

### 2. PCMDI/pcmdi_metrics — The Evaluation Standard
- **Why it matters:** PCMDI metrics are how the climate community evaluates Earth System Models against observations. If SRM is ever deployed, we need metrics to evaluate its effects. This is governance infrastructure disguised as software.
- **Key commits (Sep 2–4, 2026):** 15 commits in 3 days for v4.2.1 release:
  - `6419050`: Bump version to 4.2.1
  - `90cbc50`: **Prevents roundoff to 1.00 in mean_climate figures** — precision fix for climate metrics
  - `ac634d7`: Rechunk data to higher order than rolling operation (performance for large ESM datasets)
  - `71a0497`: Extremes chunking merge — new capability for extreme event metrics
  - `83fbdda`: Add AIMIP page (Aquabotics/AI-model intercomparison project — SRM-relevant)
- **Episode angle:** "15 commits in 3 days: the quiet release that decides which climate models get trusted — and whether SRM can be evaluated."

### 3. ClimateMARGO/ClimateMARGO.jl — The Optimization Framework
- **Why it matters:** MARGO (Model for Optimizing Mitigation, Adaptation, and Geoengineering) is an idealized climate-economic model that explicitly includes geoengineering as a policy variable. It's the closest thing to an SRM policy simulator.
- **Key commits:**
  - `d916f36` & `6d9ba7a`: Two README updates on Aug 17, 2026 — **revival signal** after 2.5 years of dormancy (last code commit: Oct 2023)
  - `57d4da7`: Unit conversions fix (Oct 2023)
  - `12a0ce6`: JuMP and Ipopt compat upgrade (Nov 2022)
  - Earlier: Henri Drake's heavy development period (Jan–Feb 2022) — 9 commits in 2 weeks
- **Episode angle:** "ClimateMARGO slept for 2 years, then woke up with README updates. Is the geoengineering optimization community reawakening?"

### 4. yanpefnsc/orbital-climate-simulator — The Democratization Signal
- **Why it matters:** This is a NEW interactive SRM simulation — a drone fleet dashboard that models solar radiation management from space. Built in a single day (Sep 15–16, 2026), 12 commits in 24 hours.
- **Key commits (Sep 15–16, 2026):**
  - `d40da35`: feat: add interactive Streamlit dashboard
  - `2c5137c`: feat: integrate SQLite database for drone telemetry
  - `f6919f8`: feat: add matplotlib visualizer for drone positions and radiation decay
  - `7e1edf5`: feat: implement V1 base drone simulation logic
  - `db10508`: fix: update drone telemetry and simulation state
- **Episode angle:** "Someone built an SRM drone simulator in a day. Is this the 'democratization' wave, or is it too crude to matter?"

### 5. hausfath/srm-forever — The Economics Model
- **Why it matters:**纯Python interactive model comparing SRM-forever vs mitigation+CDR costs. Uses Weitzman certainty-equivalent discounting — a sophisticated economic framework.
- **Key commits (Aug 26, 2026):** 4 commits in one day:
  - `9999436`: Interactive SRM-forever vs mitigation+CDR cost model
  - `9ee822a`: Price abatement as a vintage annuity
  - `aa9bc0f`: Adopt Weitzman certainty-equivalent discounting; add discount-rate essay
  - `61df1a4`: Add effective discount rate chart
- **Episode angle:** "4 commits, one day, a complete SRM economics model. The 'srm-forever' thought experiment, now interactive."

### 6. brandonhimpfen/awesome-geoengineering — The Curation Layer
- **Why it matters:** Curated list of geoengineering resources — the most actively maintained non-institutional project in the solar geoengineering space.
- **Key commits:**
  - `8d0a800`: Update README (Sep 6, 2026) — most recent maintenance
  - `5926daf`: Update README (Sep 5, 2026)
  - `a6e8359`: Update to v2.0.0 (May 5, 2026)
  - Pattern: 2 updates in Sep 2026, then v2.0.0 in May, then regular monthly updates
- **Episode angle:** "The most active geoengineering project on GitHub is a curated list, not a simulation. What does that tell us?"

---

## Governance Tools Found

| Repo | Description | Status |
|------|-------------|--------|
| **PCMDI/pcmdi_metrics** | CMIP6 model evaluation metrics — de facto governance standard for climate model trust | ACTIVE (v4.2.1, Sep 2026) |
| **hausfath/srm-forever** | SRM economics — cost comparison model | ACTIVE (Aug 2026) |
| **ClimateMARGO/ClimateMARGO.jl** | Climate-economic optimization with geoengineering as variable | DORMANT (2.5 yr gap, revival signal) |
| **brandonhimpfen/awesome-geoengineering** | Curated resource list — governance through curation | ACTIVE (Sep 2026) |

-Only 3 governance-adjacent tools exist for solar geoengineering, and only one (PCMDI metrics) is actively maintained.

---

## Key Patterns for the Episode

1. **Institutional dominance:** The two most active repos (WRF, PCMDI) are institutional. Community-driven SRM tools are tiny or absent.
2. **The physics-python gap:** WRF is Fortran. PCMDI is Python. ClimateMARGO is Julia. There's no unified SRM simulation stack.
3. **Democratization is nascent but real:** orbital-climate-simulator and srm-forever are individuals building interactive tools. They're small but they exist.
4. **Dormancy is the norm:** ClimateMARGO slept for 2.5 years. Most repos have no meaningful activity in the last year.
5. **The governance gap:** Only 3 governance-adjacent tools for the entire solar geoengineering domain. Physics has outpaced policy infrastructure.

---

*Research conducted September 2026 for the Climate Technology & Geoengineering podcast series.*