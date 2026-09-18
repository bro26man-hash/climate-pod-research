# ☀️ Solar Geoengineering — Project Discoveries
## Podcast Episode Research: Solar Radiation Management (SRM)

**Last Updated:** September 2026 | **Research Version:** v4

---

## 🔍 Executive Summary

Our GitHub research across 10+ search queries reveals a solar geoengineering ecosystem that is **highly institutional but thin on SRM-specific code**. The climate simulation infrastructure (WRF, PCMDI, MDTF) is vibrant and actively maintained, but explicit solar geoengineering modules are scarce. The SRM discourse lives more in academic papers than in open-source repositories.

---

## 📊 Key Projects Profiled

### 1. WRF — Weather Research and Forecasting Model
| Field | Detail |
|-------|--------|
| **Repository** | `wrf-model/WRF` |
| **Stars** | 1,763 ★ |
| **Language** | Fortran |
| **License** | open-source |
| **Last Activity** | June 8, 2026 (v4.8.0 release) |
| **Contributors** | 15+ active in recent window |

**Why It Matters for Our Episode:**
WRF is the foundational atmospheric model for virtually all climate and weather simulation. Its v4.8.0 release (June 2026) includes direct solar radiation physics updates — specifically a correction for Earth-outgoing-top-of-atmosphere (EOT) solar radiation calculation. This is the kind of base simulation capability that any SRM model would build upon.

**Key Recent Commits:**
- `06d4240` — Merge release-v4.8.0 (Jun 8, 2026) ← **Major release**
- `0708348` — README and version updated to v4.8.0 (Jun 6, 2026)
- `e836cd6` — **Correction for EOT calculation for solar radiation** (May 28, 2026) ← Directly relevant!
- `6a289e1` — Turned off tempo_aerosolaware and tempo_hailaware (Jun 5, 2026) ← Aerosol parameterization changes
- `8299919` — Updated MYNN-EDMF pointer, removed icloud_bl package (May 27, 2026)
- `9c87d29` — New namelists for ShinHong PBL and revised MMM surface layer (May 20, 2026)

**Episode Angle:** "The building blocks of solar geoengineering simulation already exist in WRF's radiation scheme — but they're designed for natural conditions, not engineered interventions. What would it take to add an SRM module?"

---

### 2. PCMDI Metrics — Model Evaluation Toolkit
| Field | Detail |
|-------|--------|
| **Repository** | `PCMDI/pcmdi_metrics` |
| **Stars** | 133 ★ |
| **Language** | Python |
| **Last Activity** | September 4, 2026 (v4.2.1) |

**Why It Matters:**
PCMDI provides the CMIP6 evaluation toolkit — the gold standard for assessing whether climate models are accurate. If solar geoengineering were to be governed internationally, you'd need verified models. PCMDI is the verification infrastructure.

**Episode Angle:** "Before you can regulate solar geoengineering, you need to agree on what 'right' looks like. PCMDI is the yardstick — and it's quietly one of the most important tools in climate governance."

---

### 3. MDTF Diagnostics — Process-Oriented Model Evaluation
| Field | Detail |
|-------|--------|
| **Repository** | `NOAA-GFDL/MDTF-diagnostics` |
| **Stars** | 80 ★ |
| **Language** | Jupyter Notebook |
| **Last Activity** | August 14, 2026 |

**Why It Matters — The Precipitation-Buoyancy POD:
The most ocean-relevant diagnostic in open source. The precipitation-buoyancy POD (Process-Oriented Diagnostic) was the subject of 5 commits on June 19, 2026 alone — developers pushed multiple updates to `MCS_precip_buoy_stats.rst` in a single day. This diagnostic evaluates whether models correctly simulate the relationship between precipitation and atmospheric buoyancy — critical for understanding how solar radiation management might alter global precipitation patterns.

**Key Recent Commits:**
- `87f8105` — Merge PR #825 (Aug 14, 2026)
- `4cfc99c`, `699de27`, `d6bc6d0`, `3904d29` — **4 updates to MCS_precip_buoy_stats.rst on June 19, 2026** ← Intensive development day!
- `33024ad` — **Add MCS precipitation-buoyancy statistics POD** (Jun 19, 2026) ← New diagnostic feature!
- `2df59f6` — Merge PR #823 (Jun 8, 2026)
- `16f936c`, `b96127e` — README updates (Jun 8, 2026)
- `95991fc` — Add quarterly metrics workflow for traffic logging (Jun 1, 2026)

**Episode Angle:** "Climate models need to get precipitation right if we're going to simulate sunlight blocking. NOAA's MDTF just got a major upgrade to its precipitation diagnostic — and it came in a single-day blitz that tells us this is a hot topic."

