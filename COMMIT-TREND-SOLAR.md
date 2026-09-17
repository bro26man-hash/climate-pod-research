# 📊 Solar Geoengineering — Commit Trend Summary

**Data source:** GitHub API — 6 repositories, ~5 most recent commits each, pulled Sep 2026

---

## Repositories Analyzed

| Repo | Stars | Lang | Last Commit | Activity Level |
|------|-------|------|-------------|----------------|
| ClimateMARGO/ClimateMARGO.jl | 73 | Julia | Aug 17, 2026 | 🔄 Revival (2 commits after 2yr gap) |
| wrf-model/WRF | 1,761 | Fortran | Sep 2026 | 🔥 Highly Active (v4.8.0 release) |
| NOAA-GFDL/MDTF-diagnostics | 80 | Jupyter | Aug 14, 2026 | 🔥 Active (v4.2.1 release) |
| jlehtomaa/OOCC_2021 | 2 | Python | Nov 15, 2021 | 💤 Dormant (5yr no commits) |
| PSLmodels/Geo-DICE | 2 | Matlab | 2026 | 💤 Low Activity |
| brandomhimpfen/awesome-geoengineering | 4 | Python | Sep 6, 2026 | 🔄 Maintained |

---

## Key Findings

### 1. The "Two-Speed Ecosystem"
- **Fast tier:** WRF, MDTF-diagnostics — institutional funding → continuous commits → regular releases
- **Slow tier:** OOCC_2021, Geo-DICE,ClimateMARGO — individual/small-team → dormant for years → occasional README bumps
- **Implication:** SRM simulation depends on tools built for other purposes. The dedicated SRM code layer is thin.

### 2. ClimateMARGO's Aug 2026 Anomaly
- Two README updates on the same day (d916f36, 6d9ba7a) after 2+ years of complete silence
- Prior significant commit: Oct 2023 (unit_conversions.jl fix referencing community issue #86)
- Before that: Jul 2023 (PlutoDB link), Nov 2022 (Project.toml bump)
- **Interpretation:** Could be a release prep, a reproducibility push, or just a maintenance flutter. The fact that the same author makes both commits suggests a single maintainer, not a community revival.

### 3. The Fortran Lock-In
- WRF (1,761★) and most atmospheric models are Fortran-based
- The newer ocean/climate tools (Oceananigans.jl, veros, ClimateMARGO.jl) have moved to Julia/Python
- But the SRM simulation pipeline still depends on Fortran atmospheric dynamics
- **Cultural implication:** The SRM modeling community inherits the WRF stack but can't easily extend it

### 4. Governance Gap
- Only 1 of 6 solar repos (OOCC_2021) addresses governance/policy modeling
- All others are physics/modeling tools
- **Episode implication:** We lack open-source tools for the *political* dimension of SRM

---

## Commit Timeline (Most Recent per Repo)

```
2026-09-16  Oceananigans.jl: closure fix, partial cell fix, solver optimization (Julia)
2026-09-15  veros: dependabot bumps (Python)
2026-08-17  ClimateMARGO.jl: README x2 (Julia)
2026-08-14  MDTF-diagnostics: last recorded update (Jupyter)
2026-06-*   WRF: v4.8.0 release window (Fortran)
2024-02-12  openair-cyan: OSHWA certification commits (Python)
2021-11-15  OOCC_2021: last commit — bibtex update (Python)
```

---

## Research Gaps Identified

1. **No open-source SRM physics model** — No pure-play solar radiation management codebase with active development
2. **No governance/policy simulation for SRM** — OOCC_2021 is the only attempt and it's dormant
3. **No Python-based atmospheric model** — The accessibility barrier is Fortran; a Python SRM model doesn't exist
4. **No interactive SRM economics tool** — DICE/Geo-DICE are static; no live, adjustable SRM policy simulator

---

*Analysis date: Sep 2026 | Method: GitHub commit API + repository search*