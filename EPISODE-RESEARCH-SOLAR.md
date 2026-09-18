# 🌞 Episode Research: Solar Geoengineering
## "The Building Blocks Without the Blueprint"

---

## Episode Premise

Solar geoengineering can be simulated with existing climate tools — but nobody has built the simulation tools for geoengineering itself. This episode explores the gap between climate simulation capability and solar radiation management implementation.

---

## Key Metrics (As of September 2026)

| Metric | Value |
|--------|-------|
| Total solar-themed repos found | 5 with meaningful activity |
| Total commits analyzed | 60+ |
| SRM-specific repositories | **0** |
| Institutional repos (active) | 3 (WRF, PCMDI, MDTF) |
| Academic repos (dormant) | 2 (ClimateMARGO, srm-forever) |
| Peak commit activity | 5 commits in 1 day (MDTF, Jun 19, 2026) |

---

## The Cast of Characters

### WRF (1,763★) — The Heavyweight
- **What:** The primary weather/climate simulation model used worldwide
- **Why it matters:** Any SRM scenario would need WRF-level atmospheric physics
- **What's missing:** No SRM module. It simulates nature, not intervention.
- **Fresh evidence:** v4.8.0 release (Jun 2026) with solar radiation physics correction
- **Quote for episode:** *"We can model the Earth's radiation budget perfectly. We just can't model what we'd do to it."

### MDTF-diagnostics (80★) — The Ruler
- **What:** Process-oriented diagnostic toolkit for climate model evaluation
- **Why it matters:** Before governing SRM, you need to verify models are right
- **Fresh evidence:** 5-commit sprint on Jun 19, 2026; new precipitation-buoyancy POD
- **Quote for episode:** *"MDTF is a ruler, not a crystal ball. It measures accuracy. It doesn't predict what happens when you block the sun."

### ClimateMARGO.jl (73★) — The Phantom
- **What:** Climate-economic modeling framework (Julia)
- **Why it matters:** Would be used for SRM cost-benefit analysis
- **Fresh evidence:** 2 README updates after 2-year dormancy (Aug 2026); zero code commits
- **Quote for episode:** *"Two README updates and the ghost wakes up. But no code. Just marketing."

### srm-forever (0★) — The Prophet in the Wilderness
- **What:** Interactive SRM economics model using Weitzman discounting
- **Why it matters:** The theoretical framework for "forever" decisions
- **Fresh evidence:** Conceptually critical; zero stars; zero community
- **Quote for episode:** *"The most important question in SRM economics lives in a repo that nobody watches."

---

## Interview Angles / Questions for Experts

1. **To a climate modeler:** "WRF just fixed its solar radiation calculation. If you wanted to add an SRM module tomorrow, what would you need? Is it technically hard or politically impossible?"

2. **To a governance scholar:** "MDTF spent a full day sprinting on precipitation diagnostics. Should SRM governance have the equivalent infrastructure? What would it look like?"

3. **To an economist:** "ClimateMARGO went dormant for 2 years then got 2 README updates. What does that tell you about the political economy of solar geoengineering research?"

4. **To srm-forever's author:** "You wrote the book on Weitzman discounting applied to SRM. Why does your repo have zero stars? Do you think the community isn't ready, or aren't you inviting them in?"

---

## Sound Design Notes

- **Opening:** WRF v4.8.0 release announcement tone → then silence → "But there's a catch..."
- **Transition 1:** The Jun 19 sprint (5 commits in a day) → rapid-fire delivery → "Something was happening that day..."
- **Transition 2:** ClimateMARGO's phantom revival → slowing down → "Wake up... but the lights are off..."
- **Closing:** srm-forever's zero stars → quiet, contemplative → "Nobody's watching the most important question."

---

## Additional Resources

- [WRF v4.8.0 Release](https://github.com/wrf-model/WRF)
- [MDTF-diagnostics Repository](https://github.com/NOAA-GFDL/MDTF-diagnostics)
- [ClimateMARGO.jl Documentation](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- [srm-forever — Weitzman Discounting for SRM](https://github.com/hausfath/srm-forever)
- [PCMDI Metrics v4.2.1](https://github.com/PCMDI/pcmdi_metrics)

---

*Research conducted via GitHub API — commit histories pulled September 2026*