# 🎙️ Solar Geoengineering Episode — Production Notes
## Compiled from GitHub Research — September 2026

---

## Episode Title (Provisional)
**"The Empty Sky: Why GitHub Has No Solar Geoengineering Model"**

## Runtime Target
25–35 minutes

---

## Act Structure

### Act I: The Paradox (5 min)
**Opening:** We searched GitHub for every solar geoengineering repository. The most used atmospheric model on Earth (WRF, 1,761★) silently maintains solar radiation physics. But repos that *explicitly* simulate SRM? The候车 station is empty.

**Key stat:** 55 commits across 6 solar geoengineering repos in our sample. Only 5 commits were directly physics-relevant. The rest are documentation, configuration, or bug fixes to general models.

**The hook:** "If you want to simulate solar geoengineering on GitHub, you'd download a model built for weather forecasting and hope it works. That's like performing surgery with a kitchen knife — it's technically possible, but nobody designed it for that purpose."

### Act II: The Infrastructure Lie (10 min)
**The WRF Story:** WRF is not a geoengineering tool. It's a weather model. But its solar radiation scheme is the closest thing we have to an SGE simulation standard. In May 2026, a critical solar radiation calculation was corrected (commit e836cd6). This means that *every previous SRM simulation using WRF had a systematic error in its solar radiation calculations.*

**Talking point:** The fix was made by weiwangncar at NCAR. It was reviewed through GitHub's PR process. It was merged by Anthony Islas. Seven contributors have committed to WRF in the last 30 days. This is the most rigorously maintained solar-relevant code on GitHub — and it doesn't know it's a geoengineering tool.

**GCCS-Core Detour:** Then there's KOSASIH's "Global Climate Control System" — 9 stars, 15 commits all on one day, zero actual simulation code. It's a project skeleton named like a hydra and built like a placeholder. But it tells us something about how people *imagine* solar geoengineering: as a control system, not a climate intervention.

### Act III: The Governance Void (10 min)
**OOCC_2021's Ghost:** jlehtomaa's solar geoengineering governance model. 15 commits over 4 months in 2021. A complete academic lifecycle: develop, refine, publish, die. The code is still there. The paper still cites it. But nobody maintains it.

**The question:** If the best governance model for SRE is a dead repo, what does that say about our preparedness for the real-world governance challenge?

**ClimateMARGO's Resurrection:** Fons van der Plas's climate-economic model woke up in August 2026 after 2 years of silence with two README updates. Is this a signal or noise? The model optimizes SGE deployment trade-offs. If it's being revived, it might mean someone sees renewed policy relevance. If it's just housekeeping, it's a false alarm.

### Act IV: The What-If (5 min)
**What would a real SGE simulation repo look like?**
- Modular factions: stratospheric aerosol module, ocean feedback module, vegetation response module
- Ensemble running: parameter uncertainty, scenario permutations
- Open data: injected mass, radiative forcing outputs, climate response fields
- Community governance: issue tracking for scenario proposals, PR review for physics changes

**Why doesn't it exist?**
- Funding: No grant agency funds open-source SGE simulation
- stigma: Researchers avoid "geoengineering" labels for career safety
- Complexity: Full SGE simulation requires climate model resolution + chemistry + dynamics
- Governance: The topic is politically radioactive

---

## 🎤 Audience Engagement Prompts

1. "Would you trust a solar geoengineering model maintained by a single PhD student on a weekend?"
2. "If WRF's solar radiation fix invalidates past SRM results, who's responsible for re-running those experiments?"
3. "Is 'Global Climate Control System' the most ambitious and empty repo on GitHub, or a prophecy?"

## 📎 Sources & Links
- [wrf-model/WRF](https://github.com/wrf-model/WRF) — v4.8.0, 1,761★
- [ClimateMARGO/ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl) — Climate-economic SGE optimization, 73★
- [KOSASIH/GCCS-Core](https://github.com/KOSASIH/GCCS-Core) — "Global Climate Control System", 9★
- [jlehtomaa/OOCC_2021](https://github.com/jlehtomaa/OOCC_2021) — SGE governance model, 2★
- [pixnum-hub/GeoVision](https://github.com/pixnum-hub/GeoVision) — "Geoengineering Simulator", 0★
- [hausfath/srm-forever](https://github.com/hausfath/srm-forever) — SRM economics, 0★
