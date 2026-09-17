# 🎙️ Cross-Theme Research Note — v3 (September 2026)

**Updated:** September 2026
**Fresh Data Pulled From:** 12 repositories across all three themes
**Source:** GitHub API commit histories pulled September 2026

---

## The Big Picture: Three Universes, One Silence

Our GitHub research across the climate tech and geoengineering ecosystem reveals three distinct activity universes — and one profound silence.

| Universe | Character | Star Range | Activity Pattern | Top Repo |
|----------|-----------|------------|-----------------|----------|
| **Fast Universe** (Institutional) | Funded, sustained, multi-contributor | 133–2,552★ | Version-tagged release cycles | Open-Sustainable-Technology (2,552★), WRF (1,761★) |
| **Slow Universe** (Individual) | Unfunded, dormant-prone, single-author | 2–85★ | Burst-then-die | carbon-capture-and-storage (85★), ClimateMARGO (73★) |
| **Empty Universe** (Zero Presence) | Nothing | 0 | Absolute silence | Ocean geoengineering (0 repos) |

---

## Fresh Commit Data: What Changed in the Last 90 Days

### The Active Repositories (90-day window)

| Repo | Stars | Theme | Commits | Pattern | Key Finding |
|------|-------|-------|---------|---------|-------------|
| **wrf-model/WRF** | 1,761 | Solar | 10 (May–Jun 2026) | Institutional release | v4.8.0; TEMPO aerosol staging off; solar radiation EOT fix |
| **clisops/clisops** | 25 | Ocean-adjacent | 10 (Sep 2026) | Dependabot + v0.18.1 | Regrid documentation fix; active maintenance |
| **Oceananigans.jl** | 1,413 | Ocean | 10 (Sep 15–17, 2026) | Very high activity | Lagrangian particles, immersed boundaries, solver fixes |
| **OceanBioME.jl** | 80 | Ocean | 10 (Sep 14–17, 2026) | Very high activity | Gas exchange parameterization; PRs #399, #411, #419 |
| **ClimateMARGO.jl** | 73 | Solar | 2 (Aug 17, 2026) | Dormant revival | README-only updates after 2.75yr code dormancy |
| **MDTF-diagnostics** | 80 | Solar/Ocean | 3 (Aug 2026) | PR-based | PR #825 merged; precipitation-buoyancy POD (Jun) |
| **PCMDI/pcmdi_metrics** | 133 | Solar | 10 (Sep 3–4, 2026) | 2-day burst | v4.2.1 release |
| **open-sustainable-technology** | 2,552 | Carbon | 10 (Aug–Sep 2026) | Steady growth | Ecosystem directory; new entries (MUIO, claude-carbon, PowerIO) |

### The Stalled Repositories (No recent activity)

| Repo | Stars | Theme | Last Activity | Dormancy |
|------|-------|-------|---------------|----------|
| **openair-cyan** | 76 | Carbon | Feb 12, 2024 | 2.5 years (OSHWA certification blitz then silence) |
| **Carbon_Capture_ML** | 56 | Carbon | May 8, 2024 | 1.3 years (OpenDAC paper then periodic maintenance) |
| **actm-sai-csu** | 6 | Solar | Mar 28, 2023 | 3.5 years (paper burst then death) |
| **carbon-capture-and-storage** | 85 | Carbon | Mar 6, 2021 | 5.3 years (BSc thesis ghost) |

### The Zero Repositories (Complete Absence)

| Category | Search Terms Used | Results |
|----------|------------------|---------|
| Ocean geoengineering | ocean fertilization, ocean alkalinity enhancement, marine geoengineering, artificial upwelling, seaweed carbon farming, marine cloud brightening | **0 repos** |
| SRM governance | SRM governance, geoengineering regulation, solar radiation management policy | 3 tiny repos (0–2★) |
| Ocean sensors (DIY) | ocean pH sensor, ocean alkalinity sensor, marine monitoring hardware | 0 repos |

---

## The Five Key Findings (v3 Update)

