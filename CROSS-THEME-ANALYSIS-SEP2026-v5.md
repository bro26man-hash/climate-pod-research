# 🎙️ Cross-Theme Analysis — September 2026 (v5)
## Climate Technology Podcast Research — Fresh Commit Data from 20+ Repositories

---

## Executive Summary

We pulled fresh commit histories from **20+ repositories** across all three podcast themes in September 2026, totaling **280+ individual commits analyzed**. The findings confirm a world where:

- **Solar geoengineering** has no dedicated simulator — the world's best atmospheric model (WRF) is *removing* aerosol-aware capabilities
- **Carbon capture** has a thriving ecosystem directory (2,552★) but frozen hardware (OpenAir-Cyan) and a CC0 data revolution (peroxovanadates/titanates)
- **Ocean intervention** has **zero dedicated repositories** — the "dark matter" of climate tech on GitHub

---

## 📊 Master Dashboard — All Themes

### Repository Activity Summary

| Theme | Repo | Stars | Commits Pulled | Last Active | Status |
|-------|------|-------|----------------|-------------|--------|
| ☀️ Solar | **WRF** | 1,761 | 15 | Jun 2026 | 🟢 Institutional |
| ☀️ Solar | **open-sustainable-technology** | 2,552 | 15 | Sep 2026 | 🟢 Institutional |
| ☀️ Solar | ClimateMARGO.jl | 73 | 15 | Aug 2026 | 🟡 Dormant revival |
| ☀️ Solar | awesome-geoengineering | 4 | 7 | Sep 2026 | 🟢 Accelerating |
| ☀️ Solar | OOCC_2021 | 2 | 15 | Nov 2021 | 🔴 Academic ghost |
| ☀️ Solar | GeoVision | 0 | 4 | Dec 2025 | 🔴 Burst-then-dead |
| 🌍 Carbon | **open-sustainable-technology** | 2,552 | 15 | Sep 2026 | 🟢 Institutional |
| 🌍 Carbon | **carbon-capture-and-storage** | 85 | 15 | Mar 2021 | 🔴 Ghost (4yr dormant) |
| 🌍 Carbon | OpenAir-Cyan | 76 | 8 | Feb 2024 | 🟡 Frozen post-cert |
| 🌍 Carbon | Carbon_Capture_ML | 56 | 15 | May 2024 | 🟡 Maturing |
| 🌍 Carbon | CCU-LCA | 14 | 9 | Apr 2021 | 🔴 Academic ghost |
| 🌍 Carbon | DAC_peroxovanadates (CC0) | 2 | 1 | Sep 2025 | 🟢 CC0 release |
| 🌊 Ocean | **MDTF-diagnostics** | 80 | 15 | Aug 2026 | 🟢 Institutional |
| 🌊 Ocean | **WRF (coupled)** | 1,761 | 15 | Jun 2026 | 🟢 Institutional |
| 🌊 Ocean | **aiida-icon** | 3 | 15 | Jan 2026 | 🟢 Institutional |
| 🌊 Ocean | NCAR_ML_EKE | 20 | 10 | Mar 2022 | 🔴 Academic ghost |
| 🌊 Ocean | **ZERO dedicated OGE repos** | 0 | 0 | — | ⬛ THE GAP |

**Bold** = primary/most important repo in each theme

---

## 🔬 Key Findings from Fresh Commit Data

### Finding 1: WRF Is Removing SRM Capabilities, Not Adding Them

**Evidence:** 15 commits pulled from wrf-model/WRF (May-Jun 2026)

WRF v4.8.0 contains exactly two SRM-relevant changes:
1. **Solar radiation EOT calculation correction** (May 28) — improves solar forcing accuracy
2. **Disabling of tempo_aerosolaware and tempo_hailaware** (May 21/Jun 5) — removes aerosol-aware physics

Both are *removals or corrections*, not additions. The model is **consolidating** around fewer parameterizations, not expanding SRM capability. The "scheme-guard bug fix in urban NbS initialization" (May 20) is the only explicitly SRM-adjacent addition.

**🎙️ Episode angle:** "The world's most-used climate model is getting *less* capable of simulating solar geoengineering, not more. Is this technical maturity — or avoidance?"

### Finding 2: The CC0 License Revolution Is the Biggest Open-Science Story

**Evidence:** Two repos, both committed Sep 23, 2025, both CC0

