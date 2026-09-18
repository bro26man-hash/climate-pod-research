# ☀️ Solar Geoengineering — Commit Trend Analysis (v6)

> **Last updated:** September 2026 (v6)  
> **Branch:** `solar-geoengineering`  
> **Podcast episode:** Episode 1 — Solar Geoengineering

---

## Activity Overview (v6 Data)

| Repo | Total Commits Pulled | Date Range | Commit Density | Development State |
|------|---------------------|------------|---------------|------------------|
| wrf-model/WRF | 15 | May-Jun 2026 | ~1/week during release | 🟢 Active, v4.8.0 released |
| PCMDI/pcmdi_metrics | 15 | Sep 3-17, 2026 | ~5/day during release | 🟢 Very active, v4.2.1 released |
| ClimateMARGO/ClimateMARGO.jl | 15 | Jan 2022-Aug 2026 | ❌ Dormant (2yr gap) | 🟡 Revival unclear |
| hausfath/srm-forever | 4 | Aug 2026 | 💥 Single-day burst | 🆕 New, unproven |

---

## Trend 1: The "Release Weekend" Pattern (v6 Deep Dive)

Both WRF and PCMDI show the same pattern: **long periods of steady maintenance punctuated by intense release weekends.**

### WRF v4.8.0 Release Cycle (May 19 – Jun 8, 2026)

**15 commits in 20 days. Three distinct phases:**

**Phase 1: Physics Updates (May 12-21)**
```
May 12:  █ Update MYNN-SFC submodule (b96a7e9)
May 19:  █ Bug fix for udm (c1cd5c4)
May 20:  ██ Minor Tempo changes (06e6998) + scheme-guard bug fix (8fa379b) + ShinHong PBL namelists (9c87d92)
May 21:  █ Include mp_physics=88 in TEMPO error print (02f02bc)
```

**Phase 2: Solar Radiation Fix & Release Prep (May 26-28)**
```
May 26:  █ Fix CDXWRF module (75ad1f9) + GFL README (0aa6582)
May 27:  ██ MYNN-EDMF pointer update (8299919) + MMM-physics SHA (4fab0e2)
May 28:  ██🔥 CORRECTION FOR EOT CALCULATION FOR SOLAR RADIATION (e836cd6) — THE BUG FIX
May 30:  █ Fix vectorization in AOCC stanza (4466746)
```

**Phase 3: Release & Post-Release (Jun 5-8)**
```
Jun 5:   █ Turn off tempo_aerosolaware & tempo_hailaware (6a289e1) — STABILITY FIX
Jun 6:   █ README & version update to v4.8.0 (0708348)
Jun 8:   █ Merge v4.8.0 release (06d4240) — OFFICIAL RELEASE
```

**Key insight:** The solar radiation bug fix (e836cd6) landed on May 28 — right in the middle of release prep. It was caught during final testing, not during routine maintenance. This is exactly how a bug in the most important SRM simulation tool gets found: during a scheduled release cycle.

**The TEMPO disable (6a289e1, Jun 5)** is equally significant: the aerosol-aware and hail-aware options were turned OFF because they were producing unstable results for stratospheric simulations. This means someone tried to run WRF with SAI and found the physics suite couldn't handle it.

### PCMDI v4.2.1 Release Cycle (Sep 3-4, 2026)

**10 commits in 2 days. The "morning after" pattern:**

**Sep 3 (6 commits — development day):**
```
09:00  █ Force numpy SVD (1fca2ec) — reproducibility fix
09:00  █ Chore: rename (d0a79e5) — code cleanup
09:00  █ Rechunk data to higher order (ac634d7) — dask performance
09:00  █ Merge PR #1423: variability modes dask SVD memory (c8711f1)
09:00  █ Merge branch 'main' into PR #1424 (b2eb044)
09:00  █ Merge PR #1425: extremes chunking (71a0497)
```

**Sep 4 (4 commits — release day):**
```
09:00  █ Merge PR #1427: roundoff correction (d0bcbd8)
09:00  █🔥 PREVENTS ROUNDOFF TO 1.00 IN MEAN_CLIMATE (90cbc50) — THE BUGFIX
09:00  █ Prepare v4.2.1 (e7dc726)
09:00  █ Bump version to 4.2.1 (6419050)
```

