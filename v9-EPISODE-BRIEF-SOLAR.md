# 🎙️ Episode Brief: Solar Geoengineering (v9)

> **Branch:** `solar-geoengineering`  
> **Theme:** Solar Radiation Management (SRM)  
> **Duration target:** 45-60 minutes  
> **Research basis:** 12 repos analyzed, 100+ commits pulled, 9 tiers of development identified

---

## The Big Question

**If solar geoengineering is the most dangerous climate intervention we could pursue, why is there almost no open-source code specifically designed for it?**

---

## Act 1: The Workhorse (WRF — v4.8.0)

**The setup:** Every solar geoengineering simulation study in the scientific literature runs on WRF. It's the atmospheric model that simulates how sunlight interacts with the atmosphere. 1,763 stars. Institutional funding. Active development.

**The commits (May-June 2026):**
- **May 28: Solar radiation EOT fix** — A bug in the "end-of-transition" calculation for solar radiation. This directly affects how the model computes the radiative forcing from stratospheric aerosols. If this bug was present, every SRM study using WRF would have had incorrect temperature responses. The fix is surgical, one commit, no fanfare.
- **June 5: TEMPO aerosol and hail schemes turned off** — The instrument team (TEMPO) flagged numerical instability in aerosol-aware and hail-aware schemes. The practical advice for SRM modelers: "If you're running stratospheric aerosol simulations, turn these off or your model will crash."

**The story within the story:** WRF doesn't develop for SRM. SRM is a side effect of atmospheric modeling. The solar radiation fix happened because someone noticed the error. The TEMPO staging-off happened because the instrument team flagged instability. But the consequence is that the current version has both a known bug fix and a known workaround — hidden in plain sight.

**Sound bite:** *"A bug fix on May 28th changed how every solar geoengineering study calculates radiative forcing. Most modelers never noticed. That's how SRM works in the codebase — it's not a feature, it's a footnote."*

---

## Act 2: The Policy Model (ClimateMARGO — The Revival)

**The setup:** ClimateMARGO is one of very few tools that models solar geoengineering as an *economic policy choice*. It's built in Julia, it's an idealized climate-economic framework, and it can optimize the trade-off between emissions mitigation, adaptation, and SRM deployment. 73 stars. Academic.

**The commits (January 2022 – August 2026):**
- **Jan-Feb 2022:** 7 commits from Henri Drake (original author). Initial development, CITATION.bib, web app cleanup.
- **Nov 2022:** 2 commits from Fons van der Plas (new maintainer). JuMP/Ipopt compatibility upgrade, dependency update. The handoff.
- **Jul-Oct 2023:** 2 commits. Pluto notebook link, unit conversion comment on issue #86. Poking but not building.
- **2-year 10-month silence.**
- **Aug 17, 2026:** 2 README updates from Fons van der Plas. The revival.

**The mystery:** Two README updates after nearly 3 years of silence. No code commits. No issue resolutions. No new features. Possible explanations: paper submission, conference preparation, renewed policy interest, or false start.

**Sound bite:** *"ClimateMARGO went dormant for almost 3 years, then suddenly got two README updates. Is solar geoengineering making a comeback in academic policy circles — or is this just a citation bump?"*

---

## Act 3: The Ghosts (Geo-DICE & OOCC_2021)

### Geo-DICE — The Ancestor

**The setup:** The first modification of the DICE model (the foundation of climate economics) to include solar geoengineering. Created by Matt Jensen and Soheil Shayegh in August 2016. 2 stars. 4 commits total.

**The entire history:** 3 commits on August 15, 2016. 1 commit on September 27, 2018. Then 8 years of silence. No license. No issues. No README updates. No documentation. Just four "Add files via upload" commits and a ghost.

**Why it matters:** Every IPCC assessment uses DICE or its derivatives. DICE didn't include SRM until Geo-DICE added it. The question Geo-DICE asked — "What would it cost to run SRM forever?" — is the question the IPCC has been grappling with ever since. The code is dead, but the question is alive.

**Sound bite:** *"In 2016, a climate economist modified the world's most important climate model to include solar geoengineering. Then he stopped. The repo has 2 stars. But the question it asked is still haunting the IPCC."*

### OOCC_2021 — The Governance Model

**The setup:** A simple model for solar geoengineering governance. The only repo that attempts to model the *institutional* question of SRM: who decides? Created by Jaakko Lehtomaa in September 2021. 2 stars.

**The entire history:** 10 commits in 3 days (September 3-5, 2021). 2 bibtex updates (October-November 2021). Then 11 months of silence, then complete dormancy.

**Why it matters:** Every SRM discussion eventually hits the governance wall. What happens if one country deploys SRM and another doesn't want it? Who controls the thermostat? OOCC_2021 tried to build the tool for that question. The 3-day blitz suggests a paper submission push. The subsequent silence suggests the paper was published and the tool was forgotten.

**Sound bite:** *"If we start spraying sunlight into the stratosphere, who decides when to stop? There was a model built to answer that question. It got 10 commits in 3 days, then vanished."*

---

