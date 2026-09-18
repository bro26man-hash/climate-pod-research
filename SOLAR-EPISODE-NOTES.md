# 🌞 Solar Geoengineering — Episode Notes
## Episode Planning Document (September 2026)

---

## Episode Title (Working)
"The Model Gap: Why Solar Geoengineering Has No Open-Source Simulation"

---

## Core Thesis
The open-source world has incredible tools for *evaluating* climate — but almost nothing for *simulating* solar radiation management. The entire SRM modeling pipeline runs through institutional, closed-source general circulation models. GitHub, the world's largest open-source collaboration platform, has **zero** repositories for simulating SRM interventions. This gap is itself a story about power, access, and governance.

---

## Key Talking Points

### 1. The Solar Radiation Bug (May 28, 2026)
- **What happened:** A developer fixed the Earth Outgoing Longwave (EOT) radiation calculation in WRF v4.8.0
- **Why it matters:** If the solar radiation calculation was wrong, every SRM simulation using WRF produced flawed data
- **Question to explore:** How many policy documents and field-test permits were justified using data with this known error?
- **Commit:** `e836cd6` — "correction for EOT calculation for solar radiation"

### 2. The Aerosol Scheme Toggle (June 5, 2026)
- **What happened:** WRF v4.8.0 deactivated `tempo_aerosolaware` and `tempo_hailaware`
- **Why it matters:** These are aerosol-aware cloud physics schemes — directly relevant to how models treat stratospheric aerosol injection
- **Question to explore:** Were these schemes failing? Were they being replaced? Or is this just cleanup?

### 3. The PCMDI Velocity (September 3–4, 2026)
- **What happened:** 10 commits in 2 days for v4.2.1 release
- **Why it matters:** PCMDI metrics are the validation toolkit for CMIP6 — the gold standard for climate model evaluation
- **Question to explore:** What was the urgency? A journal deadline? A policy report? And does faster validation mean SRM results are being rushed?

### 4. The Precip-Buoyancy POD (June 19, 2026)
- **What happened:** 5 commits in one day adding a precipitation-buoyancy statistics diagnostic to MDTF
- **Why it matters:** This is the most ocean-relevant diagnostic in open source — and it's for evaluating model accuracy, not simulating interventions
- **Question to explore:** Would a true ocean geoengineering model need this diagnostic? Or is it irrelevant to deliberate interventions?

### 5. Weitzman Discounting & the Termination Shock
- **What happened:** `srm-forever` was created in a single day (August 26, 2026) with a complete economic model using Weitzman certainty-equivalent discounting
- **Why it matters:** It provides the theoretical framework for understanding the "termination shock" — the risk that stopping SRM causes rapid warming
- **Question to explore:** If SRM costs are modeled as a vintage annuity, does that change the political calculus? Who pays for forever?

### 6. The Governance Vacuum
- **What happened:** `climate-intervention-governance` was released (August 23, 2026) — a 12-skill Claude Code plugin for tracking SRM legal/regulatory status
- **Why it matters:** It's the first real governance intelligence tool for SRM, and it's built as a Claude plugin, not a public website
- **Question to explore:** Is governance-by-AI-plugin the future of SRM oversight? Who audits the auditor?

---

## Interview Questions (Draft)
1. "If you were a policymaker deciding whether to fund an SRM field test, would you trust the output of a model with a known solar radiation bug?"
2. "Why is there no open-source GCM with an SRM module? Is it a technical barrier or a political one?"
3. "The WRF maintainers deactivated two aerosol schemes. Should the community have been consulted before that change?"
4. "What would a truly open-source SRM simulation platform look like? And who would build it?"
5. "Is the absence of SRM code on GitHub a governance signal — a way of saying 'we don't want this to be democratized'?"

---

## Guest Outreach Ideas
- **weiwangncar** (WRF maintainer, NCA/Davis) — technical authority on WRF physics
- **Jiwoo Lee** (PCMDI, LLNL) — CMIP6 metrics and validation
- **Wei-Ming Tsai** (NOAA GFDL) — ocean-atmosphere interaction diagnostics
- **Fons van der Plas** (ClimateMARGO) — climate-economic modeling
- **hausfath** (srm-forever) — SRM economics and discounting theory
- **Zereo0317** (climate-intervention-governance) — SRM regulatory tracking

---

## References
- [WRF v4.8.0 Release](https://github.com/wrf-model/WRF/releases)
- [PCMDI Metrics v4.2.1](https://github.com/PCMDI/pcmdi_metrics)
- [MDTF-diagnostics](https://github.com/NOAA-GFDL/MDTF-diagnostics)
- [ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- [srm-forever](https://github.com/hausfath/srm-forever)
- [Climate Intervention Governance Plugin](https://github.com/Zereo0317/climate-intervention-governance)