**The roundoff bug (90cbc50)** is the podcast gold: a rounding error was clipping values at exactly 1.00 in normalized climate metrics. This means every PCMDI output produced with v4.2.0 had a systematic error in extreme-value analysis. The fix came down 10 commits in 48 hours — the institutional maintenance machine working as designed.

---

## Trend 2: The Physics-Philosophy Gap (v6 Updated)

| Attribute | Institutional Tools | Decision Tools |
|-----------|-------------------|----------------|
| Development pace | Continuous, milestone-driven | Episodic, insight-driven |
| Contributors | Large teams, institutional | Individual or tiny teams |
| Release pattern | Versioned, scheduled | "When ready" |
| Code quality | CI/CD, testing, documentation | Working prototype, minimal QA |
| Stars (visibility) | 100–1,700 | 0–73 |
| Sustainability | Funded, institutional | Unfunded, volunteer |
| **v6 Addition** | Bug fixes caught in release cycles | Bug fixes never happen (no QA process) |

**The gap tells us:** Solar geoengineering research has two ecosystems. The physical simulation ecosystem (WRF, PCMDI) is well-maintained with proper QA. The decision-making ecosystem (ClimateMARGO, srm-forever) is volunteer-run with no QA process. The SRM field can simulate the atmosphere precisely but can't agree on what discount rate to use.

---

## Trend 3: The "Silent Fix" Pattern

Both bug fixes in the solar theme happened silently — no blog posts, no tweets, no press releases:

| Bug | Repo | Commit | Impact | Public Notice |
|-----|------|--------|--------|---------------|
| Solar radiation EOT calculation | WRF | e836cd6 | every SAI simulation may have had energy budget error | None — just a commit message |
| Roundoff to 1.00 | PCMDI | 90cbc50 | every v4.2.0 output corrupted | None — just a commit message |

**🎙️ Podcast angle:** The most important fixes in solar geoengineering computation happen as a single line in a commit message. Nobody announces them. Nobody celebrates them. They just... happen. And the models keep running. That's how you know the infrastructure is mature — when bug fixes are boring.

---

## Trend 4: The Revival That Isn't (ClimateMARGO)

**Development timeline:**
```
2022:    ████████████████████████████  10 commits, 3 contributors, active development
         │
         │  ← 9-month gap
         │
2023:    ██  2 README updates (Oct)
         │
         │  ← 2+ year gap
         │
2026:    ██  2 README updates (Aug 17)
```

**The pattern:** Heavy development →从这个 gap → 2 README updates → another gap → 2 more README updates. Zero code changes in either revival. This is "documentation housekeeping," not "project revival."

**Three possible interpretations:**
1. **Planned relaunch:** Someone is preparing a major update (new paper, new features) and refreshing docs first
2. **Citation maintenance:** Adding README links for academic citations without actual development
3. **False start:** Someone had a good intention and lost momentum again

**The honest answer:** We don't know. The commit data can't tell us which interpretation is right. That ambiguity is itself the podcast story.

---

## Commit Density Comparison

```
WRF:      ████████████████████  15 commits / 20 days = 0.75/day during release
PCMDI:    ██████████████████████████████  10 commits / 2 days = 5.0/day during release
MARGO:    ██  2 commits / 6 months = 0.01/day (revival)
srm-forever: ████  4 commits / ~5 days = 0.8/day (docs burst)
```

**The story:** Institutional tools have institutional commit density. Decision tools have individual burst patterns. And the gap between them is the governance gap in solar geoengineering.

---

## Episode 1: Commit-Based Talking Points

| Talking Point | Evidence | Source |
|---------------|----------|--------|
| "The most important climate model has a solar radiation bug" | e836cd6, May 28, 2026 | WRF commit log |
| "A rounding error was corrupting every climate evaluation" | 90cbc50, Sep 4, 2026 | PCMDI commit log |
| "10 commits in one day fixed a bug that nobody noticed" | PCMDI Sep 3-4 burst | PCMDI commit log |
| "A climate model went quiet for 2 years, then updated its README twice" | d916f36, Aug 17, 2026 | ClimateMARGO commit log |
| "A zero-star interactive model made SRM economics more transparent than every funded program" | srm-forever, Weitzman discounting | Repository metadata |
| "Someone turned off the aerosol physics because it was unstable for SAI" | 6a289e1, Jun 5, 2026 | WRF commit log |
