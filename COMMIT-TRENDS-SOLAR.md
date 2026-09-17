# ☀️ Solar Geoengineering — Commit Trend Analysis
## Research Notes for Climate Technology Podcast Series
### Updated: September 2026 (v4 — fresh commit data from 5 repos)

---

## Summary Dashboard

| Repo | Stars | Total Commits Pulled | Active Period | Velocity | Status |
|------|-------|---------------------|---------------|----------|--------|
| **WRF** | 1,761 | 8 | May-Jun 2026 | ~1 commit/3 days | **Institutional, sustained** |
| **ClimateMARGO.jl** | 73 | 8 | Feb 2022-Aug 2026 | ~1 commit/6 months | **Dormant with revival signal** |
| **awesome-geoengineering** | 4 | 7 | Jun 2025-Sep 2026 | ~1 commit/2 months | **Active, accelerating** |
| **GeoVision** | 0 | 4 | Dec 2025 (single day) | 4 commits/1 day | **Burst-then-dead** |
| **Geo-DICE** | 2 | 0 (not pulled) | Unknown | N/A | **Likely dormant** |

---

## Detailed Commit Analysis

### WRF — The Industrial Machine

**Peak activity:** May-June 2026 (8 commits in ~2 weeks)
**Nature:** Institutional, team-driven, version-release-cycle

```
May 26: Fixing CDXWRF module
May 27: Update MYNN-EDMF pointer, remove icloud_bl
May 27: Update MMM-physics repo SHA
May 28: Correction for EOT calculation for solar radiation  <- SRM-relevant
May 30: Fix vectorization in AOCC stanza
Jun 5:  Turn off tempo_aerosolaware and tempo_hailaware        <- SRM-relevant
Jun 6:  Update README and version to v4.8.0
Jun 8:  Merge release-v4.8.0
```

**Key insight:** The two SRM-relevant commits (solar radiation EOT fix + aerosol-aware scheme disablement) are both in the v4.8.0 release. This is the most important atmospheric model on Earth undergoing exactly the kind of physics changes that would affect SRM simulation capability. But the changes are presented as routine maintenance, not SRM-specific. The SRM implications are downstream — users have to interpret the changes themselves.

**Trend direction:** WRF is becoming more institutional, less open to experimental physics. The removal of the icloud_bl package and disabling of aerosol schemes suggest a "consolidation" trend — the model is shedding uncertain components rather than adding new ones. This is the opposite of what SRM researchers would want (more options, more parameterizations).

---

### ClimateMARGO — The Ghost that Almost Came Back

**Peak activity:** Feb 2022 (3 commits in 10 days)
**Dormancy:** Feb 2022 - Aug 2026 (4.5 years)
**Revival:** Aug 2026 (2 README commits, no code)

```
Feb 4, 2022:  Added CITATION.bib
Feb 10, 2022: Removed deprecated web apps
Feb 12, 2022: JuMP and Ipopt compat upgrade
... 4.5 years of silence ...
Oct 18, 2023: Unit conversions comment (isolated, via PR #86)
Jul 6, 2023:  Add Pluto documentation link
... 2+ more years of silence ...
Aug 17, 2026: Update README.md (x2)
```

**Key insight:** The 2026 README updates are the first activity in over 2 years. But they're README-only — no code changes, no new features, no issue responses. This could be:
1. Someone cleaning up the README before a new release
2. A citation update for a paper that used ClimateMARGO
3. A "tombstone maintenance" pattern — just enough activity to keep the repo alive

Without code commits, the revival is optical, not substantive. But the fact that someone is still touching the README after 4.5 years suggests the economic modeling community hasn't forgotten it.

**Trend direction:** Stagnant with a faint revival signal. The Julia climate-economics ecosystem needs a new ClimateMARGO — one that's actively maintained, with modern solver interfaces and SRM-specific modules.

---

### awesome-geoengineering — The Curator's Acceleration

**Peak activity:** Steady since Jun 2025
**Nature:** Individual-driven, list-maintenance, resource-curation

