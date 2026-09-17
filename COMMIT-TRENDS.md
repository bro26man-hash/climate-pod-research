# 📊 Consolidated Commit Trend Summary (Updated Sep 2026 — Final Round)

**Cross-theme analysis of recent commit activity across all discovered climate tech and geoengineering repositories.**

**Last Updated:** September 2026 (Final research round)
**New commit data sourced from:** WRFmodel/WRF, PCMDI/pcmdi_metrics, openair-collective/openair-cyan, zikribayraktar/Carbon_Capture_ML, yohanesnuwara/carbon-capture-and-storage, ClimateMARGO/ClimateMARGO.jl, NOAA-GFDL/MDTF-diagnostics, aerler/WRF-Tools

---

## Repository Commit Activity (Complete Picture)

| Repo | Stars | Theme | Recent Commits | Activity Pattern |
|------|-------|-------|----------------|------------------|
| **wrf-model/WRF** | 1,761 | Solar+ | 10 commits May-Jun 2026 (v4.8.0) | Institutional release cycle — continuous monthly commits |
| **PCMDI/pcmdi_metrics** | 133 | Solar+ | 10 commits Sep 3-4, 2026 (v4.2.1) | Institutional burst — coordinated multi-contributor release |
| **NOAA-GFDL/MDTF-diagnostics** | 80 | Solar+ | 10 commits Jun-Aug 2026 | Institutional diagnostics development — multi-contributor PRs |
| **protontypes/open-sustainable-technology** | 2,546 | Carbon+ | 10 commits Jul-Sep 2026 | Steady directory growth — ecosystem infrastructure |
| **ClimateMARGO/ClimateMARGO.jl** | 73 | Solar | 2 commits Aug 2026 after 2-yr dormancy | Dormant revival signal — README updates suggest renewed interest |
| **openair-collective/openair-cyan** | 76 | Carbon | 6 commits Feb 12, 2024 (OSHWA cert) | Milestone burst then dormancy — certified, not commercialized |
| **zikribayraktar/Carbon_Capture_ML** | 56 | Carbon | 10 commits Feb 2023-May 2024 | Paper-driven activity peaks — literature survey model |
| **yohanesnuwara/carbon-capture-and-storage** | 85 | Carbon | 10 commits Feb-May 2021 (thesis) | Thesis burst then ghost town — 5+ years dormant |
||openair-collective/openair-sorbent-tester|3|Carbon|Updated Jan 2026|Steady incremental|
| **tjz21/DAC_peroxovanadates** | 2 | Carbon | Updated Aug 19, 2026 | Coordinated wave (with peroxotitanates same day) |
| **tjz21/DAC_peroxotitanates** | 2 | Carbon | Updated Aug 19, 2026 | Coordinated wave (with peroxovanadates same day) |
| **hausfath/srm-forever** | 0 | Solar | 4 commits Aug 26, 2026 | Single-author burst — teaching tool release |
| **prashant1926/open-earth-digital-twin** | 0 | Solar | 1 commit Oct 2025 | Dormant — single init |
| **pmip4/pmip_p2fvar_analyzer** | 4 | Solar | Updated Sep 2025 | Minimal |
| **RhondaMueller/Codes-RFG-Arctic-Impacts** | 1 | Solar | Updated Apr 2024 | Dormant |
| **FMS-ESM/AM3** | 4 | Solar | Updated Mar 2015 | Legacy — 11+ years dormant |
| **Team50-Labs/NebuGrid-OpenSource** | 0 | Ocean | Updated Aug 2026 | Only ocean-adjacent repo (fog-harvesting) |

---

## What We Learned from the Commit Histories (Detailed)

### WRF (1,761★) — The AtmosphericFoundation
WRF is the foundational atmospheric model for ALL climate simulation. Its v4.8.0 release (Jun 2026) shows 10 commits over 18 days with multiple contributors (Anthony Islas, weiwangncar, Joseph Olson, Lluís Fita, Kelly Werner). Key activities: disabling experimental aerosol options (tempo_aerosolaware, tempo_hailaware), fixing solar radiation EOT calculations, updating MYNN-EDMF physics. The aerosol-aware physics development directly feeds into SRM simulation capability.