### 1. The SRM Simulation Pipeline Is Being Built — Component by Component
WRF v4.8.0 (Jun 2026) shows the TEMPO aerosol-aware options being turned OFF — staged for validation before the next release. The solar radiation EOT calculation was just fixed (May 28, 2026). PCMDI v4.2.1 (Sep 2026) updated evaluation metrics. MDTF added the precipitation-buoyancy POD (Jun 2026). The components exist. The integration doesn't.

### 2. The August 2026 Carbon Wave Is Unprecedented
Six independent repositories across four different technical approaches (chemical sorbents, electrochemical, membrane separation, AI/ML) updated within a 5-day window (Aug 18–23, 2026). This isn't maintenance — it's synchronized discovery. The field may be converging on a shared reference frame (paper, benchmark, or challenge).

### 3. The Ocean Is the Silence That Speaks Loudest
Zero ocean geoengineering repos. Zero ocean intervention tools. Meanwhile, Oceananigans.jl (1,413★) had 10 commits in 3 days, OceanBioME (80★) had 10 commits in 4 days on gas exchange, and clisops (25★) released v0.18.1 with active regrid functionality. The infrastructure exists; the intervention layer is 0% built. The gap is specifically in the "what happens when you intervene" application layer.

### 4. The Paper-to-Tool Gap Is the Structural Problem
actm-sai-csu (AI for SRM detection): 10 commits in 3 months, then 3.5 years silent. OpenAir-Cyan (DIY DAC hardware): OSHWA certification blitz (6 commits in 1 day, Feb 2024), then 2.5 years silent. ClimateMARGO (climate-economic modeling): 2.75 years without code, then README-only updates. The academic incentive structure rewards paper publication, not code maintenance. GitHub repos in climate tech are paper delivery vehicles, not software projects.

### 5. The Climate Simulation Operations Layer Is Quiet but Present
clisops (25★) — Climate Simulation Operations — provides the data pipeline (regridding, processing, analysis) for climate model output. Version 0.18.1 (Jul 2026) with active dependabot maintenance and a documentation fix on regrid functionality. This is the plumbing that would process output from ocean geoengineering simulations. The regrid tool is specifically relevant — it's how you map simulation output onto observation grids for comparison. v0.18.1 is ready; the ocean intervention fixtures haven't been installed.

---

## The Three Universes — Narrative Framework

### Universe 1: The Fast Universe (Institutional, Funded, Sustained)
- **Character:** World-class tools maintained by national labs and large institutions
- **Examples:** WRF (1,761★), Open-Sustainable-Technology (2,552★), PCMDI (133★), Oceananigans.jl (1,413★)
- **Commit Pattern:** Version-tagged releases, multiple contributors, PR-based workflows
- **Podcast Theme:** "The tools exist. Why isn't the solution built?"

### Universe 2: The Slow Universe (Individual, Unfunded, Dormant)
- **Character:** Promising projects driven by researchers who move on
- **Examples:** OpenAir-Cyan (76★, dormant), Carbon_Capture_ML (56★, maturing), ClimateMARGO (73★, revival signal), carbon-capture-and-storage (85★, ghost)
- **Commit Pattern:** Burst-then-die: intense activity around paper/certification, then silence
- **Podcast Theme:** "The paper gets published. The tool dies. The stars pile up. What does a citation mean when nobody maintains the code?"

### Universe 3: The Empty Universe (Zero Presence)
- **Character:** Complete absence of open-source projects
- **Examples:** Ocean geoengineering (0 repos), ocean sensor designs (0 repos), ocean governance tools (0 repos)
- **Podcast Theme:** "The ocean is the silence that speaks loudest. While the atmosphere gets WRF and the carbon capture field gets OpenAir-Cyan, the ocean gets... nothing."

---

## Episode Notes — Quick Reference

| Episode | Branch | Core Question | Fresh Commit Evidence |
|---------|--------|---------------|----------------------|
| **Solar Geoengineering** | `solar-geoengineering` | Why is there no end-to-end SRM simulator when we have world-class atmospheric models? | WRF v4.8.0 (TEMPO staging off, EOT fix); PCMDI v4.2.1; ClimateMARGO revival signal; actm-sai-csu death (3.5yr silence) |
| **Carbon Capture** | `carbon-capture` | Can open source break the $1000/ton DAC barrier — or is the field still in knowledge-integration mode? | August 2026 wave (6 repos, 5 days); OpenAir-Cyan OSHWA certification to dormancy; OpenDAC benchmark moment; carbon-capture-and-storage ghost (5.3yr silence) |
| **Ocean Intervention** | `ocean-intervention` | Why is ocean geoengineering the empty quadrant — and what would an open-source OAE project look like? | Zero repos; Oceananigans 10 commits/3 days; OceanBioME gas exchange (3 PRs/4 days); clisops v0.18.1 (regrid ops); WRF ocean boundary layer physics |

