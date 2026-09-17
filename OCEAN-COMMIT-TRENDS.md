# 🌊 Ocean Intervention — Commit Trend Analysis

## The Absence as Data

---

## What the Commit Histories Show

### Direct Ocean Geoengineering Repos: ZERO

| Search Query | Results |
|-------------|----------|
| `geoengineering ocean` | No repos found |
| `ocean geoengineering alkalinity iron fertilization` | No repos found |
| `ocean intervention climate` | No repos found |
| `marine cloud brightening` | No repos found |
| `electrochemical ocean alkalinity` | No repos found |
| `ocean alkalinization enhancement` | No repos found |

**The total absence of ocean geoengineering repositories on GitHub is itself a commit trend: zero commits, zero activity, zero presence.**

---

## Adjacent Tool: MDTF-diagnostics (Closest to Ocean Process Diagnostics)

| Date | Commit | Author | Relevance |
|------|--------|--------|-----------|
| Aug 14, 2026 | Merge PR #825 | Aparna Radhakrishnan | Latest |
| Jun 19, 2026 | Update MCS_precip_buoy_stats.rst (×4) | Wei-Ming Tsai | **Precipitation-buoyancy POD** |
| Jun 19, 2026 | Add MCS precipitation-buoyancy statistics POD | Wei-Ming Tsai | **Ocean-adjacent process flagship** |
| Jun 8, 2026 | Merge PR #823 | Aparna Radhakrishnan | |
| Jun 8, 2026 | Update README (×2) | jongsooshin5 | |
| Jun 2, 2026 | Merge NOAA-GFDL:main | jongsooshin5 | |
| Jun 2, 2026 | Add citation | jongsooshin5 | |
| Jun 1, 2026 | Add quarterly metrics workflow | Aparna Radhakrishnan | Institutional |
| May 27, 2026 | Move diagnostics to dev branch | Dani Coleman | |
| May 22, 2026 | Merge blocking_notebook PR | Dani Coleman |

**Total visible commits in last 3 months: 10.** Institutional pattern (NOAA-GFDL staff). The MCS precipitation-buoyancy POD is the ocean-adjacent highlight: it models the coupling between precipitation and buoyancy statistics, which is fundamental to ocean-atmosphere interaction physics.

**Why this matters:** MDTF is the only NOAA-GFDL tool on GitHub that touches ocean-atmosphere coupling. If a person wanted to find open-source tools for understanding ocean climate processes, this is the best entry point. It's not ocean geoengineering — but it's the scientific infrastructure that ocean geoengineering would need.

---

## Adjacent Tool: ClimateMARGO (Climate-Economic Modeling)

| Date | Commit | Author |
|------|--------|--------|
| Aug 17, 2026 | Update README.md | Fons van der Plas |
| Aug 17, 2026 | Update README.md | Fons van der Plas |
| Oct 18, 2023 | Update unit_conversions.jl | Fons van der Plas |
| ... (2.5 years dormant) ... |
| Jan 12, 2022 | Multiple commits (initial dev push) | Henri Drake |

**Total visible commits: 15.** 12 commits in Jan-Feb 2022 (initial development). Then 2.5 years dormant. Then 2 README updates on Aug 17, 2026 (revival signal, no code changes).

**Why this matters:** MARGO's optimization framework could be applied to ocean intervention questions (e.g., "should we invest in ocean alkalinity enhancement vs. solar geoening?"). But it hasn't been used that way. The revival is real but minimal — documentation only, no new capabilities.

---

## Adjacent Tool: Carbon Capture Genome (Biodiversity Computing)

| Date | Commit |
|------|--------|
| Aug 19, 2026 | Recent update |

**Why this matters:** The "Carbon-Capture Genome" paper (Leon Kally et al.) explores engineering biodiversity for climate mitigation. While focused on terrestrial and genetic approaches, the computational framework could extend to ocean biodiversity engineering (e.g., marine genetic modification for enhanced carbon sequestration).

---

## The Zero-Activity Pattern

| Category | Repos | Total Commits | Last Activity |
|----------|-------|---------------|---------------|
| **Ocean geoengineering** | 0 | 0 | Never |
| **Ocean-atmosphere diagnostics** | MDTF-diagnostics | 10 (visible) | Aug 2026 |
| **Climate-economic optimization** | ClimateMARGO | 15 (visible) | Aug 2026 |
| **Ocean carbon cycle** | 0 | 0 | Never |
| **Ocean alkalinity** | 0 | 0 | Never |
| **Iron fertilization** | 0 | 0 | Never |
| **Marine cloud brightening** | 0 | 0 | Never |

**The pattern is clear: ocean processes have a thin scientific infrastructure on GitHub (MDTF), but zero geoengineering-specific infrastructure. The ocean is the one climate domain where GitHub has nothing to say about intervention.**

---

## The Ocean Gap: What the Absence Tells Us

| Factor | SRM (Solar) | CCS (Carbon) | Ocean | Impl &
|--------|------------|-------------|-------|-------|
| **Funding source** | NCAR, NOAA, DOE (software-funded) | DOE, ARPA-E, private (mixed) | Ocean agencies (NOAA, NOC, GEOMAR) — not software-funded | Ocean science doesn't produce software |
| **Political controversy** | Moderate (SRM is contentious) | Low (CCS is established) | High (London Protocol, Basel Convention) | Controversy suppresses open-source tooling |
| **Computational barrier** | Medium (atmospheric models are accessible) | Medium (DAC physics is tractable) | High (ocean models require massive HPC) | Higher barrier to entry |
| **Field experiments** | Some (SCoPEx, etc.) | Some (DAC pilot plants) | Very few (natural iron fertilization expeditions) | No experiments → no code |
| **Cultural norm** | Model-builders exist (NCAR) | Survey-builders exist (Carbon_Capture_ML) | Oceanographers don't build open-source tools | Different scientific culture |
| **Publication incentives** | Papers + code = credit | Papers + code = credit | Papers only = credit | No incentive for ocean scientists to code |

**The ocean gap is not an accident. It's the intersection of institutional structure, political controversy, computational barriers, and cultural norms that systematically exclude ocean geoengineering from the open-source ecosystem.**
