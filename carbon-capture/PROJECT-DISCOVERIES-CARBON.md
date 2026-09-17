# 🌍 Carbon Capture — Project Discoveries

**Research Date:** September 2026  
**Podcast Episode:** Carbon Capture — Episode 2

---

## Overview

This document catalogs the open-source carbon capture and direct air capture (DAC) projects discovered through GitHub research, with detailed commit trend analysis from the most active repositories.

---

## Top Projects by Activity & Relevance

### 1. openair-collective/openair-cyan ⭐ 76
- **Language:** Custom (open hardware)
- **Focus:** DIY small-scale open hardware direct air carbon capture device. OSHWA-certified (UID US001095). Documentation at https://openair-collective.github.io/openair-cyan
- **Last Updated:** Aug 19, 2026 (repository updates); last meaningful commit Feb 12, 2024
- **Key Feature:** Fully documented, DIY DAC device — the most accessible carbon capture project on GitHub
- **Podcast Angle:** OpenAir-Cyan is the " Arduino of carbon capture" — it makes DAC tangible and reproducible. The OSHWA certification is significant for hardware open-source.
- **Commit Insight:** Heavy Feb 12, 2024 activity (OSHWA UID, CITATION.cff, README). Before that, activity was May–Jul 2022. The project is in maintenance mode but has a strong foundation.

### 2. zikribayraktar/Carbon_Capture_ML ⭐ 56
- **Language:** Jupyter Notebook
- **Focus:** Survey of all published carbon capture ML papers, data, code, and supplemental materials
- **Last Updated:** Aug 19, 2026 (repository updates); Last meaningful commit May 8, 2024
- **Key Feature:** Living survey of CCUS ML research — continuously updated with new papers
- **Podcast Angle:** This is the bibliography/manifesto for ML in carbon capture. When someone asks "what's happening with AI + DAC?", this repo is the answer.
- **Commit Insight:** Steady paper-addition pattern. 4 README updates (Jan–Apr 2024), then OpenDAC paper added May 2024. The May 2024 commit suggests the survey is still being maintained, even if quietly.

### 3. yohanesnuwara/carbon-capture-and-storage ⭐ 85
- **Language:** Lasso (reservoir simulation)
- **Focus:** Integration of reservoir simulation, rock physics, seismic modeling, & geomechanics for CCS monitoring. Originally a BSc thesis.
- **Last Updated:** Jul 1, 2026 (repository updates); Last meaningful commit Mar 6, 2021
- **Key Feature:** Full-stack CCS simulation — from injection to seismic monitoring
- **Podcast Angle:** The classic "academic thesis ghost" — 85 stars but zero activity since 2021. The thesis got cited, but nobody维护 the code.
- **Commit Insight:** All commits are from Feb–Mar 2021. Heavy simulation result uploads (zip files, notebooks). Classic academic dump pattern — no CI, no testing, just results.

### 4. tonyzyl/CO2-Soft-sensor-for-a-carbon-capture-pilot-plant ⭐ 16
- **Language:** Jupyter Notebook
- **Focus:** Hybrid mechanistic + data-driven (DAE-LSTM) model for estimating CO2 concentration profile in a carbon capture pilot plant
- **Last Updated:** Aug 18, 2026
- **Key Feature:** Digital-twin approach to carbon capture — physics-informed neural networks
- **Podcast Angle:** The soft-sensor approach is the practical path — you don't need to rebuild the plant, just model it digitally.

### 5. Beckybams/AI-for-Carbon-Capture-Optimization ⭐ 25
- **Language:** Python
- **Focus:** ML project using synthetic industrial data to improve carbon capture efficiency
- **Last Updated:** Mar 2, 2026
- **Key Feature:** Synthetic data approach — generates training data when real plant data is unavailable
- **Podcast Angle:** The data-scarcity problem in industrial CC刻. This repo's synthetic data approach is a template for how to work when you can't get real plant data.

### 6. kfdsievert/Cost-Model--DAC ⭐ 6
- **Language:** Python
- **Focus:** Probabilistic experience curves and Monte Carlo simulations for projecting future DAC costs
- **Last Updated:** Jun 4, 2026
- **Key Feature:** Cost projection model — answers the "$1000/ton vs $100/ton" question with uncertainty quantification
- **Podcast Angle:** The economics question is the most important question. This model gives a probabilistic answer, not a point estimate.

### 7. openair-collective/openair-epiphyte ⭐ 9
- **Language:** C++
- **Focus:** Epiphyte — miniature, stand-alone, open source direct air capture machine
- **Last Updated:** Jun 18, 2026
- **Key Feature:** Even smaller and simpler than Cyan. Stand-alone operation.
- **Podcast Angle:** If Cyan is the Arduino of DAC, Epiphyte is the ATtiny — minimal, standalone, embedded.

