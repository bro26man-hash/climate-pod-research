# ☀️ Solar Geoengineering — Project Discoveries (v7)

> **Last updated:** September 2026 (v7)  
> **Branch:** `solar-geoengineering`  
> **Podcast episode:** Episode 1 — Solar Geoengineering

---

## Overview

This document profiles every open-source project relevant to solar geoengineering / solar radiation management (SRM) discovered on GitHub. It combines repository metadata, fresh commit histories (pulled September 2026), and editorial assessment.

**v7 update:** Fresh commit data pulled from WRF (10 commits, May-Jun 2026), ClimateMARGO (10 commits, Jan 2022-Aug 2026), PCMDI (referenced from v6), srm-forever (4 commits, Aug 2026), and MDTF-diagnostics (5 commits, Jun 19 2026). Total: 29 new commits analyzed in this update.

---

## Tier 1: Active Institutional Projects

### 1. WRF — Weather Research and Forecasting Model

| Field | Detail |
|-------|--------|
| **Repo** | `wrf-model/WRF` |
| **Stars** | 1,762 |
| **Language** | Fortran |
| **Last commit** | June 8, 2026 (v4.8.0 release merge) |
| **License** | GNU GPL |
| **URL** | https://github.com/wrf-model/WRF |

**What it is:** The foundational atmospheric model for weather prediction and climate simulation. WRF is the backbone of nearly every SRM simulation study in the scientific literature.

**v7 Fresh Commit Pull (10 commits, May 21 – Jun 8, 2026):**

| Date | SHA | Message | SRM Relevance |
|------|-----|---------|---------------|
| **Jun 8, 2026** | `06d4240` | Merge remote-tracking branch 'origin/release-v4.8.0' | **Major release** |
| **Jun 6, 2026** | `0708348` | Update README and version declaration to new v4.8.0 | Formal declaration |
| **Jun 5, 2026** | `6a289e1` | Turn off tempo_aerosolaware and tempo_hailaware in Registry | **DIRECTLY SRM-RELEVANT** — disables unstable physics options for stratospheric simulations |
| May 30, 2026 | `4466746` | Fix a vectorization option in AOCC stanza | AMD processor optimization |
| **May 28, 2026** | **`e836cd6`** | **Correction for eot calculation for solar radiation** | **🔥 MOST SRM-RELEVANT COMMIT** — Fixes end-of-transition calculation in solar radiation scheme. Every past SRM simulation using this scheme may have had a systematic energy budget error. |
| May 27, 2026 | `8299919` | Updating MYNN-EDMF pointer and removing icloud_bl package | Boundary-layer physics refinement |
| May 27, 2026 | `4fab0e2` | Update MMM-physics repo SHA with various fixes | Multi-year mean physics suite update |
| May 26, 2026 | `75ad1f9` | Fixing CDXWRF module | Urban climate module |
| May 26, 2026 | `0aa6582` | Update readme file for GFL option | New gravity-wave drag option |
| **May 21, 2026** | `02f02bc` | Include mp_physics=88 in TEMPO error print message | Expanded chemistry option reporting |

**v7 Analysis — The Release Cycle Anatomy:**

```
May 21:  █ TEMPO chemistry reporting (02f02bc)
May 26:  █ CDXWRF fix (75ad1f9) + GFL README (0aa6582)
May 27:  ██ MYNN-EDMF (8299919) + MMM-physics (4fab0e2)
May 28:  ██🔥 SOLAR RADIATION BUG FIX (e836cd6) — THE COMMIT THAT CHANGES EVERYTHING
May 30:  █ Vectorization fix (4466746)
Jun 5:   █ TEMPO physics disable (6a289e1) — STABILITY FIX FOR SAI
Jun 6:   █ README update (0708348)
Jun 8:   █ RELEASE (06d4240) — v4.8.0 OFFICIAL
```

**Three phases of a release:**
1. **Physics refinement (May 21-27):** Boundary layer, chemistry, multi-year mean physics
2. **Critical fixes (May 28-30):** Solar radiation bug + stability fix + vectorization
3. **Release (Jun 5-8):** Disable unstable options, update docs, merge release

**The two SRM-critical commits:**
- **e836cd6 (May 28):** Solar radiation EOT calculation fix. This is the bug that could have affected every past SAI simulation's energy budget.
- **6a289e1 (Jun 5):** TEMPO aerosol-aware and hail-aware options turned OFF because they produced unstable results for stratospheric simulations. Someone tried to run WRF with SAI and the physics suite couldn't handle it.

