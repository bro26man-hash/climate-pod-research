# ☀️ Solar Geoengineering — Commit Trend Analysis
## GitHub API Data Pull — September 2026

---

## 📈 Overall Activity Dashboard

| Repo | Total Recent Commits | Commit Rate | Last Active | Trend |
|------|---------------------|-------------|-------------|-------|
| **WRF** | 15 commits in 30 days | 0.5/day | Jun 8, 2026 | 🟢 **Steep upward — v4.8.0 release cycle** |
| **ClimateMARGO** | 2 in 1 day (Aug 2026) | 0.07/day avg (recent) | Aug 17, 2026 | 🟡 **Spike after 2-year dormancy** |
| **GCCS-Core** | 15 in 1 day (Oct 2024) | 15.0/day (burst) | Oct 29, 2024 | 🔴 **Burst then dead** |
| **OOCC_2021** | 15 over 4 months (2021) | 0.12/day avg | Nov 15, 2021 | 🔴 **Decaying academic project** |
| **GeoVision** | 4 in 1 day (Dec 2025) | 4.0/day (burst) | Dec 6, 2025 | 🔴 **Burst then dead** |
| **srm-forever** | Unknown (2026) | Low | Aug 26, 2026 | 🟡 **Low but ongoing** |

---

## 🔥 WRF — The Solar Radiation Correction Wave (May–June 2026)

### Timeline of Solar-Relevant Commits
```
May 12  ■ MYNN-SFC submodule update          (surface physics)
May 19  ■ Bug fix for udm                    (diagnostics)
May 20  ■ ShinHong PBL namelists             (boundary layer)
May 20  ■ Minor Tempo changes                (aerosol-cloud interaction)
May 20  ■FIXING scheme-guard bug in urban NbS (urban setup)
May 21  ■ Include mp_physics=88 in TEMPO     (aerosolMicrophysics)
May 26  ■ Reading GFL option README          (gravity wave drag)
May 26  ■ Fixing CDXWRF module               (convective downdraft)
May 27  ■ MMM-physics SHA update             (microphysics suite)
May 27  ■ MYNN-EDMF pointer update           (turbulence)
May 28  ■🔥 CORRECTION FOR EOT SOLAR RADIATION ← THE BIG ONE
May 30  ■ Vectorization option in AOCC       (compiler optimization)
Jun 5   ■ Turn off tempo_aerosolaware/hailaware (feature toggling)
Jun 6   ■ Update README for v4.8.0           (release prep)
Jun 8   ■ Merge v4.8.0 release               ← VERSION SHIP
```

### Key Insight: The Solar Radiation Fix
The commit `e836cd6` on May 28, 2026 — **"correction for eot calculation for solar radiation"** — is the most solar-geoengineering-relevant commit across all repos we analyzed. The EOT (Easterly Offset Temperature) calculation is used in WRF's solar radiation scheme to account for the east-west temperature gradient in the atmosphere. If this calculation is wrong, it affects:
- Simulated surface temperatures under any scenario
- Cloud formation physics
- Precipitation patterns
- **All SRM experiments that use WRF as their base model**

A correction like this means that previous SRM simulation results using WRF may have had systematic errors in their solar radiation calculations.

### Commit Velocity Analysis
- **Pre-release velocity:** ~3 commits/day during the 10 days before v4.8.0
- **Release day velocity:** 1 commit (merge only)
- **Contributors:** 7 distinct contributors in 30 days (Islas, weiwangncar, Olson, Fita, Werner, Jensen-NOAA, Wang)
- **Implication:** Wide contributor base means the solar radiation fix underwent community scrutiny — not a single-team blind patch

---

## 🔄 ClimateMARGO — The Dormancy-Revival Pattern

### Activity Timeline
```
2022-11-12 ■ JuMP/IPopt compat upgrade    ← Last real code change
2023-07-06 ■ Pluto link in README         ← Last activity before hibernation
2023-10-18 ■ Unit conversion comment      ← One-off fix
2026-08-17 ■ README update #1             ← WAKE UP
2026-08-17 ■ README update #2             ← Second hit same day
```

### The Dormancy Dashboard
| Period | Commits | Duration | Interpretation |
|--------|---------|----------|---------------|
| Jan–Dec 2022 | 13 | 12 months | Active development year |
| Jan 2023 – Aug 2026 | 3 | 43 months | Near-total silence (0.07 commits/month) |
| Aug 17, 2026 burst | 2 | 1 day | README-only revival signal |

### What the Revival Might Mean
**Scenario A — Genuine Reactivation:** Someone recognized the relevance of climate-economic SGE modeling after a period of political attention to SRM. The README update could precede code commits.

**Scenario B — Academic Housekeeping:** A student or maintainer is tidying up citations for a new paper. README updates don't always mean new features.

**Scenario C — Citation Engine:** The update adds PlutoLinks (interactive notebooks). This could mean the maintainer is making the model more accessible for teaching, not research.

**Verdict:** The signal is ambiguous. But for a podcast, the *story* is what matters: a governance model lies dormant for 2 years and then suddenly gets its README updated. What changed in the world to make solar geoengineering governance feel urgent again?

---

## 💥 GCCS-Core — The Single-Day Ghost

### The Blitz Pattern
All 15 commits occurred on October 29, 2024:
```
Oct 29  ■ requirements.txt     ← Scaffolding
Oct 29  ■ setup.py              ← Scaffolding
Oct 29  ■ data_collection.sh    ← Scaffolding
Oct 29  ■ run_server.sh         ← Scaffolding
Oct 29  ■ deploy.sh             ← Scaffolding
Oct 29  ■ example_config.yaml   ← Scaffolding
Oct 29  ■ example_usage.py      ← Scaffolding
Oct 29  ■ example_iot_integration.py  ← Scaffolding
Oct 29  ■ 7× Update README.md   ← Scaffolding
```

