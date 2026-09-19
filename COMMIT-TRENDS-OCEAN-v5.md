# 🌊 Ocean Intervention — Commit Trends (v5 Update)
## Trend Analysis for Climate Pod Episode (October 2026)

---

## Velocity Summary

| Repo | Stars | Commits Pulled | Active Period | Velocity Pattern |
|------|-------|----------------|---------------|------------------|
| MDTF-diagnostics | 80 | 10 | Jun–Aug 2026 | 🔴 Steady institutional — 6 commits/74 days |
| WRF | 1,763 | 10 | May–Jun 2026 | 🔴 Institutional — 10 commits/19 days (ocean-adjacent) |
| ClimateMARGO | 73 | 10 | Aug 2026 + dormant | 🟡 Faint revival — 2 README updates after 2.5yr sleep |
| Marine-Cloud-Brightening | Low | 10 | Jun 16, 2026 | 🟡 **Burst** — 10 commits/1 day, then silence |
| Governance tracker | Low | N/A | Aug 2026 | 🟡 Recently active |
| **Ocean geoengineering** | — | — | — | **⚫ ZERO** |

---

## Trend 1: The Zero-Result Pattern

After 15+ search queries across every relevant keyword combination, the result is **unanimous and unmovable**: zero ocean geoengineering repositories on GitHub.

This isn't a single query that failed. It's a **systematic absence** across:
- Direct search terms ("ocean geoengineering", "marine geoengineering", "ocean intervention")
- Technique-specific terms ("ocean alkalinity enhancement", "sea salt spray injection", "ocean upwelling")
- Simulation terms ("ocean simulation climate", "ocean model geoengineering")
- Governance terms ("ocean fertilization regulatory", "London Protocol")

The absence is **not random** — it's consistent across every query type. This suggests the gap is structural, not accidental.

**Episode angle:** "We searched 15 different ways. Zero results. This isn't a missing repo — it's a missing ecosystem."

---

## Trend 2: The Precip-Buoyancy POD (MDTF's Ocean Signal)

**MDTF-diagnostics** (NOAA-GFDL) had the most recent ocean-adjacent activity: 5 commits on Jun 19, 2026, all updating `MCS_precip_buoy_stats.rst` — a Process-Oriented Diagnostic (POD) for precipitation-buoyancy statistics in the tropical ocean-atmosphere system.

**What this is:** The precip-buoyancy POD evaluates how well climate models reproduce the relationship between precipitation and buoyancy (temperature/salinity) in the tropical ocean. This is fundamental to understanding ocean-atmosphere coupling.

**What this ISN'T:** It's not a simulation of ocean interventions. It doesn't model ocean alkalinity enhancement, Sea salt spray, or any deliberate ocean modification.

**The paradox:** The most ocean-relevant code on GitHub **checks model accuracy**, not **models interventions**. The evaluation infrastructure exists; the intervention infrastructure is absent.

**Episode angle:** "The ocean's most important code on GitHub is a grading rubric, not a simulation. We can evaluate how well models do ocean physics, but no one has written the code to simulate ocean geoengineering."

---

## Trend 3: The ClimateMARGO Faint Signal

**ClimateMARGO.jl** had two README updates on Aug 17, 2026 by Fons van der Plas — the first activity after 2+ years of dormancy (last code commit: Oct 2023).

**Why this matters for the ocean episode:** ClimateMARGO is an idealized climate-economic model that includes **ocean coupling**. It's not ocean-specific, but it's the closest thing to an ocean-aware climate economics tool on GitHub. The faint README update suggests Fons may be re-engaging with the project — and if he gets fresh code commits, ClimateMARGO could bridge the gap between institutional climate modeling (WRF, PCMDI) and individual ocean intervention research.

**But the gap remains:** ClimateMARGO models the *economics* of climate with ocean coupling. It doesn't model *ocean interventions*. The tool can answer "what's the optimal climate policy?" but not "what's the optimal ocean geoengineering strategy?"

---

## Trend 4: MCB as Ocean-Adjacent Proxy

**Marine-Cloud-Brightening** (meneskoksal) is the closest thing to ocean intervention code on GitHub:
- It's a **marine** technique (seawater spray into marine clouds)
- It involves **ocean-atmosphere interaction** (the seawater comes from the ocean)
- It had a **10-commit burst** on Jun 16, 2026
- Multiple contributors (meneskoksal, julkrag, LenaPredl) suggest collaborative research

But MCB is technically **solar geoengineering**, not ocean intervention. It brightens clouds to reflect sunlight — it doesn't modify the ocean itself.

**The distinction matters for the episode:** MCB is the **gateway drug** argument. If marinecloud brightening works and is acceptable, does it open the door to ocean alkalinity enhancement, sea salt spray, and other ocean-based interventions? Or is the ocean a fundamentally different category that MCB doesn't relate to?

---

## Trend 5: The Governance Vacuum (Ocean Version)

The London Protocol is the only international regulatory framework that explicitly addresses ocean geoengineering (specifically, ocean fertilization). But:

