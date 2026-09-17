# 🎙️ Episode Research Index
## Quick-Reference Guide for All Three Podcast Episodes

---

## Episode 1: The Empty Sky — Solar Geoengineering

### Core Question
Why is there no open-source solar geoengineering simulation model on GitHub?

### Key Evidence
- **WRF (1,761★):** The most important atmospheric model on Earth just fixed its solar radiation calculation. Commit e836cd6, May 28, 2026. But it's not a geoengineering tool.
- **ClimateMARGO (73★):** Dormant for 2 years, then 2 README updates in one day. Is it waking up?
- **GCCS-Core (9★):** "Global Climate Control System" — 15 commits in one day, zero simulation code.
- **OOCC_2021 (2★):** The best governance model for SGE is a dead repo from 2021.
- **GeoVision (0★):** "Geoengineering Simulator" — 4 commits, no simulation code.

### Commit Evidence
| Repo | Stars | Recent Commits | Status |
|------|-------|----------------|--------|
| WRF | 1,761 | 15 (monthly) | 🟢 Very Active — v4.8.0 |
| ClimateMARGO | 73 | 2 (after 2yr gap) | 🟡 Revival? |
| GCCS-Core | 9 | 15 (one-day burst) | 🔴 Dormant since 2024 |
| OOCC_2021 | 2 | 15 (2021) | 🔴 Dormant since 2021 |
| GeoVision | 0 | 4 (one-day) | 🔴 Dormant since 2025 |
| srm-forever | 0 | Low (2026) | 🟡 Low Activity |