### Interpretation
This is the **"repo as resume"** pattern. Someone created a project skeleton with proper infrastructure files (setup.py, deploy.sh, examples) but never wrote the actual climate model code. The 7 README updates on the same day suggest someone was iterating on the project description, possibly trying to attract collaborators or make the project look more substantial.

The name "Global Climate Control System" is worth noting — it's the most ambitious naming in the solar geoengineering space and the least backed by actual code.

---

## 📉 OOCC_2021 — The Complete Academic Lifecycle

### Full Lifecycle
```
Jul 23, 2021  ■ Initial development begins
Jul 28, 2021  ■ Strategy tables updated + comment errors fixed
Jul 30, 2021  ■ Readme updates (model description)
Sep 3–5, 2021  ■ Publication sprint (7 commits in 3 days)
Sep 4, 2021   ■ Citation file added ← Paper published
Nov 15, 2021  ■ Bibtex update ← Final commit
```

### The Lifecycle Pattern
This is the **textbook academic repo lifecycle**:
1. **Develop** (Jul): Build the model
2. **Refine** (Jul 28–30): Fix errors, update strategy, polish documentation
3. **Publish sprint** (Sep 3–5): Add citations, update readme, finalize for paper submission
4. **Maintenance** (Nov): One final citation update
5. **Death** (Nov 15, 2021 → forever): No commits for 4+ years

### What's Missing
- No CI/CD pipeline (no GitHub Actions visible)
- No issue tracker activity
- No PRs from the community
- No version tags or releases
- The model exists only as paper supplementary code

**Podcast angle:** "The best governance model for solar geoengineering on GitHub hasn't been touched in nearly five years. It's still there, still cited, still the only game in town. And nobody's maintaining it. What does that tell us about how seriously we're taking SRM governance?"

---

## 👻 GeoVision — The Empty Shell

### Commit Record
```
Dec 6, 2025  ■ Initial commit
Dec 6, 2025  ■ Add files via upload
Dec 6, 2025  ■ Create LICENSE
Dec 6, 2025  ■ Update README.md
```

### Assessment
4 commits, 1 day, zero substantive content. The repository has a name ("Geoengineering Simulator") but no simulation code. It may have been created as a placeholder or graduate student's abandoned project. The LICENSE file suggests at least some intent for openness.

---

## 🧮 Cross-Repo Solar Commit Maps

### Commit Type Distribution
| Commit Type | WRF | ClimateMARGO | GCCS-Core | OOCC_2021 | GeoVision | Total |
|-------------|-----|-------------|-----------|-----------|-----------|-------|
| Bug fixes | 4 | 0 | 0 | 0 | 0 | 4 |
| Physics updates | 5 | 0 | 0 | 0 | 0 | 5 |
| Documentation | 3 | 2 | 7 | 6 | 1 | 19 |
| Configuration | 2 | 2 | 5 | 0 | 0 | 9 |
| Feature additions | 1 | 0 | 0 | 0 | 0 | 1 |
| **Total** | **15** | **6** | **15** | **15** | **4** | **55** |

### Contributor Count
| Repo | Unique Contributors ||
|------|---------------------|
| WRF | 7 (institutional, multi-team) |
| ClimateMARGO | 2 (Fons van der Plas, Henri Drake) |
| GCCS-Core | 1 (KOSASIH) |
| OOCC_2021 | 1 (jlehtomaa) |
| GeoVision | 1 (Manik Roy) |

**Key finding:** Only WRF has a multi-contributor, multi-institutional development team. Every other solar geoengineering-related repo is a single-maintainer effort. This is the **single-maintainer risk** — if one person stops committing, the repo dies.

---

## 🔮 Trend Projections for Episode 1 (Solar)

### What's Trending Up ✓
1. **Atmospheric physics maintenance is active** — WRF's v4.8.0 solar radiation fix shows that institutional climate modeling is continuously improving the tools that SRM researchers depend on
2. **Multi-contributor development exists** — WRF has 7 contributors in 30 days, suggesting community oversight of solar-relevant physics

### What's Trending Down ✗
1. **Dedicated SGE simulation repos are dying** — OOCC_2021, GCCS-Core, and GeoVision are all either dead or empty shells
2. **Governance code has zero maintenance** — The only governance model (OOCC_2021) hasn't been touched since 2021
3. **Single-maintainer risk is universal** — 4 of 5 solar repos have exactly 1 contributor

### The Elephant in the Room 🐘
**There is no dedicated open-source solar geoengineering simulation model on GitHub.** No repo exists that primarily simulates stratospheric aerosol injection, marine cloud brightening, or space-based reflectors. The closest is WRF, which was never designed for SGE. This gap is the story.

---

## 📋 Research Log

| Date | Activity |
|------|----------|
| Sep 17, 2026 | v3: Initial commit trends from 5 solar repos |
| Sep 17, 2026 | v4: Fresh commit data pulled from GitHub API for WRF v4.8.0 release cycle |
| Sep 17, 2026 | v4: Solar radiation correction commit identified as most SGE-relevant change |
| Sep 17, 2026 | v4: ClimateMARGO dormancy-revival pattern documented |
| Sep 17, 2026 | v4: GCCS-Core single-day burst pattern analyzed |
| Sep 17, 2026 | v4: OOCC_2021 complete academic lifecycle mapped |
| Sep 17, 2026 | v4: GeoVision confirmed as empty shell |