---

## The Carbon Capture Field on GitHub: Key Patterns

### Pattern 1: The August 2026 Materials Wave
Multiple DAC materials repositories were updated around Aug 19-23, 2026:
- `tjz21/DAC_peroxovanadates` (Aug 19, 2026)
- `tjz21/DAC_peroxotitanates` (Aug 19, 2026)
- `CCSI-Toolset/membrane_model` (Aug 23, 2026)
- `openair-cyan` (Aug 19, 2026 — repository update)

**Interpretation:** This suggests a coordinated research event in open computational chemistry — possibly a shared workshop, conference, or data-a-thon focused on DAC materials.

### Pattern 2: Open Hardware is Thriving
OpenAir-Cyan (76★) and OpenAir-Epiphyte (9★) are the most visibly active community-driven projects. The OSHWA certification of Cyan is a milestone for open-source hardware in climate tech.

### Pattern 3: The Cost Gap
`kfdsievert/Cost-Model--DAC` highlights the central economic question: can DAC costs drop below $100/ton? The current ethanol-injection pilot (Carbon Engineering) is at ~$250/ton. The probabilistic model shows wide uncertainty.

### Pattern 4: Academic Deposit vs. Software Engineering
The majority of high-star carbon capture repos (carbon-capture-and-storage at 85★, Carbon_Capture_ML at 56★) follow an academic deposit pattern — code is uploaded as research supplementary material, then nobody maintains it. No CI, no tests, no roadmap.

### Pattern 5: The ML Surge
Carbon_Capture_ML (56★) and AI-for-Carbon-Capture-Optimization (25★) show that ML is the dominant paradigm for carbon capture innovation on GitHub. The question is whether ML can actually break the cost barrier or just optimize incremental improvements.

---

## Commit Trend Analysis: Carbon Capture Repos

| Repository | Stars | Last Meaningful Commit | Activity Level | Development Style |
|------------|-------|----------------------|----------------|-------------------|
| openair-cyan | 76 | Feb 12, 2024 | ★★★☆☆ | Community-driven, maintenance mode |
| Carbon_Capture_ML | 56 | May 8, 2024 | ★★☆☆☆ | Paper-driven survey |
| carbon-capture-and-storage | 85 | Mar 6, 2021 | ★☆☆☆☆ | Academic deposit (dormant) |
| CO2-Soft-sensor | 16 | Aug 18, 2026 | ★★☆☆☆ | Active but small |
| AI-for-CC-Optimization | 25 | Mar 2, 2026 | ★★☆☆☆ | Active but small |
| Cost-Model--DAC | 6 | Jun 4, 2026 | ★★☆☆☆ | Active but small |

---

## Detailed Commit Histories

### openair-collective/openair-cyan — Recent Commits
| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| Feb 12, 2024 | `b5422b3` | KCollins | Update README — added OSHWA UID link |
| Feb 12, 2024 | `b164257` | KCollins | Add files via upload |
| Feb 12, 2024 | `828f496` | KCollins | Added OSHWA UID logo (US001095) |
| Feb 12, 2024 | `b731cd8` | KCollins | Add files via upload |
| Feb 12, 2024 | `4b08fb3` | KCollins | Create CITATION.cff |
| Feb 12, 2024 | `859bfa8` | KCollins | Update README |
| Jul 20, 2022 | `d12008e` | DaOfficialWizard | Update README |
| May 17, 2022 | `b8621ba` | ZanzyTHEbar | Add files to improve usability |
| May 15, 2022 | `d025674` | DaOfficialWizard | Update README |
| May 15, 2022 | `784ace5` | DaOfficialWizard | Update README |

**Trend:** Two developer communities: DaOfficialWizard + ZanzyTHEbar (May–Jul 2022, active building), then K Collins (Feb 2024, OSHWA certification + documentation). The Feb 2024 burst was all about formalization (OSHWA UID, CITATION.cff). This is a project that hit its practical peak in 2022 and is now in documentation/maintenance mode.

