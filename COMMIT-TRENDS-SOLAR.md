# ☀️ Solar Geoengineering — Commit Trend Analysis

> Updated: September 2026 | Analyzes 5 repos, 36+ commits

---

## Executive Summary

The solar geoengineering theme on GitHub reveals a **two-tier ecosystem**: large, institutionally maintained atmospheric models with steady commit velocity, and small, individual theoretical repos with sparse but meaningful activity. There is **no dedicated SRM simulation software** — the entire theme is parasitic on climate models built for other purposes.

---

## Trend 1: Institutional Velocity (WRF + PCMDI)

### WRF's Solar Commitment Pattern
- **10 commits in recent window**, dominated by version release (v4.8.0) and solar radiation scheme fixes
- **Pattern:** Burst-then-steady. Major releases trigger commit clusters; between releases, maintenance is quiet
- **Climate context:** WRF's solar radiation scheme is the computational backbone for any SRM simulation. Changes here directly affect how aerosol direct forcing is computed
- **⚠️ Podcast insight:** When WRF updates its radiation scheme, it's not "for geoengineering" — it's for weather forecasting. But the same code paths are used by SRM researchers. This is the quiet infrastructure of solar geoengineering science.

### PCMDI's Two-Day Blitz
- **10 commits in 48 hours** for v4.2.1 release
- **Pattern:** Institutional sprint followed by stability. PCMDI operates on a release-cycle model, not continuous deployment
- **Climate context:** PCMDI metrics are the gold standard for evaluating whether a climate model (and by extension, an SRM simulation) is credible
- **⚠️ Podcast insight:** The speed of PCMDI's v4.2.1 release suggests growing institutional urgency around model evaluation. If SRM is going to be taken seriously as a policy option, the evaluation infrastructure must be bulletproof.

---

## Trend 2: The Ocean-Adjacent Signal (MDTF)

### Precipitation-Buoyancy POD: The Ocean's Best Friend
- **5 commits on June 19, 2026 alone** — an intense single-day development push
- **What it does:** Evaluates how well climate models capture the vertical coupling between ocean buoyancy and precipitation — a fundamental climate process that SRM could disrupt
- **Why it matters for ocean intervention:** If solar geoengineering changes the hydrological cycle (reducing evaporation, altering monsoon patterns), the precipitation-buoyancy POD is how you'd detect it. It's the diagnostic bridge between solar and ocean themes.
- **⚠️ Podcast insight:** This is the single most important find for our ocean episode. The most ocean-relevant diagnostic tool in open source isn't an ocean model — it's a climate evaluation tool. The ocean's voice in the code world is indirect.

---

## Trend 3: Dormant Revival vs. Active Development (ClimateMARGO vs. srm-forever)

### ClimateMARGO: The Ambiguous Awakening
- **2 README updates** after 2+ years of dormancy (Aug 17, 2026)
- **Zero code commits** in the revival window
- **Interpretation A (optimistic):** Someone is preparing the tool for a new policy-modeling study that couples climate physics with economic impacts
- **Interpretation B (pessimistic):** It's a ghost repo — someone updated the README to make it look alive for a grant proposal or CV
- **⚠️ Podcast insight:** ClimateMARGO's revival is the perfect metaphor for geoengineering governance: lots of talking, no doing. Or maybe it's just getting started. You don't know which story you're in until the code commits start flowing.

### srm-forever: The Theoretical Anchor
- **4 focused commits** on Weitzman certainty-equivalent discounting
- **Zero stars, but maximum intellectual density**
- **What it does:** Computes the cost of maintaining SRM indefinitely under uncertainty. Uses economist Martin Weitzman's framework for handling low-probability, high-consequence risks
- **⚠️ Podcast insight:** This repo proves that the most important SRM work happens outside the spotlight. While other repos accumulate stars, srm-forever is asking the question that matters: *What's the forever cost?*

---

## Trend 4: The Missing Discipline

### What You Don't Find
- **No marine cloud brightening models** — MCB is the mostgeoengineering-specific SRM approach, yet there's zero open-source code
- **No stratospheric aerosol injection models** — SAI is the most-studied SRM approach in literature, but no dedicated simulation tools exist on GitHub
- **No circle molecule or aerosol chemistry models** — the microphysics of how sulfate aerosols form, coagulate, and precipitate is not modeled in any open-source SRM-specific tool

### What This Means
The entire solar geoengineering software ecosystem is **derivative** — it relies on tools built for weather forecasting, climate projection, and economic modeling. Nobody has built SRM-specific software. This is either:
1. **A maturity signal:** The existing models are good enough; SRM just plugs into them
2. **A governance signal:** Nobody wants to build dedicated SRM tools because of the moral hazard debate
3. **A gap signal:** The field is so young that dedicated tools haven't emerged yet

---

## Comparative Commit Velocity Chart

```
WRF       ████████████████████  High (10 commits, institutional)
PCMDI     ████████████████████  High (10 commits in 2 days, institutional burst)
MDTF      ██████████            Moderate (5 commits, targeted)
srm-forever ████████            Low (4 commits, focused)
ClimateMARGO ██                 Dormant (2 README updates, zero code)
```

---

## 🔑 Key Takeaways for the Podcast

1. **WRF is the silent backbone** — every SRM simulation lives inside WRF's radiation scheme, but nobody builds SRM tools *for* WRF
2. **PCMDI's velocity is the evaluation story** — if SRM is going to be policy-relevant, the evaluation infrastructure must keep pace
3. **MDTF's precipitation-buoyancy POD bridges solar and ocean** — the most ocean-relevant diagnostic is in the solar theme's repo
4. **ClimateMARGO's ambiguous revival is the governance parable** — talking about SRM economics vs. actually computing it
5. **srm-forever is the intellectual dark horse** — zero stars, maximum depth, the question that outlives all the others
6. **The missing tools are the real story** — no MCB code, no SAI models, no aerosol chemistry. The ecosystem is hollow.

---

*Data source: GitHub API, pulled September 2026. Commit counts are approximate based on API pagination.*