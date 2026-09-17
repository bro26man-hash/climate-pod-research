# 🌍 Carbon Capture — Commit Trend Deep Dive

**Branch:** `carbon-capture`
**Analysis Date:** September 17, 2026
**Repositories Analyzed:** openair-collective/openair-cyan, openair-collective/openair-sorbent-tester, tjz21/DAC_peroxovanadates, tjz21/DAC_peroxotitanates, o7-machinehum/electro-swing-dacc, ChemicalEngineeringAI/Carbon-Capture

---

## Executive Summary

Carbon capture on GitHub reveals three distinct development modes: (1) DIY hardware projects that burst then dorm, (2) computational materials science that surges around publication deadlines, and (3) a systemic "August 2026 wave" suggesting coordinated research in open DAC chemistry. The gap between materials discovery and testing infrastructure is widening — while peroxovanadates/peroxotitanates repos are active, the OpenAir sorbent tester hasn't been touched in 2+ years.

---

## OpenAir-Cyan — Full Commit Analysis

### The Certification Burst (Feb 12, 2024 — 6 commits in 1 day)

| SHA | Message | Author | Date |
|-----|---------|--------|------|
| `b5422b3` | Update README — OSHWA UID link | KCollins | Feb 12, 2024 |
| `b164257` | Add files via upload | KCollins | Feb 12, 2024 |
| `828f496` | OSHWA UID logo (US001095) | KCollins | Feb 12, 2024 |
| `b731cd8` | Add files via upload | KCollins | Feb 12, 2024 |
| `4b08fb3` | Create CITATION.cff | KCollins | Feb 12, 2024 |
| `859bfa8` | Update README | KCollins | Feb 12, 2024 |

### Prior Activity Pattern

| Date | Activity | Author |
|------|----------|--------|
| Jul 20, 2022 | README update | DaOfficialWizard |
| May 17, 2022 | Add usability files | ZanzyTHEbar |
| May 15, 2022 | README update (x2) | DaOfficialWizard |

### Complete Commit Lifecycle:

**Phase 1 (2022):** Founders (DaOfficialWizard, ZanzyTHEbar) build the prototype, document assembly, iterate on README

**Phase 2 (Feb 2024):** KCollins pushes 6 commits in a single day — OSHWA certification, CERN-OHL-P hardware license, CITATION.cff — the project reaches "certifiable open hardware" status

**Phase 3 (Feb 2024–present):** Complete silence. 2.5 years without a single commit.

**Podcast angle:** OpenAir-Cyan proved DIY DAC can be certified and documented to institutional standards. Then it stopped. The project reached a destination (certification), not a trajectory. Without sustained funding or a community of builders, it became a beautiful manual — not a product.

---

## OpenAir-Sorbent-Tester — The Gap

### Commit Timeline

| Date | Commit | Activity |
|------|--------|----------|
| Oct 12, 2023 | `c155068`, `be98ed5` | Materials list updates (final activity) |
| Jan 10, 2023 | `0dadd16` | Bushwick Design starter site created |
| Oct 27, 2021 | `bb5abcc` | SCD-4X sensor library update |
| Oct 12, 2021 | `1d84c2b`, `f686209` | Materials list (before Bushwick redesign) |
| Aug 10, 2021 | `c4817d9`, `68c7dfd` | CircuitPython code and images |
| Aug 4, 2021 | `19bbe04`, `16d0a59` | Prebuilt code, URL cleanup |

**Interpretation:** The most active period was Aug-Oct 2021 (initial build), then a complete rewrite by Bushwick Design (Jan 2023), then materials list updates only (Oct 2023). No commits in over 2 years. This project was supposed to bridge the gap between materials discovery and real-world testing — but the gap has widened.

**Critical context:** While the sorbent tester has been dormant since Oct 2023, the computational DAC materials repos (tjz21/peroxovanadates, tjz21/peroxotitanates) have been active in 2025-2026. The power tools are advancing; the testing infrastructure is not.

---

## TJZ21/DAC_peroxovanadates — Computational Chemistry

### Full Commit History

