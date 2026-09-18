# 🎙️ Cross-Theme Commit Trend Summary v7 (September 2026)

> **Branch:** `main`  
> **Podcast series:** Climate Technology & Geoengineering  
> **Data pulled:** September 2026 via GitHub API  
> **Total repos analyzed:** 11 (WRF, PCMDI, MDTF-diagnostics, ClimateMARGO, awesome-geoengineering, GCCS-Core, ShennongWM-G, lithos-carbon, open-sustainable-technology, openair-cyan, DAC_peroxovanadates)

---

## The Three Universes (v7)

| Universe | Theme | Repos | Total Commits | Developer Count | Development Character |
|----------|-------|-------|----------------|-----------------|----------------------|
| **🌐 Fast Universe** | Solar + Carbon infrastructure | WRF, PCMDI, Open-Sustainable-Tech, lithos-carbon | 40+ | 6+ | Institutional, funded, sustained, versioned releases |
| **🌱 Slow Universe** | Individual researchers | ClimateMARGO, awesome-geoengineering, MDTF, Carbon_Capture_ML, OpenAir-Cyan, ShennongWM-G, GCCS-Core | 70+ | 6 | Dormant cycles, README-only revivals, bulk uploads |
| **⛰️ Empty Universe** | Ocean intervention | **ZERO** | **0** | **0** | **Complete absence — the largest governance signal** |

---

## Master Commit Timeline (All 11 Repos, v6+v7 Data)

### September 2026 — The Active Month

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                                                                             │
│  Sep 17  ████ PCMDI: modpath single-file patch (90a4bc1)                   │
│           └─ Edge-case fix; real-world usage pressure                        │
│                                                                             │
│  Sep 16  ████ lithos-carbon: final rescore artifacts (d672544)             │
│           └─ 10th commit in 18 days; MCP correction cycle continues          │
│                                                                             │
│  Sep 06  ████ awesome-geoengineering: README update (8d0a800)               │
│           └─ Latest in accelerating cadence (202d → 55d → 54d → 1d gaps)    │
│                                                                             │
│  Sep 05  ████ awesome-geoengineering: README update (5926daf)               │
│           └─ Double-header day; v2.0.0 momentum continues                     │
│                                                                             │
│  Sep 04  ████████ PCMDI: 7 commits in ONE DAY (v4.2.1 release)             │
│           └─ Prepare → Bug fix → Merge → CITATION → Merge → Bump → Merge     │
│           └─ Roundoff bug (1.00 display) fixed during release prep           │
│                                                                             │
│  Sep 03  ████ PCMDI: extremes chunking merge (71a0497)                      │
│           └─ Performance optimization for large dataset processing           │
│                                                                             │
│  Sep 01  ████ lithos-carbon: rescore artifacts (63d08bb)                    │
│           └─ Third consecutive week of MCP corrections                        │
│                                                                             │
│  Aug 30  ████ lithos-carbon: 3 commits (slug corrections + attribution)     │
│           └─ "Record who wrote each artifact" — provenance layer added        │
│                                                                             │
│  Aug 29  ████ lithos-carbon: "Publish delivery model" (39aaecd)             │
│           └─ "What was measured, not a new score" — methodology transparency  │
│                                                                             │
│  Aug 17  ██ ClimateMARGO: TWO README updates (6d9ba7a + d916f36)            │
│           └─ 2yr 10mo dormancy broken; zero code commits; unclear intent      │
│                                                                             │
│  Aug 14  ████ MDTF: PR #825 merge (87f8105)                                │
│           └─ Sole author merges own PR; single-contributor ecosystem          │
│                                                                             │
│  Jun 19  █████ MDTF: Precip-buoyancy POD big bang (5 commits, 1 file)       │
│           └─ 1 code commit + 4 documentation commits; all same day           │
│                                                                             │
│  Jun 08  ████ WRF: v4.8.0 release merge (06d4240); MDTF: README updates     │
│           └─ Major version shipped; solar radiation fix was the anchor        │
│                                                                             │
│  May 28  ████🔥 WRF: CORRECTION FOR EOT CALCULATION FOR SOLAR RADIATION      │
│           └─ THE MOST SRM-RELEVANT COMMIT; potential replication crisis       │
│                                                                             │
│  May 05  ████ awesome-geoengineering: v2.0.0 release (a6e8359)              │
│           └─ Major version bump after 10 months of curation                  │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## The Five Signals (v7 Deep Dive)

### Signal 1: The "Release Weekend" Pattern 🔥

**Where:** WRF (May 19–Jun 8), PCMDI (Sep 3–4), MDTF (Jun 19)  
**What:** Long quiet periods punctuated by intense development bursts  
**Why it matters:** SRM researchers should know that the models they use undergo rapid, compressed development cycles. A version release isn't just a feature add — it can include **solar radiation corrections** and **physics option shutdowns** that change the model's behavior fundamentally.

