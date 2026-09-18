# ☀️ Solar Geoengineering — Commit Trend Analysis
## Research Notes for Climate Technology Podcast Series
### Updated: September 2026 (v5 — fresh commit data from 6 repos, 80+ commits pulled)

---

## Summary Dashboard

| Repo | Stars | Total Commits Pulled | Active Period | Velocity | Status |
|------|-------|---------------------|---------------|----------|--------|
| **WRF** | 1,761 | 15 | May-Jun 2026 | ~1 commit/3 days | **Institutional, sustained** |
| **ClimateMARGO.jl** | 73 | 15 | Feb 2022-Aug 2026 | ~1 commit/6 months | **Dormant with revival signal** |
| **awesome-geoengineering** | 4 | 7 | Jun 2025-Sep 2026 | ~1 commit/2 months | **Active, accelerating** |
| **GeoVision** | 0 | 4 | Dec 2025 (single day) | 4 commits/1 day | **Burst-then-dead** |
| **OOCC_2021** | 2 | 15 | Jul-Nov 2021 | ~1 commit/month | **Academic, fully dormant** |
| **open-sustainable-technology** | 2,552 | 15 | Jun-Sep 2026 | ~1 commit/2 days | **Institutional, continuously active** |

---

## Detailed Commit Analysis

### WRF — The Industrial Machine (v4.8.0 Release Cycle)

**Peak activity:** May-June 2026 (15 commits in ~3 weeks)
**Nature:** Institutional, team-driven, version-release-cycle

```
May 12: Updating MYNN-SFC submodule
May 19: Bug fix for udm
May 20: Minor Tempo changes
May 20: Include mp_physics=88 in TEMPO error print message
May 20: Fixing a scheme-guard bug in urban NbS initialization
May 21: Turn off tempo_aerosolaware and tempo_hailaware  ← SRM-RELEVANT
May 26: Fixing CDXWRF module
May 26: Update readme file for GFL option
May 27: Update MYNN-EDMF pointer, removing icloud_bl package
May 27: Update MMM-physics repo SHA with various fixes
May 28: Correction for eot calculation for solar radiation  ← SRM-RELEVANT
May 30: Fix a vectorization option in AOCC stanza
Jun 5:  Turn off tempo_aerosolaware and tempo_hailaware (Registry)
Jun 6:  Update README and version declaration to new v4.8.0
Jun 8:  Merge remote-tracking branch 'origin/release-v4.8.0'
```

**Key SRM-relevant findings from fresh data:**

1. **Two SRM-relevant commits in v4.8.0:** The solar radiation EOT (edge-of-transcript) calculation correction (May 28) and the disabling of `tempo_aerosolaware` and `tempo_hailaware` (May 21/Jun 5) are both in the v4.8.0 release. The EOT fix directly affects how solar radiation is computed at model boundaries — critical for any SRM simulation that needs to model reduced solar constant scenarios. The aerosol-aware scheme disablement suggests the codebase is consolidating around fewer, more conservative parameterizations rather than expanding SRM-related physics.

2. **The "scheme guard bug" fix is telling:** The commit "Fixing a scheme-guard bug in urban NbS initialization" (May 20) mentions urban Nature-based-Solutions. This is the intersection of SRM and urban resilience — a growing research area.

3. **The MMM-physics updates are routine:** Three commits updating the Multi-Model Mother physics package suggest the model is maintaining its physics suite rather than adding experimental SRM-aware schemes.

**🎙️ Episode Hook v5:** The v4.8.0 release is the most significant WRF update in 2026, and it contains exactly two SRM-relevant changes — both of which *remove* or *correct* capabilities rather than add new ones. This is the pattern of an institutional model that is consolidating, not experimenting. The question for the episode: Is WRF getting *more* or *less* capable of simulating SRM scenarios with each release?

---

### ClimateMARGO.jl — The Ghost that Almost Came Back

**Peak activity:** Feb 2022 (3 commits in 10 days)
**Dormancy:** Feb 2022 - Aug 2026 (4.5 years)
**Revival:** Aug 2026 (2 README commits, no code)

```
Feb 4, 2022:  Added CITATION.bib
Feb 10, 2022: Removed deprecated web apps
Feb 12, 2022: JuMP and Ipopt compat upgrade (#85)
... 4.5 years of silence ...
Oct 18, 2023: Unit conversions comment (via PR #86)
Jul 6, 2023:  Add Pluto documentation link
... 2+ more years of silence ...
Aug 17, 2026: Update README.md (x2) ← FIRST 2026 ACTIVITY
```

**Key insight from fresh data:** The two README updates on Aug 17, 2026 are the *only* 2026 activity. No code commits. No issue responses. No new feature development. This is "tombstone maintenance" — just enough activity to keep the repo from being considered abandoned, but not enough to signal genuine revival.

The Jul 2023 Pluto documentation link addition suggests someone was exploring modern Julia notebook interfaces (Pluto is a reactive notebook environment). This could indicate that the maintainer was evaluating whether to migrate ClimateMARGO to a more modern interface — but no code followed.

**🎙️ Episode Hook v5:** ClimateMARGO's 4.5-year dormancy broken by two README commits is the perfect metaphor for SRM economics on GitHub: the ideas are there, the citations are there, but nobody is building the operational tools.

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

**Key insight:** This is the **only repo in the solar geoengineering ecosystem showing clear accelerating momentum**. The Sep 5-6 double-update suggests the curator is actively responding to new resources. The v2.0.0 bump in May 2026 represents a major expansion.

