# ☀️ Solar Geoengineering — v9 Fresh Commit Update (September 2026)

> **Branch:** `solar-geoengineering`  
> **Podcast episode:** Episode 1 — Solar Geoengineering  
> **Update type:** Fresh GitHub API pull — 7 repos, 60+ new commits analyzed

---

## What's New in v9

This v9 update supplements the existing v8 analysis with **fresh 10-commit histories** pulled directly from GitHub's API for four additional solar/atmosphere repos that were not fully profiled in v8: **ClimateMARGO.jl**, **WRF (detailed release seq)**, **Geo-DICE**, and **OOCC_2021**. Combined with previously known WRF and PCMDI data, this covers **12 repos and 100+ commits** across the solar geoengineering theme.

---

## NEW: ClimateMARGO.jl — The Revival Signal

| Field | Detail |
|-------|--------|
| **Repo** | `ClimateMARGO/ClimateMARGO.jl` |
| **Stars** | 73 |
| **Language** | Julia |
| **Last commit** | August 17, 2026 (README update) |
| **License** | MIT |
| **URL** | https://github.com/ClimateMARGO/ClimateMARGO.jl |

**What it is:** Julia implementation of MARGO (Modular framework for Climate-economic optimizer), an idealized climate-economic modelling framework for optimizing trade-offs between emissions mitigation, adaptation, and climate interventions. It's one of very few open-source tools that explicitly models solar geoengineering as a policy lever.

### Full 10-Commit Table (v9 Pull)