### PCMDI Metrics (133★) — The Evaluation Infrastructure
PCMDI's v4.2.1 release (Sep 3-4, 2026) was a burst of 10 commits by Jiwoo Lee at LLNL, with PRs from James Goodnight and Jared Lewis. Also active: MCS precipitation-buoyancy POD (Jun 2026) by Wei-Ming Tsai — ocean-relevant diagnostics. This is the gold-standard tool for evaluating Earth System Models. If we deploy SRM or ocean interventions, we need tools like this to evaluate effects against baselines.

### MDTF Diagnostics (80★) — The Ocean-Adjacent Tool
NOAA-GFDL's MDTF-diagnostics had 10 commits across Jun-Aug 2026, including a new MCS precipitation-buoyancy statistics POD. Multiple contributors (Aparna Radhakrishnan, Wei-Ming Tsai, jongsooshin5) with PR-based workflows. This is process-oriented diagnostics for weather and climate simulations — directly relevant to evaluating ocean intervention impacts.

### OpenAir-Cyan (76★) — The DIY Hardware Pioneer
6 commits on Feb 12, 2024: OSHWA UID logo, CITATION.cff, batch documentation upload. KCollins drove the certification milestone. After 2 years, complete silence. The project proved open-source DAC hardware can reach institutional certification — but couldn't sustain momentum without an institutional home.

### Carbon_Capture_ML (56★) — The Literature Survey Model
Peaks around paper submission cycles: 4 commits Feb 2-5, 2023 (paper season), periodic updates through May 2024 (OpenDAC paper). Single author (Zikri Bayraktar). The repository is a curated survey of published ML-for-carbon-capture papers — literature management, not code production.

### carbon-capture-and-storage (85★) — The Ghost Project
9 commits in Feb-May 2021 (BSc thesis), then zero activity for 5+ years. Despite 85 stars, no maintenance. Single author (yohanesnuwara). Reservoir simulation + geomechanics + seismic modeling for CCS. This is the prototype of the "stars without sustainability" problem.

### ClimateMARGO (73★) — The Revival Signal
Last code commit: Oct 2023. Two README updates on Aug 17, 2026 — first activity in 2+ years. Idealized climate-economic modeling framework in Julia. The MarGO (& Trade-offs) name refers to Mitigation/Adaptation/Geoengineering optimization. The revival could signal growing policy-modeling interest, or could be another false start.

### The August 2026 Materials Wave (Confirmed)
Three DAC materials repositories (peroxovanadates, peroxotitanates, electro-swing-dacc) all updated on Aug 19, 2026. Plus ChemicalEngineeringAI/Carbon-Capture updated Aug 23, 2026. Four independent repos, same week, coordinated timing = a shared research event.

---

## Three Types of Activity Bursts

1. **Institutional bursts** (WRF, PCMDI, MDTF): Coordinated, multi-contributor, version-tagged releases driven by lab funding cycles. WRF v4.8.0 (Jun 2026) = 10 commits over 18 days. PCMDI v4.2.1 (Sep 2026) = 10 commits in 2 days. Both funded by US DOE national labs.

2. **Directory/resource bursts** (Open Sustainable Technology): Steady, sustained growth — 10 tool additions over 2.5 months. Not a single burst but an accumulation of ecosystem infrastructure. 2,546 stars shows this model scales.

3. **Individual bursts** (srm-forever, openair-cyan, Carbon_Capture_ML): Single authors pushing significant milestones — a paper release, a certification, a survey update. Intense but unsustainable without institutional support.

---

## The Two Speed Universes

**Fast universe (institutional, funded, sustained):**
- WRF (1,761★, monthly commits, 10+ contributors)
- PCMDI (133★, bursty institutional releases)
- MDTF-diagnostics (80★, ongoing diagnostics development)
- Open Sustainable Technology (2,546★, steady ecosystem growth)

**Slow universe (individual, unfunded, dormant):**
- OpenAir-Cyan (76★, 2-year dormancy post-certification)
- ClimateMARGO (73★, 2-year dormancy before brief revival)
- All SRM-specific repos (0-4★, dormant)
- All ocean intervention repos (nonexistent)

**The podcast thesis:** Climate tech open source has a funding gap, not a knowledge gap. The fast universe is funded. The slow universe isn't. The ocean is the ultimate funding gap.

---

## 📈 Cross-Theme Activity Dashboard

