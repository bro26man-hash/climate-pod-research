# ☀️ Solar Geoengineering Episode — Quick Reference Card (v5)
*October 2026 — Ready for Production*

---

## Episode Title Ideas
- "Sun Dims: The Code Behind Solar Geoengineering"
- "The SRM Economics Problem: Why Cheap Sun-Dimming May Not Be So Cheap"
- "Who Owns the Sky? The Governance Vacuum in Solar Geoengineering"

## Key Stats
- **7 key repos analyzed** across 3 trend patterns
- **70+ commits** examined from WRF, PCMDI, srm-forever, MCB, ClimateMARGO, governance tracker, and orbital-climate-sim
- **3 trend patterns:** Institutional steady-state, burst-and-sleep, governance emergence
- **1 paradigm shift:** Weitzman certainty-equivalent discounting in srm-forever
- **1 critical fix:** WRF's solar radiation EOT calculation (May 28)
- **1 critical fix:** PCMDI's roundoff to 1.00 in mean_climate figures (Sep 4)
- **1 regulatory vacuum:** No international SRM governance framework exists
- **0 ocean geoengineering repos** (see Ocean episode)

## The Three Universes (Updated)
- **🔴 Fast Universe:** WRF, PCMDI — institutional, funded, continuous, boring, essential
- **🟡 Slow Universe:** srm-forever, MCB, ClimateMARGO — individual, dormant, burst pattern, creative, fragile
- **🟢 Emerging Universe:** Governance tracker — new, small, but signaling a shift from science to politics

## Top Interview Angles
1. **The WRF developer:** "Why did you turn off the aerosol schemes in v4.8.0? Does this slow down SRM research?"
2. **The srm-forever author:** "Why did you switch to Weitzman discounting? Does it change the SRM-vs-mitigation answer?"
3. **The governance tracker maintainer:** "Who has the legal authority to deploy SRM? Who stops them if they do it unilaterally?"
4. **The MCB researcher:** "Is marine cloud brightening a legitimate tool or a gateway to larger SRM deployments?"
5. **The PCMDI developer:** "If your metrics have a roundoff bug, how confident can we be in CMIP6 SRM evaluations?"

## Segment Structure (45 min)
| Segment | Time | Key Question |
|---------|------|-------------|
| Cold Open | 2 min | What if the sun-dimming simulation had a bug in its sunlight calculation? |
| The Science | 15 min | How do we simulate SRM? WRF, PCMDI, and the precision problem |
| The Economics | 12 min | Is SRM actually cheap? The Weitzman discounting revolution |
| The Governance | 10 min | Who decides who decides? The regulatory vacuum |
| The Ethics | 8 min | Marine cloud brightening — localized tool or gateway drug? |
| The Future | 5 min | ClimateMARGO's revival and what optimal SRM+CDR allocation looks like |

## Key Quotes for Show Notes
- "The aerosol schemes that simulate sun-dimming were turned off by default in the world's most widely used climate model." (WRF v4.8.0)
- "A roundoff bug in climate metrics could mask small but important temperature differences — the kind that matter for SRM evaluation." (PCMDI v4.2.1)
- "Under deep uncertainty, the certainty-equivalent discount rate can be much lower than the expected-rate discount rate — which changes the SRM-vs-mitigation calculation entirely." (Weitzman 2012, adopted by srm-forever)
- "There is no international body with authority to mandate, permit, or prohibit SRM deployment." (Governance gap)

## Cross-References
- 🌍 Carbon episode: `carbon-capture/COMMIT-TRENDS-CARBON-v5.md`
- 🌊 Ocean episode: `ocean-intervention/COMMIT-TRENDS-OCEAN-v5.md`
- 📊 Cross-theme analysis: `main/CROSS-THEME-ANALYSIS-v5.md`

*Updated: October 2026 — v5 with fresh commit data from 7 repos*