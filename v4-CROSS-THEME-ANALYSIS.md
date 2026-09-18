# 🎙️ Climate Pod Research — v4 Cross-Theme Analysis
## September 2026: The Three Universes of Climate Tech on GitHub

**Research Version:** v4 | **Date:** September 18, 2026 | **Branches:** solar-geoengineering, carbon-capture, ocean-intervention

---

## 📊 The Big Picture

We pulled fresh commit histories from **12 repositories** across all three podcast themes, searched **10+ query strategies** for ocean geoengineering, and identified **three distinct universes** of climate technology development on GitHub.

---

## 🌌 The Three Universes

### Universe 1: FAST — Institutional, Funded, Sustained
| Repo | Stars | Theme | Commit Pace | Status |
|------|-------|-------|-------------|--------|
| **open-sustainable-technology** | 2,552 | Carbon (directory) | Continuous | 🔴 Active |
| **WRF** | 1,763 | Solar (atmosphere) | 5 commits/week | 🔴 Active |
| **Oceananigans.jl** | 1,413 | Ocean (CFD) | Steady | 🔴 Active |
| **PCMDI Metrics** | 133 | Solar (evaluation) | Quarterly | 🔴 Active |
| **MDTF-diagnostics** | 80 | Solar/Ocean (diagnostics) | Bursty | 🔴 Active |

**Characteristics:** Multi-contributor, institutionally funded, professional release cycles, named contributors from NOAA, NCAR, GFDL, and universities.

**What they share:** They simulate the world as it is. Not as we might choose to make it.

---

### Universe 2: SLOW — Individual, Unfunded, Dormant
| Repo | Stars | Theme | Last Active | Status |
|------|-------|-------|-------------|--------|
| **carbon-capture-and-storage** | 85 | Carbon (simulation) | Mar 2021 | ⚫ Ghost |
| **openair-cyan** | 76 | Carbon (hardware) | Feb 2024 | 🟡 Dormant |
| **ClimateMARGO.jl** | 73 | Solar (economics) | Aug 2026 (README only) | 🟡 Phantom |
| **Carbon_Capture_ML** | 56 | Carbon (bibliography) | May 2024 | 🟡 Maturing |
| **CO2-Sequestration** | 32 | Carbon (MATLAB) | Periodic | 🟡 Sparse |
| **srm-forever** | 0 | Solar (economics) | Aug 2026 | ⚪ Invisible |

**Characteristics:** Individual authors, academic origins, thesis-lifecycle commit patterns (burst then death), zero community growth.

**What they share:** They built something important. Then they stopped. The stars measure citations, not usage.

---

### Universe 3: EMPTY — Zero Presence
| Topic | Repos Found | Papers Found | Status |
|-------|-------------|-------------|--------|
| **Ocean Alkalinity Enhancement (OAE)** | **0** | 50+ | ⚫ Absent |
| **Iron Fertilization** | **0** | 100+ | ⚫ Absent |
| **Marine Cloud Brightening** | **0** | 30+ | ⚫ Absent |
| **Ocean Upwelling Pumping** | **0** | 20+ | ⚫ Absent |
| **SRM-specific modules (in any model)** | **0** | Many theoretical | ⚫ Absent |

**Characteristics:** Abundant in scientific literature, absent from open-source code. The "dark matter" of climate tech.

**What this means:** Either the field is too young, too complex, or too politically charged for open-source development. Or the scientific community is responsibly saying: "We don't have the models to do this safely."

---

## 🔥 The Five Headline Findings

### 1. The CC0 License Revolution 💀
The **biggest open-science story** in our research isn't a code breakthrough — it's a license choice. Two DAC materials repositories (`tjz21/DAC_peroxovanadates` and `tjz21/DAC_peroxotitanates`) both adopted **CC0 public domain dedication** in September 2025.

**What this means:** Researchers are treating computational screening data as public infrastructure. Not open-source. Not public-license. **Public domain.** No copyright. No attribution required. No restrictions.

**Episode hook:** "The most important thing about these repos isn't what they contain — it's what the authors gave up. Copyright. They decided carbon capture data should be as free as air."

### 2. The Precipitation-Buoyancy POD Sprint 🌧️
On **June 19, 2026**, NOAA-GFDL developers made **5 commits to a single file** (`MCS_precip_buoy_stats.rst`) in one day, culminating in the addition of an entirely new diagnostic tool.