1. **The London Protocol has no enforcement mechanism** — it can regulate waste dumping at sea, but ocean fertilization is not classified as "waste"
2. **The CBD moratorium applies to SRM** — not explicitly to ocean geoengineering
3. **No international body has authority over the ocean's climate** — the ocean is a global commons, but no governance institution has jurisdiction over its climate system

The governance tracker (Zereo0317) is the first tool to map this vacuum, but it's a tracker — not a solution.

**Episode angle:** "The London Protocol was written in 2006, before anyone seriously proposed ocean geoengineering. It's trying to fit a square peg into a round hole."

---

## The Three Universes (Updated v5)

```
┌─────────────────────────────────────────────────────────┐
│                    🔴 FAST UNIVERSE                      │
│           Institutional, funded, continuous              │
│                                                          │
│  WRF (1,763★)    PCMDI (133★)    MDTF (80★)             │
│   Atmosphere       Evaluation     Evaluation              │
│   Modeling         Infrastructure  Infrastructure         │
│                                                          │
│  Ocean-adjacent but not ocean-focused                    │
├─────────────────────────────────────────────────────────┤
│                    🟡 SLOW UNIVERSE                      │
│             Individual, dormant, burst pattern            │
│                                                          │
│  ClimateMARGO (73★)   MCB (Low★)    Governance (Low★)   │
│   Climate Econ +        Marine Cloud              Regulator │
│   Ocean coupling        Brightening                 Tracker  │
│   Faint revival         10-commit burst             Aug 2026  │
├─────────────────────────────────────────────────────────┤
│                    ⚫ EMPTY UNIVERSE                    │
│                  Ocean geoengineering                   │
│                                                          │
│  ZERO repositories. ZERO code. ZERO governance.          │
│                                                          │
│  The ocean is the dark matter of climate tech on GitHub —  │
│  invisible, undetected, and yet presumably massive in the │
│  scientific literature.                                  │
└─────────────────────────────────────────────────────────┘
```

---

## Commit Heat Map

```
Repo                      | Jun '26 | Jul '26 | Aug '26 | Sep '26 | Oct '26 | ...
--------------------------|---------|---------|---------|---------|---------|----
MDTF-diagnostics         | ████░░  | ██░░░░  | ██░░░░  | ░░░░░░  | ░░░░░░  |  (precip-buoyancy burst Jun)
WRF (ocean-adjacent)     | ████████| ░░░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  |  (v4.8.0 release)
ClimateMARGO             | ░░░░░░  | ░░░░░░  | ██░░░░  | ░░░░░░  | ░░░░░░  |  (faint README revival)
MCB (ocean-adjacent)     | ████████| ░░░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  |  (10-commit burst Jun)
Governance tracker       | ░░░░░░  | ░░░░░░  | ██░░░░  | ░░░░░░  | ░░░░░░  |  (recent)
Ocean geoengineering     | ░░░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  |  (ZERO — always)
```

**Pattern:** The ocean-adjacent universe (MCB, ClimateMARGO, MDTF) shows intermittent activity — bursts and faint revivals. But the ocean-intervention universe itself is **permanently dark**. No commits, no repos, no code.

---

## What to Watch Next Quarter

1. **Will ClimateMARGO get fresh code?** Fons van der Plas's README updates suggest re-engagement. A new release with ocean-coupled optimization would be the first ocean-adjacent signal since MDTF's precip-buoyancy POD.
2. **Will MCB produce published results?** The Jun 16 burst of temperature and cloud-cover analysis notebooks suggests a research team. If they publish, it could be the first open-source marine cloud brightening study.
3. **Will any ocean geoengineering repo appear?** The probability is low based on historical data, but if any researcher decides to build ocean intervention tools, it would be a front-page story for the podcast.
4. **Will the governance tracker grow?** If ocean geoengineering governance becomes a hot topic (after any real-world experiments), this tracker could become essential.
5. **Will WRF add ocean coupling?** The next WRF release (v4.9.0 or v5.0.0) could include improved ocean-atmosphere coupling, which would be the institutional world's reaches toward the ocean.

---

## The Ocean Episode: The Big Question

The ocean episode's thesis should be:

**The GitHub vacuum for ocean geoengineering is not an accident — it's a signal.**

Five hypotheses explain the absence:
1. **Funding gap** — ocean research is underfunded relative to its potential
2. **Governance chilling** — London Protocol ambiguity may deter code development
3. **Complexity gap** — ocean geoengineering requires coupled ocean-atmosphere models with biogeochemistry
4. **Community gap** — no one is gathering at GitHub to build ocean intervention tools
5. **Ethical taboo** — "dumping things in the ocean" triggers strong political reactions

The podcast episode should argue that the vacuum is **not just a data point** — it's a **governance signal**. The ocean is the only climate intervention domain where there is no code, no community, and no governance. This makes it the most interesting and most dangerous frontier in climate tech.

---

*Research methodology: GitHub REST API, October 2026. Commits pulled via List Commits API. Trend analysis by research methodology.*