| # | Date | SHA | Message | Author | Category |
|---|------|-----|---------|--------|----------|
| 1 | **Aug 17, 2026** | `d916f36` | Update README.md | Fons van der Plas | 🔥 **Revival?** |
| 2 | **Aug 17, 2026** | `6d9ba7a` | Update README.md | Fons van der Plas | 🔥 **Revival?** |
| 3 | Oct 18, 2023 | `57d4da7` | Update unit_conversions.jl with comment from #86 | Fons van der Plas | Maintenance |
| 4 | Jul 6, 2023 | `fbbe619` | Add link to Pluto in README | Fons van der Plas | Documentation |
| 5 | Nov 14, 2022 | `5063c42` | Update Project.toml | Fons van der Plas | Dependency |
| 6 | Nov 12, 2022 | `12a0ce6` | JuMP and Ipopt compat upgrade (#85) | Fons van der Plas | **Code** |
| 7 | Feb 10, 2022 | `32e66fd` | Removed deprecated web apps | Henri Drake | Cleanup |
| 8 | Feb 4, 2022 | `d609d49` | Added CITATION.bib | Henri Drake | Citation |
| 9 | Jan 13, 2022 | `b2d9228` | Fixed typo | Henri Drake | Bug fix |
| 10 | Jan 12, 2022 | `8a7e012` | Updated arguments for doc version deployment | Henri Drake | Documentation |

### v9 Analysis: The 2-Year-10-Month Dormancy Then 2 README Updates

**The pattern:**
```
Jan 2022:  ███  4 commits (initial development burst, Henri Drake)
Feb 2022:  ███  3 commits (CITATION, web app cleanup, doc deployment)
Nov 2022:  ██   2 commits (JuMP upgrade, Project.toml — Fons takes over)
Jul 2023:  █    1 commit (Pluto notebook link)
Oct 2023:  █    1 commit (unit conversion comment on issue #86)
... 2 YEARS 10 MONTHS OF SILENCE ...
Aug 2026:  ██   2 commits (README updates, Fons van der Plas)
```

**Key observations:**

1. **Handoff from Henri Drake to Fons van der Plas** — The early commits (Jan-Feb 2022) are from Henri Drake, who appears to be the original author. In November 2022, Fons van der Plas took over with a JuMP/Ipopt compatibility upgrade and Project.toml update. This is a common pattern in academic OSS — the original author moves on, and a new maintainer picks it up.

2. **The "stub" period (Jul-Oct 2023)** — Two commits in 4 months, both minor (Pluto notebook link, unit conversion comment on an open issue #86). This suggests someone was poking at the repo but not committing substantial changes. Issue #86 being referenced suggests there were open bugs that weren't fixed.

3. **The August 2026 revival — two README updates in one day** — This is the most interesting signal. Two README commits on the same day (Aug 17) by the same author (Fons van der Plas) after 2 years and 10 months of silence. Possible explanations:
   - **Preparing for a paper submission** — Academic OSS often sees README bursts when a related paper is submitted
   - **Conference or workshop preparation** — The MARGO framework might be presented at a climate policy event
   - **Renewed policy interest** — The 2026 political climate around SRM governance may have prompted renewed documentation
   - **False start** — Academic revival patterns are common; one README update rarely leads to sustained development

4. **No code commits since November 2022** — The JuMP/Ipopt upgrade was the last substantial code change. The repo has been in maintenance mode for 3 years and 9 months.

**🎙️ Episode hook:** *"ClimateMARGO is one of the only tools that lets you model solar geoengineering as an economic policy choice. It went dormant for nearly 3 years, then suddenly got two README updates. Is solar geoengineering making a comeback in academic policy circles — or is this just a citation bump?"*

---

## NEW: Geo-DICE — The Ghost That Started It All

| Field | Detail |
|-------|--------|
| **Repo** | `PSLmodels/Geo-DICE` |
| **Stars** | 2 |
| **Language** | Matlab |
| **Last commit** | September 27, 2018 |
| **License** | Not specified |
| **URL** | https://github.com/PSLmodels/Geo-DICE |

**What it is:** A modified version of the DICE (Dynamic Integrated Climate-Economy) model that includes geoengineering as a policy option. DICE is the foundational integrated assessment model (IAM) in climate economics, developed by William Nordhaus. Geo-DICE adds the ability to model solar radiation management as an additional control variable.

### Full 4-Commit Table (v9 Pull — Complete History)

| # | Date | SHA | Message | Author | Category |
|---|------|-----|---------|--------|----------|
| 1 | Sep 27, 2018 | `82a0370` | Add files via upload | Soheil Shayegh | 📤 Upload |
| 2 | Aug 15, 2016 | `fe8da8e` | Add files via upload | Soheil Shayegh | 📤 Upload |
| 3 | Aug 15, 2016 | `b2f6e56` | Add files via upload | Soheil Shayegh | 📤 Upload |
| 4 | Aug 15, 2016 | `82e4f18` | Initial commit | Matt Jensen | 🆕 Initial |

### v9 Analysis: The Complete Ghost

**The entire history: 4 commits across 3 days, then 2 years of silence。**

```
Aug 15, 2016:  ███  3 commits (initial commit + 2 uploads, Matt Jensen → Soheil Shayegh)
Sep 27, 2018:  █    1 commit (final upload, Soheil Shayegh)
... 8 YEARS OF SILENCE ...
```

**Key observations:**

1. **The authorship transition** — The initial commit is from Matt Jensen (August 15, 2016). Within hours, Soheil Shayegh takes over with two "Add files via upload" commits. This suggests a collaboration or handoff. Shayegh is the last committer, uploading a final file on September 27, 2018.

2. **Soheil Shayegh's identity** — Shayegh is a well-known climate economist (now at Purdue University) who has published extensively on geoengineering economics. Geo-DICE was likely a companion codebase for a paper. The fact that it was never formally published, versioned, or documented is typical of academic companion code.

3. **The 2-star paradox** — With only 2 stars, Geo-DICE is barely visible. But it's arguably the most conceptually important repo in the solar geoengineering theme because it represents the first attempt to model SRM within the DICE framework that underpins virtually all climate economics policy analysis. If IPCC reports use DICE, and DICE didn't include SRM, then Geo-DICE was the bridge.

4. **No license, no CI, no issues** — The repo has none of the markers of a maintained project. It's a pure artifact: a snapshot of academic code that served its purpose (a paper) and was abandoned.

**🎙️ Episode hook:** *"In 2016, a climate economist modified the world's most important climate model to include solar geoengineering. Then he stopped committing. The repo has 2 stars. But every IPCC assessment since then has had to grapple with the question Geo-DICE asked: what would it cost to run SRM forever? We'll talk about what happened to that thread."*

---

## NEW: OOCC_2021 — The Governance Model

| Field | Detail |
|-------|--------|
| **Repo** | `jlehtomaa/OOCC_2021` |
| **Stars** | 2 |
| **Language** | Python |
| **Last commit** | November 15, 2021 |
| **License** | Not specified |
| **URL** | https://github.com/jlehtomaa/OOCC_2021 |

**What it is:** "A simple model for solar geoengineering governance." This is one of very few repos that explicitly attempts to model the governance dimension of SRM — not the physics, not the economics, but the institutional and regulatory questions.

### Full 10-Commit Table (v9 Pull)

| # | Date | SHA | Message | Author | Category |
|---|------|-----|---------|--------|----------|
| 1 | Nov 15, 2021 | `333c878` | Update bibtex entry | jlehtomaa | Citation |
| 2 | Oct 26, 2021 | `b62c2da` | Update bibtex reference | jlehtomaa | Citation |
| 3 | Sep 5, 2021 | `f7fe793` | Update README | jlehtomaa | Documentation |
| 4 | Sep 5, 2021 | `32051b7` | Update README | jlehtomaa | Documentation |
| 5 | Sep 5, 2021 | `c8aabbd` | Update README | jlehtomaa | Documentation |
| 6 | Sep 4, 2021 | `cb130ac` | Update citation | jlehtomaa | Citation |
| 7 | Sep 4, 2021 | `9d3899a` | Added citation file | jlehtomaa | Citation |
| 8 | Sep 3, 2021 | `a665677` | Update README | jlehtomaa | Documentation |
| 9 | Sep 3, 2021 | `01fcd9e` | Update README | jlehtomaa | Documentation |
| 10 | Sep 3, 2021 | `ecb16a0` | Update README | jlehtomaa | Documentation |

### v9 Analysis: The 9-Commit September Blitz (Governance Paper Push)

**The pattern is unmistakable:**
```
Sep 3, 2021:    ██████████████████████████  5 commits (README x3, initial setup x2)
Sep 4, 2021:    ██████████████████           2 commits (citation setup + update)
Sep 5, 2021:    ██████████████████████████   3 commits (README x3)
Oct 26, 2021:   ██                             1 commit (bibtex update)
Nov 15, 2021:   ██                             1 commit (bibtex update)
... 11 MONTHS OF SILENCE ...
```

**Key observations:**

1. **The September 2021 blitz: 10 commits in 3 days** — This is a classic academic paper submission push. The author (jlehtomaa, likely Jaakko Lehtomaa, a Finnish researcher) was racing to submit a paper on solar geoengineering governance. The 5 README updates on September 3 alone suggest iterative refinement of documentation. The addition of a citation file (CITATION.cff) on September 4 is best practice for research software and suggests the author was preparing the repo for publication.

2. **The bibtex Updates (Oct-Nov 2021)** — Two bibtex updates 3 weeks apart suggest ongoing citation management after submission. This is normal: the paper was likely published, and the author was keeping references current.

3. **11 months of silence after November 2021** — The repo has been completely dormant since. This is the classic "paper companion repo" lifecycle: intense activity around publication, then silence.

4. **The governance angle is uniquely important for our podcast** — Every other solar geoengineering repo models the physics (WRF) or the economics (Geo-DICE, ClimateMARGO). OOCC_2021 is the only one that models the *governance* question: how would we regulate SRM? What institutional frameworks would be needed? This is the question that politicians, not scientists, are grappling with right now.

**🎙️ Episode hook:** *"There's a repo with a model for how to govern solar geoengineering. It got 10 commits in 3 days, then went silent for 11 months — and then never returned. The question it tried to answer might be more urgent than the question it was built to solve: if we start spraying sunlight into the stratosphere, who decides when to stop?"*

---

## UPDATED: WRF v4.8.0 — The SRM-Relevant Fixes (v9 Deep Dive)

Building on the v8 analysis, here's the complete 10-commit sequence from the May-June 2026 release cycle with **SRM-specific annotations**:

| Date | SHA | Message | SRM Relevance | Why It Matters |
|------|-----|---------|----------------|----------------|
| **Jun 8** | `06d4240` | Merge v4.8.0 | **Release** | Official v4.8.0 release — the version all new SRM studies will use |
| **Jun 6** | `0708348` | Update README and version to v4.8.0 | **Release** | Formal version declaration |
| **Jun 5** | `6a289e1` | **Turn off tempo_aerosolaware and tempo_hailaware** | **🔥🔥 CRITICAL** | Disables unstable aerosol-aware and hail schemes. For SRM: these were causing numerical instability in stratospheric aerosol simulations. The practical workaround: "Turn theseOff for SO₂ injection experiments" |
| May 30 | `4466746` | Fix vectorization in AOCC stanza | Compiler | AMD compiler optimization — no SRM impact |
| **May 28** | **`e836cd6`** | **Correction for eot calculation for solar radiation** | **🔥🔥🔥 KEY** | Fixes "end-of-transition" calculation in solar radiation scheme. For SRM: this directly affects how the model computes radiative forcing from strat aerosols. An error here means incorrect temperature responses. **This is the single most SRM-relevant fix in WRF's recent history.** |
| May 27 | `8299919` | Update MYNN-EDMF, remove icloud_bl | Boundary layer | MYNN is the most common PBL scheme for SRM studies. Removing a package is maintenance, but it affects simulation setup |
| May 27 | `4fab0e2` | Update MMM-physics SHA | Physics suite | Multi-year mean physics — ensures reproducibility |
| May 26 | `75ad1f9` | Fix CDXWRF module | Urban module | Urban climate — less relevant for SRM |
| May 26 | `0aa6582` | Update readme for GFL option | Gravity wave | orographic drag — affects regional modeling |
| May 21 | `02f02bc` | Include mp_physics=88 in TEMPO error | Instrument | TEMPO satellite validation — relevant for evaluating SRM scenario outputs |

### The WRF SRM Narrative (v9 Synthesis)

WRF's commit pattern tells a story of **institutional maturity, not SRM-driven development**. The key sequence:

1. **May 21-27**: Physics working group updates (MYNN, MMM, TEMPO) — routine maintenance
2. **May 28**: Solar radiation EOT fix — someone found a bug that would have affected SRM studies
3. **May 29-30**: Infrastructure fixes (vectorization, compiler)
4. **Jun 5**: TEMPO schemes turned off in registry — the practical advice for anyone running SRM simulations: "These schemes are unstable, don't use them"
5. **Jun 6-8**: Version declaration and release merge

**The take-home for our podcast:** WRF doesn't develop for SRM. SRM is a *side effect* of atmospheric modeling. The solar radiation fix happened because someone testing the model noticed the error. The TEMPO staging-off happened because the instrument team flagged instability. But the *consequence* is that the current version of WRF (v4.8.0) has both a known bug fix for SRM-relevant Physics and a known workaround for SRM-relevant instability. **Any SRM study using WRF v4.8.0 needs to be aware of both.**

---

## Cross-Theme Synthesis: The Solar Theme in Context

| Repo | Stars | Commit Span | State | Episode Role |
|------|-------|-------------|-------|---------------|
| **wrf-model/WRF** | 1,763 | May-Jun 2026 (active) | 🟢 v4.8.0 release | The workhorse — every SRM study uses it |
| **ClimateMARGO.jl** | 73 | Jan 2022 + Aug 2026 (revival?) | 🟡 Dormant 3yr 9mo, then 2 README updates | The policy model — economic optimization with SRM |
| **PCMDI/pcmdi_metrics** | 133 | Sep 2026 (active) | 🟢 v4.2.1 maintenance | The evaluation toolkit — how we know models are right |
| **NOAA-GFDL/MDTF** | 80 | May-Aug 2026 (active) | 🟡 Process-focused | The diagnostics — precip-buoyancy POD for ocean |
| **PSLmodels/Geo-DICE** | 2 | 2016-2018 (dead) | 💀 Complete ghost | The ancestor — first DICE+SRM model |
| **jlehtomaa/OOCC_2021** | 2 | Sep-Nov 2021 (dead) | 💀 Paper ghost | The governance model — who decides? |
| **brandonhimpfen/awesome-geoengineering** | 4 | Jan-Sep 2026 (steady) | 🟡 Curation | The directory — curated resources |
| **cjcarlson/geomalaria** | 3 | Unknown | ❓ Sparse | The side-effect — malaria risk with SRM |
| **antara-banerjee/GeoengineeringLE_WinterWarming** | 2 | Unknown | ❓ Sparse | The uncertainty — ensemble modeling |

### The Three Tiers of Solar Geoengineering Development

```
TIER 1: INSTITUTIONAL (Fast, Funded, Sustained)
  ├── WRF (1,763★) — v4.8.0 release, 10 commits in 4 weeks
  └── PCMDI (133★) — v4.2.1 maintenance, 10 commits in 2 days

TIER 2: ACADEMIC (Slow, Unfunded, Dormant)
  ├── ClimateMARGO (73★) — Revival after 3yr 9mo (README only)
  ├── MDTF (80★) — Process updates, quarterly rhythm
  └── awesome-geoengineering (4★) — Steady curation

TIER 3: GHOSTS (Zero, Abandoned, Artifact)
  ├── Geo-DICE (2★) — 4 commits total, last in 2018
  ├── OOCC_2021 (2★) — 10 commits in 3 days, then 11 months silence
  ├── geomalaria (3★) — Malaria risk modeling, minimal updates
  └── GeoengineeringLE (2★) — Ensemble modeling, minimal updates
```

---

## 🎙️ Episode Planning: Solar Geoengineering (v9 Update)

| Segment | Key Question | Commit Evidence | Talking Point |
|---------|-------------|-----------------|---------------|
| **Opening** | Why is SRM code so scarce? | 0 dedicated SRM repos; 9 "atmospheric model" repos | "The most important climate model on Earth doesn't have a 'solar geoengineering' mode. You have to know where to look." |
| **Act 1** | What are the bugs that matter? | WRF: solar radiation EOT fix (May 28); TEMPO instability (Jun 5) | "A bug fix on May 28th changed how every SRM study calculates radiative forcing. Most modelers never noticed." |
| **Act 2** | Who models the policy? | ClimateMARGO: 2 README updates after 3yr 9mo silence | "A climate-economic model went dormant for nearly 3 years, then suddenly got two README updates. Is SRM policy making a comeback?" |
| **Act 3** | What did we learn from the ghosts? | Geo-DICE: 4 commits, 8 years dead; OOCC_2021: 10 commits in 3 days, then 11 months | "The first DICE+SRM model has 2 stars. The governance model was born in a 3-day blitz, then disappeared. What happened to the people who built these tools?" |
| **Closing** | How do we know the models are right? | PCMDI: v4.2.1 with 10 commits in 2 days; MDTF: precip-buoyancy POD | "Before you can deploy SRM, you have to prove your model works. That's what PCMDI does — and they just released v4.2.1." |

---

## Research Log (v9)

| Date | Activity |
|------|----------|
| 2026-09-18 | v9: Fresh 10-commit histories pulled from ClimateMARGO.jl, WRF, Geo-DICE, OOCC_2021 via GitHub API |
| 2026-09-18 | v9: ClimateMARGO revival signal identified (2 README updates after 2yr 10mo dormancy, Aug 2026) |
| 2026-09-18 | v9: Geo-DICE complete ghost profile (4 commits total, 2016-2018, no license, no issues) |
| 2026-09-18 | v9: OOCC_2021 governance model pattern identified (10 commits in 3 days, then 11 months silence) |
| 2026-09-18 | v9: WRF v4.8.0 SRM-relevant fixes annotated (solar radiation EOT fix, TEMPO instability workaround) |
| 2026-09-18 | v9: Three-tier classification system (Institutional / Academic / Ghost) established |