| Repo | Quiet Period | Burst Period | Burst Size | Critical Content |
|------|-------------|-------------|-----------|-----------------|
| WRF | ~6 months | 20 days | 15 commits | Solar radiation EOT fix; TEMPO disable |
| PCMDI | months | 1 day | **7 commits** | Roundoff bug (1.00 display); v4.2.1 |
| MDTF | 2 months | 1 day | 5 commits | Precip-buoyancy POD (ocean's only tool) |

### Signal 2: The CC0 Liberation Event 🌍

**Where:** `tjz21/DAC_peroxovanadates` & `tjz21/DAC_peroxotitanates` (Sep 2025)  
**What:** Two researchers chose public domain dedication (CC0) for computational screening data  
**Why it matters:** This is the **open-science ideal in action**. Not CC-BY (attribution required), not MIT (permissive but still copyrighted), but **CC0 — no rights reserved**. The data is infrastructure, not intellectual property.

**Combine with lithos-carbon's "delivery model" publication** (Aug 29, 2026): The carbon capture ecosystem is developing **both** the tools (API scoring) and the philosophy (methodology transparency) to make data truly open.

### Signal 3: The AI Governance Lab 🤖

**Where:** `open-sustainable-technology` (Jul 19, 2026)  
**What:** Mandatory AI-disclosure checkbox added to every PR  
**Why it matters:** This is the **first concrete governance response** to AI-generated contributions in climate tech OSS. The community is figuring this out in real time — no playbook, no precedent, just a checkbox that says "Did you use AI to generate this entry?"

**v7 addition:** The refinement happened within **24 hours** (`c4c9fe7` create → `be14281` refine). This is serious, ongoing attention — not a token gesture.

### Signal 4: The Sole-Contributor Risk 👤

**Where:** MDTF-diagnostics (Wei-Ming Tsai, entire ecosystem)  
**What:** One developer wrote all code, all docs, filed all PRs, merged all merges  
**Why it matters:** The most ocean-relevant tool in open source has **zero redundancy**. If Wei-Ming stops, the precip-buoyancy POD disappears. There's no community succession plan. This is the fragility of individual-driven OSS.

**ClimateMARGO is structurally similar** but different in kind: Fons van der Plas (and previously Henri Drake) are the only contributors. The 2-year dormancy (Oct 2023 → Aug 2026) shows what happens when the sole contributor moves on to other priorities.

### Signal 5: The Ocean Silence 🌊

**Where:** Across all 15 search queries, 11 repos, 12+ commit histories  
**What:** ZERO ocean geoengineering repositories, ZERO ocean intervention commits, ZERO dedicated developers  
**Why it matters:** This is the **largest governance signal in climate tech**. If we can't simulate ocean interventions, we can't evaluate them. If we can't evaluate them, we can't govern them. The silence on GitHub is not an oversight — it's an **absence of decision**.

**The one bright spot:** MDTF's precip-buoyancy POD (Jun 19, 2026) is the only tool that could detect ocean intervention signals in observational data. But it evaluates models, not interventions. It's a diagnostic, not a simulator.

---

## The Commit Velocity Comparison (v7)

| Repo | Time Span | Total Commits | Avg Velocity | Peak Velocity | Status |
|------|-----------|---------------|-------------|--------------|--------|
| **WRF** | 30 days | 15 | 0.5/day | 3/day (release) | 🟢 v4.8.0 shipped |
| **PCMDI** | 15 days | 10 | 0.67/day | **7/day (release)** | 🟢 v4.2.1 shipped |
| **lithos-carbon** | 18 days | 10 | 0.56/day | 2/day (burst) | 🟢 Weekly rhythm |
| **MDTF** | 73 days | 10 | 0.14/day | **5/day (big bang)** | 🟡 Single-contributor |
| **awesome-geo** | 435 days | 7 | 0.016/day | 2/day (double-header) | 🟢 Accelerating |
| **open-sustainable-tech** | 105 days | 15 | 0.14/day | 3/day (sustained) | 🟢 Institutional |
| **ClimateMARGO** | 1696 days | 10 | 0.006/day | 2/day (revival) | 🟡 Dormant-then-README |
| **ShennongWM-G** | 5 days | 5 | 1/day | 1/day (launch) | 🟢 New, active |
| **GCCS-Core** | 1 day | 9 | 9/day | 9/day (bulk upload) | ⚪ Dead since upload |

---

## Episode Planning Matrix (v7 Updated)

| Episode | Branch | Lead Story | Structural Insight | The Big Question |
|---------|--------|-----------|-------------------|-----------------|
| **☀️ Solar** | `solar-geoengineering` | The solar radiation bug (WRF `e836cd6`) — potential replication crisis in every published SRM simulation | Release Weekend pattern: institutional models undergo compressed development bursts | *If the model's solar physics had a bug, what were past simulations concluding about SRM effectiveness?* |
| **🌍 Carbon** | `carbon-capture` | The scorecard that scores itself (lithos-carbon: "what was measured, not a new score") + CC0 liberation of DAC screening data | Two-Speed Ecosystem: institutional curation vs. individual liberation | *Can open source + CC0 data break the $1000/ton DAC cost barrier?* |
| **🌊 Ocean** | `ocean-intervention` | The silence: 15 queries, 0 repos, 0 commits, 0 developers | The One Bright Spot (MDTF's POD) is a diagnostic, not a simulator | *What would the GitHub for ocean intervention look like? And why doesn't it exist yet?* |

---

## Cross-Theme Connections (v7)

| Connection | Repos Involved | Insight |
|------------|---------------|---------|
| **The Bug Chain** | WRF (solar radiation fix) → PCMDI (roundoff display bug) | Both are silent errors in evaluation infrastructure. Both were fixed during release prep, not discovered by users. |
| **The Documentation Ratio** | MDTF (1 code : 4 docs) → lithos-carbon (delivery model publication) | Both prioritize transparency and usability over raw feature development. |
| **The Governance Lab** | open-sustainable-tech (AI checkbox) → lithos-carbon (attribution layer) | Both are building infrastructure for **accountable** contributions — who made this, and was AI involved? |
| **The Silence Echo** | Ocean gap (0 repos) → ClimateMARGO (3yr dormancy) | Both are absences that speak volumes. Ocean: nobody decided to build. ClimateMARGO: someone stopped. |
| **The CC0 Bridge** | DAC_peroxovanadates (data liberation) → lithos-carbon (methodology transparency) | Both are about **removing barriers** — legal barriers (CC0) and knowledge barriers (open methodology). |

---

## Quick Reference: Most Important Commits (v7)

| Rank | Commit | Repo | Date | Why It Matters |
|------|--------|------|------|---------------|
| 🥇 | `e836cd6` | WRF | May 28, 2026 | Solar radiation EOT correction; possible replication crisis |
| 🥈 | `33024ad` | MDTF | Jun 19, 2026 | Only ocean-relevant diagnostic in open source |
| 🥉 | `39aaecd` | lithos-carbon | Aug 29, 2026 | "Publish delivery model" — methodology transparency for carbon scoring |
| 4 | `33024ad` + 4 docs | MDTF | Jun 19, 2026 | 1:4 code-to-doc ratio; the gold standard for accessible science tools |
| 5 | `c4c9fe7` | open-sustainable-tech | Jul 19, 2026 | First AI governance mechanism in climate tech OSS |
| 6 | `06d4240` | WRF | Jun 8, 2026 | v4.8.0 release; TEMPO options disabled 3 days prior |
| 7 | `6419050` | PCMDI | Sep 4, 2026 | v4.2.1 release; 7 commits in one day; roundoff bug fixed |
| 8 | `9fc3682` | ShennongWM-G | May 24, 2026 | Proper launch pattern: code + docs + citation in 5 days |
| 9 | `8d0a800` | awesome-geoengineering | Sep 6, 2026 | Accelerating curation cadence; v2.0.0 momentum |
| 10 | `33024ad` | MDTF | Jun 19, 2026 | Single-developer ocean ecosystem; zero redundancy |

---

## 🔗 Branch Links

| Branch | File | Theme |
|--------|------|-------|
| `solar-geoengineering` | `FRESH-COMMIT-UPDATE-SEP2026-SOLAR.md` | ☀️ Solar Geoengineering |
| `carbon-capture` | `FRESH-COMMIT-UPDATE-SEP2026-CARBON.md` | 🌍 Carbon Capture |
| `ocean-intervention` | `FRESH-COMMIT-UPDATE-SEP2026-OCEAN.md` | 🌊 Ocean Intervention |

---

## 📋 Update Log

| Version | Date | Changes |
|---------|------|----------|
| v1–v6 | Sep 2026 | Progressive analysis from 8–12 repos; ecosystem mapping; gap analysis; episode planning |
| **v7** | **Sep 2026** | **Fresh API pull from 11 repos; 5 structural signals identified; Release Weekend pattern documented; CC0 liberation event cross-referenced with lithos-carbon delivery model; AI governance refinement cycle (24h) tracked; sole-contributor risk flagged across MDTF and ClimateMARGO; 15-query ocean search log; cross-theme connection mapping; episode planning matrix updated** |