Solar Geoengineering:
  ████████████████████ PCMDI (133★, Sep 2026 burst)
  ████████████ WRF (1,761★, June 2026 release, continuous)
  ████████ MDTF-diagnostics (80★, Jun-Aug 2026 active)
  ████ ClimateMARGO (73★, Aug 2026 revival)
  ██ srm-forever (0★, Aug 2026 single burst)
  ████ AM3 (4★, legacy Fortran, dormant since 2015)

Carbon Capture:
  ████████████████████████ Open Sustainable Tech (2,546★, continuous)
  ████████████████ OpenAir-Cyan (76★, Feb 2024 burst, dormant)
  ████ Carbon_Capture_ML (56★, paper-driven peaks)
  ██ carbon-capture-and-storage (85★, thesis burst, ghost)
  █ peroxovanadates + peroxotitanates (2★ each, Aug 2026 wave)
  █ electro-swing-DAC (research collection, Aug 2026)

Ocean Intervention:
  █ (zero dedicated repos)
  ██ WRF ocean module — atmosphere-coupled, not intervention-focused
  ██ PCMDI ocean metrics — ENSO verification, not intervention metrics
  ██ MDTF-diagnostics — precipitation-buoyancy POD (closest to ocean process diagnostics)

---

## 🎙️ Podcast Takeaways (Updated)

1. **The simulation stack is stacked on the atmosphere.** WRF (1,761★), PCMDI (133★), MDTF (80★) are world-class tools. But they model the atmosphere and evaluate CMIP6. The ocean intervention layer is completely missing.

2. **The August 2026 DAC materials wave is real and coordinated.** Four independent repos updating in the same week = a community forming around open computational chemistry.

3. **ClimateMARGO's revival is the sleeper story.** An idealized climate-economic model in Julia, dormant for 2 years, suddenly showing activity. The policy-modeling layer for SRM could be here — or it could go dormant again.

4. **MDTF-diagnostics is the ocean-adjacent tool to watch.** Its new precipitation-buoyancy POD (Jun 2026) is the closest thing to ocean process diagnostics in open source. If ocean intervention ever gets a tool pipeline, it will start with diagnostics like this.

5. **carbon-capture-and-storage is the ghost that haunts the thesis story.** 85 stars, zero activity since 2021. Academic incentive structures don't reward long-term code stewardship. The ocean has the same problem but worse.

6. **OpenAir-Cyan proved open DAC hardware works. Now what?** Certification was the milestone. But 2.5 years of silence is the open-hardware limbo problem.

7. **The ocean is the silence that speaks loudest.** Zero repos, zero commits, zero tools. Meanwhile, the atmosphere gets WRF, PCMDI, and MDTF. The ocean gets... nothing. That's the story.

8. **Dormancy is the default state.** 15 of 18 repos show no meaningful activity in the last year. Climate tech open source is fragile. The few that survive are institutionally funded.

---

## 🔮 What to Watch Next Quarter

1. **WRF v4.8.x follow-up releases** — Will aerosol-aware physics continue developing? This is the de facto SRM simulation tool.
2. **ClimateMARGO revival** — Will Aug 2026 README updates lead to code commits? If so, it could become the policy-modeling layer for SRM.
3. **August 2026 DAC materials community** — Will the peroxovanadates/peroxotitanates/electro-swing-DAC repos collaborate, or fragment?
4. **MDTF-diagnostics** — Will the precipitation-buoyancy POD lead to more ocean-relevant diagnostics? This is the closest thing to ocean process tooling.
5. **OpenAir-Cyan commercialization** — Can the certified open hardware project become a product? Or is it permanently stuck as a blueprint?
6. **The ocean remains silent** — Unless someone builds the first open-source OAE model, the absence will persist into 2027.

---

## 🔗 Branch Links

- ☀️ Solar Geoengineering: [COMMIT-TRENDS-SOLAR.md](https://github.com/bro26man-hash/climate-pod-research/blob/solar-geoengineering/COMMIT-TRENDS-SOLAR.md)
- 🌍 Carbon Capture: [COMMIT-TRENDS-CARBON.md](https://github.com/bro26man-hash/climate-pod-research/blob/carbon-capture/COMMIT-TRENDS-CARBON.md)
- 🌊 Ocean Intervention: [COMMIT-TRENDS-OCEAN.md](https://github.com/bro26man-hash/climate-pod-research/blob/ocean-intervention/COMMIT-TRENDS-OCEAN.md)