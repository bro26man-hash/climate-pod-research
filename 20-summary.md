# 📋 Cross-Theme Research Summary

> **Primary Branch:** `main`  
> **Compiled From:** `solar-geoengineering`, `carbon-capture`, `ocean-intervention`  
> **Date:** 2026-09-16

---

## Top Project Discoveries Across All Themes

| Rank | Repo | Stars | Theme | Language | Last Updated | Key Insight |
|------|------|-------|-------|----------|-------------|-------------|
| 1 | protontypes/open-sustainable-technology | 2,546 | All | Python | Sep 2026 | Definitive OSS climate-tech directory; essential starting point |
| 2 | wrf-model/WRF | 1,761 | Solar | Fortran | Sep 2026 | Most active climate sim; ocean & aerosol physics locked inside |
| 3 | ClimateMARGO/ClimateMARGO.jl | 73 | Both | Julia | Aug 2026 | geo-economic optimization; bridges Solar & Carbon |
| 4 | JGCRI/xanthos | 38 | Solar | Python | Aug 2023 | Hydrologic framework; silent since 2023 |
| 5 | NOAA-GFDL/MDTF-diagnostics | 80 | Ocean | Jupyter | Aug 2026 | Climate simulation diagnostics incl. ocean |
| 6 | roocs/clisops | 25 | Solar | Python | Sep 2026 | Climate data ops; bot-maintained only |
| 7 | pixnum-hub/GeoVision | — | Solar | HTML | Dec 2025 | Geoengineering simulator; one-shot upload, no momentum |
| 8 | RhondaMueller/Codes-RFG-Arctic-Impacts | 1 | Solar | Python | Apr 2024 | Regional SRM impact; single author |
| 9 | terranexum/OpenCarbon | 2 | Carbon | — | Jul 2023 | DAC systems; silent since 2023 |
| 10 | tjz21/DAC_peroxovanadates | 2 | Carbon | — | Aug 2026 | DAC materials; part of Aug 2026 surge |
| 11 | tjz21/DAC_peroxotitanates | 2 | Carbon | — | Aug 2026 | DAC materials; part of Aug 2026 surge |
| 12 | o7-machinehum/electro-swing-dacc | — | Carbon | — | Aug 2026 | DIY electro-swing DAC; open hardware frontier |
| 13 | cjcarlson/geomalaria | 3 | Solar | R | — | Malaria risk in SRM world; health impacts |
| 14 | jlehtomaa/OOCC_2021 | 2 | Solar | Python | — | SRM governance model; conceptual |
| 15 | pslmodels/Geo-DICE | 2 | Solar | MATLAB | — | DICE with geoengineering cost-benefit |
| 16 | FMS-ESM/AM3 | 4 | Solar | Fortran | Mar 2015 | Legacy GFDL atmospheric model; used in SRM studies |

---

## Cross-Theme Commit Trend Summary

### Solar Geoengineering
- **Pattern:** Codebase is sparse; most SRM simulation happens in closed academic labs (GFDL, NCAR). Legacy Fortran models (AM3, 2015) coexist with new Jupyter notebook experiments.
- **Active Repos:** ClimateMARGO.jl (bursty), clisops (bot-only)
- **Silent Repos:** GeoVision (one-shot), AM3 (legacy)
- **Key Gap:** The physics layer (aerosol, radiation, ocean coupling) is institutional. The policy/economic layer is open.

### Carbon Capture
- **Pattern:** Two modes visible — atomic material-science updates (vanadates, titanates) and bursty system-engineering commits (OpenCarbon). The August 2026 surge in DAC materials repositories suggests a new wave of open computational chemistry for next-gen sorbents.
- **Active Repos:** DAC materials (surging Aug 2026), electro-swing DAC (new)
- **Silent Repos:** OpenCarbon (2023), ClimateMARGO (bursty maintenance)
- **Key Gap:** Systems engineering lags materials science by years.

### Ocean Intervention
- **Pattern:** The breakout finding — virtually zero dedicated ocean geoengineering repositories on GitHub. The experimental complexity, governance sensitivity, and institutional siloing of ocean research create the biggest open-source gap in climate tech.
- **Active Repos:** Adjacent only (WRF, MDTF, clisops)
- **Silent Repos:** All ocean-specific categories are empty
- **Key Gap:** The entire ocean intervention layer is missing from OSS climate tech.

---

## The Starkest Contrast

| Dimension | Solar ☀️ | Carbon 🌍 | Ocean 🌊 |
|-----------|----------|-----------|----------|
| **Open repos exist?** | Yes (sparse) | Yes (surging) | ❌ Virtually none |
| **Last major activity** | Jun 2026 (WRF) | Aug 2026 (materials) | N/A |
| **Maintainer situation** | Single-author + institutional | New wave + silent legacy | No ecosystem |
| **Hardware/DAC** | N/A | Emerging (DIY) | N/A |
| **Governance modeling** | Conceptual (OOCC_2021) | None | None |
| **Biggest gap** | Physics simulation open access | Systems engineering tools | Entire domain absent |

---

## 🎙️ Series-Level Takeaways

1. **Open-source climate tech is unevenly distributed.** Solar has sparse code; carbon has a materials surge; ocean has nothing.
2. **Institutional lock-in is the pattern.** The most powerful models (WRF, CAM) are closed; what's open tends to be early-stage or single-author.
3. **The materials-vs-systems split is a recurring theme.** In both carbon and (incidentally) in SRM, the *design* layer opens faster than the *deployment* layer.
4. **The ocean is the canary.** If ocean geoengineering can't get open-source traction despite its urgency, that tells us something fundamental about the barriers.
5. **Governance precedes code.** Every domain lacking governance modeling (SRM, ocean) also lacks simulation code. Open-source needs a social license first.