### Sources
- [PROJECT-DISCOVERIES-SOLAR.md](https://github.com/bro26man-hash/climate-pod-research/blob/solar-geoengineering/PROJECT-DISCOVERIES-SOLAR.md)
- [COMMIT-TRENDS-SOLAR.md](https://github.com/bro26man-hash/climate-pod-research/blob/solar-geoengineering/COMMIT-TRENDS-SOLAR.md)
- [SOLAR-EPISODE-NOTES.md](https://github.com/bro26man-hash/climate-pod-research/blob/solar-geoengineering/SOLAR-EPISODE-NOTES.md)
- [SOLAR-RECOMMENDATIONS.md](https://github.com/bro26man-hash/climate-pod-research/blob/solar-geoengineering/SOLAR-RECOMMENDATIONS.md)

---

## Episode 2: The Carbon Capture Directory Trap

### Core Question
Has the carbon capture community built a map instead of a territory?

### Key Evidence
- **open-sustainable-technology (2,552★):** The biggest climate-tech repo is a directory, not a tool.
- **openair-cyan (76★):** OSHWA-certified DIY DAC hardware. Then silence since Feb 2024.
- **Carbon_Capture_ML (56★):** A living literature review — 15 months of papers, then slow decline.
- **CC0 revolution (2★ each):** DAC materials researchers dedicating all data to public domain on the same day.
- **MEA simulation fork (1★→updated):** Active process engineering in a fork, not the original.

### Commit Evidence
| Repo | Stars | Recent Commits | Status |
|------|-------|----------------|--------|
| open-sustainable-technology | 2,552 | Continuous | 🟢 Very Active |
| openair-cyan | 76 | 10 (one-day burst, 2024) | 🔴 Frozen after certification |
| Carbon_Capture_ML | 56 | 15 (over 18mo, last May 2024) | 🟡 Slow Decay |
| carbon-swarm | 2 | 3 (one-day burst, Apr 2026) | 🔴 Dormant |
| DAC_peroxovanadates (CC0) | 2 | Active (Sep 2025) | 🟢 Active — CC0 data |
| MEA simulation fork | 1 | Sep 13, 2026 | 🟢 Active (recent) |

### Sources
- [PROJECT-DISCOVERIES-CARBON.md](https://github.com/bro26man-hash/climate-pod-research/blob/carbon-capture/PROJECT-DISCOVERIES-CARBON.md)
- [COMMIT-TRENDS-CARBON.md](https://github.com/bro26man-hash/climate-pod-research/blob/carbon-capture/COMMIT-TRENDS-CARBON.md)

---

## Episode 3: The Ocean Gap

### Core Question
Why does GitHub have zero ocean geoengineering repositories when the ocean is 71% of Earth's surface?

### Key Evidence
- **Zero dedicated repos:** After 10+ search queries, no ocean intervention code exists on GitHub.
- **aiida-icon (3★):** 15 commits, 14 contributors, institutional quality. But makes it easier to run climate models — not to simulate ocean interventions.
- **NCAR_ML_EKE (20★):** Perfect paper lifecycle. MOM6 integrated. Then 4+ years of silence.
- **Oceananigans.jl (1,413★):** Beautiful ocean physics. No intervention modules.
- **Every ocean modeling layer exists** (physics, biogeochemistry, ice, waves, coastal, GPU, ML, workflow) — **none have geoengineering overlays.**

### Commit Evidence
| Repo | Stars | Recent Commits | Status |
|------|-------|----------------|--------|
| aiida-icon | 3 | 15 (7 months) | 🟢 Active — CSCS-backed |
| NCAR_ML_EKE | 20 | 10 (4+ years ago) | 🔴 Dormant since 2022 |
| Oceananigans.jl | 1,413 | (from v2) | 🟢 Active — but no intervention |
| veros | 187 | (not pulled) | 🟢 Active — no intervention |
| **Total OGE repos** | **0** | **—** | **⬛ THE GAP** |

### Sources
- [PROJECT-DISCOVERIES-OCEAN.md](https://github.com/bro26man-hash/climate-pod-research/blob/ocean-intervention/PROJECT-DISCOVERIES-OCEAN.md)
- [COMMIT-TRENDS-OCEAN.md](https://github.com/bro26man-hash/climate-pod-research/blob/ocean-intervention/COMMIT-TRENDS-OCEAN.md)

---

## 🤝 Cross-Theme Sharing Points

These stories appear in all three episodes:
1. **The Directory Beats the Tool** — every theme has a meta-repo outshining actual technology
2. **The Single-Day Burst** — 5 repos show the "launch then die" pattern
3. **The Stars-Measure-Citations Problem** — 2,552★ for a directory ≠ 2,552 working tools
4. **The Single-Maintainer Risk** — 62% of repos have exactly 1 contributor
5. **The Governance Vacuum** — SGE governance code is older than the physics code
6. **The CC0 Revolution** — computational data as public infrastructure (carbon theme)
7. **The Burst Pattern** — infrastructure creation without sustained development (all themes)

---

## 📅 Research Timeline

| Date | Milestone |
|------|-----------|
| Sep 3, 2026 | Repository created; initial research notes pushed |
| Sep 17, 2026 | v1: 8 repositories analyzed; 3 branches created; notes pushed |
| Sep 17, 2026 | v2: Ocean gap confirmed; ecosystem analysis expanded |
| Sep 17, 2026 | v3: 12 repositories analyzed; detailed profiles and trend analyses pushed |
| Sep 17, 2026 | v4: Fresh WRF v4.8.0 data pulled; solar radiation fix identified |
| Sep 17, 2026 | v4: ClimateMARGO revival pattern documented |
| Sep 17, 2026 | v4: aiida-icon institutional quality confirmed (CSCS, 14 contributors) |
| Sep 17, 2026 | v4: NCAR_ML_EKE academic lifecycle completed in analysis |
| Sep 17, 2026 | v4: Cross-theme dashboard built; episode planning finalized |
| Sep 17, 2026 | v4: All notes pushed to all branches with fresh commit data |

---

## 🔗 Quick Links

| Resource | Link |
|----------|------|
| Repository | https://github.com/bro26man-hash/climate-pod-research |
| ☀️ Solar branch | https://github.com/bro26man-hash/climate-pod-research/tree/solar-geoengineering |
| 🌍 Carbon branch | https://github.com/bro26man-hash/climate-pod-research/tree/carbon-capture |
| 🌊 Ocean branch | https://github.com/bro26man-hash/climate-pod-research/tree/ocean-intervention |
| ☀️ Solar discoveries | https://github.com/bro26man-hash/climate-pod-research/blob/solar-geoengineering/PROJECT-DISCOVERIES-SOLAR.md |
| 🌍 Carbon trends | https://github.com/bro26man-hash/climate-pod-research/blob/carbon-capture/COMMIT-TRENDS-CARBON.md |
| 🌊 Ocean gap | https://github.com/bro26man-hash/climate-pod-research/blob/ocean-intervention/PROJECT-DISCOVERIES-OCEAN.md |
| 📊 Cross-theme (main) | https://github.com/bro26man-hash/climate-pod-research/blob/main/CROSS-THEME-ANALYSIS-SEP2026.md |
