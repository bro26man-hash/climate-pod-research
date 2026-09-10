# 🌊 Ocean Intervention — Research Notes

**Source:** GitHub API-based project discovery + commit-history analysis
**Branch:** `ocean-intervention`
**Scope:** Ocean-based geoengineering — ocean alkalinity enhancement (OAE), iron fertilization, seaweed, upwelling manipulation

---

## ✦ Project Discoveries

| # | Project | Repo | Stars | Last Activity | Note |
|---|---------|------|------|---------------|------|
| 1 | **Oceananigans.jl** (GPU ocean simulation) | [CliMA/Oceananigans.jl](https://github.com/CliMA/Oceananigans.jl) | 1,333 ⭐ | Sep 2026 | The *only* vibrant open ocean code; infrastructure for any OAE/upwelling build |
| 2 | **OceanParameterizations.jl** | [CliMA/OceanParameterizations.jl](https://github.com/CliMA/OceanParameterizations.jl) | (small) | — | Core ocean physics param stack; building-block layer |
| 3 | **SM2** (Spectral Ocean Model) | [NOAA-GFDL/SM2](https://github.com/NOAA-GFDL/SM2) | ~2 ⭐ | Apr 2019 | Legacy operational ocean model; effectively dormant (last commit 2019) |
| 4 | **NebuGrid-OpenSource** (fog harvest/drip irr) | [Team50-Labs/NebuGrid-OpenSource](https://github.com/Team50-Labs/NebuGrid-OpenSource) | 0 ⭐ | Aug 2026 | Water-sourcing(cs) framing, not marine geoengineering per se |

**The striking finding:** virtually **no dedicated ocean-geoengineering repositories** exist on GitHub. Oceananigans is the lone bright spot — and it is *general ocean modelling infrastructure*, not OAE/iron/fertilization code. Everything else is legacy, small, or framework-level.

**Other/roadmap finds** (mentioned in prior research logs as targets, not yet found as active repos):
- Planetary Technologies — OAE/seaweed field work (institutional, limited open code)
- NOAA-GFDL ocean models — institutional, Fortran (legacy)

---

## 📈 Commit Trend Summary

- **Oceananigans.jl — the singular dominant open ocean repo.** The same near-daily, multi-contributor rhythm seen in its atmosphere sibling: late-September 2026 commitsSpan type stability, tripolar-grid distribution (`distribute tripolar grid helper`), immersed-boundary fixes (`mask_immersed_field_xy!`), and tracer boundary conditions. This is generationally ahead of legacy Fortran ocean models and is the codebase any open ocean-geoengineering effort would inherit.
- **NOAA-GFDL/SM2** — essentially fossilised: two commits (initial import Jun 2018, data-path update Apr 2019). Institutional operational ocean modelling is not an open-source development story.
- **OceanParameterizations.jl** — framework/physics layer, important as a building block but not a geoengineering application.
- **The ocean-geoengineering vacuum:** Unlike the atmosphere (ClimaAtmos) or land carbon (ClimaLand), there is **no active, open, purpose-built ocean intervention simulator**. The compute/physics predecessor (Oceananigans) exists and is world-class; the application layer — OAE alkalinity benchmarking, iron-fertilization bloom modelling, seaweed growth/leaching — is an empty quadrant.

---

## 💡 Talking Points

1. **The empty quadrant.** Ocean geoengineering has the *least* open-source code of the three themes. Why: (a) extreme experimental complexity (mesoscale biogeochemistry), (b) governance sensitivity (London Protocol / London Convention on ocean fertilization), (c) institutional siloing (NOAA, NERC, GEOTRACES) that keeps work internal.
2. **The promising inverse.** Because the physics/infrastructure layer is solved (Oceananigans, arguably the best open ocean code on Earth), the *barrier to building* open OAE/upwelling tools is lower than it looks — the missing ingredient is the *application* and *governance* will, not the compute.
3. **What would "open OAE" look like?** A reproducibility-first, benchmarked Oceananigans sub-project tracking alkalinity enhancement scenarios — pH, carbonate chemistry, ecological response — with open parameter sweeps. The tech exists; the coordinated build doesn't.
4. **Iron fertilization & seaweed** are even more dormant in open code than OAE. Iron fertilization carries the heaviest governance baggage (see GIEDP, LSB). Seaweed/kelp is mostly incipient (Planetary Technologies) and field-not-code.
5. **Episode angle — "Why is the ocean the empty quadrant, and should we fill it?"** The answer sits at the intersection of science (anybody could build on Oceananigans), policy (London Protocol restrictions), and funding (the research councils that *could* mandate openness don't).

---

## 🔑 Key Terminology

- **OAE (Ocean Alkalinity Enhancement)** — adding alkalinity (limestone slurry, electrochemical) to drive ocean CO₂ uptake and shift carbonate chemistry.
- **Iron fertilization** — micronutrient (Fe) addition to trigger phytoplankton blooms / biological carbon pump.
- **Seaweed / kelp farming** — biomass cultivation for carbon export (sinking, biochar) or feed.
- **Upwelling / downwelling manipulation** — altering nutrient/CO₂ exchange via pumped or natural circulation.
- **mesoscale biogeochemistry** — the turbulent, sub-grid mixing that makes ocean CDR hard to model/fertilize predictably.
- **London Protocol / London Convention** — the governing framework restricting ocean fertilization; the governance anchor.
- **GEOTRACES** — the global marine geochemistry survey programme; background-data backbone.

---

*Commit data pulleded from GitHub API: CliMA/Oceananigans.jl (Sep 2026), NOAA-GFDL/SM2 (2019), CliMA/OceanParameterizations.jl. Note: ocean-geoengineering-specific open code is largely absent — this "gap" is a first-order finding, not a search failure.*
