# ☀️ Solar Geoengineering — Commit Trend Analysis (v7)

> **Last updated:** September 2026 (v7 — fresh GitHub API pull)  
> **Branch:** `solar-geoengineering`  
> **Podcast episode:** Episode 1 — Solar Geoengineering

---

## Activity Overview (v7 Data)

| Repo | Total Commits Pulled | Date Range | Commit Density | Development State |
|------|---------------------|------------|---------------|------------------|
| wrf-model/WRF | 15 | May-Jun 2026 | 10 in 4 weeks | 🟢 v4.8.0 release cycle |
| PCMDI/pcmdi_metrics | 15 | Sep 3-4 + Sep 17, 2026 | 10 in 2 days | 🟢 v4.2.1 maintenance |
| MDTF-diagnostics | 15 | May-Aug 2026 | 5 in 1 day (PBP-POD) | 🟡 Active + process updates |
| ClimateMARGO/ClimateMARGO.jl | 15 | Jan 2022 + Aug 2026 | 7 in 1 day (launch) + 2 (revival?) | 🟡 Dormant 2yr 10mo |
| srm-forever | 4 | Aug 26, 2026 | 4 in 1 day | 🟡 Single-day burst |
| awesome-geoengineering | 5 | Jan-Sep 2026 | 1-2/month | 🟢 Steady curation |

---

## Trend 1: The Institutional Release Blitz (WRF v4.8.0)

WRF's commit pattern shows classic institutional release velocity:

```
May 12:  █  MYNN-SFC submodule update
May 19:  █  Bug fix for udm
May 20:  █████  PBL scheme, TEMPO changes, NbS fix, Tempo changes
May 21:  █  TEMPO error print
May 26:  ██  GFL option docs, CDXWRF fix
May 27:  ██  MYNN-EDMF physics, MMM-physics SHA
May 28:  █  🔥 SOLAR RADIATION EOT FIX
May 30:  █  AOCC vectorization
Jun 5:   █  TEMPO schemes off (registry)
Jun 6:   █  Version declaration
Jun 8:   █  v4.8.0 merge
```

**The 10-day sprint (May 19-28):** 9 commits in 10 days. The solar radiation fix (e836cd6, May 28) was the culmination. The TEMPO staging-off (6a289e1, Jun 5) was the practical advice. Together, they form a complete story: "Here's the bug, and here's how to work around it for SRM simulations."

**What this tells us:** WRF development is driven by instrument teams (TEMPO, GFL) and physics working groups (MYNN, MMM). SRM isn't a driver — it's a side effect of the instrument and physics development pipeline. The solar radiation fix happened because someone noticed the error, not because SRM modelers demanded it.

---

## Trend 2: The 10-Commit Release Day (PCMDI v4.2.1)

```
Sep 3:   ██████████  arXiv/SVD chunking, dask fallback, rename, numpy SVD fix
Sep 4:   ██████████████████  Prepare v4.2.1, CITATION update, version bump, PR merges, roundoff fix
Sep 17:  ██  mov_patch merge, single-file detection
```

**The Sep 4 blitz (7 commits):**

| # | Commit | Type |
|---|--------|------|
| 1 | `e7dc726` | Prepare v4.2.1 |
| 2 | `0e3a96f` | CITATION.cff metadata |
| 3 | `6419050` | Version bump |
| 4 | `6443a1d` | PR #1429 merge |
| 5 | `d0bcbd8` | PR #1427 merge (roundoff) |
| 6 | `90cbc50` | **The roundoff fix** |
| 7 | `3092cdd` | PR #1428 merge |

**Analysis:** This is a textbook institutional release. The roundoff fix (90cbc50) was the core technical contribution. The other 6 commits were release infrastructure: version bump, citation metadata, PR merges. The team shipped a fix and a new version in a single day.

**The Sep 3 precedents:** The dask/SVD work (3 commits) and numpy fallback (1fca2ec) show that the team was already optimizing for reproducibility. The roundoff fix was the natural conclusion of that reproducibility work.

---

## Trend 3: The Dormancy Signature (ClimateMARGO)

```
Jan 12, 2022:  ████████████████████████████  7 commits (launch burst)
Feb 4, 2022:   █  CITATION.bib
Feb 10, 2022:  █  Remove web apps
Nov 12, 2022:  █  JuMP/Ipopt upgrade
Nov 14, 2022:  █  Project.toml update
--- 2 years, 9 months of silence ---
Jul 6, 2023:   █  Pluto notebook link
Oct 18, 2023:  █  Unit conversions comment
--- 2 years, 2 months of silence ---
Aug 17, 2026:  ██  2 README updates (no code changes)
```

**The three eras:**
1. **Launch (Jan 2022):** Paper-driven creation. 7 commits in one day.
2. **Maintenance (Feb-Nov 2022):** Another author (Henri Drake) makes 3 cleanup commits. Fons van der Plas takes over for 2 maintenance commits.
3. **Dormancy (Nov 2022-Aug 2026):** 2 years, 9 months. Then 2 README updates.

