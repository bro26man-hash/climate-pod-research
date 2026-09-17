# 🌍 Carbon Capture — Commit Trend Analysis

**Last Updated:** September 2026
**Source Repositories Analyzed:** openair-collective/openair-cyan, zikribayraktar/Carbon_Capture_ML, yohanesnuwara/carbon-capture-and-storage, openair-collective/openair-sorbent-tester

---

## Repository-by-Repository Commit Histories

### 1. openair-collective/openair-cyan — 76 Stars (The Flagship)

| Date | Commit | Author |
|------|--------|--------|
| Feb 12, 2024 | OSHWA UID link in README | KCollins |
| Feb 12, 2024 | Batch upload (6 files) | KCollins |
| Feb 12, 2024 | OSHWA UID logo added | KCollins |
| Feb 12, 2024 | Batch upload (documentation) | KCollins |
| Feb 12, 2024 | CITATION.cff created | KCollins |
| Feb 12, 2024 | README update | KCollins |
| Jul 20, 2022 | README update | DaOfficialWizard |
| May 17, 2022 | Usability improvements | ZanzyTHEbar |
| May 15, 2022 | README update | DaOfficialWizard |
| May 15, 2022 | README update | DaOfficialWizard |

**Key Insight:** 6 commits on a single day (Feb 12, 2024) — the OSHWA certification milestone. After 2 years of activity, the project went dormant. The burst pattern is typical of hardware projects: intense activity around certification/funding, then silence.

**Trending Signal:** OpenAir-Cyan proved that DIY open-source hardware can reach institutional-grade certification (OSHWA UID US001095, CERN-OHL-P license, CITATION.cff). But it couldn't sustain momentum. The project needed an institution or funder to continue.

---

### 2. zikribayraktar/Carbon_Capture_ML — 56 Stars (The ML Survey)

| Date | Commit | Author |
|------|--------|--------|
| May 8, 2024 | OpenDAC paper added | Zikri Bayraktar |
| Apr 25, 2024 | README update | Zikri Bayraktar |
| Mar 15, 2024 | README update | Zikri Bayraktar |
| Jan 21, 2024 | README update | Zikri Bayraktar |
| Jan 21, 2024 | README update | Zikri Bayraktar |
| Mar 1, 2023 | New paper | Zikri Bayraktar |
| Feb 16, 2023 | MOFsimplify paper added | Zikri Bayraktar |
| Feb 5, 2023 | Process paper added | Zikri Bayraktar |
| Feb 5, 2023 | Process paper added | Zikri Bayraktar |
| Feb 2, 2023 | New paper added | Zikri Bayraktar |

**Key Insight:** A research survey/project that peaks around paper submission cycles. 4 commits on Feb 2-5, 2023 (paper season), then periodic updates. The May 2024 OpenDAC paper addition shows the field is moving toward open DAC materials datasets.

**Trending Signal:** The ML-for-carbon-capture survey pattern — curating published research rather than producing new code — is the dominant open-source mode for this field. Repositories are literature management tools, not simulation tools.

---

### 3. yohanesnuwara/carbon-capture-and-storage — 85 Stars (The Legacy Simulation)

| Date | Commit | Author |
|------|--------|--------|
| Mar 6, 2021 | Simulation result add | yohanesnuwara |
| Mar 6, 2021 | File deletion (cleanup) | yohanesnuwara |
| Mar 6, 2021 | Case 3C simulation result | yohanesnuwara |
| Mar 6, 2021 | Folder cleanup | yohanesnuwara |
| Mar 6, 2021 | Folder organization | yohanesnuwara |
| Mar 6, 2021 | Injection sim results | yohanesnuwara |
| Mar 3, 2021 | CO2 EOS notebook | yohanesnuwara |
| Mar 1, 2021 | First file created | yohanesnuwara |
| Feb 25, 2021 | Geomechanics simulation data | yohanesnuwara |
| May 4, 2020 | Initial setup | yohanesnuwara |

**Key Insight:** All activity in a single burst (Feb-May 2021) — a BSc thesis project. 9 commits in 3 months, then complete silence despite 85 stars.

**Trending Signal:** Academic thesis projects get stars but don't get maintained. The 85 stars suggest the topic is in demand, but the single-author, single-paper model means zero long-term sustainability.

---

### 4. The August 2026 Materials Wave (Coordinated Activity)

| Repo | Date | Activity |
|------|------|----------|
| tjz21/DAC_peroxovanadates | Aug 19, 2026 | Commit update |
| tjz21/DAC_peroxotitanates | Aug 19, 2026 | Commit update |
| o7-machinehum/electro-swing-dacc | Aug 19, 2026 | Research collection update |

**Key Insight:** Three separate DAC materials repositories were all updated on the exact same day (Aug 19, 2026). This suggests a coordinated research event — possibly a paper submission, a preprocessing wave, or a community push to make DAC materials computation reproducible.

**Trending Signal:** The computational chemistry of DAC sorbents is becoming codified. Peroxovanadates and peroxotitanates are being implemented as open computational implementations (SCI protocols). This is the Reproducible Research movement meeting materials science.

---

## Five Key Findings

1. **Hardware projects burst then die.** OpenAir-Cyan had 6 commits in 1 day (certification), then silence. The mechanism is clear: a PhD student or researcher drives the project, publishes, moves on, and nobody maintains the repo.

2. **Literature surveys are the dominant open-source mode.** Carbon_Capture_ML (56 stars) curates papers; it doesn't simulate anything. This suggests the field is still in the knowledge-integration phase, not the tool-building phase.

3. **Academic thesis projects are ghosts.** carbon-capture-and-storage (85 stars) has zero activity since May 2021. Stars does not equal maintenance. The academic incentive structure doesn't reward long-term code stewardship.

4. **The August 2026 wave is the most significant signal.** Three DAC materials repos updating on the same day is unusual and suggests a coordinated community effort around computational sorbent discovery.

5. **System integration is the missing layer.** Nobody is building the "deploy DAC at scale" code. Materials science is active; system engineering is absent.

---

## What This Means for Your Podcast

- The **OpenAir-Cyan story is your hero narrative**: a DIY open-source DAC device that got OSHWA certified — proving it can happen — but then went dormant because there was no institutional home.
- The **August 2026 materials wave** gives you a "what's new" hook: computational sorbent discovery is becoming reproducible and open. This is where the field is moving.
- The **maintenance gap** is the structural story: across all carbon capture repos, nobody is building long-term community infrastructure. This mirrors the broader climate-tech open-source problem.

---

## Updated Episode Questions

1. Can open source break the $1000/ton DAC cost barrier? The materials science is accelerating (Aug 2026 wave), but the engineering integration is absent.
2. What kills open-source hardware projects? OpenAir-Cyan's story — certification to dormancy — is a case study in what happens when the researcher moves on.
3. Are peroxides the sorbent of the future? The coordinated August 2026 commits on vanadates and titanates suggest a research community forming.
4. Will electro-swing DAC change the economics? The voltage-switchable sorbent approach could break the energy bottleneck — but the GitHub presence is still just a literature review.
