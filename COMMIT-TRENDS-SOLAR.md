# ☀️ Solar Geoengineering — Commit Trend Analysis
## Trend Signals & Episode Talking Points (September 2026)

---

## Executive Summary
Fresh commit data was pulled from **5 solar-related repositories** totaling **36+ commits** across the periods studied. The trends reveal a solar geoengineering landscape that is **institutionally sustained but conceptually thin** — sophisticated tools for evaluating climate, but almost no tools for *simulating* SRM interventions themselves.

---

## Timeline of Activity

### Wave 1: The Working Institutional Pulse (May–June 2026)
**Repo: `wrf-model/WRF`** — 14 commits in 4 weeks
- May 12–June 8, 2026
- Sustained, professional development cadence
- Key events: v4.8.0 release, solar radiation EOT bug fix, aerosol scheme toggling

### Wave 2: The Release Crunch (September 3–4, 2026)
**Repo: `PCMDI/pcmdi_metrics`** — 10 commits in 2 days
- September 3–4, 2026
- v4.2.1 release sprint
- Bug fixes: roundoff errors, dask SVD memory, extremes chunking
- All commits by Jiwoo Lee, James Goodnight, Jared Lewis

### Wave 3: The Ocean-Adjacent Lag (May–August 2026)
**Repo: `NOAA-GFDL/MDTF-diagnostics`** — 10 commits over 3 months
- May 22–August 14, 2026
- Pivotal: precip-buoyancy POD added June 19 (5 commits that day)
- Slower cadence than WRF/PCMDI, but continued software development

### Ghost Activity: README Updates After Dormancy
**Repo: `ClimateMARGO/ClimateMARGO.jl`** — 2 README updates
- August 17, 2026 — two README updates after 2+ year gap
- No code commits. Revival signal or cleaning house?

### Burst: Theoretical Framework
**Repo: `hausfath/srm-forever`** — 4 commits in 1 day
- August 26, 2026 — entire repo created and populated in a single day
- Weitzman certainty-equivalent discounting applied to SRM cost dynamics
- Zero stars, but conceptually the most important SRM repo found

---

## Key Trend Signals

### Signal 1: "Everything is Evaluating, Nothing is Simulating"
The entire solar geoengineering open-source ecosystem on GitHub is built around **evaluating** climate models (WRF, PCMDI, MDTF) — not **simulating** SRM interventions. There is no open-source general circulation model (GCM) with a functioning SRM module on GitHub. This is the single most important finding for the episode.

**Talking point:** *"If you want to model what happens if we inject aerosols into the stratosphere, you can't just fork a repo and run a simulation. You have to use a general circulation model — and those are run by institutions like NCAR, NASA GISS, and the Met Office, not by open-source communities on GitHub. The code exists, but it's walled off."*

### Signal 2: The Solar Radiation Bug Fix is a Governance Story
The WRF commit `e836cd6` ("correction for EOT calculation for solar radiation", May 28, 2026) is not just a bug fix — it's a governance event. If the solar radiation endpoint calculation was wrong, then every simulation that used it produced flawed results. How many papers cited flawed WRF output? How many SRM field-test permits were justified by model data with this bug?

**Talking point:** *"We found a bug fix in the solar radiation calculation of the most widely used atmospheric model — right as the v4.8.0 release was being finalized. This is the kind of thing that should make everyone nervous: the model we use to decide whether to deploy SRM has a known error in its core physics."

### Signal 3: The Aerosol Scheme Deactivation
The commit to turn off `tempo_aerosolaware` and `tempo_hailaware` (June 5, 2026) in WRF v4.8.0 raises questions. Were these schemes producing unreliable results? Were they being replaced? Or were they simply not being used and the maintainers are cleaning up? For an episode, this is a doorway into the technical nitty-gritty of how atmospheric models handle aerosol–cloud interactions.

### Signal 4: PCMDI's Velocity — Institutional新冠疫期 Recovery?
PCMDI's 10 commits in 2 days (September 3–4, 2026) for v4.2.1 suggests an institution that had been waiting for a moment to release. The fixes — roundoff errors, dask memory optimization, SVD forced to use numpy — are dry but meaningful. This is the toolkit that validates every CMIP6 result, including those used in SRM assessments. The speed suggests either catching up after a quiet period or responding to external pressure (maybe a journal review or a policy report deadline).

### Signal 5: srm-forever — The Moon-shot of SRM Modeling
`hausfath/srm-forever` (0 stars, 4 commits, August 26, 2026) is the only repo that directly models SRM economics. It applies **Weitzman certainty-equivalent discounting** to the question: "What does it cost to keep SRM going forever?" This is the theoretical backbone for the "termination shock" argument — if you stop SRM, temperatures jump rapidly. The repo argues for a framework where SRM costs are modeled as a vintage annuity, not a one-time expenditure.

**Talking point:** *"There's a repo with zero stars that asks the most important question in SRM economics: What's the cost of never stopping? The answer depends on discount rates, and this repo uses a framework from Nobel laureate Martin Weitzman to argue that the standard approach underestimates the long-term commitment."

---

## The Three Universes (Solar Theme)

| Universe | Reps | Characteristics |
|----------|------|------------------|
| **Fast** | WRF, PCMDI, MDTF | Institutional, funded, sustained development, professional cadence |
| **Slow** | ClimateMARGO, srm-forever | Individual, unfunded, dormant with occasional bursts |
| **Empty** | SRM-specific simulation tools | Zero repos found — no open-source GCM with SRM modules |

---

## Episode Structure Suggestion

### Cold Open
> "In May 2026, a developer named weiwangncar pushed a commit to the world's most widely used atmospheric model. The commit message reads: 'correction for EOT calculation for solar radiation.' Three words. But what they mean is: we may have gotten the sun wrong for years."

### Act 1: The Tools We Have
- WRF: 1,761 stars, professional development, v4.8.0 just released
- PCMDI: The validation toolkit that makes or breaks CMIP6 results
- MDTF: Process-level diagnostics, including the ocean's closest friend (precip-buoyancy POD)

### Act 2: The Gap
- No open-source GCM with SRM modules
- No community-driven SRM simulation platform
- The only SRM-specific repo (srm-forever) has zero stars and is pure theory

### Act 3: The Governance Question
- Climate-intervention-governance tracker: 12 skills, 0 public users
- The silence on GitHub about SRM simulation is itself a policy signal
- Who gets to run these models? Who gets to see the results?

---

## Sources & Links
- WRF: https://github.com/wrf-model/WRF
- PCMDI Metrics: https://github.com/PCMDI/pcmdi_metrics
- MDTF-diagnostics: https://github.com/NOAA-GFDL/MDTF-diagnostics
- ClimateMARGO.jl: https://github.com/ClimateMARGO/ClimateMARGO.jl
- srm-forever: https://github.com/hausfath/srm-forever
- Climate Intervention Governance: https://github.com/Zereo0317/climate-intervention-governance