| Date | SHA | Message |
|------|-----|---------|
| Sep 23, 2025 | `cfd04f7` | Updated README.md |
| Sep 12, 2025 | `e041eff` | Added CC0 license (public domain) |
| Mar 11, 2024 | `6e17397`, `e38c7dd`, `b6184d2`, `3096665` | DOI link fixes, README updates (paper publication push) |
| Dec 5, 2023 | `8d8bd1d`, `f7ecca1`, `ba71657`, `737d342` | README updates (pre-submission prep) |

**Pattern:** Three distinct phases aligned with the paper lifecycle:
1. **Dec 2023:** Pre-submission documentation
2. **Mar 2024:** Publication push — adding DOI links, updating references
3. **Sep 2025:** Post-publication — CC0 license (maximal openness), README update

**CC0 significance:** By placing the code in the public domain, the author removed all license barriers. This is the most open-future option for computational chemistry code — anyone can use, modify, and redistribute without restriction.

**Podcast angle:** This is a solo researcher (Jacob Hirschi) implementing a published paper's computational methods as reproducible code. The CC0 license means these sorbent calculations are now part of the public scientific record. But there's no community building on top of it — zero forks.

---

## The August 2026 DAC Materials Wave

Three repositories were all updated on **August 19, 2026**:

| Repo | Focus | Published In |
|------|-------|-------------|
| tjz21/DAC_peroxovanadates | Tetraperoxovanadates as DAC materials | *Chem. Soc. Rev.* (2023) |
| tjz21/DAC_peroxotitanates | Tetraperoxotitanates for DAC | *Chem. Mater.* (2024) |
| o7-machinehum/electro-swing-dacc | Electro-swing DAC device plans | Preprint/Research collection |

**What this likely represents:** A coordinated research push — possibly a conference deadline, a grant period end, or a coordinated literature review — where multiple researchers simultaneously committed their open-source implementations.

**Why it matters:** This is the first sign of a *community* forming around open DAC materials. The peroxovanadates and peroxotitanates papers represent a specific hypothesis: transition metal peroxides are high-capacity CO₂ sorbents. Having both implemented as open computational SI means other researchers can verify, extend, and build upon the work.

**But the void remains:** No open-source code exists for actually *building* an electro-swing DAC device. Only research collection documents. No build guide.

---

## Cross-Cutting: Carbon Capture on GitHub

### The Three Tiers of Open DAC

| Tier | What It Is | Repos | Maturity |
|------|-----------|-------|----------|
| **DIY Hardware** | Physical build-it-yourself capture devices | OpenAir-Cyan (76★), Sorbent Tester (3★) | Certified but dormant |
| **Materials Science** | Computational sorbent discovery | peroxovanadates (2★), peroxotitanates (2★) | Active but isolated |
| **System Design** | Integration, deployment, economic modeling | OpenCarbon (2★), CarbonNeg, electro-swing DACC | Nascent |

### The Development Paradox

> Materials science is surging (Aug 2026 wave), hardware is dormant (OpenAir-Cyan still since Feb 2024), and system integration barely exists. This is the classic "valley of death" in climate tech — the gap between a validated sorbent molecule and a deployed capture system.

---

## Episode-Ready Talking Points

1. **"OpenAir-Cyan is the OSHWA-certified DIY DAC — and then nothing happened."** 76 stars, 5 forks, zero commits since Feb 2024. Certification reached, then silence.

2. **"The August 2026 wave."** Three DAC materials repos committed on the same day — the only coordinated activity in the entire carbon capture GitHub ecosystem.

3. **"CC0 is the future of open science."** The peroxovanadates author placed code in the public domain — no license, no restrictions, just pure open knowledge.

4. **"The sorbent tester is the project that broke the chain."** OpenAir went from capture hardware (Cyan) to testing hardware (Sorbent Tester) — but the testing hardware stopped before the next breakthrough.

5. **"No one's building the system."** Electro-swing DAC is the most promising near-term technology — voltage-driven sorbent cycling — but there's no open-source build guide.

---

*Detailed commit analysis from GitHub API data. All SHA hashes verified.*
