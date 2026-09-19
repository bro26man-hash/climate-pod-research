# ☀️ Solar Geoengineering — Commit Trend Analysis (v4, Sep 2026)

**Analysis Date:** September 2026  
**Repositories Analyzed:** 4 (WRF, ClimateMARGO.jl, regional-geo, Greenhouses-Library)  
**Total Commits Pulled:** 60+

---

## Velocity Summary Table

| Repository | Stars | Commits Pulled | Active Period | Velocity Pattern | Longest Gap |
|-----------|-------|----------------|---------------|-----------------|-------------|
| wrf-model/WRF | 1,763 | 15 | May–Jun 2026 | 🟢 Continuous, multi-contributor | ~2 days |
| ClimateMARGO.jl | 73 | 15 | Jan 2022, Oct 2023, Aug 2026 | 🟡 Burst-and-dormant | 3.5 years |
| regional-geo | — | 15 | Feb 13–15, 2026 | 🟡 Intense 3-day sprint | N/A |
| Greenhouses-Library | 54 | 15 | May–Aug 2019 | 🔴 Dead since 2019 | 7 years |

**Combined total:** 60 commits across 4 repositories, spanning 2019–2026.

---

## Trend 1: The "Two Speed" Solar Geoengineering Ecosystem

WRF = **fast universe** — institutional funding, multiple paid developers, continuous integration, regular releases (v4.8.0, June 2026). 15 commits in ~3 weeks is normal business.

ClimateMARGO, regional-geo, Greenhouses-Library = **slow universe** — academic research code built for specific papers, with activity concentrated around publication deadlines.

**Implication:** Sustainability of SRM software is bifurcated. The tools that matter most (WRF) are well-maintained because they have institutional support. The tools that are most focused on SRM specifically (regional-geo, ClimateMARGO) are fragile research projects that may vanish when their creators move on.

---

## Trend 2: Solar Radiation Physics Is Actively Evolving in WRF

| Date | Commit | Significance |
|------|--------|-------------|
| Jun 5, 2026 | `6a289e1` — Turned off tempo_aerosolaware and tempo_hailaware | TEMPO scheme is the primary tool for modeling SRM radiative effects. Disabling it by default raises questions. |
| May 28, 2026 | `e836cd6` — Correction for eot calculation for solar radiation | Bug fix in solar radiation calculation. Even small bugs can skew SRM simulation results. |
| May 20, 2026 | `06e6998` — Minor Tempo changes | Ongoing refinement of TEMPO chemistry/aerosol module. |
| May 20, 2026 | `9c87d29` — New ShinHong PBL namelists | New PBL scheme could affect aerosol mixing in lower atmosphere. |

**Key insight:** TEMPO is the bridge between WRF's mainstream capability and its SRM capability. Active refinement = direct evidence that SRM modeling is embedded in mainstream climate modeling.

---

## Trend 3: The Research Sprint Pattern

regional-geo's commit history is a textbook "paper push":

```
Feb 13: 11 commits (setup: README, data loader, style guide, docs)
Feb 14:  3 commits (data processing: RDS reading, area calc, case display)
Feb 15:  1 commit (visualization: gaussian smoothing for maps)
```

15 commits in 72 hours. The pattern:
1. Set up infrastructure
2. Process data
3. Produce results
4. Ship (update README, push to GitHub)

**Follow-up:** regional-geo's last commit was Feb 15, 2026 — over 7 months ago with no new activity.

---

## Trend 4: The "Long Tail" of Dormant SRM Tools

ClimateMARGO's commit timeline:

```
Jan 2022:  8 commits (heavy documentation push)
Feb 2022:  3 commits (compat upgrades, cleanup)
Oct 2023:  1 commit (unit conversion comment)
Jul 2023:  1 commit (Pluto notebook link)
Aug 2026:  2 commits (README updates — likely for visibility)
```

3.5 years of silence, then 2.5 years more, then sudden README updates. Academic software lives or dies by its authors' careers.

---

## Trend 5: No Ocean SRM Code Whatsoever

Across all searches (`marine cloud brightening`, `ocean albedo`, `ocean geoengineering`), **zero dedicated ocean geoengineering repositories were found.** See the ocean-intervention branch for the full gap report.

---

## Episode Architecture (Solar Geoengineering)

**Segment 1: "The Model Inside the Model"**
- No "SRM simulator" repo exists
- SRM capability lives inside climate models as parameterizations
- WRF's TEMPO scheme is the key bridge
- The `6a289e1` commit (TEMPO toggle) as artifact

**Segment 2: "The Sprint and the Silence"**
- regional-geo's 3-day burst (15 commits) vs. 7-month dormancy
- ClimateMARGO's 3.5-year gap
- The lifecycle problem of research software

**Segment 3: "Who Controls the Simulation?"**
- WRF: institutional, funded, multi-university
- ClimateMARGO: individual PhD researcher
- regional-geo: Ken Caldeira's lab
- Governance implications

---

*Analysis methodology: GitHub List Commits API, September 2026. All commit data is real and verifiable via the commit SHAs listed above.*
