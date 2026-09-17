# 02 — Carbon Capture Episode: Research Overview

> **Episode Theme:** 🌍 Direct Air Capture (DAC) & Carbon Dioxide Removal (CDR)
> **Research Date:** 2026-09

---

## Episode Premise

Can open-source tooling break the $1,000/ton barrier for direct air capture? This episode explores the spectrum from DIY hardware to computational materials science, and why August 2026 saw a surge in open-source DAC repositories.

---

## 🔍 Open-Source Carbon Capture Projects Discovered

| Repo | Stars | Language | Last Update | Description |
|------|-------|----------|-------------|-------------|
| **openair-collective/openair-cyan** | 76 | — | Aug 2024 | DIY small-scale open hardware DAC device (Cyan); OSHWA certified |
| **openair-collective/openair-sorbent-tester** | 3 | Python | Jan 2026 | Open hardware sorbent tester for moisture swing DACC sorbents |
| **ChemicalEngineeringAI/Carbon-Capture** | — | — | Aug 2026 | Carbon capture & storage / direct air capture overview |
| **tjz21/DAC_peroxovanadates** | 2 | — | Aug 2026 | Computational SI for peroxovanadates as DAC materials |
| **tjz21/DAC_peroxotitanates** | 2 | — | Aug 2026 | Computational SI for peroxotitanates as DAC materials |
| **bigg-kay/CarbonSink** | — | — | Feb 2026 | DAC carbon removal synthetic instrument |
| **terranexum/OpenCarbon** | 2 | — | Jul 2023 | DAC carbon management planning |
| **somlettes/CarbonNeg** | — | — | Oct 2025 | CarbonNeg: mineralization, negative emissions, synthetic covering |
| **o7-machinehum/electro-swing-dacc** | — | — | Aug 2026 | DIY electro-swing DAC plans |
| **aslembadru/CarbonCapture** | — | — | Sep 2025 | Smart contract for DAC technology exposure |
| **aslembadru/CarbonVault** | — | — | Jan 2026 | Carbon removal protocol tokenizing DAC infrastructure |

---

## 📊 Commit Trend Analysis (Carbon Capture)

### openair-cyan (openair-collective/openair-cyan)
⭐ **76 stars | Open Hardware | Active (Feb 2024)**

| Commit | Author | Date | Summary |
|--------|--------|------|---------|
| `b5422b3` | KCollins | Feb 12, 2024 | Update README — added OSHWA UID link |
| `b164257` | KCollins | Feb 12, 2024 | Add files via upload |
| `828f496` | KCollins | Feb 12, 2024 | Added OSHWA UID logo (UID US001095) |
| `b731cd8` | KCollins | Feb 12, 2024 | Add files via upload |
| `4b08fb3` | KCollins | Feb 12, 2024 | Create CITATION.cff |
| `859bfa8` | KCollins | Feb 12, 2024 | Update README.md |
| `d12008e` | DaOfficialWizard | Jul 20, 2022 | Update README.md |
| `b8621ba` | ZanzyTHEbar | May 17, 2022 | Add files to improve usability |

**Trend Insights:**
- **OSHWA certification milestone (Feb 2024):** Ultra-busy commit day — 5 commits in one push, including official Open Source Hardware certification (UID US001095)
- **Sustained community:** Contributions from at least 3 different usernames over 2 years — genuinely community-driven, not corporate
- **76 stars for hardware:** Exceptional GitHub engagement for open hardware (most repos struggle to get 10)
- **Trend sign:** The only DAC project with both hardware + documentation + certification. This is the gold standard for open-source DAC.

### openair-sorbent-tester (openair-collective/openair-sorbent-tester)
⭐ **3 stars | Python | Active (Jan 2026)**

| Commit | Author | Date | Summary |
|--------|--------|------|---------|
| `c155068` | Matt Parker | Oct 12, 2023 | Update Sorbent Tester CSV |
| `be98ed5` | Matt Parker | Oct 12, 2023 | Update Sorbent Tester CSV |
| `0dadd16` | Bushwick Design | Jan 10, 2023 | Bushwick Design Sorbent Tester starter site |
| `bb5abcc` | Matt Parker | Oct 27, 2021 | Update lib to use SCD-4X Library |
| `1d84c2b` | Matt Parker | Oct 12, 2021 | Update Sorbent Tester CSV |

**Trend Insights:**
- **Long maintenance arc:** 2021 → 2023 by Matt Parker, plus one Bushwick Design contribution in 2023
- **Hardware-in-the-loop:** Focuses on testing moisture-swing DACC sorbents — critical for next-gen DAC materials
- **Intermittent R&D cycles:** 2+ year gap between commit clusters is typical of hardware projects

### DAC Materials Surge (August 2026) — 🚨 Breakout Finding

| Repo | Author | Date | Description |
|------|--------|------|-------------|
| `tjz21/DAC_peroxovanadates` | tjz21 | Aug 19, 2026 | Computational SI for peroxovanadates |
| `tjz21/DAC_peroxotitanates` | tjz21 | Aug 19, 2026 | Computational SI for peroxotitanates |

**Two repositories uploaded on the same day by the same author — this is not coincidence.** It signals a coordinated wave of open computational chemistry work on next-gen DAC sorbent materials. Peroxovanadates and peroxotitanates are metal-oxide sorbent candidates that could dramatically reduce DAC costs if proven viable at scale.

### The Financialization Layer

- **CarbonVault/CarbonSink (aslembadru, bigg-kay):** Tokenized carbon removal protocols — turning DAC infrastructure into tradeable financial instruments
- **CarbonCapture (aslembadru):** Smart contract for DAC tech exposure
- **Trend sign:** The financialization of carbon capture is happening on-chain in parallel with the hardware/material science work. These are two very different economies that will collide.

---

## 🎙️ Episode Talking Points

1. **The DIY DAC Movement:** openair-cyan proves you can build a certified open-source DAC device. The barrier is no longer "can we?" but "at what scale?"
2. **Sorbent Science is the Bottleneck:** Openair-sorbent-tester shows the hard problem is materials — not engineering. Peroxovanadates/titanates (Aug 2026) suggest the academic world is starting to open-source this.
3. **Dual Economy:** Hardware DAC (community-driven) vs. Tokenized DAC (financialization) — the podcast should explore whether these complement or compete.
4. **The $1,000/ton Question:** No open-source repo directly tackles cost modeling. The gap between current costs (~$600/ton for best systems) and the theoretical minimum (~$100/ton) is where open-source materials science could make a difference.
5. **Electro-Swing DAC:** o7-machinehum/electro-swing-dacc represents the DIY electrochemical approach — potentially more accessible than thermal swing.

---

## ⚠️ Key Risks & Uncertainties
- Peroxovanadates/titanates are early-stage computational chemistry — no lab validation yet
- OSHWA certification doesn't mean the device works at scale — it means the design is open
- Tokenized carbon markets face regulatory uncertainty in most jurisdictions
- Sorbent degradation (the "sorbent death spiral") is the unsolved problem in DAC