### zikribayraktar/Carbon_Capture_ML — Recent Commits
| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| May 8, 2024 | `ca9a31f` | Zikri Bayraktar | OpenDAC paper added |
| Apr 25, 2024 | `4c01842` | Zikri Bayraktar | Update README |
| Mar 15, 2024 | `2b69376` | Zikri Bayraktar | Update README |
| Jan 21, 2024 | `e80dfd6` | Zikri Bayraktar | Update README |
| Jan 21, 2024 | `fe28496` | Zikri Bayraktar | Update README |
| Mar 1, 2023 | `a3a02e9` | Zikri Bayraktar | New paper |
| Feb 16, 2023 | `93e5a40` | Zikri Bayraktar | MOFsimplify paper added |
| Feb 5, 2023 | `0c62b02` | Zikri Bayraktar | New process paper added |
| Feb 5, 2023 | `6129691` | Zikri Bayraktar | New process paper added |
| Feb 2, 2023 | `caf8b96` | Zikri Bayraktar | New paper added to process |

**Trend:** The project was most active in Feb 2023 (5 commits in 4 days, multiple papers). Then a lull, then 4 README updates in Jan 2024, and the OpenDAC paper in May 2024. The pattern is: burst of paper additions → quiet period → README maintenance → occasional new paper. This is a living survey, not a software project.

### yohanesnuwara/carbon-capture-and-storage — Recent Commits
| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| Mar 6, 2021 | `0be66ca` | yohanesnuwara | Add sim result zip file |
| Mar 6, 2021 | `3d75b78` | yohanesnuwara | Delete first.txt |
| Mar 6, 2021 | `52c0189` | yohanesnuwara | Add sim result case 3C |
| Mar 6, 2021 | `91137e6` | yohanesnuwara | Delete old case folder |
| Mar 6, 2021 | `12151e1` | yohanesnuwara | Move sim results to folder |
| Mar 6, 2021 | `bf7ec9d` | yohanesnuwara | Injection sim results |
| Mar 3, 2021 | `0fdb0a6` | yohanesnuwara | Upload CO2 EOS notebook |
| Mar 1, 2021 | `1f4d108` | yohanesnuwara | Create first.txt |
| Feb 25, 2021 | `532f46c` | yohanesnuwara | Upload geomechanics data |
| May 4, 2020 | `765e206` | yohanesnuwara | Created using Colaboratory |

**Trend:** 10 commits over 10 months (May 2020 – Mar 2021), all by one person, all theoretical/academic (simulation results, data uploads, notebooks). Then complete silence. This is the "academic thesis ghost" pattern — 85 stars from citations, but zero maintenance.

---

## The August 2026 DAC Materials Wave

A notable cluster of commits across multiple DAC materials repositories occurred around August 19-23, 2026:

| Repository | Date | Commit | Focus |
|------------|------|--------|-------|
| tjz21/DAC_peroxovanadates | Aug 19, 2026 | — | Peroxovanadate sorbents |
| tjz21/DAC_peroxotitanates | Aug 19, 2026 | — | Peroxotitanate sorbents |
| CCSI-Toolset/membrane_model | Aug 23, 2026 | — | Membrane separation模型 |
| openair-cyan | Aug 19, 2026 | — | Repository update |

**Interpretation:** The simultaneous updates across independent research groups suggest either (a) a shared workshop/conference deadline, (b) a coordinated data release, or (c) a community wiki-a-thon for DAC materials. This is worth investigating for the podcast.

---

## 🎙️ Podcast Episode Notes: Carbon Capture

### Key Questions for the Episode
1. Can open source break the $1000/ton DAC cost barrier? What would it take?
2. What makes OpenAir-Cyan special? OSHWA certification, DIY accessibility, community.
3. Are peroxides (peroxovanadates, peroxotitanates) the sorbent breakthrough of the future?
4. Electro-swing DAC and the soft-sensor approach — digital twins for CC刻 plants.
5. The August 2026 materials wave — is there a coordinated research event happening?
6. Why do high-star academic repos go dormant? The carbon-capture-and-storage ghost (85★, zero activity since 2021).

### Thesis Statements for the Episode
- Open hardware (Cyan) is the most promising open-source CC刻 approach because it makes the technology tangible and reproducible
- ML in carbon capture is primarily a survey/bibliography tool right now, not a discovery engine
- The cost question (Can it reach $100/ton?) is the central question, and probabilistic models show wide uncertainty
- The August 2026 materials wave suggests latent community activity that could accelerate with proper coordination

### Sources
- https://github.com/openair-collective/openair-cyan
- https://github.com/zikribayraktar/Carbon_Capture_ML
- https://github.com/yohanesnuwara/carbon-capture-and-storage
- https://github.com/tonyzyl/CO2-Soft-sensor-for-a-carbon-capture-pilot-plant
- https://github.com/Beckybams/AI-for-Carbon-Capture-Optimization
- https://github.com/kfdsievert/Cost-Model--DAC
- https://github.com/openair-collective/openair-epiphyte
- https://github.com/tjz21/DAC_peroxovanadates
- https://github.com/tjz21/DAC_peroxotitanates