# ☀️ Solar Geoengineering — Project Discovery Catalog

**Last Updated:** September 2026
**Research Method:** GitHub repository search ("geoengineering", "climate simulation", "solar radiation management", "SRM") + cross-reference with "awesome-geoengineering" curated list

---

## Tier 1: Major Projects (100+ Stars, Active Development)

### WRF — 1,761 Stars (NCAR/NOAA)
- **URL:** https://github.com/wrf-model/WRF
- **Language:** Fortran
- **Focus:** The Weather Research and Forecasting model — the foundational atmospheric model for all climate simulation
- **Latest:** v4.8.0 (Jun 2026) — active institutional release cycle
- **SRM Relevance:** TEMPO aerosol-aware physics modules; MYNN-EDMF ocean boundary layer physics; solar radiation EOT calculations
- **Why It Matters:** If you're going to simulate solar geoengineering, you need to simulate the atmosphere first. WRF is the tool. The aerosol microphysics development is the SRM pipeline.

### PCMDI Metrics — 133 Stars (LLNL)
- **URL:** https://github.com/PCMDI/pcmdi_metrics
- **Language:** Python
- **Focus:** Earth System Model evaluation toolkit — CMIP6 metrics, benchmarking, comparison
- **Latest:** v4.2.1 (Sep 2026) — 10-commit burst release
- **SRM Relevance:** The evaluation infrastructure. If SRM is deployed, we need tools to measure whether it worked. PCMDI is that infrastructure.
- **Why It Matters:** Governance requires measurement. PCMDI provides the yardsticks.

### MDTF-Diagnostics — 80 Stars (NOAA-GFDL)
- **URL:** https://github.com/NOAA-GFDL/MDTF-diagnostics
- **Language:** Jupyter Notebook
- **Focus:** Process-oriented diagnostics for weather and climate simulations
- **Latest:** Aug 2026 (active PR-based development)
- **SRM Relevance:** New MCS precipitation-buoyancy POD (Jun 2026) — directly relevant to marine cloud brightening evaluation
- **Why It Matters:** The closest thing to ocean-intervention evaluation tooling in open source.

---

## Tier 2: Emerging Projects (20-100 Stars)

### ClimateMARGO — 73 Stars
- **URL:** https://github.com/ClimateMARGO/ClimateMARGO.jl
- **Language:** Julia
- **Focus:** Idealized climate-economic modeling (Mitigation/Adaptation/Geoengineering trade-offs)
- **Latest:** Aug 2026 README updates after 2-year dormancy
- **Why It Matters:** The policy-modeling layer for SRM. The revival signal is worth watching.

### Open Sustainable Technology — 2,552 Stars
- **URL:** https://github.com/protontypes/open-sustainable-technology
- **Language:** Multi-language directory
- **Focus:** Comprehensive directory of 2,500+ open-source climate tech projects
- **Latest:** Sep 2026 (steady ecosystem growth)
- **Why It Matters:** The ecosystem infrastructure. This is the "github.com/awesome-climate-tech" that makes everything else discoverable.

### Awesome Geoengineering — 4 Stars
- **URL:** https://github.com/brandonhimpfen/awesome-geoengineering
- **Language:** Python (curated list)
- **Focus:** Curated list of geoengineering projects, research, organizations, tools
- **Latest:** Sep 2026
- **Why It Matters:** The gateway drug for this research. Good starting point for discovering the ecosystem.

---

## Tier 3: Niche / Dormant Projects (<20 Stars)

| Repo | Stars | Language | Focus | Status |
|------|-------|----------|-------|--------|
| srm-forever | 0 | HTML | Interactive SRM economics model | Single burst (Aug 2026) |
| Geo-DICE (PSLmodels) | 2 | MATLAB | Modified DICE with geoengineering | Dormant |
| ClimateLeonardo/GeoengineeringLE | 2 | Python | Economic modeling of geoengineering | Unknown |
| OOCC_2021 | 2 | Python | Simple SRM governance model | Dormant |
| AM3 (FMS-ESM) | 4 | Fortran | Atmospheric general circulation model | Dormant since 2015 |
| PMIP p2fvar analyzer | 4 | - | Paleoclimate model analyzer | Minimal activity |
| open-earth-digital-twin | 0 | TeX | Agent-based Earth system simulation | Manifesto stage, no code |

---

## The Discovery Gap: What's NOT on GitHub

| Missing Category | Why It's Missing |
|-----------------|------------------|
| End-to-end SRM simulation pipeline | Requires combining WRF + aerosol models + ocean models — no one has assembled this |
| SRM governance/regulatory tools | srm-forever exists but is a toy; serious governance code doesn't exist |
| SRM risk assessment tools | Arctic impacts, monsoon disruption — only represented in academic papers |
| Open-source CESM/SAM for SRM | CESM has SRM capabilities but they're not in a dedicated public repo |

---

## 🎙️ Episode Hooks

1. **The atmosphere is well-modeled, but SRM isn't.** WRF, PCMDI, MDTF are world-class — but nobody has strung them together into an SRM simulator.

2. **The governance tools are toys.** The only "SRM simulator" with a web interface (srm-forever) is a single-author teaching tool. The serious governance work happens in papers, not code.

3. **ClimateMARGO could be the sleeper.** A Julia-based climate-economic model, dormant for 2 years, suddenly showing README activity. The policy-modeling layer for SRM might be waking up.

4. **The discovery infrastructure is thriving.** Open Sustainable Technology (2,552★) and Awesome Geoengineering are making the ecosystem discoverable — which is the foundation everything else needs.