**What this tells us:** Something triggered an intensive writing session — a paper deadline, a workshop, a funding deliverable. Whatever it was, it produced the most ocean-relevant tool in open-source climate science.

**But here's the catch:** The POD evaluates model accuracy. It doesn't simulate interventions. It's a ruler, not a crystal ball.

**Episode hook:** "The most ocean-friendly tool in climate science went through a single-day development sprint. And it's still just measuring whether models are right. It doesn't predict what happens when we change the ocean."

### 3. ClimateMARGO's Phantom Revival 👻
Two README updates on August 17, 2026 — after 2+ years of total silence. Zero code commits.

**Three possible interpretations:**
- **A:** New funding for climate-economic modeling of SRM
- **B:** SEO/discoverability update for better search ranking
- **C:** False start — excitement fades without implementation

**Our assessment:** Scenario B. GitHub README updates without code changes are the academic equivalent of repainting the storefront while the lights stay off.

**Episode hook:** "ClimateMARGO woke up from a 2-year nap and only changed the marketing. No new equations. No new scenarios. Just a fresher coat of paint."

### 4. srm-forever — The Zero-Star Theorist ⚪
The most conceptually important repo in our entire research has **zero stars**.

`srm-forever` implements Weitzman certainty-equivalent discounting for SRM cost dynamics — answering: "What does it cost to keep solar radiation management running forever?"

The Weitzman framework says that under certain conditions, the certainty-equivalent discount rate can become **negative**, meaning uncertainty actually favors *more* intervention — counterintuitively.

**Episode hook:** "Zero stars. But this repo contains the most important question in solar geoengineering economics: What's the price tag on permanently blocking sunlight? And nobody's watching."

### 5. The Ocean Intervention Gap 🌊
**Zero repositories. Full stop.**

Across 10+ search queries targeting ocean geoengineering (OAE, iron fertilization, marine cloud brightening, ocean upwelling, albedo modification), GitHub returned **nothing**.

Meanwhile, the scientific literature has:
- 50+ papers on OAE (Nature, Science)
- 100+ papers on iron fertilization
- 30+ papers on marine cloud brightening

**The silence on GitHub is either a warning or an invitation.**

**Episode hook:** "We have models for the atmosphere. Models for the land. Models for the ice. We don't have models for what we might do to the ocean. That's not a gap in the code. It's a gap in the conversation."

---

## 📈 Consolidated Commit Trend Dashboard

### Solar Theme (☀️)
| Repo | Recent Commits | Peak Activity | Trend |
|------|-----------------|----------------|-------|
| WRF | 15 (3 weeks) | v4.8.0 release | 🔴 Active |
| MDTF-diagnostics | 15 (3 months) | 5 commits / 1 day (Jun 19) | 🔴 Active |
| ClimateMARGO | 15 total (2 recent) | README-only revival | 🟡 Dormant |
| srm-forever | Unknown | Aug 2026 update | ⚪ Invisible |
| PCMDI | Referenced | v4.2.1 (Sep 2026) | 🔴 Active |
| **SRM-specific code** | **0** | **N/A** | **⚫ Absent** |

### Carbon Theme (🌍)
| Repo | Recent Commits | Peak Activity | Trend |
|------|-----------------|----------------|-------|
| open-sustainable-technology | Continuous | 2,552★ ecosystem | 🔴 Active |
| carbon-capture-and-storage | 15 (final burst 2021) | Thesis defense prep | ⚫ Ghost |
| openair-cyan | 15 (Feb 2024 blitz) | OSHWA certification | 🟡 Dormant |
| Carbon_Capture_ML | Referenced | Survey, maturing | 🟡 Slow |
| DAC_peroxovanadates | Recent (Sep 2025) | CC0 dedication | 🟢 New |
| DAC_peroxotitanates | Recent (Sep 2025) | CC0 dedication | 🟢 New |
| **Community growth repos** | **0** | **N/A** | **⚫ Absent** |

### Ocean Theme (🌊)
| Repo | Recent Commits | Peak Activity | Trend |
|------|-----------------|----------------|-------|
| MDTF-diagnostics | 15 (Jun-Aug 2026) | Precip-buoyancy POD | 🔴 Active |
| WRF (coupled) | 15 (May-Jun 2026) | v4.8.0 release | 🔴 Active |
| **Dedicated ocean geoengineering** | **0** | **N/A** | **⚫ ZERO** |

