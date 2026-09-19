# ☀️ Solar Geoengineering — Supplemental Repo Profiles (v5 Update)
## Additional Repositories & Commit Trend Deep-Dive
*September 2026 — complements PROJECT-DISCOVERIES-SOLAR.md and COMMIT-TRENDS-SOLAR.md*

---

## New Repos Discovered in This Research Pass

These repositories were identified in a secondary search round and provide important context for the solar geoengineering episode. They were **not** in the original v4 research notes.

---

### 1. WRF Regional Aerosol Injection (`Sustainable-Solutions-Lab/regional-geo`)
- **Stars:** 0 | **Language:** Python | **License:** None
- **Last activity:** February 15, 2026 (16 commits, all in one batch)
- **Authors:** Ken Caldeira (all commits)
- **What it is:** Analysis of WRF-Chem regional climate model simulations exploring the effects of **stratospheric sulfate aerosol injection** on regional climate.

#### Experimental Design
| Dimension | Values | Description |
|-----------|--------|-------------|
| Episode | `240527`, `240727` | May 2024 (dry season) and July 2024 (wet season) |
| Ensemble | `e1`, `e2`, `e3` | Three ensemble members per episode |
| Emission Rate | `ctl`, `1000`, `10000`, `100000` | SO₂ injection rate in t/h (0, 1 kt/h, 10 kt/h, 100 kt/h) |
| Injection Region | `5x5` | 5×5 grid cell injection in domain d02 |

**Total expected cases:** 2 × 3 × 4 = **24 cases**

#### Commit History (16 commits, all Feb 13-15, 2026)
**Burst pattern → dormant since.** All 16 commits in 3 days:

| Date | Commit | Phase |
|------|--------|-------|
| Feb 15 | `gaussian smoothing` | Analysis polish |
| Feb 14 | `improved maps and analysis` | Analysis iteration |
| Feb 14 | `show individual cases` | Analysis iteration |
| Feb 14 | `fixing figures` | Analysis iteration |
| Feb 13 | `start analysis` | **Analysis begins** |
| Feb 13 | `read rds files` | Data pipeline |
| Feb 13 | `area calculation` | Data pipeline |
| Feb 13 | `Add data loader documentation` | Documentation |
| Feb 13 | `Remove defensive checks from data loader` | Code cleanup |
| Feb 13 | `Add data loader utility` | **Initial code** |
| Feb 13 | `updated README.md` | Documentation |
| Feb 13 | `Add file dimension patterns to README` | Documentation |
| Feb 13 | `Merge data documentation into main README` | Docs consolidation |
| Feb 13 | `Add comprehensive README for WRF input data` | Documentation |
| Feb 13 | `Add CLAUDE.md style guide` | Project setup |
| Feb 13 | `Initial project setup` | **Project bootstrap** |