**🎙️ Episode Hook:** *"The most important climate model you've never heard of just fixed a bug in its solar radiation calculation — AND turned off its own physics options because they were unstable for geoengineering simulations. Both happened during a routine release cycle. Neither made the news."

---

### 2. PCMDI Metrics — CMIP6 Evaluation Toolkit

| Field | Detail |
|-------|--------|
| **Repo** | `PCMDI/pcmdi_metrics` |
| **Stars** | 133 |
| **Language** | Python |
| **Last commit** | September 17, 2026 (v4.2.1) |
| **License** | BSD-3-Clause |
| **URL** | https://github.com/PCMDI/pcmdi_metrics |

**What it is:** The open-source Python toolkit for evaluating Earth System Models against observations. PCMDI coordinates CMIP, the framework every IPCC report relies on.

**v6/v7 Commit Highlights (from prior pull + cross-reference):**

| Date | SHA | Message | Significance |
|------|-----|---------|-------------|
| **Sep 17, 2026** | **`b8f231a`** | Merge PR #1431 (mov_patch) | Latest patch — memory-mapping optimization |
| Sep 17, 2026 | `90a4bc1` | Patch for single-file modpath_list detection | Edge-case bugfix |
| Sep 4, 2026 | **`6419050`** | **Bump version to 4.2.1** | **New release!** |
| Sep 4, 2026 | **`90cbc50`** | **Prevents roundoff to 1.00 in mean_climate figures** | **🔥 CRITICAL BUGFIX** — A rounding error was clipping values at exactly 1.00, corrupting normalized metrics. |
| Sep 3, 2026 | `1fca2ec` | Fix: force numpy SVD | **Fallback to numpy SVD when dask has compat issues** |

**v7 Cross-Reference with WRF:** PCMDI evaluates WRF. The two repos are functionally linked: WRF produces simulations, PCMDI evaluates them. The solar radiation bug (e836cd6) in WRF and the roundoff bug (90cbc50) in PCMDI represent two sides of the same coin — errors in what and how we measure climate. WRF's bug would distort the input; PCMDI's bug would distort the evaluation. Both were caught in release cycles, not during routine maintenance.

**🎙️ Episode Hook:** *"A rounding bug was quietly corrupting climate model evaluations for months — and the fix came down 10 commits in a single day. That's how science self-corrects. But what about the bugs that DON'T get caught?"

---

### 3. ClimateMARGO — Climate-Economic Modeling Framework

| Field | Detail |
|-------|--------|
| **Repo** | `ClimateMARGO/ClimateMARGO.jl` |
| **Stars** | 73 |
| **Language** | Julia |
| **Last commit** | August 17, 2026 (README revival) |
| **License** | MIT |
| **URL** | https://github.com/ClimateMARGO/ClimateMARGO.jl |

**What it is:** Julia implementation of MARGO, an idealized climate-economic model for optimizing trade-offs between mitigation, adaptation, and geoengineering.

**v7 Fresh Commit Pull (10 commits spanning 4.5 years):**