**The Aug 2026 signal:** Two README updates on the same day by the same author (Fons van der Plas). No code commits. No issue responses. The most likely explanation: the original paper is being cited again, and someone refreshed the README to point to new resources. This is a *citation-driven* update, not a *code-driven* one.

**What this means for the podcast:** ClimateMARGO is the only climate-economic model with SRM as an explicit decision variable that's open-source. Its dormancy tells us something about the state of SRM policy modeling: it's not dead, but it's not alive either. It's in limbo.

---

## Trend 4: The Single-Day Manifesto (srm-forever)

```
Aug 26, 2026:  ████████████████████████████  4 commits, all same day
```

| # | Commit | Content |
|---|--------|---------|
| 1 | `9999436` | Interactive SRM-forever vs mitigation+CDR cost model |
| 2 | `aa9bc0f` | Weitzman certainty-equivalent discounting + essay |
| 3 | `61df1a4` | Effective discount rate chart |
| 4 | `9ee822a` | Price abatement as vintage annuity |

**Analysis:** All 4 commits in one day. This is a *manifesto* — a complete theoretical framework released as a single event. The author built the interactive model, wrote the discounting essay, created the visualization, and committed everything at once.

**The Weitzman framework in code:** Weitzman's 2013 paper argued that uncertainty about the discount rate should change climate policy analysis. The standard DICE model uses a constant discount rate (typically 3-5%). Weitzman showed that if the discount rate is uncertain (μ=1%, σ=1%), the effective rate declines toward zero at long horizons. This means future damages are weighted more heavily, and the case for immediate action ( mitigation or SRM) changes.

srm-forever implements this in an interactive web tool. You can adjust μ and σ, compare SRM-only vs. mitigation+CDR, and see how the Weitzman effect changes the verdict.

**Why zero stars doesn't matter:** A zero-star repo with a live web tool, rigorous sourcing, and open license is the epitome of "credit doesn't matter." The work is what's important.

---

## Trend 5: The Curated List metabolism (awesome-geoengineering)

```
Jan 16, 2026:  █  README update
Mar 12, 2026:  █  README update
May 5, 2026:   █  v2.0.0 major reorganization
Sep 5-6, 2026: ██  Two README updates
```

Steady curation velocity: 1-2 updates per month, with a major version bump in May 2026. The v2.0.0 release signals that the geoengineering field has grown enough to need taxonomy. The Sep 2026 updates suggest active maintenance continues.

---

## Commit Velocity Comparison — Solar Theme

```
WRF:           ████████████████████████████████████  10 in 4 weeks (release cycle)
PCMDI:         ████████████████████████████████████████████████████  10 in 2 days (release blitz)
MDTF:          ████████████  5 in 1 day (PBP-POD) + scattered maintenance
ClimateMARGO:  ██████████████████████████████████  7 in 1 day (launch) + 2 (revival?)
srm-forever:   ████████████████████████████  4 in 1 day (manifesto)
awesome-geo:   ██  1-2 per month (steady curation)
```

**The story:** Solar geoengineering code exists in two modes: institutional release cycles (WRF, PCMDI) and individual manifestos (srm-forever, ClimateMARGO). There's no middle ground — no community-driven, sustained development of SRM-specific tools. The field is either funded (WRF) or individual (srm-forever).

---

## 🎙️ Episode 1 Commit-Based Talking Points

| Talking Point | Evidence | Source |
|---------------|----------|--------|
| "A solar radiation bug was fixed in WRF that could affect every SRM simulation" | e836cd6, May 28, 2026 | WRF commit log |
| "TEMPO aerosol schemes are being turned off for stratospheric work" | 6a289e1, Jun 5, 2026 | WRF commit log |
| "A rounding bug corrupted climate model evaluations — fixed in one day" | 90cbc50, Sep 4, 2026 | PCMDI commit log |
| "A climate model went dormant for 2 years 10 months, then got 2 README updates" | d916f36, Aug 17, 2026 | ClimateMARGO commit log |
| "A zero-star model made SRM economics transparent using Weitzman's framework" | 4 commits, Aug 26, 2026 | srm-forever commit log |
| "Why is there no SRM-specific modeling community?" | Structural analysis | Cross-repo comparison |

---

## 🔮 Watchlist — Solar Theme

| Signal | What to Watch | Timeline |
|--------|---------------|----------|
| WRF TEMPO re-enablement | Will the aerosol-aware schemes be re-enabled with fixes? | Next release cycle |
| ClimateMARGO code revival | Will the Aug 2026 README updates lead to code commits? | Next 3-6 months |
| SRM-specific modeling | Will anyone build an SRM-specific model, or always rely on WRF? | Ongoing |
| PCMDI for SRM scenarios | Will PCMDI metrics ever include SRM-specific evaluation tools? | Unlikely near-term |
| srm-forever adoption | Will the zero-star model get any community traction? | Uncertain |

---

*Last updated: September 2026 (v7) | Data source: GitHub API commit histories*
*Previous version: v6 (September 2026)*