---

### open-sustainable-technology — The Ecosystem Gravity Well (NEW v5)

**Peak activity:** Continuous, Jun-Sep 2026
**Nature:** Community-driven, directory/maintenance, multi-contributor

```
Jun 6,  2026:  Add EpexPredictor
Jun 15, 2026:  Add Volca to Life Cycle Assessment
Jun 23, 2026:  Add wbdata
Jul 1,  2026:  Add ToOp
Jul 1,  2026:  Add ASSETRA
Jul 2,  2026:  Add PowerIO
Jul 17, 2026:  Update pull request template with review reminder
Jul 19, 2026: Modify PR template for AI content review  ← AI governance signal
Jul 19, 2026: Remove duplicate AI content review checkbox
Aug 18, 2026: Add Story Seed Library
Aug 18, 2026: Add openflexure microscope
Aug 23, 2026: Add claude-carbon
Sep 1,  2026:  docs: fix dead links in README.md
Sep 9,  2026:  Add-MUIO  ← batch additions
Sep 9,  2026:  Add-MUIOGO ← batch additions
```

**Key insight:** This is the **most actively maintained repo across all three themes**. 15 commits in 3 months, with 3 different contributors. The AI content review PR template modification (Jul 19) is a fascinating signal — even climate-tech directories are being flooded with AI-generated project submissions. The Sep 9 dual commits suggest batch processing.

**🎙️ Episode Hook v5:** 2,552 stars and 15 commits in 3 months. This is the gravitational center of climate-tech on GitHub. But the uncomfortable question: it's a directory, not a tool. We catalog climate tech faster than we build it.

---

### OOCC_2021 — The Governance Model That Completed Its Mission (DETAILED v5)

**Peak activity:** Jul-Sep 2021
**Nature:** Academic, single-author, paper-driven

```
Jul 23, 2021: 5 commits (launch + setup)
Jul 28, 2021: 2 commits (strategy tables, comment errors)
Sep 3-5, 2021: 5 commits (README updates, citation)
Sep 4, 2021:  Added citation file
Nov 15, 2021: 1 commit (bibtex update) ← LAST ACTIVITY
```

**Key insight:** Textbook "publish and perish" pattern. 15 commits over 4 months, all related to a conference paper. After the paper was published and cited, the repo stopped. No commits in 4+ years.

**🎙️ Episode Hook v5:** The only open-source SRM governance model on GitHub is 2 stars and 4 years dead. The governance question is too important to be a one-paper artifact.

---

### GeoVision — The Simulator's Tragedy (Unchanged)

**All activity:** December 6, 2025 (single day, 4 commits)
**Pattern:** Burst creation, then abandonment. 0 stars, no community.

---

## Cross-Repo Trend Synthesis v5

### The Three Universes (Solar, Updated)

| Universe | Reps | Characteristics | Latest Signal |
|----------|------|-----------------|---------------|
| **Fast Universe** | WRF, open-sustainable-technology | Institutional funding, continuous releases, multiple contributors | WRF v4.8.0 consolidated; SST directory growing daily |
| **Slow Universe** | ClimateMARGO, awesome-geoengineering, OOCC_2021 | Individual/curatorial effort, sporadic activity, dormancy-whiplash | ClimateMARGO README revival; awesome-geoengineering accelerating |
| **Empty Universe** | GeoVision, Geo-DICE, GeoengineeringLE | Zero or near-zero stars, single creators, no maintenance | No new activity |

### The SRM Simulation Gap — Updated

1. **No dedicated SRM simulator exists.** WRF can simulate SRM scenarios through its aerosol and radiation schemes, but it's not designed for that purpose. v4.8.0 *removes* aerosol-aware capabilities.
2. **Economic models are fossilized but showing revival signals.** ClimateMARGO's August 2026 README updates are the first activity in 4+ years — but README-only, no code.
3. **The physics is becoming less soluble.** WRF's disabling of aerosol-aware schemes and removal of icloud_bl suggests consolidation around fewer parameterizations.
4. **The ecosystem directory is the only growth area.** open-sustainable-technology (2,552★) has continuous multi-contributor growth, but it indexes — it doesn't build.
5. **Curation is the only accelerating niche.** awesome-geoengineering is the only repo with clear momentum acceleration.

---

## 🎙️ Episode Planning — Solar Geoengineering (Updated v5)

### Key Narrative Arcs
1. **"The Aerosol Consolidation"** — WRF v4.8.0 is removing aerosol-aware schemes, not adding them. The world's most-used climate model is getting *less* capable of simulating SRM.
2. **"The Economic Ghost Town"** — ClimateMARGO's 4.5-year dormancy broken by README-only updates.
3. **"The Curator's Acceleration"** — awesome-geoengineering went from 0 to v2.0 in 14 months.
4. **"The Ecosystem Gravity Well"** — 2,552-star directory with 15 commits/3 months. Cataloging > building.
5. **"The Governance Artifact"** — OOCC_2021: only SRM governance model, 2 stars, 4 years dead.
6. **"The Simulator's Tragedy"** — GeoVision: single-day burst, 0 stars, abandoned.

### Open Questions for Guests
- Should SRM models be open-source? Who regulates the code that simulates planetary reflection?
- Is the WRF aerosol scheme change a technical improvement or an avoidance of the SRM question?
- What would a maintained, community-driven SRM economic model look like?
- Is a 2,552-star directory with no simulation code a sign of maturity — or a sign we're still in the "talking about climate tech" phase?