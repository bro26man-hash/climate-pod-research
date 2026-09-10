# ☀️ Solar Geoengineering — Episode Outline

**Branch:** `solar-geoengineering`
**Format:** Modular, ~40–50 min episode

---

## Scene 1 — The Thought Experiment (Cold Open)
- "What if we could turn down the thermostat?" — introduce radiative forcing in plain terms.
- Framing: SRM not as "solving" climate change but as a high-stakes, reversible(ish) modulating tool.
- The core tension: powerful enough to lower global mean temperature, invisible enough to be governed by almost no one.

## Scene 2 — How Much Actually Gets Researched Openly?
- Poll the audience/guests: name an open-source SRM simulator. (Silence is the point.)
- The finding: dedicated open SRM code barely exists; real work lives inside closed institutional models (GFDL, NCAR) while the open world builds *components* (ClimaAtmos, Oceananigans).
- Introduce the "simulation gap" as the show's guiding thread.

## Scene 3 — The Open Pieces That Do Exist
- **ClimaAtmos.jl** — the star open atmosphere code; monthly releases, cloud microphysics & albedo work → the most honest open lever for aerosol–cloud forcing.
- **CESM** — the institutional workhorse; mention who can actually run SRM scenarios today (and why it's hard to join).
- **Oceananigans.jl** — the over-performing ocean component; GPU + global-geometry → the ocean sidekicks (upwelling, OAE) would chain onto this.
- **ClimateMARGO.jl** — cost-optimal deployment trajectories; what happens when an optimizer goes quiet.

## Scene 4 — Cloud Albedo, the Unquantified Lever
- Why getting droplet nucleation right under perturbed chemistry is harder than the dynamics.
- ClimaAtmos's TKE/updraft-drag and CloudMicrophysics upgrades as the quietly important work.
- The implication: an open SRM simulator needs *this* physics before it needs anything else.

## Scene 5 — Verification is the Real Bottleneck
- Once you *can* simulate SRM, the show doesn't end — you need observational verification (satellite retrievals, deployment monitoring).
- Why regional impact (Arctic-focused radiometric codes) matters more to governance than global mean forcing.
- The "termination risk" thought-experiment close: who holds the off switch?

## Out-Cue / Discussion Questions
1. If you had to build an open SRM simulator next year, which component do you start with?
2. Should SRM research be open-sourced given governance asymmetry?
3. Which is harder — the physics fidelity or the verification backbone?

---

*Source commits: ClimaAtmos v0.42.8→v0.42.9, ClimaLand v1.12.0→v1.12.1, Oceananigans TripolarGrid/Zarr I/O (Aug–Sep 2026).*
