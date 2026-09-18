# 🌍 Carbon Capture — Project Discoveries

**Branch:** `carbon-capture` | **Last Updated:** September 2026 (v4)

Detailed profiles of open-source repositories relevant to direct air capture (DAC), carbon capture and storage (CCS), carbon removal technologies, and the open-science infrastructure around them.

---

## Tier 1: The Open-Source Climate-Tech Directory

### 1. Open Sustainable Technology
- **Repo:** [protontypes/open-sustainable-technology](https://github.com/protontypes/open-sustainable-technology)
- **Stars:** 2,552 | **Language:** Markdown/YAML | **Last commit:** September 9, 2026
- **Focus:** A comprehensive, community-curated directory of 2,500+ open-source climate technology projects. Not a single tool, but the **GitHub of climate tech.**
- **Why it matters for carbon capture:** This is the ecosystem map. If you want to find open-source DAC code, CCS simulators, or carbon accounting tools, you start here. It's the single most important organizational artifact in the carbon-capture GitHub ecosystem.

**Recent Commit Highlights (15 commits pulled):**
| Date | Commit | Addition | Significance |
|------|--------|----------|-------------|
| Sep 9, 2026 | Add-MUIO (#1638) | MUIO | New carbon removal/offset standard entry |
| Sep 9, 2026 | Add-MUIOGO (#1639) | MUIOGO | Complementary standard entry |
| Sep 1, 2026 | Fix dead links in README | Maintenance | Ongoing curation quality |
| Aug 23, 2026 | Add claude-carbon (#1633) | AI tool | AI-assisted carbon accounting tool |
| Aug 18, 2026 | Add Story Seed Library (#1630) | Narrative | Climate storytelling resources |
| Aug 18, 2026 | Add openflexure microscope (#1631) | Hardware | Open-source scientific instrument |
| Jul 19, 2026 | AI content review PR template | Governance | New quality gate for entries |
| Jul 2/1, 2026 | Add PowerIO, ASSETRA, ToOp | Multiple | Energy, assessment, optimization tools |
| Jun 23, 2026 | Add wbdata, Volca LCA | Data/tools | World Bank data, LCA tool |
| Jun 6, 2026 | Add EpexPredictor | Prediction | Electricity price prediction tool |

**🎙️ Episode Hook:** This repo adds 2–3 new entries per month, consistently. It's not a sprint — it's a marathon. The August 2026 addition of "claude-carbon" (an AI tool for carbon accounting) signals that the climate-tech community is starting to use AI as a curation and analysis layer. The July 2026 PR template for AI content review is equally significant: the community is building governance for AI-generated entries.

---

## Tier 2: DIY Open Hardware

### 2. OpenAir-Cyan
- **Repo:** [openair-collective/openair-cyan](https://github.com/openair-collective/openair-cyan)
- **Stars:** 76 | **Language:** Various | **Last commit:** February 12, 2024
- **Focus:** DIY small-scale open hardware direct air carbon capture device. **OSHWA-certified** (Open Source Hardware Association UID US001095). Documentation at https://openair-collective.github.io/openair-cyan
- **Why it matters:** This is the closest thing to a "People's DAC" — an open-source, DIY-commissionable, hardware-certified direct air capture device. It's the bridge between the maker movement and carbon removal.

**Recent Commit Highlights (15 commits pulled):**
| Date | Commit | Significence |
|------|--------|-------------|
| Feb 12, 2024 | OSHWA UID link added to README | Hardware certification complete |
| Feb 12, 2024 | 7 commits in a single day | **One-day blitz: files, CITATION.cff, README update** |
| Jul 20, 2022 | README update | Last activity before blitz |
| May 17, 2022 | Usability improvements (files added) | Minor enhancement |
| May 5–7, 2022 | CodeQL analysis workflow setup | CI/CD basics |
| May 2022 | GitHub workflows deleted | Possible platform migration |

**🎙️ Episode Hook:** The entire development history fits in two periods: an early 2022基础设施建设阶段 (CodeQL, README, usability), then a single dramatic day on February 12, 2024 when 7 commits—including the OSHWA certification UID—landed. Then: silence. Two years of nothing. The question isn't whether OpenAir-Cyan works; it's whether open-source hardware can sustain itself without institutional funding after the initial push.

---

## Tier 3: Reference & Survey Repositories

### 3. Carbon Capture ML Survey
- **Repo:** [zikribayraktar/Carbon_Capture_ML](https://github.com/zikribayraktar/Carbon_Capture_ML)
- **Stars:** 56 | **Language:** Python/Markdown | **Last commit:** May 8, 2024
- **Focus:** A curated survey of machine learning papers and code for carbon capture. Not a single model, but a **taxonomy of the ML-for-CCS field.**
- **Why it matters:** It maps the landscape. Which materials are being studied? Which ML methods are applied? Where are the gaps? This is the "state of the field" paper that updates itself.

**Recent Commit Highlights (15 commits pulled):**
| Date | Commit | Significence |
|------|--------|-------------|
| May 8, 2024 | OpenDAC paper added | Direct Air Capture literature expanded |
| Apr 25, 2024 | README update | Curation maintenance |
| Mar 15, 2024 | README update | Curation maintenance |
| Jan 21, 2024 | 2 README updates | adding/searching papers |
| Mar–Feb 2023 | 7 commits in 1 week | Initial rapid population: papers, processes, surrogates |
| Jan 2023 | Citation info updated, DOI fix | Quality control |

**🎙️ Episode Hook:** This repo went from zero to a full survey in one week (Feb 2023)—then spent 14 months slowly adding papers. The May 2024 OpenDAC paper addition is the most recent signal. The pattern suggests: "build the taxonomy fast, then maintain it slowly." But the 14-month gaps between updates raise a question: is this a living document or a frozen snapshot?

---

## Tier 4: The CC0 Revolution — Computational DAC Materials

### 4. DAC Tetraperoxovanadates
- **Repo:** [tjz21/DAC_peroxovanadates](https://github.com/tjz21/DAC_peroxovanadates)
- **Stars:** 2 | **Language:** DIGITAL Command Language (DFT inputs) | **License:** CC0-1.0 | **Last commit:** September 23, 2025
- **Focus:** Computational supporting information for the *Chemical Science* paper "Implementing Tetraperoxovanadates as Direct Air Capture Materials" (DOI: 10.1059/D3SC05381D). Contains cluster-model and solid-state DFT structures, Gaussian and CASTEP input files.
- **Why it matters:** This is a **practical example of the CC0 open-science movement in computational DAC.** The researchers didn't just publish the paper—they put the entire computational dataset on GitHub under a public domain dedication.

**Recent Commit Highlights (15 commits pulled):**
| Date | Commit | Significence |
|------|--------|-------------|
| Sep 23, 2025 | Updated README.md | Final touch-up after CC0 adoption |
| **Sep 12, 2025** | **Added CC0 license** | **🚨 Major signal: researchers dedicating computational screening data to public domain** |
| Mar 11, 2024 | Fixed DOI link, added paper DOI | Reference quality |
| Dec 2023 | 6 commits (README updates, image additions) | Post-publication refinement |
| Nov 30, 2023 | Model comparison image, PNG→PDF fix | Visualization work |

**🎙️ Episode Hook:** On September 12, 2025, someone added a CC0 license to a repository containing DFT calculation inputs for a direct air capture paper. That's it. That's the headline. But the implications are enormous: researchers are treating computational screening data as **public infrastructure**, not intellectual property. The entire dataset—every structure, every energy calculation, every transition state—is now available to anyone, for any purpose, forever. This is the open-science revolution happening one CC0 license at a time.

---

### 5. DAC Tetraperoxotitanates
- **Repo:** [tjz21/DAC_peroxotitanates](https://github.com/tjz21/DAC_peroxotitanates)
- **Stars:** 2 | **Language:** Not specified (CASTEP .cell/.param) | **License:** CC0-1.0 | **Last commit:** September 23, 2025
- **Focus:** Computational supporting information for the *Chemistry of Materials* paper "Tetraperoxotitanates for High Capacity Direct Air Capture of Carbon Dioxide" (DOI: 10.1021/acs.chemmater.4c01795). Solid-state unit-cell optimizations using CASTEP.
- **Why it matters:** Same CC0 pattern as peroxovanadates. Same group (Nyman lab at Oregon State, Zuehlsdorff as maintainer). Two papers, two repos, same philosophy: computational screening data belongs to the public.

**Recent Commit Highlights (10 commits pulled):**
| Date | Commit | Significence |
|------|--------|-------------|
| Sep 23, 2025 | Updated README.md | Final touch-up |
| **Sep 12, 2025** | **Added CC0 license** | **🚨 Same pattern: CC0 adoption Sep 12, 2025** |
| Jul 11, 2024 | 5 commits (README cleanup, CASTEP reference, output files) | Post-publication curation |
| May 31, 2024 | TiO5CO3 files added | Data expansion |
| May 28, 2024 | Initial README created | Repo launch |

**🎙️ Episode Hook:** The CC0 license was added to both DAC materials repos on the exact same day: September 12, 2025. This wasn't coincidence—it was a conscious decision by the same research group. When you see two repositories, both with 2 stars, both adopting CC0 on the same day, you're witnessing a **movement**, not a moment. The Nyman lab is telling the world: computational screening data is not a publication supplement—it's a public utility.

---

## Tier 5: Ghost Repos — High Stars, No Activity

### 6. yohanesnuwara/carbon-capture-and-storage
- **Stars:** 85 | **Last commit:** March 6, 2021 | **Status:** 💀 Dormant ghost
- **Focus:** Reservoir simulation + geomechanics for CCS
- **Why it matters despite dormancy:** 85 stars means it was cited/bookmarked heavily. But it's been dead for 4+ years. Stars measure citations, not usability.

### 7. CO2-Sequestration
- **Stars:** 32 | **Status:** 💀 Dormant ghost (mentioned in v3 analysis)
- **Last activity:** 2019

### 8. ChemicalEngineeringAI/Carbon-Capture
- **Last activity:** August 2026 (recently touched)
- **Focus:** Wikipedia links to CCS and DAC overviews
- **Why it matters:** It's a stub, but its August 2026 activity suggests someone still finds it useful as a starting point.

---

## 🆕 New in v4: The CC0 Adoption Wave

The September 12, 2025 CC0 licensing of both DAC peroxometal repos represents a **coordinated open-science declaration** that appears for the first time in our data. This is not an isolated event—it's part of a broader pattern in computational materials science:

| Signal | Evidence | Implication |
|--------|----------|------------|
| **Two repos, one day** | Both DAC repos got CC0 on Sep 12, 2025 | Coordinated group decision, not individual choice |
| **Star count vs. impact** | 2★ each, but cited in Chemical Science + Chemistry of Materials | Citations don't need stars on GitHub |
| **License as governance** | CC0 removes all restrictions | Future researchers can build on this without legal friction |
| **Precedent** | First CC0 adoption in our carbon-capture dataset | May inspire other computational DAC groups to follow |

**🎙️ Episode Hook:** The CC0 revolution in DAC materials is quiet but profound. While the press covers billion-dollar DAC startups, the actual scientific infrastructure is being built by a lab at Oregon State University putting DFT input files on GitHub under a public domain dedication. The future of carbon capture may depend less on venture capital and more on whether researchers are willing to share their computational data freely.

---

## Summary Table: Carbon Theme Repos

| Repo | Stars | License | Last Activity | Status | Episode Angle |
|------|-------|---------|--------------|--------|--------------|
| protontypes/open-sustainable-technology | 2,552 | — | Sep 2026 (active) | ✅ Sustained ecosystem | "The GitHub of climate tech" |
| openair-collective/openair-cyan | 76 | OSHWA | Feb 2024 (dormant) | ⚠️ One-day blitz, then frozen | "Can open-source hardware survive without funding?" |
| zikribayraktar/Carbon_Capture_ML | 56 | — | May 2024 (dormant) | ⚠️ Taxonomy, slowly maintained | "Is a living document still alive if it stops updating?" |
| tjz21/DAC_peroxovanadates | 2 | **CC0** | Sep 2025 (dormant) | 🆕 CC0 revolution | "The public domain DAC dataset" |
| tjz21/DAC_peroxotitanates | 2 | **CC0** | Sep 2025 (dormant) | 🆕 CC0 revolution | "Two repos, one day, one movement" |
| yohanesnuwara/carbon-capture-and-storage | 85 | — | Mar 2021 (ghost) | 💀 Dormant | "Stars measure citations, not usefulness" |

---

## 🎙️ Cross-Cutting Narrative Threads for Carbon Episode

1. **The Ecosystem Map** — Open Sustainable Technology with 2,552 stars is the GitHub of climate tech. It's not a model or a device; it's a directory. But directories are infrastructure—they help you find everything else. Without them, the ecosystem is fragmented.

2. **The One-Day Blitz** — OpenAir-Cyan's OSHWA certification day (Feb 12, 2024): 7 commits, a certification UID, CITATION.cff, and a full README update. Then nothing for 2 years. The story of DIY open-source hardware: fast builds, slow maintenance, fragile sustainability.

3. **The Living Document** — Carbon Capture ML went from zero to full survey in one week, then added papers over 14 months. The OpenDAC addition in May 2024 is the most recent heartbeat. Is this a living document or a frozen snapshot? The answer changes how we think about "open-source research."

4. **The CC0 Revolution** — Two repos, 2 stars each, same lab, same day (Sep 12, 2025), same license (CC0). The Nyman lab didn't just publish papers—they dedicated the entire computational dataset to the public domain. This is the open-science movement in its purest form: no copyright, no restrictions, no friction.

5. **The Ghost Stars** — 85-star carbon-capture-and-storage has been dead since 2021. 32-star CO2-Sequestration since 2019. Stars measure citations, not usability. The most-starred repos may be the least useful ones.

---

## Data Sources

All commit data pulled fresh from GitHub API on September 19, 2026:
- `protontypes/open-sustainable-technology` — 15 commits (page 1)
- `openair-collective/openair-cyan` — 15 commits (page 1)
- `zikribayraktar/Carbon_Capture_ML` — 15 commits (page 1)
- `tjz21/DAC_peroxovanadates` — 15 commits (page 1)
- `tjz21/DAC_peroxotitanates` — 10 commits (page 1)
- `yohanesnuwara/carbon-capture-and-storage` — from search metadata (dormant)

---

## Research Log

| Date | Activity |
|------|----------|
| 2026-09-19 | v4: Fresh commit histories pulled from 6 carbon-capture repos; project discoveries, CC0 analysis, and episode brief pushed to branch |
| 2026-09-17 | v3: Previous analysis completed (incorporated into README) |
| 2026-09-03 | Initial research notes created |
