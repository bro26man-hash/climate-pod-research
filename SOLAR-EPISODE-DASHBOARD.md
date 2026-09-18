# ☀️ Solar Geoengineering Episode — Research Dashboard
*September 2026*

---

## Quick Reference Card

| Field | Detail |
|-------|--------|
| **Episode Title (Working)** | "The Sun Switch: Code, Carbon, and Climate Control" |
| **Theme** | Solar Radiation Management (SRM) |
| **Primary Repos** | WRF, PCMDI/pcmdi_metrics, MDTF-diagnostics |
| **Secondary Repos** | ClimateMARGO.jl, srm-forever |
| **Total Commits Analyzed** | 50 from 5 repositories |
| **Most Active Repo** | PCMDI (10 commits in 2 days) |
| **Most Critical Fix** | WRF solar radiation eot calculation (May 28, 2026) |
| **Biggest Gap** | No SRM deployment simulator exists |

---

## Repo Quick Scores

| Repo | Stars | Language | Activity | Episode Value |
|------|-------|----------|----------|---------------|
| **WRF** | 1,761 | Fortran | Continuous | ★★★★★ — The simulation engine |
| **PCMDI** | 133 | Python | Burst mode | ★★★★★ — The evaluation ruler |
| **MDTF** | 80 | Python | Steady | ★★★★ — The ocean link |
| **ClimateMARGO** | 73 | Julia | Dormant | ★★★ — The policy ghost |
| **srm-forever** | 0 | Julia | Minimal | ★★ — The philosophical anchor |

---

## Key Dates Timeline

```
May 21 ─ WRF: TEMPO error handling
May 26 ─ WRF: CDXWRF fix + GFL documentation
May 27 ─ WRF: MMM physics update + MYNN-EDMF update
May 28 ─ WRF: SOLAR RADIATION eot FIX
Jun  5 ─ WRF: Aerosol parameterization turnoff
Jun  6 ─ WRF: v4.8.0 README update
Jun  8 ─ WRF: v4.8.0 RELEASE + merge
Jun  8 ─ MDTF: Module integration + README updates
Jun 19 ─ MDTF: 5 commits + NEW precip-buoyancy POD
Aug 17 ─ ClimateMARGO: Mystery README updates (2x)
Sep  3 ─ PCMDI: Extremes chunking PR merged
Sep  4 ─ PCMDI: 10 commits + v4.2.1 RELEASE + roundoff fix
Sep 17 ─ PCMDI: Latest patch
```

---

## Story Arcs

### Arc 1: "The Fix That Changed Everything"
The May 28 solar radiation fix in WRF means every SRM simulation using previous versions had a timing error. This is the kind of behind-the-scenes story that makes technical podcasting compelling — the clock was wrong.

### Arc 2: "The 48-Hour Burst"
PCMDI's September 4 explosion of activity (10 commits, 6 PRs, version bump, critical roundoff fix) suggests either an impending publication or an urgent community response. What triggered it?

### Arc 3: "The Ocean in the Machine"
MDTF's precipitation-buoyancy POD is the only tool that connects solar geoengineering scenarios to ocean and water cycle impacts. It was added on a single day (June 19) by one scientist. What prompted it?

### Arc 4: "The Ghost with a Pulse"
ClimateMARGO's two README updates after 2+ years of silence. Is geoengineering optimization making a comeback, or is this just academic housekeeping?

### Arc 5: "The Zero-Star Prophet"
srm-forever asks the most important question in SRM policy with zero community adoption. The gap between theoretical importance and practical engagement is the story.

---

## Questions for Potential Guests

1. **To a WRF developer:** "How do you fix a solar radiation bug without invalidating years of published research?"
2. **To a PCMDI maintainer:** "What does the extremes_chunking feature mean for SRM impact assessment?"
3. **To a climate economist:** "Is ClimateMARGO's dormancy a signal that geoengineering optimization isn't ready for prime time?"
4. **To a policy scholar:** "Who should maintain srm-forever? Should there be an open-source SRM policy institute?"

---

*Dashboard compiled from GitHub API data, September 2026.*