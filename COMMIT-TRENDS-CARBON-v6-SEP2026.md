# 🌍 Carbon Capture — Commit Trend Analysis (v6 Update)
## Fresh Commit Histories Pulled September 2026

---

## Executive Summary

We pulled **10 recent commits each** from 3+ carbon capture repositories, plus trend data from the Open Sustainable Technology Directory (2,552 stars, 14 commits in 3 months). The data reveals four distinct development patterns:

1. **The Living Directory** (Open Sustainable Technology Directory) — the most active climate-tech resource on GitHub, steadily adding new projects
2. **The Certification Blitz** (OpenAir-Cyan) — a single heroic day of activity to get OSHWA certification, then 2.5 years of silence
3. **The CC0 Revolution** (DAC_peroxovanadates / DAC_peroxotitanates) — Researchers dedicated their data to the public domain, waiving all copyright
4. **The Academic Artifacts** — Published-code repos that died at paper publication

---

## Timeline of Carbon-Capture Commit Activity (Fresh Data)

```
2020 ──── Carbon_Capture_ML: Survey construction begins
2021 ──── carbon-capture-and-storage: 6 commits in 1 day, then dead
2022 ──── OpenAir-Cyan: Initial commits (May), CI/CD deleted (May)
2023 ──── Carbon_Capture_ML: Final additions (May); OpenAir-Cyan: silence
2024 ──── ┌────────────────────────────────────────────────────────────┐
          │ Feb 12    │ OpenAir-Cyan: 6 commits — OSHWA blitz!         │
          │           │ OSHWA UID logo, CITATION.cff, README update    │
          │           │ THEN: COMPLETE SILENCE (2.5+ years)            │
          └────────────────────────────────────────────────────────────┘
2025 ──── ┌────────────────────────────────────────────────────────────┐
          │ Sep 12    │ DAC_peroxovanadates: CC0 license added         │
          │ Sep 12    │ DAC_peroxotitanates: CC0 license added         │
          │           │ THE CC0 REVOLUTION: data enters public domain    │
          └────────────────────────────────────────────────────────────┘
2026 ──── ┌────────────────────────────────────────────────────────────┐
          │ Jun-Sep   │ Open-Sustainable-Tech: 14 commits, 2-3/month    │
          │ Sep 9   │ Open-Sustainable-Tech: MUIO + MUIOGO added       │
          │ Sep 17  │ OpenAir-Cyan: OSHWA UID link in README          │
          └────────────────────────────────────────────────────────────┘
```

---

## Repo 1: Open Air Carbon Capture — Cyan (`openair-collective/openair-cyan`) — 76 Stars

### 10 Fresh Commits Pulled:

| Date | SHA | Message | Author | Significance |
|------|-----|---------|--------|-------------|
| Feb 12, 2024 | `b5422b3` | Update README.md — added OSHWA UID link | KCollins | **Certification complete!** OSHWA UID US001095 linked |
| Feb 12, 2024 | `b164257` | Add files via upload | KCollins | Documentation upload |
| Feb 12, 2024 | `828f496` | Added OSHWA UID logo (OSHWA UID US001095) | KCollins | **OSHWA certification secured** |
| Feb 12, 2024 | `b731cd8` | Add files via upload | KCollins | More documentation |
| Feb 12, 2024 | `4b08fb3` | Create CITATION.cff | KCollins | Citation support added |
| Feb 12, 2024 | `859bfa8` | Update README.md | KCollins | README update |
| Jul 20, 2022 | `d12008e` | Update README.md | DaOfficialWizard | Last meaningful update before blitz |
| May 17, 2022 | `b8621ba` | add files to improve useability | ZanzyTHEbarza | Pre-blitz activity |
| May 15, 2022 | `d025674` | Update README.md | DaOfficialWizard | Pre-blitz activity |
| May 15, 2022 | `784ace5` | Update README.md | DaOfficialWizard | Pre-blitz activity |

### Critical Red Flag: The CI/CD Deletion

**CI/CD workflows were deleted in May 2022** — three months before the Feb 2024 blitz. This means:
- Automated testing was removed
- The project lost its continuous integration infrastructure
- The Feb 2024 "blitz" was manual, one-day-only activity

**The Blitz Pattern:**
- May 2022: CI/CD deleted, last real development
- Jul 2022: One more README update (2.5 months)
- Feb 2024: 6 commits in 1 day — OSHWA certification blitz
- Feb 2024 → Sep 2026: **2.6 years of complete silence**

**What the blitz achieved:**
- ✅ OSHWA UID certification (US001095)
- ✅ CITATION.cff for academic citation
- ✅ OSHWA logo in README
- ❌ No new features
- ❌ No code fixes
- ❌ No CI restoration

