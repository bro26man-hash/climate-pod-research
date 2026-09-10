# 🌊 Ocean Intervention — Episode Outline

**Branch:** `ocean-intervention`
**Format:** Modular, ~40–50 min episode

---

## Scene 1 — The Empty Quadrant (Cold Open)
- Run a live/githubexplorer "search for open ocean geoengineering code" — and find *almost nothing*.
- Contrast with the atmosphere (ClimaAtmos) and land (ClimaLand): two themes with thriving open stacks.
- The hook: **ocean geoengineering is the empty quadrant** — and that absence is itself the story.

## Scene 2 — The One Bright Spot: Oceananigans.jl
- 1,333★, near-daily commits, GPU-accelerated, global (TripolarGrid) — arguably the best open ocean code on the planet.
- But it's *general ocean modelling infrastructure*, not OAE/iron/fertilization. It's the foundation nobody's built the geoengineering house on yet.
- Introduce the "Oceananigans-as-infrastructure" idea: the physics is solved; the application layer is wide open.

## Scene 3 — Why Is the Ocean So Empty in Open Source?
- Three locks:
  1. **Experimental complexity** — mesoscale biogeochemistry is viciously hard to model and observe.
  2. **Governance sensitivity** — London Protocol / London Convention constraints on ocean fertilization; iron fertilization can't just be Gitea-merged.
  3. **Institutional siloing** — NOAA, NERC, GEOTRACES keep work internal/legacy (Fortran, SM2 fossilised at 2 commits since 2018).
- Compare/constra with the atmosphere: why did the Julia stack flourish there but not the ocean?

## Scene 4 — What Would "Open OAE" Actually Look Like?
- A reproducibility-first Oceananigans sub-project: alkalinity enhancement scenarios (pH, carbonate chemistry, ecological response), open parameter sweeps, benchmarked against GEOTRACES background.
- The tech already exists to *build* it. What's missing is coordinated build + governance framing.
- Brief, honest note on iron fertilization and seaweed: even more dormant/code-less than OAE; heaviest governance baggage.

## Scene 5 — Should We Fill the Quadrant?
- The case *for* open ocean-geoengineering code: transparency, governance legitimacy, accelerating a field that needs both.
- The case for caution: governance restrictions, ecological risk, the "publish blueprints for ocean manipulation" tension.
- Frame: the question isn't *can* we build it (we can, on Oceananigans), but *should* we, and under what open governance.

## Out-Cue / Discussion Questions
1. If you woke up tomorrow and Oceananigans had a first-class OAE module — what would it need to be credible to a regulator?
2. Is the ocean-geoengineering open-source gap a problem to fix, or a sensible caution to respect?
3. How do you open-source something the London Protocol essentially tells you not to do at scale?

---

*Source commits: CliMA/Oceananigans.jl (Sep 2026), NOAA-GFDL/SM2 (2019), CliMA/OceanParameterizations.jl. Gap finding based on GitHub search absence confirmed via API.*
