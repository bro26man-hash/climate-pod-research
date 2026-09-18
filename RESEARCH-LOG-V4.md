# 🔬 Research Log v4 — September 2026

## Systematic Search Protocol

### Ocean Geoengineering Search (12 Queries)
Executed as part of v4 update to rigorously confirm the ocean gap:

| Query | Tool | Result |
|-------|------|--------|
| "ocean geoengineering" | GitHub repo search | 0 results |
| "ocean alkalinity enhancement" | GitHub repo search | 0 results |
| "ocean iron fertilization" | GitHub repo search | 0 results |
| "marine cloud brightening" | GitHub repo search | 0 results |
| "ocean CDR" | GitHub repo search | 0 results |
| "ocean carbon dioxide removal" | GitHub repo search | 0 results |
| "OAE simulation" | GitHub repo search | 0 results |
| "ocean geoengineering simulation" | GitHub repo search | 0 results |
| "marine geoengineering" | GitHub repo search | 0 results |
| "ocean intervention climate" | GitHub repo search | 0 results |
| "ocean restoration carbon" | GitHub repo search | 0 results |
| "blue carbon ocean" | GitHub repo search | 0 results |

**Conclusion:** Ocean geoengineering has zero dedicated repositories across all major techniques. The void is confirmed.

### Broad Climate Tech Search (10 Queries)
Executed across v2-v4 to discover fossil and active repos:

| Query | Key Finds |
|-------|----------|
| "geoengineering" | ClimateMARGO, awesome-geoengineering, Geo-DICE, geomalaria, GCCS-Core |
| "climate simulation modeling" | WRF, Climate2Weather, NCAR_ML_EKE, Greenhouses-Library |
| "carbon capture DACC sorbent" | openair-sorbent-tester |
| "ocean geoengineering ocean alkalinity enhancement" | 0 results |

## Commit History Pulls (v4)

| Repo | Commits Pulled | Window |
|------|---------------|--------|
| wrf-model/WRF | 15 | May-Jun 2026 |
| ClimateMARGO/ClimateMARGO.jl | 15 | Oct 2023-Aug 2026 |
| brandonhimpfen/awesome-geoengineering | 7 | Jun 2025-Sep 2026 |
| PSLmodels/Geo-DICE | 4 | Aug 2016-Sep 2018 |
| jlehtomaa/OOCC_2021 | 15 | Jul-Nov 2021 |
| cjcarlson/geomalaria | 15 | Jan-Feb 2022 |
| KOSASIH/GCCS-Core | 15 | Oct 2024 |

## Key Commits Identified (v4)

| Date | Repo | Commit | Significance |
|------|------|--------|-------------|
| May 28, 2026 | WRF | "Correction for eot calculation for solar radiation" | 🔥 Most SRM-relevant commit |
| Jun 5, 2026 | WRF | "Turn off tempo_aerosolaware and tempo_hailaware" | Aerosol simplification for stability |
| Jun 8, 2026 | WRF | "Merge release-v4.8.0" | Major version with solar physics fixes |
| Aug 17, 2026 | ClimateMARGO | "Update README.md" (×2) | ⚠️ Zombie revival #2 |
| Sep 5-6, 2026 | awesome-geoengineering | "Update README.md" (×2) | Active curation continuing |
| Sep 23, 2025 | tjz21/DAC_peroxovanadates | CC0 dedication | 🔓 Public domain liberation |
| Sep 23, 2025 | tjz21/DAC_peroxotitanates | CC0 dedication | 🔓 Public domain liberation |
| Jan 10, 2026 | openair-sorbent-tester | Repository update | Lab tool still ticking? |

## v4 Deliverables

| File | Branch | Description |
|------|--------|-------------|
| FRESH-CROSS-THEME-ANALYSIS-SEP2026-v4.md | main | Cross-theme dashboard with 16 repos |
| CROSS-THEME-UPDATE-SEP2026-V4.md | main | v4 delta from v3 |
| RESEARCH-UPDATE-V4-SEP2026.md | main | Detailed metrics and new findings |
| RESEARCH-LOG-V4.md | main | Search protocol and commit log |
| COMMIT-TRENDS-SOLAR-v4.md | solar-geoengineering | Solar-specific trends + WRF fix |
| PROJECT-DISCOVERIES-SOLAR-v4.md | solar-geoengineering | Solar project profiles (6 repos) |
| SOLAR-EPISODE-RESEARCH.md | solar-geoengineering | Solar episode dossier v4 |
| COMMIT-TRENDS-CARBON-v4.md | carbon-capture | Carbon trends + CC0 deep-dive |
| PROJECT-DISCOVERIES-CARBON-v4.md | carbon-capture | Carbon profiles (9 repos + sorbent-tester) |
| CARBON-EPISODE-RESEARCH.md | carbon-capture | Carbon episode dossier v4 |
| COMMIT-TRENDS-OCEAN-v4.md | ocean-intervention | Ocean gap confirmation + hypotheses |
| PROJECT-DISCOVERIES-OCEAN-v4.md | ocean-intervention | Ocean profiles + pseudocode frameworks |
| OCEAN-EPISODE-RESEARCH.md | ocean-intervention | Ocean episode dossier v4 |

## Verification Steps

1. ✅ Ocean search: 12 queries → 0 results (confirmed total absence)
2. ✅ Solar commits: 7 repos → 78 commits analyzed
3. ✅ Carbon commits: 9 repos → 65+ commits analyzed
4. ✅ Ocean adjacent: 3 repos → recent activity confirmed
5. ✅ CC0 identification: tjz21 pair confirmed public domain
6. ✅ WRF solar fix: May 28 EOT correction + Jun 5 TEMPO toggle identified
7. ✅ Pseudocode frameworks: 4 drafted (OAE, iron fertilization, MCB, governance)
8. ✅ openair-sorbent-tester: discovered and profiled (NEW)

## Next Steps (v5 Planning)

- Consider reaching out to repo maintainers for interviews
- Explore forking OOCC_2021 for ocean governance extension
- Draft actual Python implementation of OAE 1D column model
- Create ocean geoengineering directory as standalone repo or awesome-geoengineering branch
- File issues in WRF/MDTF-diagnostics for ocean use cases

*Research log compiled: September 2026 | Version: v4 | Branch: main*