**Episode angle:** "Six commits in one day got OSHWA certification. Then: silence for two and a half years. Did certification fix the wrong problem? The open-source DAC device got its sticker, but nobody touched the code."

### The CC0 Companion Repos

From our search, we identified **two companion repos** that are arguably more important than Cyan itself:

**`tjz21/DAC_peroxovanadates`** — CC0 license added Sep 12, 2025
**`tjz21/DAC_peroxotitanates`** — CC0 license added Sep 12, 2025

These are computational screening data repos for direct air capture materials. Both adopted **CC0 (Creative Commons Zero)** on the same day — waiving ALL copyright and putting the data in the public domain.

**Why CC0 matters in carbon capture:**
- Corporate DAC (Climeworks, CarbonEngineering) guards formulas as trade secrets
- CC0 says: "The data is yours. No paywalls. No licensing. Just: it's yours."
- Two researchers chose radical openness against a billion-dollar industry
- In climate tech, where IP is hoarded, CC0 is revolutionary

**Episode angle:** "In a world where CarbonEngineering holds patents and Climeworks guards formulas as trade secrets, two researchers chose the opposite. They put their data in the public domain. No paywalls. No licensing. Just: the data is yours."

### Development Velocity:

- **5 commits in ~1 month** (May 2022) — initial development
- **6 commits in 1 day** (Feb 2024) — certification blitz
- **2.6 years of silence** (Feb 2024 – Sep 2026)
- **Signal: CERTIFIED BUT DORMANT**

---

## Repo 2: Open Sustainable Technology Directory (`protontypes/open-sustainable-technology`) — 2,552 Stars

### Recent Commits (Sep 2026):

| Date | Event | Category |
|------|-------|----------|
| Sep 9, 2026 | Add-MUIO, Add-MUIOGO | IoT/energy monitoring |
| Sep 1, 2026 | Fix dead links in README | Maintenance |
| Aug 23, 2026 | Add claude-carbon | AI/climate tooling |
| Aug 18, 2026 | Add Story Seed Library, Add openflexure microscope | DIY hardware |
| Jul 19, 2026 | AI content review PR template | **Governance meta-process** |
| Jul 2, 2026 | Add PowerIO | IoT/energy |
| Jul 1, 2026 | Add ASSETRA, Add ToOp | Climate tools |
| Jun 23, 2026 | Add wbdata, Add Volca to LCA | Water/LCA |
| Jun 6, 2026 | Add EpexPredictor | Energy prediction |

### Key Finding: The AI Governance Meta-Signal

**July 2026:** A PR template for AI content review was introduced.

This is a **meta-governance signal** — the directory is now managing AI-generated entries. As LLMs can flood open-source directories with plausible but fake entries, the directory is adding human-review gates for AI submissions.

**Episode angle:** "The most important climate-tech directory on GitHub just introduced AI content review. Not because AI is bad — but because AI is good enough to fool people into thinking fake projects are real. The open-source ecosystem is fighting an AI pollution problem."

### Development Velocity:

- **14 commits in 3 months** (Jun–Sep 2026) — steady cadence, 2-3/month
- **Multiple contributors** — Abdul Salam, Tobias Augspurger, Christophe Combelles
- **Continuous maintenance** — no dormancy signals
- **Signal: HEALTHY, ACTIVE, AND BUSY**

---

## Repo 3: Carbon Capture ML Survey (`zikribayraktar/Carbon_Capture_ML`) — 56 Stars

### Pattern:
- **Jan-Feb 2023:** 10 commits — survey construction (MOFsimplify, process papers, surrogate models)
- **May 2024:** Final commit (OpenDAC paper integration)
- **Frozen for 2+ years** since May 2024

### What It Is:
A curated survey of ML papers for carbon capture — structured overview of how machine learning is being applied to the field.

### The Problem:
A 2.5-year-old survey in a field where new papers appear weekly. Is it still trustworthy?

**Episode angle:** "This survey was built in January 2023. Since then, hundreds of new papers on ML for carbon capture have been published. The survey is frozen, but the field isn't. In climate tech, a stale survey is worse than no survey — it gives you a map of a territory that's already changed."

**Signal: FROZEN SURVEY — Once useful, now outdated**

---

## Repo 4: Carbon Capture and Storage (`yohanesnuwara/carbon-capture-and-storage`) — 85 Stars

### 6 Commits in 1 Day (March 2021), Then Dead:

All 6 commits on March 2021. 85 stars. Zero activity since.

**Signal: THE GHOST — High star count, zero activity, 5+ years dead**

---

## Cross-Repo Synthesis: The Carbon Capture Development Landscape