---

### 4. ClimateMARGO.jl — Climate-Economic Modeling Framework
| Field | Detail |
|-------|--------|
| **Repository** | `ClimateMARGO/ClimateMARGO.jl` |
| **Stars** | 73 ★ |
| **Language** | Julia |
| **Last Activity** | August 17, 2026 (README update) |

**Why It Matters:**
MARGO (Modular framework for优化的 trade-offs between emissions Mitigation, Adaptation, and cOst) is an idealized climate-economic model. It's the type of tool that would be used to evaluate the cost-benefit economics of solar geoengineering vs. mitigation vs. adaptation.

**Key Recent Commits — The Revival Signal:**
- `d916f36` — Update README.md (Aug 17, 2026) ← **First activity in 2+ years!**
- `6d9ba7a` — Update README.md (Aug 17, 2026) ← Second README update same day
- `57d4da7` — Unit conversions update with comment from PR #86 (Oct 2023) ← Last code change
- All commits between Oct 2023 and Aug 2026 are README/documentation only

**Episode Angle:** "ClimateMARGO went dormant for 2 years, then suddenly two people updated the README in the same day. Is the economic modeling community waking up to solar geoengineering questions? Or is it a false start? The silence in the code commits speaks volumes."

**⚠️ Caveat for Episode:** No actual code changes — only README updates. This could indicate new users discovering the project rather than active development.

---

### 5. srm-forever — Interactive SRM Economics Model
| Field | Detail |
|-------|--------|
| **Repository** | `hausfath/srm-forever` |
| **Stars** | 0 ★ |
| **Language** | Unknown |
| **Last Activity** | August 26, 2026 |

**Why It Matters — Despite Zero Stars:**
This is the most conceptually important repo we found for solar geoengineering, despite having zero stars. It implements **Weitzman certainty-equivalent discounting** applied to SRM cost dynamics — answering the question: "What does it cost to keep solar radiation management going forever?"

This is directly based on Martin Weitzman's theoretical framework on discounting under uncertainty, which is the economic foundation for long-term climate policy analysis.

**Episode Angle:** "Zero stars, but this might be the most important repo in our entire series. It asks the question nobody wants to answer: what's the price tag on permanently blocking sunlight? Weitzman's math says the answer is counterintuitive."

---

## 🎙️ Solar Geoengineering — Episode Talking Points

### The Core Paradox
> "There are 1,763 stars on the WRF model — the atmospheric simulation engine that would power any solar geoengineering scenario. But there are zero repos dedicated to the actual geoengineering logic. We can simulate the atmosphere perfectly. We just can't simulate what we'd do to it."

### The Infrastructure Argument
- WRF v4.8.0 was released June 2026 with solar radiation physics corrections
- MDTF's precipitation-buoyancy POD went through a 5-commit intensive day (June 19, 2026)
- PCMDI metrics v4.2.1 provides CMIP6 evaluation standards
- **None of these tools were designed for SRM — they're the infrastructure SRM would need**

### The Governance Gap
- ClimateMARGO's revival (README-only, no code) suggests policy interest but no action
- srm-forever (0★) has the theoretical framework but no community
- The gap between simulation capability and governance tooling is the story

### Key Quote for the Episode
> "We have the weather models. We have the economic models. We have the diagnostic tools. What we don't have is the decision-making framework — and that's an open-source problem."

---

## 📈 Commit Trend Summary — Solar Theme

| Repo | Recent Commits | Peak Activity | Trend |
|------|-----------------|----------------|-------|
| **WRF** | 15 in ~3 weeks | v4.8.0 release (Jun 2026) | 🔴 Active — institutional pace |
| **MDTF-diagnostics** | 15 in ~3 months | 5 commits single day (Jun 19, 2026) | 🔴 Active — diagnostic expansion |
| **ClimateMARGO** | 15 total, 2 recent | README-only revival (Aug 2026) | 🟡 Dormant with revival signal |
| **srm-forever** | Unknown | Aug 2026 update | 🟢 Maintained by individual |
| **PCMDI** | Referenced in v3 | v4.2.1 (Sep 2026) | 🔴 Active — CMIP6 standard |

**Overall Solar Theme Trend:** Infrastructure is active and well-funded. SRM-specific development is absent. The story is about capability without direction.

---

## 🔗 Links
- WRF: https://github.com/wrf-model/WRF
- MDTF-diagnostics: https://github.com/NOAA-GFDL/MDTF-diagnostics
- ClimateMARGO.jl: https://github.com/ClimateMARGO/ClimateMARGO.jl
- srm-forever: https://github.com/hausfath/srm-forever
- PCMDI Metrics: https://github.com/PCMDI/pcmdi_metrics
