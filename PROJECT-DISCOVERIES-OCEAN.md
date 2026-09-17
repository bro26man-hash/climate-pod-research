# Ocean Intervention — Project Discoveries (Updated Sep 2026)

**Branch:** ocean-intervention
**Research Date:** September 2026

---

## The Ocean Quadrant — Empty by Design

| Category | Expected Presence | Actual Presence |
|----------|-------------------|------------------|
| Ocean Alkalinity Enhancement (OAE) | Multiple repos; mineral weathering kits, sensor networks | Zero dedicated repos |
| Iron Fertilization | At least 1-2 legacy repos from 2000s experiments | Zero repos |
| Marine Cloud Brightening (MCB) | Cloud model integrations, spray mechanism designs | Zero repos |
| Artificial upwelling/downwelling | Pump designs, energy analysis | Zero repos |
| Seaweed/kelp farming for carbon | Growth models, LCA tools | Zero repos |
| Ocean acidification monitoring | pH sensor networks, data analysis | Zero ocean-specific repos |

### Only Ocean-Adjacent Project Found

| Repo | Stars | Last Commit | Description |
|------|-------|-------------|-------------|
| Team50-Labs/NebuGrid-OpenSource | 0 | Aug 20, 2026 | Fog-harvesting and drip irrigation for arid coastal environments. Not ocean geoengineering, but ocean-adjacent. |

---

## Cross-Theme Projects That Touch Ocean Topics

| Repo | Stars | Theme | Ocean Relevance |
|------|-------|-------|----------------|
| PCMDI/pcmdi_metrics | 133 | Solar | ENSO, sea ice, ocean heat content metrics — the closest thing to ocean simulation tooling |
| wrf-model/WRF | 1,761 | Solar | Ocean boundary layer physics, air-sea interaction modules |
| prashaant1926/open-earth-digital-twin-simulation | 0 | Solar | Agent-based Earth systems — could eventually model ocean interventions |

---

## What the Cross-Theme Commit Data Tells Us

### PCMDI's Ocean Activity (Sep 2026)
- 10 commits in 2 days for v4.2.1 release
- MCS precipitation-buoyancy POD added (Jun 2026) — ocean-relevant
- Evaluation infrastructure exists, but no intervention-design tools

### WRF's Ocean Physics (Jun 2026)
- v4.8.0 released — includes ocean boundary layer physics
- MYNN-EDMF updates affect air-sea coupling
- Climate model components exist, but aren't intervention tools

### Digital Twin Aspiration (Oct 2025)
- Single TeX commit — more manifesto than codebase
- Represents where the field wants to go

---

## Governance Context (Critical for Episode)

| Framework | Relevance |
|-----------|-----------|
| London Convention/Protocol | Directly regulates ocean fertilization; requires resolution of CBD parties |
| BBNJ Agreement | High seas biodiversity treaty — may affect protection zone designation |
| UN Ocean Decade | Provides a governance framework for ocean research — potential path for open-source coordination |
| SCOR | Scientific Committee on Oceanic Research — could host open ocean data |

---

## Designing an Open-Source Ocean Intervention Project

Based on patterns from the solar and carbon themes, a successful ocean open-source project needs:

1. **Sensor design sharing** — pH, pCO2, alkalinity sensors for monitoring experiments
2. **Data pipelines** — Open data formats for ocean carbonate chemistry measurements
3. **Modeling components** — Executable models of alkalinity enhancement, iron fertilization impacts
4. **Governance frameworks** — Interactive tools showing legal/regulatory landscape
5. **Community infrastructure** — Maintained repo with multiple contributors

**Nearest feasible starting point:** Open ocean monitoring sensor designs + data pipelines. The DIY hardware equivalent for ocean science.

---

## Research Gaps Identified

| Gap | Severity | Opportunity |
|-----|----------|-------------|
| No OAE sensor designs on GitHub | HIGH | Build open-source alkalinity monitoring kit |
| No iron fertilization data repositories | HIGH | Create standardized data format for enrichment experiments |
| No ocean intervention modeling tools | CRITICAL | Port WRF ocean modules to accessible, configurable tool |
| No governance/regulatory transparency tools | MEDIUM | Interactive tool showing London Protocol, BBNJ requirements |
| No ocean-carbon cycling models | MEDIUM | Simple carbonate chemistry calculator (like srm-forever for SRM) |

---

## Cross-References

- Solar Geoengineering branch: SRM simulation gap mirrors ocean gap (no SRM-specific code exists either)
- Carbon branch: OpenAir-Cyan proves DIY hardware can work — the model for ocean sensors
- Main: COMMIT-TRENDS.md for cross-theme analysis