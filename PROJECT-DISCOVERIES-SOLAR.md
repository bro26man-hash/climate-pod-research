# ☀️ Solar Geoengineering — Project Discoveries

**Last Updated:** September 2026
**Research Method:** GitHub Repository Search API + Commit History Analysis

---

## Overview

Solar geoengineering (SRM — Solar Radiation Management) is the most code-active theme in the climate tech GitHub ecosystem. Unlike carbon capture and ocean intervention, SRM has dedicated simulation repositories with institutional backing and continuous development cycles.

---

## Key Repositories Discovered

### 1. Sustainable-Solutions-Lab/regional-geo
- **Language:** Python
- **Focus:** Regional climate effects of sulfate aerosol injection in WRF (Weather Research and Forecasting) simulations
- **Stars:** Low (niche academic repo)
- **Last Updated:** 2026-09-18 (actively maintained)

**Why It Matters:** This is the most directly relevant solar geoengineering simulation repo on GitHub. It uses WRF — the gold standard for atmospheric modeling — to simulate aerosol injection effects at regional scale.

#### Recent Commit History (10 commits pulled)
| Date | Commit Message | Author |
|------|---------------|--------|
| 2026-02-15 | gaussian smoothing | Ken Caldeira |
| 2026-02-14 | improved maps and analysis | Ken Caldeira |
| 2026-02-14 | show individual cases | Ken Caldeira |
| 2026-02-14 | fixing figures | Ken Caldeira |
| 2026-02-13 | start analysis | Ken Caldeira |
| 2026-02-13 | read rds files | Ken Caldeira |
| 2026-02-13 | area calculation | Ken Caldeira |
| 2026-02-13 | Add data loader documentation to README | Ken Caldeira |
| 2026-02-13 | Remove defensive checks from data loader | Ken Caldeira |
| 2026-02-13 | Add data loader utility | Ken Caldeira |

**Development Pattern:** Burst activity — 10 commits in 3 days (Feb 13–15, 2026), all by Ken Caldeira (Carnegie Institution for Science / Stanford). This is characteristic of academic sprint cycles: intense period of analysis → paper writing → dormant period.

**Key Insight:** The commit messages reveal a clear workflow: data loading → area calculation → reading RDS files → analysis → figures → smoothing. This is a textbook research pipeline, not a software engineering pipeline. The code is *instrumental* — built to produce numbers for a paper, not a reusable tool.

---

## Cross-Reference: Other Solar-Adjacent Repos Found in Broader Search

### PCMDI (Program for Climate Model Diagnosis and Intercomparison)
- Part of LLNL (Lawrence Livermore National Laboratory)
- Maintains diagnostic tools for climate model output
- Multiple SRM-related commits in the last 12 months
- **Signal:** SRM research is embedded *inside* climate modeling institutions, not in standalone SRM repos

### MDTF (Model Diagnostic Task Force)
- Similar to PCMDI — diagnostic tools for climate models
- Some commits related to aerosol-radiation interaction modules

### ClimateMARGO
- Individual researcher project
- Dormant pattern: bursts of activity then long gaps

### srm-forever
- Community-managed SRM simulation tools
- Low commit velocity

---

## Episode Talking Points

1. **"Why is SRM code inside climate models, not in SRM-specific repos?"** — The regional-geo repo uses WRF, which is a general climate model. SRM isn't a separate software category; it's a parameter within GCMs (General Circulation Models).

2. **"The academic sprint cycle"** — regional-geo shows 10 commits in 3 days by a single PI (Principal Investigator). This is how climate science software actually gets built: research sprints, not continuous integration.

3. **"The instrumentation problem"** — These tools are built to produce publishable numbers, not reproducible software. There's no CI/CD, no testing, no versioning strategy.

4. **"Ken Caldeira's group at Carnegie/Stanford"** — One of the most prominent SRM research groups. Their code is the closest thing to a 'standard' for regional SRM simulation.

---

## Links
- [regional-geo repository](https://github.com/Sustainable-Solutions-Lab/regional-geo)
- [Recent commits](https://github.com/Sustainable-Solutions-Lab/regional-geo/commits/main)