**Episode angle:** This is a textbook **"burst and disappear"** pattern. 16 commits in 3 days, then silence for 7+ months. Ken Caldeira (co-author of the original geoengineering field's foundational papers) built the tooling, analyzed the data, and moved on. The data lives on UCAR Derecho HPC — not on GitHub. **The code is the product; the data is in a spreadsheet on a supercomputer.** This raises a key podcast question: *If the most important geoengineering research data isn't on GitHub, what IS the reproducibility crisis looking like for solar geoengineering?*

#### Key Variables in the WRF Simulations
| Variable | Description | Units |
|----------|-------------|-------|
| `T2` | 2-meter air temperature | K |
| `so4_a01`–`so4_a04` | Sulfate aerosol mass mixing ratio (4 modes) | kg/kg |
| `SWDNT`, `SWUPT` | Downward/upward shortwave at TOA | W/m² |
| `OLR` | Outgoing longwave radiation | W/m² |
| `ALBEDO` | Surface albedo | — |
| `EXTCOF55` | Aerosol extinction coefficient | m⁻¹ |
| `PM2_5_DRY` | Dry PM2.5 concentration | μg/m³ |

**Critical insight for the episode:** The ratio analysis module (`src/ratio_analysis.py`) computes **gridded contribution fields** showing which grid cells contribute most to domain-wide temperature changes. This is the science of "where does the cooling actually happen?" — a question that gets to the heart of geoengineering equity (who gets cooled, who doesn't).

---

### 2. ClimateMARGO (`ClimateMARGO/ClimateMARGO.jl`)
- **Stars:** 73 ⭐ | **Language:** Julia | **License:** BSD-3-Clause
- **Last activity:** August 17, 2026 (2 README commits)
- **Authors:** Fons van der Plas (primary), Henri Drake (earlier)
- **What it is:** Julia implementation of **MARGO** — an idealized climate-economic modeling framework for optimizing trade-offs between emissions mitigation, adaptation, and geoengineering.

#### Full Commit Timeline (10 commits pulled)
| Date | Commit | Significance |
|------|--------|-------------|
| Aug 17, 2026 | `Update README.md` | **Recent revival signal** — 3.5 years of silence broken |
| Aug 17, 2026 | `Update README.md` | Second README commit same day |
| Oct 18, 2023 | `Update unit_conversions.jl` | Minor fix (comment from PR #86) |
| Jul 6, 2023 | `add link to pluto in readme` | Minor doc link |
| Nov 14, 2022 | `Update Project.toml` | Dependency update |
| Nov 12, 2022 | `JuMP and Ipopt compat upgrade (#85)` | **Active development** — solver compatibility |
| Feb 10, 2022 | `Removed deprecated web apps` | Cleanup |
| Feb 4, 2022 | `Added CITATION.bib` | Academic attribution |
| Jan 13, 2022 | `Fixed typo` | Maintenance |
| Jan 12, 2022 | `Updated arguments for doc version deployment` | Initial dev |

**Pattern:** 2022 was the active development year (9 commits). Then a 1.5-year silence. Then sporadic commits. The **August 2026 README update is the first activity in 3.5 years** — possible revival.

**Episode angle:** *"The 73-star question"* — Why does a climate-economic model with 73 stars have only 10 commits in 4 years? Because academic tools live or die by publication cycles, not user needs. ClimateMARGO was built for a paper. The paper was cited. The repo is stable. Nobody maintains it. The Julia ecosystem moves on. The JuMP compat upgrade (Nov 2022) was likely needed because the underlying solver broke. The 2026 README touch might be someone re-linking for a new paper. **This is the lifecycle of most scientific code: build, publish, cite, forget.**

---

### 3. Geo-DICE (`PSLmodels/Geo-DICE`)
- **Stars:** 2 | **Language:** MATLAB | **License:** None
- **Last activity:** September 27, 2018 — **6 years dormant**
- **Authors:** Soheil Shayegh ( uploads), Matt Jensen (initial commit)
- **What it is:** Modified DICE (Dynamic Integrated Climate-Economy) model with geoengineering — the canonical integrated assessment model (IAM) extended with SRM.

#### Commit History (only 4 commits ever)
| Date | Commit | Significance |
|------|--------|-------------|
| Sep 27, 2018 | `Add files via upload` | Final upload |
| Aug 15, 2016 | `Add files via upload` | Second upload |
| Aug 15, 2016 | `Add files via upload` | Initial upload |
| Aug 15, 2016 | `Initial commit` | Bootstrap |

**Pattern:** **Upload-and-abandon.** 4 commits over 2 years from a climate economics lab. No tests, no CI, no README, no license. The code exists as a research artifact.

**Episode angle:** *"Geo-DICE is the fossil record of geoengineering economics."* 4 commits, 6 years dead, 2 stars. But this is one of the **most intellectually important repos** in this list — it's the DICE model with SRM. DICE won Nordhaus the Nobel Prize. Adding geoengineering to DICE means you're asking: "What's the optimal climate policy **if** we can dim the sun?" The answer shaped the Paris Agreement's 1.5°C target debate. **The most influential code can be the most neglected on GitHub.**

---

### 4. Awesome Geoengineering (`brandonhimpfen/awesome-geoengineering`)
- **Stars:** 4 | **Language:** Python | **License:** None
- **Last activity:** September 6, 2026 (most recent commit!)
- **Author:** Brandon Himpfen
- **What it is:** A curated list of geoengineering projects, research, organizations, tools, and resources — the "Awesome-list" format.

#### Commit History (7 commits)
| Date | Commit | Significance |
|------|--------|-------------|
| Sep 6, 2026 | `Update README.md` | **Active!** Most recent solar-repo commit |
| Sep 5, 2026 | `Update README.md` | Same-day pair |
| May 5, 2026 | `Update to v2.0.0` | **Version bump** — structured format |
| Mar 12, 2026 | `Update README.md` | Ongoing maintenance |
| Jan 16, 2026 | `Update README.md` | Ongoing maintenance |
| Jun 28, 2025 | `Update README.md` | First content |
| Jun 28, 2025 | `Initial commit` | Bootstrap |

**Pattern:** **The only consistently maintained solar geoengineering repo in our sample.** 7 commits over 14 months, with a version bump to v2.0.0 in May 2026. This is a one-person project with steady, deliberate updates.

**Episode angle:** *"If the most active solar geoengineering repo on GitHub is just a links list, what does that tell us?"* The `awesome-geoengineering` list is more up-to-date than most simulation tools. In a field where the core simulation code (DICE, WRF) is maintained by institutions with competing priorities, a community-curated index may be the most valuable public good. **The meta-tool outlives the tool.**

---

### 5. OOCC 2021 (`jlehtomaa/OOCC_2021`)
- **Stars:** 2 | **Language:** Python | **License:** None
- **Last activity:** November 15, 2021 — **4.5 years dormant**
- **Author:** jlehtomaa
- **What it is:** A simple model for **solar geoengineering governance** — the regulatory/international governance angle on SRM.

#### Commit History (10 commits pulled, all from 2021)
| Date | Commit | Significance |
|------|--------|-------------|
| Nov 15, 2021 | `update bibtex entry` | Citation update |
| Oct 26, 2021 | `update bibtex reference` | Citation update |
| Sep 5, 2021 | `update readme` | Conference prep |
| Sep 5, 2021 | `update readme` | Conference prep |
| Sep 5, 2021 | `update readme` | Conference prep (3x same day) |
| Sep 4, 2021 | `update citation` | Citation update |
| Sep 4, 2021 | `added citation file` | Citation setup |
| Sep 3, 2021 | `update readme` | Conference prep |
| Sep 3, 2021 | `update readme` | Conference prep |
| Sep 3, 2021 | `update readme` | Conference prep (3x same day) |

**Pattern:** **Conference-driven burst.** 7 commits in 3 days (Sep 3-5, 2021), all README updates for a conference presentation. 2 citations updates later. Then dead.

**Episode angle:** *"The governance repo that nobody forked."* This is a model for how solar geoengineering should be governed internationally. 2 stars. The conference paper was probably presented to a small room. Meanwhile, real-world SRM deployment decisions are being made without models like this. **Governance code is the least GitHub-friendly kind of code — it's never urgent, always controversial, and never has a PR.**

---

### 6. GCCS-Core (`KOSASIH/GCCS-Core`)
- **Stars:** 9 | **Language:** Python | **License:** None
- **Last activity:** October 29, 2024 — **1.5 years dormant**
- **Author:** KOSASIH
- **What it is:** The core framework for the **Global Climate Control System** — a conceptual/educational project imagining a centralized climate control system.

#### Commit History (10+ commits, all on Oct 29, 2024)
| Date | Commit |
|------|--------|
| Oct 29, 2024 | `Update README.md` (×7!) |
| Oct 29, 2024 | `Create requirements.txt` |
| Oct 29, 2024 | `Create setup.py` |
| Oct 29, 2024 | `Create data_collection.sh` |

**Pattern:** **Single-day blitz.** 8+ commits all on the same day, then silence. The 7 README updates in one day suggest significant restructuring or formatting.

**Episode angle:** *"GCCS is the Pandora's class project."* The name alone — Global Climate Control System — is the黙示录 of geoengineering: "Let's build a central system to control the climate." It's an educational framework, but the framing is telling. Who build climate control? Who controls the controllers? **Even conceptual projects embed assumptions about power, governance, and who decides what 'optimal climate' means.**

---

## Cross-Repo Solar Commit Summary Table

| Repo | Stars | Total Commits | Active Period | Pattern | Last commit |
|------|-------|---------------|---------------|---------|-------------|
| WRF (regional-geo) | 0 | 16 | Feb 13-15, 2026 | Burst → dormant | Feb 15, 2026 |
| ClimateMARGO.jl | 73 | 10 | 2022-2026 | Fragmented, possible revival | Aug 17, 2026 |
| Geo-DICE | 2 | 4 | 2016-2018 | Upload-and-abandon | Sep 2018 |
| awesome-geoengineering | 4 | 7 | 2025-2026 | Steady one-person maintenance | Sep 6, 2026 |
| OOCC_2021 | 2 | 10 | Sep-Nov 2021 | Conference burst → dormant | Nov 2021 |
| GCCS-Core | 9 | 8+ | Oct 2024 | Single-day blitz | Oct 2024 |

---

## The Five Development Patterns (Solar Geoengineering)

1. **🔥 The Burst** (regional-geo, GCCS-Core): Heavy activity in 1-3 days, then silence. Data/code created for a specific analysis or class project, then abandoned.

2. **📚 The Academic Lifecycle** (ClimateMARGO, OOCC_2021): Built for a paper/conference, cited, maintained only when a new publication requires it. Payment is citation count, not user count.

3. **🏛️ The Institutional** (WRF, PCMDI — covered in v4): Professional teams, continuous releases, critical bug fixes that affect thousands of downstream users.

4. **💤 The Fossil** (Geo-DICE): Historically important, academically influential, but completely abandoned. The code is a museum piece.

5. **🔗 The Curator** (awesome-geoengineering): One person keeping an index alive. The most sustainable model in the solar geoengineering GitHub ecosystem, because it requires the least maintenance per unit of value.

---

## Episode Architecture Suggestion

| Segment | Repo | hook |
|---------|------|------|
| **Cold open** | regional-geo | "16 commits in 3 days. Then silence. The data lives on a supercomputer in Switzerland." |
| **Act 1** | ClimateMARGO | "73 stars and 3.5 years of silence. Why does scientific code live or die by publication cycles?" |
| **Act 2** | Geo-DICE | "The DICE model won a Nobel Prize. The geoengineering version has 2 stars and no license." |
| **Act 3** | awesome-geoengineering | "The most active solar geoengineering repo on GitHub is just a links list. What does that mean?" |
| ** policies** | OOCC_2021 + GCCS-Core | "Who governs the sun? A governance model with 2 stars and a conceptual climate control system with 9 stars." |

---

*Research methodology: GitHub REST API, September 2026. Commits pulled via List Commits API. Search queries via Repository Search API.*