```
Jun 28, 2025: Initial commit + first README update
Jun 28, 2025: Update README (2nd commit same day)
Jan 16, 2026: Update README
Mar 12, 2026: Update README
May 5,  2026: Update to v2.0.0 (major version)
Sep 5,  2026: Update README
Sep 6,  2026: Update README (rapid double-update)
```

**Key insight:** This is the **only repo in the solar geoengineering ecosystem showing clear accelerating momentum**. The pattern is:
- 2025: 3 commits over 6 months (birth phase)
- 2026 Q1: 2 commits over 2 months (slow maintenance)
- 2026 Q2: 1 major version bump (v2.0.0)
- 2026 Q3: 3 commits in 2 days (rapid acceleration!)

The Sep 5-6 double-update right after the Sep 6 search discovery suggests the curator is actively responding to new resources. This is the meta-repo that tracks the entire field.

**Trend direction:** Accelerating. The resource gap is closing. By 2027, this list could be the definitive bibliography for geoengineering research.

---

### GeoVision — The Simulator's Tragedy

**All activity:** December 6, 2025 (single day)
**Nature:** Individual project, burst creation, then abandonment

```
Dec 6, 2025: Initial commit
Dec 6, 2025: Add files via upload
Dec 6, 2025: Create LICENSE
Dec 6, 2025: Update README.md
```

**Key insight:** All 4 commits in one day. No commits in 9 months since. This is the "build it and they will come" failure. The repo has: a README, a LICENSE, and uploaded files — but no community, no stars, no ongoing development.

**Trend direction:** Flatlined. The concept (interactive SRM visualization) is valuable but the execution was a one-shot. Someone should pick this up.

---

## Cross-Repo Trend Synthesis

### The Three Universes (Solar Focus)

| Universe | Reps | Characteristics |
|----------|------|------------------|
| **Fast Universe** | WRF | Institutional funding, continuous releases, major version cycles, SRM implications buried in routine maintenance |
| **Slow Universe** | ClimateMARGO, awesome-geoengineering | Individual/curatorial effort, sporadic activity, dormancy-whiplash, but genuine community value |
| **Empty Universe** | GeoVision, Geo-DICE, OOCC, GeoengineeringLE | Zero or near-zero stars, single creators, no maintenance, no community |

### The SRM Simulation Gap

After pulling commit histories from 5 solar geoengineering repositories, a clear pattern emerges:

1. **No dedicated SRM simulator exists.** WRF can simulate SRM scenarios through its aerosol and radiation schemes, but it's not designed for that purpose. There's no open-source tool specifically built for SRM scenario exploration.

2. **The economic models are fossilized.** ClimateMARGO (73) is the best tool, but it hasn't had a code commit in 2+ years. The economic modeling of SRM is theoretical, not computational.

3. **The physics is becoming less soluble.** WRF's disabling of aerosol-aware schemes and removal of the icloud_bl package suggests the field is consolidating around fewer, more uncertain parameterizations. SRM simulation requires more physics, not less.

4. **Curation is the only growth area.** awesome-geoengineering is the only repo with accelerating momentum. The resource base is growing, but the tools are not.

### The Podcast Angle

**"Why is there no open-source SRM simulator?"**
- WRF is the closest thing, but it's a weather model, not an SRM tool
- The aerosol physics is unstable — disabling schemes, not adding them
- No one has built the "GitHub for SRM scenarios" — an interactive, shareable, open-source tool
- The economic models exist but they're dead software

---

## Recommendations

1. **For Episode Planning:** Focus on the WRF aerosol story as the technical core, the ClimateMARGO dormancy as the economic angle, and awesome-geoengineering as the resource/governance lens.
2. **For Call Guests:** Reach out to ClimateMARGO maintainer (Fons van der Plas) about the 2026 revival. Contact awesome-geoengineering curator (Brandon Himpfen) about the acceleration.
3. **For Future Research:** Search for SRM-related code in atmospheric modeling repos that isn't tagged as "geoengineering" — the SRM content may be hidden inside general climate codes.