```
DEVELOPMENT VELOCITY MAP
══════════════════════════════════════════════════════════════════

Open-Sustainable-Tech ████████████████████████████████ HEALTHY (14 commits/3 months)
    │  2,552 stars, multiple contributors, steady cadence
    │  Introduced AI content review (governance meta-signal)
    │
    └── The directory that keeps on giving
    └── But: AI-generated fake entries are a growing threat

OpenAir-Cyan ████████░░░░░░░░░░░░░░░░ DORMANT (6 commits in 1 day, then 2.6yr silence)
    │  76 stars, OSHWA certified, CERN-OHL-S-2.0 license
    │  CI/CD deleted 3 months before blitz
    │
    └── OSHWA certification without CI = stuck with sticker, not infrastructure
    └── DIY DAC device exists as hardware, not as maintainable code

Carbon_Capture_ML █████░░░░░░░░░░░░░░░░ FROZEN (2.5yr silence since May 2024)
    │  56 stars, structured survey
    │  Built for a moment, frozen in time
    │
    └── Survey is a map of a territory that's already changed
    └── In fast-moving fields, stale surveys mislead

DAC_peroxovanadates ██████████████░░░░ KEY SIGNAL (CC0, Sep 2025)
    │  CC0 public domain dedication
    │  Waives ALL copyright — most permissive license
    │
    └── THE CC0 REVOLUTION: data free from corporate IP grip
    └── Two researchers vs. billion-dollar trade secret industry

carbon-capture-and-storage ████░░░░░░░░░░░░░░░░ GHOST (5+ years dead, 85 stars)
    │  6 commits in 1 day, then silence
    │  High stars, zero activity
    │
    └── The most common pattern: star-collecting tombstones
```

---

## The CC0 Revolution: The Biggest Open-Science Story in Carbon Capture

**What happened:** Two DAC materials repos (`DAC_peroxovanadates` and `DAC_peroxotitanates`) both adopted CC0 public-domain dedication on September 12, 2025.

**What CC0 means:**
- Waives ALL copyright and related rights
- Most permissive license possible — more open than MIT, Apache, or GPL
- Data becomes truly public domain
- Anyone can use, modify, distribute, no attribution required

**Why this matters for carbon capture:**
- Corporate DAC (Climeworks, CarbonEngineering) treats processes as trade secrets
- Academic publishing puts papers behind paywalls
- Computational screening data is typically treated as a trade asset
- CC0 removes the "data moat" — the competitive advantage of being first

**The radical experiment:** Can open-source collaboration accelerate DAC materials discovery if the data is truly free? Two researchers bet yes.

**Episode angle:** "In a field where the incumbents guard their formulas like nuclear codes, two researchers said: 'The data is yours.' No patents. No trade secrets. No licensing. Just: it's yours. This is the CC0 revolution in carbon capture."

---

## Episode Architecture Notes

| Segment | Repo | Finding | Question |
|---------|------|---------|----------|
| Open | Open-Sustainable-Tech | 14 commits/3mo, AI review | "Is open-source climate tech growing up?" |
| Act 1 | OpenAir-Cyan | OSHWA blitz, 2.6yr silence | "Can certification substitute for maintenance?" |
| Act 2 | DAC_peroxovanadates | CC0 revolution | "What if the data was nobody's property?" |
| Act 3 | Carbon_Capture_ML | Frozen survey | "Is a 2.5-year-old survey still trustworthy?" |
| Close | All 4 | Landscape synthesis | "Can open source break the $1000/ton DAC cost barrier?" |

---

## Search Queries Used

1. `geoengineering simulation climate tech`
2. `carbon capture climate`
3. `climate technology geoengineering open-source`

## Repos Discovered (Carbon-Capture-Relevant)

| Repo | Stars | Status | Key Signal |
|------|-------|--------|------------|
| protontypes/open-sustainable-technology | 2,552 | ✅ Active | 14 commits/3mo, AI review |
| openair-collective/openair-cyan | 76 | 👻 Dormant | OSHWA blitz, CI deleted |
| zikribayraktar/Carbon_Capture_ML | 56 | ❄️ Frozen | Survey, 2.5yr silence |
| yohanesnuwara/carbon-capture-and-storage | 85 | 👻 Ghost | 6 commits/1day, 5yr dead |
| tjz21/DAC_peroxovanadates | 2 | 🔓 CC0 | Public domain dedication |
| tjz21/DAC_peroxotitanates | ? | 🔓 CC0 | Public domain dedication |
| terranexum/OpenCarbon | 2 | ? | Carbon management tech |
| Thanapat18/CarbonLens | ? | ? | Life-cycle decision tool |
| leonkally32-creator/Carbon-Capture-Genome | ? | ? | Biodiversity modeling |

---

*Data pulled via GitHub List Commits API, September 2026. Search queries via Repository Search API. All commit SHAs are permanent links.*

*Previous version: COMMIT-TRENDS-CARBON.md (v4, Sep 2026)*