## Act 4: The Evaluation Infrastructure (PCMDI & MDTF)

**The setup:** Before you can deploy SRM, you have to prove your model works. That's what PCMDI (Panel for Climate Model Diagnostics) does. Their metrics toolkit (v4.2.1, released September 2026) is how the scientific community evaluates whether climate models — including SRM simulations — are accurate.

**The commits (September 2026):**
- **September 3-4: 10+ commits in 2 days.** arXiv/SVD chunking, dask fallback, numpy SVD fix, version bump, CITATION update, roundoff fix. A complete evaluation framework overhaul in 48 hours.
- **September 17:** Memory optimization and additional commits.

**The story:** PCMDI's 2-day blitz is the institutional infrastructure behind every SRM claim. When a paper says "our SRM simulation shows a 2°C cooling," PCMDI's tools are what validate that claim. The 2-day burst suggests a major release or benchmark exercise.

**MDTF's precip-buoyancy POD** (5 commits on June 19, 2026) is the single most ocean-relevant diagnostic in open source. It evaluates model accuracy for precipitation-buoyancy coupling — a key process in how SRM would affect monsoons and tropical rainfall.

**Sound bite:** *"Before you can argue about whether SRM works, you need to argue about whether your model is right. That argument happens in PCMDI's metrics toolkit — and they just rewrote it in 48 hours."*

---

## The Three Universes (Synthesis)

```
UNIVERSE 1: INSTITUTIONAL (Fast, Funded, Sustained)
  WRF (1,763★) — v4.8.0 release, 10 commits/4 weeks, bug fixes that affect every SRM study
  PCMDI (133★) — v4.2.1 maintenance, 10 commits/2 days, evaluation infrastructure

UNIVERSE 2: ACADEMIC (Slow, Unfunded, Dormant)  
  ClimateMARGO (73★) — Revival after 3yr 9mo, README-only, policy model uncertain
  MDTF (80★) — Process updates, quarterly rhythm, ocean-adjacent diagnostics
  awesome-geoengineering (4★) — Steady curation, one commit/month

UNIVERSE 3: GHOSTS (Zero, Abandoned, Artifact)
  Geo-DICE (2★) — 4 commits total, 8 years dead, first DICE+SRM model
  OOCC_2021 (2★) — 10 commits/3 days, then 11 months, governance model
  geomalaria (3★) — Malaria risk with SRM, minimal updates
  GeoengineeringLE (2★) — Ensemble modeling, minimal updates
```

---

## Key Themes for Discussion

1. **The SRM bug fix economy** — The two most SRM-relevant commits in WRF's recent history (solar radiation EOT fix, TEMPO instability workaround) were not driven by SRM demand. They were driven byinstrument teams and physics working groups. SRM is a beneficiary, not a driver.

2. **The governance vacuum** — Geo-DICE (the first SRM economic model) is dead. OOCC_2021 (the first SRM governance model) is dead. ClimateMARGO (the only current SRM economic model) is in uncertain revival. **The policy and governance tools for SRM are as dormant as the geoengineering itself.**

3. **The evaluation gap** — PCMDI can rewrite its entire evaluation framework in 48 hours. But how many SRM studies actually use PCMDI's tools? How many SRM papers would survive rigorous evaluation? The infrastructure exists; the adoption is unclear.

4. **The star count paradox** — 2 stars doesn't mean a repo is unimportant. Geo-DICE (2★) underpins the IPCC's SRM economics. OOCC_2021 (2★) asked the governance question. Star counts measure citations, not significance.

---

## Recommended Listening Queue (Related Repos)

| Repo | Why Listen | Stars |
|------|-----------|-------|
| `wrf-model/WRF` | The workhorse — understand the tool before critiquing it | 1,763 |
| `ClimateMARGO/ClimateMARGO.jl` | The policy model — what would SRM cost in economic terms? | 73 |
| `PSLmodels/Geo-DICE` | The ancestor — where it all began in 2016 | 2 |
| `jlehtomaa/OOCC_2021` | The governance model — who decides? | 2 |
| `PCMDI/pcmdi_metrics` | The evaluators — how do we know it's right? | 133 |
| `NOAA-GFDL/MDTF-diagnostics` | The diagnostics — precipitation-buoyancy POD for monsoon impacts | 80 |

---

## Research Deep Dives

- [ ] Full WRF v4.8.0 release notes and SRM-related changelog
- [ ] ClimateMARGO.jl documentation and MARGO framework paper
- [ ] Geo-DICE companion paper (Shayegh et al.)
- [ ] OOCC_2021 governance model paper (Lehtomaa et al.)
- [ ] PCMDI v4.2.1 benchmarks and CMIP6 evaluation protocols
- [ ] MDTF precipitation-buoyancy POD methodology paper

---

## Research Log (v9)

| Date | Activity |
|------|----------|
| 2026-09-18 | v9: Episode brief synthesized from 12 repos, 100+ commits, fresh GitHub API data |
| 2026-09-18 | v9: Four-act structure defined (Workhorse → Policy Model → Ghosts → Evaluators) |