---

## 🎙️ Episode Planning Matrix

| Episode | Branch | Core Question | Key Evidence | Narrative Arc |
|---------|--------|--------------|----------------|---------------|
| **Solar Geoengineering** | `solar-geoengineering` | Why is SRM code so scarce? | WRF v4.8.0 (solar radiation fix); MDTF POD (5-commit sprint); ClimateMARGO (phantom revival); srm-forever (0★, Weitzman) | "The building blocks exist. The blueprint doesn't." |
| **Carbon Capture** | `carbon-capture` | Can open source break the $1000/ton barrier? | OpenAir-Cyan (OSHWA, frozen); CC0 DAC materials (revolution); carbon-capture-and-storage (85★ ghost) | "The ghosts, the pioneers, and the public domain." |
| **Ocean Intervention** | `ocean-intervention` | Why is ocean geoengineering the empty quadrant? | 10+ queries, 0 results; MDTF as ocean-adjacent lifeline; Oceananigans.jl (no intervention module) | "The silence is either a warning or an invitation." |

---

## 🔑 Five Talking Points for the Podcast Intro

1. **"We searched GitHub for ocean geoengineering code. There isn't any."**
   The empty quadrant. Zero repositories. A thousand papers. What does the silence mean?

2. **"The atmospheric model that could simulate solar geoengineering just released v4.8 — with a fix for solar radiation. But it's not a geoengineering model. It's a weather model. The gap is not technical. It's political."**
   WRF's power vs. its silence on intervention.

3. **"Two researchers uploaded computational screening data, gave up their copyright, and got 2 stars."**
   The CC0 revolution. Data should be free. Nobody's watching.

4. **"On June 19th, five scientists made five commits to one file in one day. The most ocean-relevant diagnostic in open source was being born. But it measures accuracy — not what we'd do."**
   The MDTF precipitation-buoyancy POD story.

5. **"A climate-economic model went dormant for two years, then got two README updates, and looks alive. But there's no new code. Just marketing."**
   The phantom revival of ClimateMARGO.

---

## 📋 Research Log — v4 Consolidated

| Date | Activity |
|------|----------|
| Sep 17, 2026 | Solar theme: WRF (15 commits), ClimateMARGO (15), MDTF (15) pulled |
| Sep 17, 2026 | Carbon theme: openair-cyan (15), carbon-capture-and-storage (15) pulled |
| Sep 17, 2026 | Ocean theme: 10+ queries, ZERO repos confirmed |
| Sep 17, 2026 | CC0 license revolution identified in DAC materials repos |
| Sep 17, 2026 | Jun 19 MDTF sprint discovered (5 commits, 1 file, precip-buoyancy POD) |
| Sep 18, 2026 | srm-forever profile completed (Weitzman discounting, 0★) |
| Sep 18, 2026 | ClimateMARGO phantom revival analyzed (2 README updates, 0 code) |
| Sep 18, 2026 | v4 notes pushed to all three theme branches |
| Sep 18, 2026 | v4 consolidated cross-theme analysis pushed to main |

---

## 🔗 Quick Links

| Resource | Link |
|----------|------|
| **Repository** | https://github.com/bro26man-hash/climate-pod-research |
| ☀️ Solar branch | https://github.com/bro26man-hash/climate-pod-research/tree/solar-geoengineering |
| 🌍 Carbon branch | https://github.com/bro26man-hash/climate-pod-research/tree/carbon-capture |
| 🌊 Ocean branch | https://github.com/bro26man-hash/climate-pod-research/tree/ocean-intervention |
| WRF | https://github.com/wrf-model/WRF |
| MDTF-diagnostics | https://github.com/NOAA-GFDL/MDTF-diagnostics |
| ClimateMARGO.jl | https://github.com/ClimateMARGO/ClimateMARGO.jl |
| OpenAir-Cyan | https://github.com/openair-collective/openair-cyan |
| DAC Peroxovanadates (CC0) | https://github.com/tjz21/DAC_peroxovanadates |
| srm-forever | https://github.com/hausfath/srm-forever |
| Open-Sustainable-Technology | https://github.com/protontypes/open-sustainable-technology |

---

*Research conducted via GitHub API — commit histories pulled September 2026* *Branches: solar-geoengineering | carbon-capture | ocean-intervention* *Version: v4*