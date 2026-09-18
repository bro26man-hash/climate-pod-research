# 🌊 Ocean Intervention — Quick Reference Card (v4)
## Climate Pod Research | September 2026

---

## The Ocean Paradox At-a-Glance

| Metric | Value |
|--------|-------|
| Ocean coverage of Earth's surface | **71%** |
| Ocean geoengineering repositories on GitHub | **0** |
| Ocean physics commits (Oceananigans.jl) | **~4/day** |
| Ocean-adjacent diagnostics (MDTF POD) | **5 commits in 1 day** |
| Active ocean intervention code | **NONE** |

## The Three Ocean-Adjacent Repos

| Repo | Stars | Ocean Relevance | Key Feature | Intervention-Ready? |
|------|-------|------------------|-------------|-------------------|
| **CliMA/Oceananigans.jl** | 1,413 | ★★★★★ | World's best ocean physics engine | 7 of 8 pieces (see below) |
| **NOAA-GFDL/MDTF-diagnostics** | 80 | ★★★★☆ | Precipitation-buoyancy POD | Evaluation only, no intervention |
| **wrf-model/WRF** | 1,763 | ★★★☆☆ | Atmospheric model with ocean boundary | Deprecatinging aerosol physics |

## Oceananigans.jl: The 7 of 8 Pieces

### What Already Exists (Ready for Intervention)
1. ✅ **Lagrangian particle tracking** (Sep 16) — Track dispersal of intervention materials
2. ✅ **Immersed boundaries** — Model artificial seafloor structures
3. ✅ **Time-dependent forcings** — Apply solar radiation or upwelling scenarios
4. ✅ **Differentiable programming** — Optimize intervention strategies via gradient descent
5. ✅ **GPU acceleration** — Fast enough for ensemble scenario runs
6. ✅ **Output diagnostics (TimeDerivative)** — Assess intervention impacts over time
7. ✅ **Robust column solving** — Handle extreme conditions (point-source discharge)

### What's Missing (The 8th Piece)
8. ❌ **Intervention Module** — Nobody has written: no upwelling, no alkalinity, no brightening, no fertilization

## The Ocean Search Results

| Search Term | Repos Found |
|-------------|-------------|
| `"ocean geoengineering"` | **0** |
| `"marine cloud brightening"` | **0** |
| `"ocean alkalinity enhancement"` | **0** |
| `"artificial upwelling"` | **0** |
| `"ocean iron fertilization"` | **0** |
| `"marine geoengineering"` stars:>10 | **0** |

**Total: ZERO ocean geoengineering repositories.**

## The Precip-Buoyancy POD (June 19, 2026)

**What happened:** 5 commits on one file in one day.

**What it is:** A Proper Orthogonal Decomposition diagnostic for mesoscale convective systems over warm ocean waters.

**Why it matters:** If you want to simulate what happens to tropical rainfall when you interrupt ocean-atmosphere coupling (via upwelling, brightening, or alkalinity), you first need to know whether your model gets the coupling right.

**The evaluation chain:**
```
Ocean Intervention → Sea Surface Temp Change → Boundary Layer Stability → MCS Convection → Precipitation
                                              ↑
                              MDTF's POD evaluates THIS link
```

## WRF's Ocean Narrative: Better Physics, Worse Chemistry

| Date | Event | Ocean Impact |
|------|-------|---------------|
| May 28 | Solar radiation EOT fix | **Positive** — better SST for ocean boundary |
| Jun 5 | Aerosol-aware physics deprecated | **Negative** — less ocean chemistry modeling |

**Net:** WRF is improving its atmosphere-ocean **physics interface** while reducing its atmosphere-ocean **chemistry interface**.

## The Hypotheses (Ranked)

| Rank | Why Is the Ocean Empty? | Our Confidence |
|------|------------------------|----------------|
| 1 | **Governance chill** — London Protocol deters code publication | ★★★★☆ |
| 2 | **Complexity curse** — Physics + chemistry + biology = 3x SRM | ★★★☆☆ |
| 3 | **Funding gap** — Ocean interventions underfunded | ★★★☆☆ |
| 4 | **Biology barrier** — No repo models ecosystem response | ★★☆☆☆ |
| 5 | **Oceananigans paradox** — Tool too sophisticated for use | ★★☆☆☆ |

## The Cross-Theme Triangle

```
         WRF (Solar)
         /        \
        /          \
       /            \
      /              \
MDTF -------- Oceananigans.jl
(Precip-Buoyancy   (Ocean Physics)
     POD)

↓ All three tools exist ↓
↓ All three could power intervention scenarios ↓
↓ Nobody connects them ↓
```

## Five Talking Points for Episode 3

1. **The paradox** — 4 commits/day in ocean physics, 0 commits in ocean intervention
2. **The POD moment** — 5 commits on one file: the closest thing to ocean geoengineering code
3. **The 7 of 8 pieces** — Oceananigans already has the infrastructure; someone just needs to build the module
4. **The WRF deprecation** — They're getting better at ocean boundary conditions while deprecating ocean chemistry
5. **The governance question** — Did legal frameworks discourage code from ever being written?

---

*Quick reference for on-air discussion. For full analysis, see PROJECT-DISCOVERIES-OCEAN.md and COMMIT-TRENDS-OCEAN.md.*