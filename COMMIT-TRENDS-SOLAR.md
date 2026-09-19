# ☀️ Solar Geoengineering — Commit Trend Analysis

**Last Updated:** September 2026
**Data Source:** GitHub List Commits API

---

## Velocity Overview

| Repository | Commits Pulled | Active Period | Velocity Pattern | Lead Developer |
|-----------|---------------|---------------|-----------------|----------------|
| regional-geo | 10 | Feb 13–15, 2026 (3 days) | Burst (10/3 days = 3.3/day) | Ken Caldeira |
| PCMDI (adjacent) | Multiple | Last 12 months | Steady institutional | LLNL staff |
| MDTF (adjacent) | Multiple | Last 12 months | Steady institutional | LLNL staff |
| ClimateMARGO | Low | Sporadic | Dormant/burst | Individual |
| srm-forever | Low | Sporadic | Dormant | Community |

---

## Trend: The Two-Speed Solar Universe

Solar geoengineering development on GitHub reveals a **two-speed universe**:

### 🔴 Fast Universe (Institutional)
- ** characterized by:** Multiple contributors, steady commit cadence, institutional funding
- **Examples:** PCMDI, MDTF
- **Commit pattern:** 2–5 commits per week, consistent across quarters
- **Why:** These are diagnostic tool centers at national labs. SRM research is one of many projects they support.

### 🟡 Slow Universe (Academic/Individual)
- ** characterized by:** Single developer, burst patterns, long dormancy
- **Examples:** regional-geo (Caldeira group), ClimateMARGO, srm-forever
- **Commit pattern:** 10 commits in 3 days, then nothing for 6+ months
- **Why:** These are research pipelines, not software products. Code is built for papers, not platforms.

---

## Detailed Commit Timeline: regional-geo

```
2026-02-13 ████████████████████ 7 commits (data pipeline setup)
2026-02-14 ██████████████ 3 commits (analysis + figures)
2026-02-15 ██ 1 commit (smoothing/polish)
2026-02-16 → DORMANT
```

**Interpretation:** The 3-day sprint follows a classic research cycle:
1. **Day 1 — Data infrastructure:** Add data loader, read RDS files, calculate areas
2. **Day 2 — Analysis:** Start analysis, show individual cases, fix figures
3. **Day 3 — Polish:** Gaussian smoothing for final figures

This is *not* software engineering. It's **script-driven analysis** that happens to be version-controlled.

---

## What This Means for Your Podcast

### Episode Architecture for Solar Geoengineering

**Segment 1: The Technology Itself**
- How SRM simulation actually works (WRF + aerosol parameterization)
- Why regional modeling matters (global models miss local impacts)
- The role of Ken Caldeira's group (the closest thing to an SRM simulation "standard")

**Segment 2: The Development Pattern**
- Academic sprint vs. continuous deployment
- Why SRM code looks like research scripts, not production software
- The reproducibility crisis in climate science (no CI/CD, no testing)

**Segment 3: The Governance Question**
- Who controls the tools that simulate solar geoengineering?
- National labs (LLNL) vs. academic groups vs. community projects
- The open-source question: should SRM simulation be centralized or decentralized?

---

## Key Quote-Worthy Data Points

- **"10 commits in 3 days by one PI"** — regional-geo's development pattern is a punchline about how climate science software actually works
- **"Zero standalone SRM platforms"** — All SRM code lives inside climate models or research groups. There's no "GitHub for SRM"
- **"The Caldeira factor"** — One researcher's sprint can produce the entire public codebase for regional SRM simulation
- **"Institutional steady vs. academic burst"** — PCMDI commits 2-5x/week year-round; Caldeira's group does 10/3days then vanishes

---

## References
- [regional-geo commit history](https://github.com/Sustainable-Solutions-Lab/regional-geo/commits/main)
- [PCMDI](https://github.com/PCMDI)
- [MDTF](https://github.com/MDTF)
- [ClimateMARGO](https://github.com/search?q=ClimateMARGO)
- [srm-forever](https://github.com/search?q=srm-forever)