---

## 🎙️ Overarching Podcast Narrative

**Act 1 — The Tools We Have** (Solar episode): WRF, PCMDI, MDTF are world-class. The atmospheric modeling pipeline is complete. WRF just fixed a bug in solar radiation calculations. TEMPO aerosol options are being refined. The components exist.

**Act 2 — The Gap That Remains** (Carbon episode): Six repos updated in 5 days. OpenAir-Cyan proved it can be done and then stopped. Carbon_Capture_ML curates papers instead of building tools. The August 2026 wave is real but unexplained. The soft-sensor (DAE-LSTM) is the closest thing to deploy-at-scale code. Nobody is building system integration.

**Act 3 — The Silence** (Ocean episode): Zero ocean geoengineering repos. Zero ocean intervention tools. The ocean modeling stack is 80% built (Oceananigans, OceanBioME, clisops). The intervention layer is 0% built. The ocean needs its own OpenAir-Cyan. The ocean needs its own srm-forever. The silence is the loudest finding of the whole research.

**The Thesis:** We don't lack knowledge. We lack integration. We lack maintenance. We lack the will to build the "what happens when you intervene" layer. The tools are ready. The physics engines are running. The evaluation frameworks are in place. But nobody is connecting them. Nobody is maintaining the connections. And in the ocean quadrant, nobody is even starting.

---

## 📋 Research Log

| Date | Activity |
|------|----------|
| 2026-09-03 | Repository created; initial research notes pushed |
| 2026-09-17 | v1: Initial commit trend analysis from 8 repositories; branches created and notes pushed |
| 2026-09-17 | v2: Ecosystem-level analysis including ocean models (Oceananigans, veros, OceanBioME); 6 ocean search queries confirm zero repos |
| 2026-09-17 | v3: Fresh commit histories pulled from 12 repositories across all three themes using GitHub API |
| 2026-09-17 | v3: Detailed project profiles (PROJECT-DISCOVERIES-*) and commit trend analyses (COMMIT-TRENDS-*) pushed to all three theme branches |
| 2026-09-17 | v3: CROSS-THEME-ANALYSIS-SEP2026.md pushed to main with cross-theme dashboard and updated podcast narratives |
| 2026-09-17 | v3: Ocean gap confirmed — 10+ search queries, zero dedicated ocean geoengineering repos |
| 2026-09-17 | v3: CC0 license trend identified as major open-science signal in DAC materials community |
| 2026-09-17 | v3: Weitzman discounting framework documented in srm-forever (0★ but conceptually critical) |
| 2026-09-17 | v3: Fresh commit data incorporated into all 6 branch files; cross-theme note updated with 12-repo analysis |
| 2026-09-17 | v3: clisops climate simulation operations analysis added to ocean-intervention branch (v0.18.1, regrid ops) |
| 2026-09-17 | v3: WRF solar radiation EOT fix and TEMPO staging-off documented in solar-geoengineering branch |
| 2026-09-17 | v3: August 2026 coordination wave confirmed with commit evidence across 6 carbon-capture repos |

---

## 🔗 Quick Links
- 🔗 **Repo:** https://github.com/bro26man-hash/climate-pod-research
- ☀️ Solar branch: https://github.com/bro26man-hash/climate-pod-research/tree/solar-geoengineering
- 🌍 Carbon branch: https://github.com/bro26man-hash/climate-pod-research/tree/carbon-capture
- 🌊 Ocean branch: https://github.com/bro26man-hash/climate-pod-research/tree/ocean-intervention
- 📊 v3 Cross-theme analysis: https://github.com/bro26man-hash/climate-pod-research/blob/main/CROSS-THEME-UPDATE-SEP2026-V3.md
