# 🎙️ Solar Geoengineering Episode Brief

**Branch:** `solar-geoengineering` | **Version:** v4 | **Date:** September 2026

---

## Episode Title (Working)
"The Sun Screen Dilemma: Who Builds the Tools, Who Decides to Use Them?"

## Core Question
Can we trust climate models that have bugs in their radiation code to evaluate the very interventions they might be used to justify?

## Key Segments

### 1. The Bug (5 min)
- WRF v4.8.0 solar radiation EOF correction (May 28, 2026)
- What happens when the energy budget is wrong?
- How do you evaluate SAI if the baseline is off?

### 2. The Factory (7 min)
- WRF (1,762★) and PCMDI (133★) as institutional infrastructure
- Release-weekend pattern: 10 commits in 2 days for v4.2.1
- Roundoff fix: the difference between 1.00 and 0.9999

### 3. The Garage (7 min)
- ClimateMARGO's 2.8-year dormancy and ambiguous README revival
- srm-forever: the most relevant tool with zero stars
- Weitzman discounting: why the answer depends on your philosophy

### 4. The Question (5 min)
- SRM forever vs. mitigation + CDR
- The breakeven discount rate: 0.9% — inside the expert debate range
- The TCRE range straddles the verdict

## Talking Points

| Theme | Sound Byte | Source |
|-------|-----------|--------|
| "The bug that changes everything" | "A single line of code in WRF could change how we evaluate the entire solar geoengineering enterprise." | WRF commit e836cd6 |
| "The decimal that matters" | "Preventing a roundoff to 1.00 in mean climate figures — that's the difference between a correct model and a misleading one." | PCMDI commit 90cbc50 |
| "The dormant giant" | "ClimateMARGO went quiet for 2.8 years. Then the README was updated. But no code followed." | ClimateMARGO commit d916f36 |
| "The zero-star time machine" | "The most directly relevant solar geoengineering tool on GitHub has zero stars. WRF has 1,762." | srm-forever vs WFR |
| "The governance gap" | "The institutions that build the models are funded and fast. The people who ask 'should we?' are unfunded and fragile." | Cross-theme comparison |

## Suggested Listen-Along
- [ ] WRF v4.8.0 release notes: https://github.com/wrf-model/WRF/releases
- [ ] PCMDI metrics v4.2.1: https://github.com/PCMDI/pcmdi_metrics/releases
- [ ] SRM Forever interactive tool: https://hausfath.github.io/srm-forever/
- [ ] ClimateMARGO documentation: https://github.com/ClimateMARGO/ClimateMARGO.jl

## Research Files
- [PROJECT-DISCOVERIES-SOLAR.md](PROJECT-DISCOVERIES-SOLAR.md) — Detailed repo profiles
- [COMMIT-TRENDS-SOLAR.md](COMMIT-TRENDS-SOLAR.md) — Full trend analysis
- [CROSS-THEME-ANALYSIS-SEP2026-v4.md](https://github.com/bro26man-hash/climate-pod-research/blob/main/CROSS-THEME-ANALYSIS-SEP2026-v4.md) — Cross-theme dashboard (main branch)
