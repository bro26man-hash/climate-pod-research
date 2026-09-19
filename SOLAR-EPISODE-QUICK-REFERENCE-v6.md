# ☀️ Solar Geoengineering Episode — Quick Reference Card (v6)

## Episode Title: "The Sun-Timing Bug and the Cloud-Killing Update"

---

## The Single Story

The world's primary atmospheric climate model (WRF) just fixed its solar radiation calculation **and** deactivated its aerosol schemes — in the same week. What does this mean for solar geoengineering simulation?

---

## Key Facts (from commit data)

| Fact | Detail |
|------|--------|
| **WRF release** | v4.8.0, June 8, 2026 |
| **Critical fix** | `e836cd6` — solar radiation eot correction, May 28, 2026 |
| **Aerosol deactivation** | `6a289e1` — tempo_aerosolaware + tempo_hailaware turned off, Jun 5, 2026 |
| **Development pace** | 10 commits in 18 days (May 21 — Jun 8) |
| **Contributors** | Islas, weiwangncar, Olson, Fita, Werner (5 people, institutional team) |
| **ClimateMARGO status** | 2 README commits after 3-year code silence (Aug 17, 2026) |
| **Geo-DICE status** | 7 years dead (last commit Sep 2018), 4 total commits |
| **GeoengineeringLE status** | 5+ years dead (last commit Apr 2021), 10 commits in 18-day paper sprint |

---

## The Three Universes (Solar)

1. **Active Universe:** WRF — institutional, well-funded, continuous development, critical fixes
2. **Dormant Universe:** ClimateMARGO — elegant model, ghost signals, no code for 3 years
3. **Tomb Universe:** Geo-DICE + GeoengineeringLE — published and abandoned, paper-driven lifecycle

---

## Talking Points

### Opening Hook
> "The model used to simulate solar geoengineering just fixed a bug in when it calculates sunrise — and simultaneously turned off its cloud-aerosol module. If we're simulating a planet with less sun, shouldn't we keep all the instruments working?"

### The EOT Fix
- "Epoch of transit" = when the sun crosses a grid cell's meridian
- Error affects ALL simulations using WRF's solar radiation
- Small timing error — shifted peak cooling — different energy budget
- For a technology meant to shade the planet, precision is everything

### The Aerosol Deactivation
- Two aerosol schemes turned off in registry
- Possible bug, possible transition to new physics
- Undermines marine cloud brightening (MCB) simulations
- If the model can't handle clouds properly, can we evaluate MCB?

### The Dormant Pattern
- ClimateMARGO: 73 stars, 3-year silence, 2 README commits = ghost revival
- Geo-DICE: published model, 7 years dead, zero community
- GeoengineeringLE: 18-day lifespan, built for paper, not for community
- Pattern: academic code is born to die

### Closing Question
> "Is solar geoengineering code ready for prime time? Or are we simulating planet-cooling with tools that have broken sun-timers and disabled cloud modules?"

---

## Search Queries Used

1. `geoengineering simulation climate tech`
2. `geoengineering`
3. `climate simulation`
4. `solar radiation management SRM climate`
5. `climate technology geoengineering open-source`

## Repos Discovered (Solar-Relevant)

| Repo | Stars | Status | Key Signal |
|------|-------|--------|------------|
| wrf-model/WRF | 1,763 | Active | EOT fix + aerosol deactivation |
| ClimateMARGO/ClimateMARGO.jl | 73 | Dormant | README revival, no code |
| PSLmodels/Geo-DICE | 2 | Tomb | 7 years dead |
| antara-banerjee/GeoengineeringLE | 2 | Tomb | 18-day paper sprint |
| jnickla1/CESM2geoeng_documentation | ? | ? | CESM2 ocean geoeng docs |
| pixnum-hub/GeoVision | ? | ? | Geoengineering simulator |
| KOSASIH/GCCS-Core | 9 | ? | Global Climate Control System core |
| cjcarlson/geomalaria | 3 | ? | Malaria risk with SRM |
| brandonhimpfen/awesome-geoengineering | 4 | ? | Curated resource list |

---

*Last updated: September 2026 — v6 with fresh commit histories*