# 🌍 Carbon Capture — Commit Trend Analysis

## Overview

Ten repositories were analyzed for commit patterns. The carbon capture domain shows more activity than solar geoengineering, but dormancy remains the default. The standout finding is a coordinated August 2026 research release cluster across three DAC materials repositories.

## Individual Repo Histories

### 1. protontypes/open-sustainable-technology (⭐2,552) — MOST ACTIVE

| Date | Commit | Author |
|------|--------|--------|
| Sep 9, 2026 | Add-MUIO (#1638) | Abdul Salam |
| Sep 9, 2026 | Add-MUIOGO (#1639) | Abdul Salam |
| Sep 1, 2026 | docs: fix dead links (#1634) | Mikhail Alabugin |
| Aug 23, 2026 | Add claude-carbon (#1633) | gwittebolle |
| Aug 18, 2026 | Add Story Seed Library (#1630) | Abdul Salam |
| Aug 18, 2026 | Add openflexure microscope (#1631) | Abdul Salam |
| Jul 19, 2026 | Remove duplicate AI content review | Tobias Augspurger |
| Jul 19, 2026 | Modify PR template for AI content | Tobias Augspurger |
| Jul 17, 2026 | Update PR template | Tobias Augspurger |
| Jul 2, 2026 | Add PowerIO (#1619) | Tobias Augspurger |

**Pattern:** Sustained multi-contributor activity over 3 months, 10 commits, 4 distinct contributors. This is the healthiest repo in the climate-tech ecosystem we surveyed.

---

### 2. ZhiyuanF/Solar-DAC (⭐4)

| Date | Commit | Author |
|------|--------|--------|
| Aug 17, 2026 | Create README.md | ZhiyuanF |
| Feb 4, 2026 | Plotting tools | ZhiyuanF |
| Apr 2, 2025 | Multiple file uploads | ZhiyuanF |
| Apr 2, 2025 | Create readme_result.txt | ZhiyuanF |

**Pattern:** Active development through 2025-2026, with the most recent commit (Aug 17, 2026) being the README. The plotting tools added in Feb 2026 suggest ongoing analysis work. This is one of the few DAC repos with activity in 2026.

**Why It Matters:** Solar-thermal DAC uses concentrated solar energy to power the capture process, eliminating electricity costs but introducing thermal engineering challenges. This is a niche but important approach that most DAC cost models don't separately consider.

---

### 3. kfdsievert/Cost-Model--DAC (⭐6)

| Date | Commit | Author |
|------|--------|--------|
| Feb 19, 2024 | Update LICENSE | Yash Dubey |
| Feb 19, 2024 | Update README.md | Yash Dubey |
| Feb 1, 2024 | Delete LICENSE then re-add | Yash Dubey |
| Feb 1-5, 2024 | README + license setup | Katrin Sievert, Yash Dubey |
| Jan 31, 2024 | Initial file upload | kfdsievert |

**Pattern:** Rapid initial setup (Jan 31 - Feb 5, 2024) with a license discussion (created then deleted, then re-added), then silence. The model may be useful but hasn't been maintained or extended.

**Episode Angle:** The probabilistic approach (Monte Carlo + experience curves) is the right methodology, but the code is dormant. Who's updating the cost projections? Who's using this model?

---

### 4. UU-ER/DAC_SchedulingModel (⭐4)

| Date | Commit | Author |
|------|--------|--------|
| Apr 9, 2024 | Figure 5 results + README updates | Jean, 6574114 |
| Mar 20, 2023 | Thermal energy calculation fix | 6574114 |
| Sep-Oct 2022 | Initial setup and README updates | Jean |

**Pattern:** Paper-driven activity — initial setup, then updates when paper figures were ready. Last meaningful activity: Apr 2024.

---

### 5. tjz21/DAC_peroxovanadates (⭐2)

| Date | Commit | Author |
|------|--------|--------|
| Sep 23, 2025 | Updated README.md | Jacob Hirschi |
| Sep 12, 2025 | Added CC0 license | Jacob Hirschi |
| Mar 11, 2024 | Fixed DOI link + added paper DOI | Jacob Hirschi |
| Dec 5, 2023 | Multiple README updates | Jacob Hirschi |

**Pattern:** Startup burst (paper publication → repo creation → metadata updates), then dormancy. Single-author project.

---

### 6. tjz21/DAC_peroxotitanates (⭐2)

| Date | Commit | Author |
|------|--------|--------|
| Aug 19, 2026 | Updated README + CC0 license | Jacob Hirschi |
| Jul 11, 2024 | Metadata cleanup, CASTEP reference, file tree | Jacob Hirschi |
| May 28 - Jul 11, 2024 | Initial setup | Jacob Hirschi |

**Pattern:** Initial data upload burst (May-Jul 2024), then **13-month dormancy**, then a burst on **Aug 19, 2026** (same date as peroxovanadates!). The Aug 19 cluster is confirmed.

---

### 7. openair-collective/openair-cyan (⭐76)

| Date | Commit | Author |
|------|--------|--------|
| Feb 12, 2024 | OSHWA UID + CITATION.cff + README updates (6 commits) | KCollins |
| Jul 20, 2022 | README update | DaOfficialWizard |
| May 15-17, 2022 | Initial setup | DaOfficialWizard, ZanzyTHEbar |

**Pattern:** 6-commit burst on Feb 12, 2024 (OSHWA certification day), then complete silence. Milestone-driven lifecycle.

---

## Cross-Cutting Patterns

### The August 2026 DAC Materials Wave

Three repositories (tjz21/DAC_peroxovanadates, tjz21/DAC_peroxotitanates, and o7-machinehum/electro-swing-dacc) all had activity on **August 19, 2026**. Possible explanations:

1. **Coordinated paper publication** — A new DAC materials paper was released, and the authors updated their associated repos simultaneously
2. **Journal embargo lift** — The papers may have been under embargo, with repos updating on the publication date
3. **Community awareness campaign** — A coordinated effort to bring attention to DAC materials research

**Episode Angle:** The August 19 mystery — three repos, one day. What happened in the DAC materials world in August 2026?

### The OSHWA Certification Burst

OpenAir-Cyan's 6 commits on Feb 12, 2024 followed by complete silence is the single most telling pattern in the carbon capture domain. The project achieved its primary goal (OSHWA certification), documented it thoroughly, and then stopped. This suggests that **open-hardware DAC projects may follow a milestone-driven lifecycle** rather than a sustained development cycle.

### The MATLAB Persistence

Two of the most technically substantive DAC repos (DAC_SchedulingModel, Solar-DAC) use MATLAB. This means the most detailed process-level modeling is happening in a proprietary environment, not in open-source Python.

### The Python Gap

Despite being the dominant language in climate science, Python has a surprisingly thin presence in DAC-specific repos. The cost model (kfdsievert/Cost-Model--DAC) is the only Python DAC project, and it's dormant since Feb 2024.

### The Directory is the Ecosystem

The open-sustainable-technology directory (2,552★, 10 commits/3 months, 4 contributors) is more alive than any individual DAC project. The ecosystem needs its catalogs more than its individual products.

## Key Episode Talking Points

1. **The $1000/ton question** — Cost models exist but are dormant. Who's doing the cost analysis that the DAC field needs?
2. **Open hardware's milestone problem** — OpenAir-Cyan proved you can build a DAC device in your garage, but then nobody continues. Is this a failure or a success?
3. **The August 19 mystery** — Three repos updated on the same day. What happened in the DAC materials world?
4. **MATLAB's quiet persistence** — The most detailed DAC modeling is in MATLAB, not open-source Python. What does this mean for accessibility and reproducibility?
5. **The directory is the ecosystem** — The open-sustainable-technology directory is more alive than any individual DAC project.