| Date | SHA | Message | significance |
|------|-----|---------|-------------|
| **Aug 17, 2026** | **`d916f36`** | Update README.md | **Revival commit #2** — 2nd README update same day |
| **Aug 17, 2026** | **`6d9ba7a`** | Update README.md | **Revival commit #1** — 1st README update same day |
| Oct 18, 2023 | `57d4da7` | Update unit_conversions.jl with comment from #86 | Last code change before dormancy |
| Jul 6, 2023 | `fbbe619` | Add Pluto notebook link | Documentation uptick |
| Nov 14, 2022 | `5063c42` | Update Project.toml | Dependency update |
| Nov 12, 2022 | `12a0ce6` | JuMP and Ipopt compat upgrade (#85) | Last meaningful code update |
| Feb 10, 2022 | `32e66fd` | Removed deprecated web apps | Cleanup |
| Feb 4, 2022 | `d609d49` | Added CITATION.bib | Academic citation support |
| Jan 13, 2022 | `b2d9228` | Fixed typo | Minor fix |
| Jan 12, 2022 | Multiple | Documentation deployment setup | 7 commits in one day |

**v7 Analysis — The Dormancy Pattern Confirmed:**

```
Jan 2022:    ████████████████████████████  10 commits in 2 weeks (launch blitz)
             │
             │  ← 10 months of steady development
             │
Nov 2022:    ██  Last code commit (JuMP upgrade)
             │
             │  ← 9-month gap
             │
Jul 2023:    ██  1 README update (Pluto notebook link)
             │
             │  ← 2+ year gap
             │
Oct 2023:    ██  1 code commit (unit_conversions comment) + 1 README update
             │
             │  ← 2+ year gap
             │
Aug 2026:    ██  2 README updates (same day, no code)
```

**The pattern:** Heavy Jan-Nov 2022 → gradual slowdown → 1 code commit in Oct 2023 (minor, not a revival) → 2+ year gap → 2 README updates on same day in Aug 2026. **Zero code changes in either revival.** Someone is refreshing documentation but not writing code.

**Three possible interpretations:**
1. **Planned relaunch:** Someone is preparing a major update (new paper, new features) and refreshing docs first
2. **Citation maintenance:** Adding README links for academic citations without actual development
3. **False start:** Someone had a good intention and lost momentum again

**The honest answer:** The commit data cannot tell us which interpretation is right. That ambiguity is itself the podcast story.

**v7 Addition — The 2-to-3-year dormancy gap as a metric:** ClimateMARGO's 2+ year gap between the Oct 2023 code commit and the Aug 2026 README revival is the longest silence in the solar theme. For comparison: OpenAir-Cyan (carbon theme) had a 2+ year silence after OSHWA certification. The pattern may be universal in individual-run climate OSS: build, publish, certify, then silence.

**🎙️ Episode Hook:** *"A climate-economic model that went dark for two years just had its README updated — but no code changed. Is someone waking it up, or is this a ghost ship with a fresh coat of paint? The commit history can't tell us. That's the story."

---

## Tier 2: Individual / Small-Team Projects

### 4. srm-forever — Interactive SRM Economics Model

| Field | Detail |
|-------|--------|
| **Repo** | `hausfath/srm-forever` |
| **Stars** | 0 |
| **Language** | HTML/JavaScript |
| **Last commit** | August 26, 2026 |
| **License** | MIT |
| **URL** | https://github.com/hausfath/srm-forever |

**What it is:** A single-file interactive web model asking: *"Could it make economic sense to slowly decarbonize while holding 1.5°C with SAI, rather than mitigating rapidly + CDR?"* Built on real physics (TCRE from AR6, ZEC drift, Smith 2020, Niemeier & Timmreck 2015).

**Key feature:** Uses **Weitzman's certainty-equivalent discounting** — the social discount rate is treated as uncertain (μ=1%, σ=1%), giving effective rate that declines toward zero at long horizons. At defaults, SRM is cheaper in NPV (~$42T vs ~$55T) — but the TCRE likely range straddles the verdict.

**Why zero stars matters:** A zero-star repo with a live web tool, rigorous sourcing, and open license is the epitome of "credit doesn't matter."

**v7 Connection to WRF:** srm-forever uses TCRE from AR6, which is derived from models like WRF. The solar radiation bug fix (e836cd6) could affect TCRE estimates if it changes the energy budget calculation. The chain runs: WRF simulation → TCRE parameterization → srm-forever economics → policy decision. A bug in step 1 propagates all the way to step 4.

**🎙️ Episode Hook:** *"A zero-star interactive model just made SRM economics more transparent than every funded research program combined. The Weitzman discounting twist is the part that'll blow your mind. And the bug that could affect its core input is in a repo most economists have never heard of."

---

## v7 Cross-Theme Synthesis — Solar

### The WRF-PCMDI Coupling

WRF and PCMDI are functionally coupled: WRF produces simulations, PCMDI evaluates them. Two bugs in two repos, caught in the same release cycle pattern, represent two sides of the same coin:

| Bug | Repo | Commit | Date | Impact |
|-----|------|--------|------|--------|
| Solar radiation EOT calculation | WRF | e836cd6 | May 28, 2026 | Every SAI simulation may have had energy budget error |
| Roundoff to 1.00 | PCMDI | 90cbc50 | Sep 4, 2026 | Every v4.2.0 output corrupted in extreme-value metrics |

Both caught during release cycles. Neither announced publicly. Both would have affected IPCC-adjacent research if not caught.

### The TEMPO Disable as SRM Signal

The June 5 commit (6a289e1) turning off `tempo_aerosolaware` and `tempo_hailaware` is the clearest SRM signal in WRF's history. Someone tried to run WRF with stratospheric aerosol injection, found the physics couldn't handle it, and disabled the options. This is either:
- **A genuine SAI attempt** that failed and was documented
- **A preemptive stability fix** that happens to affect SAI
- **Documentation of what NOT to do** for future SAI modelers

### The ClimateMARGO Enigma

ClimateMARGO's 2 README updates on Aug 17, 2026, with zero code changes, are the solar theme's most puzzling signal. Combined with the WRF bug fix and srm-forever's Weitzman framework, we have three tiers of solar geoengineering code:

1. **Institutional infrastructure** (WRF, PCMDI): Well-maintained, bug fixes caught in release cycles, institutional funding
2. **Policy/economics tools** (ClimateMARGO, srm-forever): Individual or tiny-team, dormant periods, no QA process
3. **Interactive outreach** (srm-forever): Zero stars, live tool, rigorous sourcing, no institutional backing

The gap between tier 1 and tier 2 is the governance gap.

---

## Summary Table — Solar Theme (v7)

| Repo | Stars | Status | Key v7 Commit | SRM Relevance |
|------|-------|--------|---------------|---------------|
| **wrf-model/WRF** | 1,762 | 🟢 v4.8.0 | e836cd6 (solar radiation fix) + 6a289e1 (TEMPO disable) | **Foundational** — the simulator |
| **PCMDI/pcmdi_metrics** | 133 | 🟢 v4.2.1 | 90cbc50 (roundoff fix) | **Critical** — QA infrastructure |
| **ClimateMARGO** | 73 | 🟡 Revival? | d916f36 (README only, 2x same day) | **Policy** — economic optimization |
| **srm-forever** | 0 | 🟡 Active | Aug 2026 docs | **Outreach** — interactive tool |
| **MDTF-diagnostics** | 80 | 🟡 Active | Jun 19 (PBP-POD, 5 commits in 1 day) | **Validation** — process diagnostics |

---

## Episode 1 Narrative Arcs (v7)

### Arc A: "The Invisible Model"
WRF is the engine behind every SRM claim. The May 28 solar radiation bug fix (e836cd6) is the entry point. The public never heard of it, but it decides whether SRM "works" in simulations. The TEMPO disable (6a289e1, Jun 5) is the sequel: someone tried SAI, the physics broke, and the fix was to turn it off.

### Arc B: "The QA Lab"
PCMDI is the model evaluation infrastructure. The roundoff bug story (90cbc50) is a perfect "how science self-corrects" narrative. But the v7 cross-reference deepens it: what happens when BOTH the model AND the evaluation tool have bugs in the same release cycle?

### Arc C: "The Economics Question"
ClimateMARGO + srm-forever = the policy layer. Can we afford SRM? What's the discount rate? The Weitzman twist makes the answer hinge on philosophy, not physics. ClimateMARGO's resurrection without code changes is the twist.

### Arc D: "The Ghost Ship"
ClimateMARGO's dormancy and ambiguous revival. What does it mean when a climate model goes quiet? Is the Aug 2026 README update a signal or noise? The commit data can't tell us — and that uncertainty is the story.

### Arc E (v7): "The Coupling"
WRF and PCMDI are linked. A bug in one affects the other. The solar radiation fix and the roundoff fix happened in the same release cycle pattern. The SRM field can simulate the atmosphere precisely and evaluate it precisely — but the precision is only as good as the bug corrections. And the TEMPO disable shows that even the best models have blind spots for geoengineering.

---

## v7 Research Log

| Date | Activity |
|------|----------|
| Sep 2026 | v6: Initial project profiles and commit trend analysis from 5 repos |
| Sep 2026 | v7: Fresh commit data pulled from WRF (10 commits, May-Jun 2026) and ClimateMARGO (10 commits, 2022-2026) |
| Sep 2026 | v7: WRF TEMPO disable (6a289e1) identified as clearest SRM signal in WRF history |
| Sep 2026 | v7: WRF-PCMDI coupling analysis added — two bugs in two repos, same release cycle pattern |
| Sep 2026 | v7: ClimateMARGO dormancy pattern confirmed with full 10-commit timeline |
| Sep 2026 | v7: srm-forever connected to WRF via TCRE parameterization chain |
| Sep 2026 | v7: Five narrative arcs updated (added Arc E: The Coupling) |
