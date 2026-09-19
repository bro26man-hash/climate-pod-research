# 🎙️ Climate Pod Research — Cross-Theme Analysis v5

**Last updated:** September 2026
**Data cycle:** GitHub API, 12 repos surveyed, 80+ commits analyzed across 3 themes

---

## 📊 Unified Dashboard

| Theme | Repos Analyzed | Commits Pulled | Top Signal | Episode |
|-------|----------------|----------------|------------|---------|
| ☀️ Solar | 4 (PCMDI, regional-geo, actm-sai-csu, climate-intervention-governance) | 40+ | PCMDI's 10-commit sprint; WRF's solar radiation fix | Ep 1 |
| 🌍 Carbon | 5 (OpenAir-Cyan, ClimateMARGO, isaH93, Rudra57, OpenCarbon) | 35+ | OpenAir-Cyan's OSHWA blitz; CC0 public-domain revolution | Ep 2 |
| 🌊 Ocean | 0 dedicated (3 adjacent) | 20+ (adjacent) | Zero repos; governance gap; data desert | Ep 3 |

---

## The Three Universes

```
┌──────────────────────────────────────────────────────────────────────┐
│                   CLIMATE TECH on GitHub (Sep 2026)                  │
└──────────────────────────┬───────────────────────────────────────────┘
                           │
       ┌───────────────────┼───────────────────┐
       │                   │                   │
 ┌─────┴──────┐      ┌────┴──────┐      ┌────┴──────┐
 │ 🔴 FAST    │      │ 🟡 SLOW   │      │ ⚫ EMPTY  │
 │ UNIVERSE   │      │ UNIVERSE  │      │ UNIVERSE  │
 │            │      │           │      │           │
 │ PCMDI      │      │Climate-   │      │           │
 │ 133★       │      │MARGO 73★  │      │Ocean Geo- │
 │ 10 commits │      │OpenAir-   │      │engineering│
 │ in 2 weeks │      │CYAN 76★   │      │ ZERO repos│
 │            │      │Burst +    │      │           │
 │Institutional│     │dormancy   │      │ Marine    │
 │ evaluation │      │(2.5yr)    │      │clouds     │
 │            │      │IsaH93 DAC │      │alkalinity │
 │ WRF-Chem   │      │twin       │      │enhancement│
 │ bursts     │      │(0★)       │      │(ZERO repos│
 │            │      │Rudra57    │      │)          │
 │actm-sai-   │      │4 commits  │      │Governance:│
 │csu         │      │(1 day)    │      │ZERO repos │
 │(dormant)   │      │OpenCarbon │      │           │
 │Governance: │      │2★         │      │           │
 │Zereo0317   │      │           │      │           │
 │2 commits   │      │           │      │           │
 └────────────┘      └───────────┘      └───────────┘
```

---

## Cross-Cutting Theme #1: The Velocity Paradox

**The fastest-moving repos aren't always the most scientifically relevant.**

- PCMDI/pcmdi_metrics (133★, 10 commits in 2 weeks) evaluates climate models but doesn't simulate any geoengineering
- regional-geo (0★, 10 commits in 3 days) directly simulates sulfate aerosol injection — but has zero community
- OpenAir-Cyan (76★, 6 commits in 1 day) builds open DAC hardware — then goes dormant for 2.5 years

**Pattern:** Institutional repos are fast but general. Scientific repos are fast during bursts but then go dormant. Hardware repos are fast during certification events but then maintenance stops.

**Episode implication:** Each episode should ask: *What would it take to sustain velocity in this space?*

---

## Cross-Cutting Theme #2: The Governance Vacuum

**Only 1 governance-related repo found across all 3 themes: Zereo0317/climate-intervention-governance (2 commits, Aug 2026).**

| Theme | Governance Repos | Status |
|-------|-----------------|--------|
| Solar Geoengineering | 1 (Zereo0317) | Brand new, 2 commits |
| Carbon Capture | 0 | GAP |
| Ocean Intervention | 0 | GAP |

Governance code for climate tech is **virtually non-existent** on GitHub. The London Protocol, CBD moratorium, and UNFCCC processes are all conducted in diplomatic channels, not code. The one governance repo (Zereo0317) could be the beginning of a new category — or it could be a lone hacker's project that never gains traction.

**Episode implication:** Governance is the invisible infrastructure of climate tech. No governance code = no governance tooling = no early warning system for SRM deployment, ocean intervention experiments, or DAC land grabs.

---

## Cross-Cutting Theme #3: The Open-Source Licensing Spectrum

| Repo | License Type | Significance |
|------|-------------|--------------|
| PCMDI/pcmdi_metrics | Open source (Apache 2.0 implied) | Institutional standard, CMIP-cited |
| OpenAir-Cyan | Open hardware (OSHWA UID US001095) | Physical devices, not just code |
| ClimateMARGO | Open source + CITATION.bib | Academic citation formalized |
| regional-geo | No license specified | Academic code, unclear reuse terms |
| actm-sai-csu | No license specified | DARPA-funded, unclear public license |
| isaH93/dac-moving-bed | No license specified | Research code, no reuse rights |
| Zereo0317 | No license specified | Brand new, TBD |

