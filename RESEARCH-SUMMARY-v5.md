# 🎙️ Climate Pod Research — Cross-Theme Summary (v5, September 2026)

**Podcast Series:** Climate Technology & Geoengineering  
**Repository:** `bro26man-hash/climate-pod-research`  
**Research Date:** September 2026  
**Methodology:** GitHub REST API (Repository Search, List Commits, List Branches)

---

## 📊 Unified Commit Trend Dashboard

| Theme | Repos Analyzed | Total Commits Pulled | Top Signal | Development Pattern |
|-------|----------------|---------------------|------------|---------------------|
| ☀️ Solar | 5 | 40+ | WRF's solar radiation fix; ClimateMARGO's 2 ongoing commits | Burst-then-dormant dominates |
| 🌍 Carbon | 5 | 30+ | DAC digital twin (8 commits/1 day); OpenCarbon dormant since 2023 | Paper-push pattern universal |
| 🌊 Ocean | 3 (adjacent) | 20+ | NCAR_ML_EKE, WRF coupling, ClimateMARGO potential | **ZERO dedicated repos** |

---

## 🔬 Key Repos by Theme

### ☀️ Solar Geoengineering
1. **ClimateMARGO.jl** (73★) — Climate-economic modeling framework, Julia. Active (2 commits Aug 2026).
2. **regional-geo** — Sulfate aerosol injection in WRF. Ken Caldeira's lab. Sprint of 10 commits Feb 2026.
3. **awesome-geoengineering** (4★) — Curated resource list. Steady maintenance, 7 recent commits.
4. **Geo-DICE** (2★) — Modified DICE model with geoengineering. **Dormant since 2018.**
5. **OOCC_2021** (2★) — Solar geoengineering governance model. **Dormant since 2021.**

### 🌍 Carbon Capture
1. **dac-moving-bed-digital-twin** — Moving-bed TVSA digital twin for DAC. 8 commits all on 2026-07-03.
2. **Direct-Air-Capture** (Rudra57) — Data-driven DAC exploration. 4 commits all on 2026-06-11.
3. **OpenCarbon** (2★) — DAC coordination/roadmapping. **Dormant since 2023-07.**
4. **ClimateMARGO.jl** (cross-listed) — Economic optimization includes carbon capture as a lever.
5. **WRF** (1,763★) — Atmospheric transport modeling essential for DAC site analysis.

### 🌊 Ocean Intervention
1. **NCAR_ML_EKE** (20★) — ML for ocean climate modeling. Adjacent only.
2. **WRF** (cross-listed) — Ocean coupling via MOM6. No geoengineering modules.
3. **ClimateMARGO.jl** (cross-listed) — Could extend to ocean economic modeling.
4. **⚫ ZERO dedicated repos.** Confirmed across 8 search queries.

---

## 🎙️ The Three Universes Framework

```
┌─────────────────────────────────────────────────────────┐
│  🔴 FAST UNIVERSE (Institutional, Continuous)           │
│  WRF · NCAR_ML_EKE                                      │
│  Major institutions · Continuous development            │
│  Heavy lifting of climate simulation                    │
├─────────────────────────────────────────────────────────┤
│  🟡 SLOW UNIVERSE (Individual, Dormant Bursts)          │
│  ClimateMARGO.jl · regional-geo · awesome-geoengineering │
│  Direct-Air-Capture · dac-moving-bed-digital-twin       │
│  Individual researchers · Paper-push pattern · Dormant  │
├─────────────────────────────────────────────────────────┤
│  ⚫ EMPTY UNIVERSE (Ocean Geoengineering)               │
│  ZERO repos · ZERO commits · ZERO code                  │
│  Not sparse — *non-existent*                            │
└─────────────────────────────────────────────────────────┘
```

---

## 🎯 Episode Framing per Theme

### Episode 1: ☀️ Solar Geoengineering
**Anchor Question:** Why is SRM code inside climate models, not in SRM-specific repos?  
**Key finding:** 3 of 5 solar geoengineering repos are completely dormant. The simulation layer is dead; only the metadata layer (awesome-geoengineering) is alive. SRM physics hides inside WRF's atmospheric code.

### Episode 2: 🌍 Carbon Capture
**Anchor Question:** Can open source + CC0 break the $1,000/ton DAC cost barrier?  
**Key finding:** The "paper push" pattern dominates — burst of commits for a paper, then silence. No continuous DAC codebase exists. The field is entirely paper-driven with no community infrastructure.

### Episode 3: 🌊 Ocean Intervention
**Anchor Question:** Is the GitHub vacuum a governance signal — or a missed opportunity?  
**Key finding:** Zero ocean geoengineering repos confirmed. Five hypotheses for the gap: governance fear, physical complexity, funding structure, publication bias, and the "let someone else do it" problem.

---

## 📁 Branch Structure

| Branch | File | Description |
|--------|------|-------------|
| `main` | `RESEARCH-SUMMARY-v5.md` | This file — unified cross-theme dashboard |
| `solar-geoengineering` | `RESEARCH-NOTES-SOLAR-v5.md` | Solar project profiles, commit trends, episode talking points |
| `carbon-capture` | `RESEARCH-NOTES-CARBON-v5.md` | Carbon project profiles, commit trends, episode talking points |
| `ocean-intervention` | `RESEARCH-NOTES-OCEAN-v5.md` | Ocean gap analysis, five hypotheses, episode talking points |

---

## 🔗 Links
- **Repo:** https://github.com/bro26man-hash/climate-pod-research
- **Solar branch:** https://github.com/bro26man-hash/climate-pod-research/tree/solar-geoengineering
- **Carbon branch:** https://github.com/bro26man-hash/climate-pod-research/tree/carbon-capture
- **Ocean branch:** https://github.com/bro26man-hash/climate-pod-research/tree/ocean-intervention

---

*Research methodology: GitHub REST API, September 2026. Commits pulled via List Commits API. Search queries via Repository and Code Search APIs. Cross-theme analysis by analytical synthesis.*