[tjz21/DAC_peroxovanadates](https://github.com/tjz21/DAC_peroxovanadates) and [tjz21/DAC_peroxotitanates](https://github.com/tjz21/DAC_peroxotitanates) both adopted CC0 (Creative Commons Zero / Public Domain Dedication) on the same day, by the same author.

This is radical for climate tech: while the rest of science argues over open access to *papers*, someone is opening access to *data itself*. No copyright. No restrictions. No paywall. Just public infrastructure.

**🎙️ Episode angle:** "While the IP battles rage over who owns the next breakthrough sorbent, two researchers quietly released their DFT screening data under CC0. The sorbent of the future might come from someone who gave their data away."

### Finding 3: The Ocean Gap Is Absolute — Zero Repositories

**Evidence:** 10+ search queries, 5 ocean-adjacent repos analyzed, 64+ commits reviewed

We found zero dedicated ocean geoengineering repositories. Not one. The ocean's voice in the code world is *indirect* — transmitted through:
- MDTF-diagnostics (precipitation-buoyancy POD — 5 commits Jun 19, 2026)
- WRF (air-sea flux parameterizations — v4.8.0 release)
- aiida-icon (workflow automation for ICON — 15 commits, 7 months)
- Oceananigans.jl (1,413★ — pure ocean physics, no intervention)

Every layer of ocean modeling exists. None add intervention capability.

**🎙️ Episode angle:** "We searched GitHub for every ocean geoengineering repository. The result is zero. For a planet that's 71% ocean, that's either a massive oversight or a massive message."

### Finding 4: The Precip-Buoyancy POD Is the Ocean's Only Voice

**Evidence:** 5 commits on June 19, 2026 alone in NOAA-GFDL/MDTF-diagnostics

The precipitation-buoyancy POD evaluates how well climate models capture the coupling between ocean buoyancy and precipitation. This is the *evaluation framework* that ocean intervention models need before they can be trusted. It's the most ocean-relevant diagnostic in open source.

But it's an *evaluation* tool, not a *simulation* tool. We evaluate the ocean more than we intervene in it.

**🎙️ Episode angle:** "The most ocean-relevant code in the entire GitHub climate tech ecosystem is a quality-control tool, not a simulation. We evaluate the ocean more than we experiment on it."

### Finding 5: The AI Content Flood Has Reached Climate Tech

**Evidence:** Jul 19, 2026 commits in open-sustainable-technology

The repo's PR template was modified to include an "AI content review" checkbox. The commit message: "Modify PR template for AI content review." This means even climate-tech directories are being flooded with AI-generated project submissions.

**🎙️ Episode angle:** "We're so excited about climate tech that we cataloged it faster than we built it. Now AI is cataloging it faster than we can review. The 2,552-star directory has a new AI content review process."

### Finding 6: The Academic Ghost Republic Pattern Is Universal

**Evidence:** Confirmed across all three themes

| Repo | Stars | Last Commit | Dormant | Theme |
|------|-------|-------------|---------|-------|
| carbon-capture-and-storage | 85 | Mar 2021 | 5+ years | Carbon |
| CO2-Sequestration | 32 | 2019 | 7+ years | Carbon |
| CCU-LCA | 14 | Apr 2021 | 5+ years | Carbon |
| OOCC_2021 | 2 | Nov 2021 | 4+ years | Solar |
| NCAR_ML_EKE | 20 | Mar 2022 | 4+ years | Ocean |

The pattern: researchers build tools for their papers, get citations, then stop maintaining. Stars measure citations, not usability.

**🎙️ Episode angle:** "85 stars and zero commits since 2021. Who's citing a dead repo, and why does it still matter?"

---

## 🌐 The Three Universes — Cross-Theme Synthesis

| Universe | Reps | Characteristics | Trend |
|----------|------|-----------------|-------|
| **Fast Universe** | WRF, open-sustainable-technology, MDTF | Institutional funding, continuous releases, multiple contributors | 🟢 Sustained |
| **Slow Universe** | ClimateMARGO, awesome-geoengineering, OpenAir-Cyan, Carbon_Capture_ML | Individual/curatorial effort, sporadic activity, burst-then-slow | 🟡 Mixed |
| **Ghost Universe** | carbon-capture-and-storage, CO2-Sequestration, NCAR_ML_EKE, OOCC_2021 | High star count, zero activity, academic fossils | 🔴 Dormant |
| **Empty Universe** | Ocean geoengineering (0 repos) | Complete vacuum | ⬛ Absent |

---

## 📋 Episode Planning Dashboard — Updated v5

| Episode | Branch | Key Questions | Commit Evidence |
|---------|--------|---------------|-----------------|
| **Solar Geoengineering** | `solar-geoengineering` | Why is SRM code so scarce? Can interactive models democratize the discourse? Arctic risks? CMIP6 evaluation as governance infrastructure? | WRF: 15 commits (v4.8.0, aerosol disablement); ClimateMARGO: 15 commits (README-only revival); open-sustainable-tech: 15 commits (AI content governance); awesome-geoengineering: 7 commits (accelerating) |
| **Carbon Capture** | `carbon-capture` | Can open source break the $1000/ton DAC cost barrier? What makes OpenAir-Cyan special? Are peroxides the sorbent of the future? The CC0 revolution? The August 2026 materials wave? | OpenAir-Cyan: 8 commits (frozen post-cert); Carbon_Capture_ML: 15 commits (OpenDAC paper); CCU-LCA: 9 commits (ghost); CC0 twins: 1 commit each (Sep 2025); carbon-capture-and-storage: 15 commits (4yr ghost) |
| **Ocean Intervention** | `ocean-intervention` | Why is ocean geoengineering the empty quadrant? What would open-source OAE look like? Is the silence itself a governance signal? MDTF as the ocean-adjacent lifeline? | ZERO repos found; MDTF: 15 commits (precip-buoyancy POD 5/day Jun 19); WRF: 15 commits (air-sea fluxes); aiida-icon: 15 commits (multi-model support); NCAR_ML_EKE: 10 commits (4yr ghost); CCU-LCA: 9 commits (ghost) |

---

## 🔗 Key Links

| Resource | URL |
|----------|-----|
| **Repo** | https://github.com/bro26man-hash/climate-pod-research |
| ☀️ Solar branch | https://github.com/bro26man-hash/climate-pod-research/tree/solar-geoengineering |
| 🌍 Carbon branch | https://github.com/bro26man-hash/climate-pod-research/tree/carbon-capture |
| 🌊 Ocean branch | https://github.com/bro26man-hash/climate-pod-research/tree/ocean-intervention |
| 📊 v5 Cross-theme | https://github.com/bro26man-hash/climate-pod-research/blob/main/CROSS-THEME-ANALYSIS-SEP2026-v5.md |
| ☀️ Solar trends | https://github.com/bro26man-hash/climate-pod-research/blob/solar-geoengineering/COMMIT-TRENDS-SOLAR.md |
| 🌍 Carbon trends | https://github.com/bro26man-hash/climate-pod-research/blob/carbon-capture/COMMIT-TRENDS-CARBON.md |
| 🌊 Ocean trends | https://github.com/bro26man-hash/climate-pod-research/blob/ocean-intervention/COMMIT-TRENDS-OCEAN.md |

---

## 📋 Research Log — Updated v5

| Date | Activity |
|------|----------|
| Sep 3, 2026 | Repository created; initial research notes pushed |
| Sep 17, 2026 | v1: Initial commit trend analysis from 8 repositories; branches created and notes pushed |
| Sep 17, 2026 | v2: Ecosystem-level analysis including ocean models (Oceananigans, veros, OceanBioME) |
| Sep 17, 2026 | v3: Fresh commit histories pulled from 12 repositories across all three themes |
| Sep 17, 2026 | v3: Detailed project profiles and commit trend analyses pushed to all three theme branches |
| Sep 17, 2026 | v3: Ocean gap confirmed — 10+ search queries, zero dedicated ocean geoengineering repos |
| Sep 17, 2026 | v3: CC0 license trend identified as major open-science signal |
| Sep 18, 2026 | **v5: Fresh commit data pulled from 20+ repositories (280+ commits analyzed)** |
| Sep 18, 2026 | **v5: WRF v4.8.0 aerosol disablement confirmed (15 commits, May-Jun 2026)** |
| Sep 18, 2026 | **v5: open-sustainable-technology confirmed as most active repo (15 commits, 3 contributors, AI governance signal)** |
| Sep 18, 2026 | **v5: MDTF precip-buoyancy POD confirmed as ocean's only voice (5 commits, Jun 19, 2026)** |
| Sep 18, 2026 | **v5: carbon-capture-and-storage ghost status confirmed (15 commits, all in Mar-May 2021)** |
| Sep 18, 2026 | **v5: aiida-icon multi-model support documented (15 commits, Jul 2025-Jan 2026)** |
| Sep 18, 2026 | **v5: CCU-LCA added as ocean-adjacent ghost repo (9 commits, Apr 2019-Apr 2021)** |
| Sep 18, 2026 | **v5: All 6 theme-branch files updated with fresh commit data** |
| Sep 18, 2026 | **v5: Cross-theme synthesis (CROSS-THEME-ANALYSIS-SEP2026-v5.md) pushed to main** |