**Key finding:** The most impactful repos (PCMDI, OpenAir-Cyan) have the clearest licensing. The research-only repos (regional-geo, actm-sai-csu, isaH93) have no license — meaning they're technically not usable by anyone outside the original lab.

**Episode implication:** The "open" in open-source climate tech means different things in different repos. OSHWA certification for hardware (OpenAir-Cyan) is more rigorous than a missing LICENSE file (4 of 7 repos).

---

## Cross-Cutting Theme #4: The Missing Infrastructure

Each theme has a **one thing that doesn't exist yet** but would transform the field:

| Theme | What Exists | What's Missing |
|-------|------------|----------------|
| ☀️ Solar | Simulation (regional-geo), Evaluation (PCMDI), Detection (actm-sai-csu) | **Integration platform** — a tool that connects simulation → evaluation → detection |
| 🌍 Carbon | Hardware (OpenAir-Cyan), Physics models (isaH93), Policy (ClimateMARGO) | **Evaluation framework** — the PCMDI equivalent for DAC |
| 🌊 Ocean | Adjacent models (PCMDI, WRF-Chem) | **Everything** — datasets, parameterizations, governance tools, community |

---

## The 80-Commit Heat Map

| Date Range | Solar | Carbon | Ocean | Total |
|-----------|-------|--------|-------|-------|
| Jan 2022 – Apr 2022 (ClimateMARGO setup) | 0 | 5 | 0 | 5 |
| May 2022 – Feb 2023 (OpenAir-Cyan early, actm-sai-csu) | 10 | 6 | 0 | 16 |
| Jul 2024 (OpenAir-Cyan OSHWA) | 0 | 6 | 0 | 6 |
| Feb 2026 (regional-geo burst) | 10 | 0 | 0 | 10 |
| Jun 2026 (Rudra57, OpenCarbon) | 0 | 4 | 0 | 4 |
| Aug 2026 (ClimateMARGO revival, governance) | 0 | 2 | 0 | 2* |
| Sep 2026 (PCMDI sprint) | 10 | 0 | 0 | 10 |
| **Total Tracked** | **40+** | **35+** | **0** | **~77+** |

*Plus various single commits and README updates

**The heat map shows:** Climate tech commits on GitHub cluster in **bursts tied to papers, certifications, or version releases** — not continuous development. The only continuous activity (PCMDI) is institutional.

---

## Episode Planning Matrix

| Episode | Branch | Key Question | Top Repo | Narrative Anchor |
|---------|--------|--------------|----------|-----------------|
| **Solar Geoengineering** | `solar-geoengineering` | Why is SRM code inside climate models, not in SRM-specific repos? | PCMDI/pcmdi_metrics (133★) | "Who controls the metrics?" |
| **Carbon Capture** | `carbon-capture` | Can open source + CC0 break the $1000/ton DAC cost barrier? | openair-collective/openair-cyan (76★) | "The OSHWA blitz and the 2.5-year silence" |
| **Ocean Intervention** | `ocean-intervention` | Is the GitHub vacuum a governance signal? | ZERO repos | "The dark matter of climate tech" |

---

## Action Items for Future Research

1. **Monitor PCMDI release cadence** — if they add ocean-intervention metrics, the ground floor is built
2. **Track Zereo0317 growth** — the first governance repo could become a new category
3. **Watch for the first ocean geoengineering repo** — it could appear anytime, and when it does, everything changes
4. **License audit** — 4 of 7 repos have no LICENSE file; this is a reusable-rights crisis
5. **Integration opportunity** — the missing infrastructure (solar integration, carbon evaluation, ocean everything) is the biggest gap
6. **Cross-reference with academic literature** — verify that the GitHub absence matches the publication absence

---

## Repository Links

| Repo | URL | Stars | Velocity |
|------|-----|-------|----------|
| PCMDI/pcmdi_metrics | https://github.com/PCMDI/pcmdi_metrics | 133 | 🔴 Fast |
| openair-collective/openair-cyan | https://github.com/openair-collective/openair-cyan | 76 | 🟡 Slow (burst) |
| ClimateMARGO/ClimateMARGO.jl | https://github.com/ClimateMARGO/ClimateMARGO.jl | 73 | 🟡 Slow (dormant) |
| Sustainable-Solutions-Lab/regional-geo | https://github.com/Sustainable-Solutions-Lab/regional-geo | 0 | 🟡 Slow (burst) |
| eabarnes1010/actm-sai-csu | https://github.com/eabarnes1010/actm-sai-csu | 6 | 🟡 Dormant |
| Arcomano1234/SPEEDY-ML | https://github.com/Arcomano1234/SPEEDY-ML | 8 | 🟡 Adjacent |
| IsaH93/dac-moving-bed-digital-twin | https://github.com/IsaH93/dac-moving-bed-digital-twin | 0 | 🟡 Niche |
| Zereo0317/climate-intervention-governance | https://github.com/Zereo0317/climate-intervention-governance | 0 | ⚫ Newborn |
| Rudra57/Direct-Air-Capture | https://github.com/Rudra57/Direct-Air-Capture | 0 | ⚫ Newborn |

---

*Research methodology: GitHub REST API (Search Repositories + List Commits), September 2026. All commit data pulled via List Commits API.*

*Cross-theme analysis by: bro26man-hash (climate-pod-research series)*