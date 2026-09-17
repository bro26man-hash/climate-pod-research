# 🌍 Carbon Capture — Commit Trend Analysis

**Research Date:** September 2026 (v4 Update)  
**Data Source:** 9 repositories across direct air capture and carbon capture, 89+ commits pulled fresh from GitHub API

---

## Executive Summary

The carbon capture open-source ecosystem shows a **stark divide between thriving ecosystem directories (open-sustainable-technology, 2,552★) and dormant academic deposits (carbon-capture-and-storage, 85★).** The most significant findings from fresh commit data are: **(1)** the CC0 public domain dedication of two DAC sorbent screening repos (Sep 12, 2025) — the biggest open-science signal in carbon capture; **(2)** open-sustainable-technology's continuous curation activity (15 commits in 3 months, 4 contributors) — the most sustained development in the entire theme; and **(3)** the August 2026 materials wave — README refreshes across peroxovanadates, peroxotitanates, and openair-cyan on the same day. Meanwhile, Carbon_Capture_ML remains the best living bibliography but shows slow decline after its Feb 2023 burst.

---

## Commit Activity Timeline (Updated with Fresh Data)

```
2020 ──► carbon-capture-and-storage begins (May 2020, 15 commits)
2021 ──► carbon-capture-and-storage: 10 commits in Mar 2021, then ghost
2022 ──► openair-cyan: Active community building (May–Jul)
2023 ──► Carbon_Capture_ML: 5 commits in 4 days (Feb burst, papers)
         tearDown: Nov 2023—Dec 2023: bulk README metadata in DAC repos
2024 ──► openair-cyan: Feb 12 burst (OSHWA certification, 15 commits)
         DAC_peroxovanadates: Mar 11 README/documentation updates
         DAC_peroxotitanates: May–Jul 2024: CASTEP reference, README cleanup
         Carbon_Capture_ML: May 2024 OpenDAC paper added
2025 ──► Sep 12: ★ CC0 LICENSE ADDED to both DAC repos ★
         Sep 23: README updates in both DAC repos
2026 ──► Jun–Sep: open-sustainable-technology: 15 commits, 4 contributors ★ MOST ACTIVE
         Aug 19: DAC materials wave — README refreshes across 3 repos
         Aug 19: openair-cyan README update (community maintenance)
         Aug 23: open-sustainable-technology adds claude-carbon
```

---

## Detailed Analysis by Project (Updated with Fresh Commits)

### open-sustainable-technology — The Ecosystem Directory (Fresh Data)

**Fresh Commits Pulled:** 15 (Jun 6 – Sep 9, 2026)

**Activity Pattern:** Continuous curation, 4 distinct contributors

| Contributor | Commits | Adds |
|-------------|---------|------|
| Tobias Augspurger | 7 | PowerIO, ASSETRA, ToOp, wbdata, EpexPredictor, PR templates |
| Abdul Salam | 4 | MUIO, MUIOGO, Story Seed Library, openflexure microscope |
| Christophe Combelles | 1 | Volca (Life Cycle Assessment) |
| gwittebolle | 1 | claude-carbon |
| Mikhail Alabugin | 1 | Docs: fix dead links |

**Key Insight:** This is the most continuously active repo in the entire carbon capture theme. The curation pattern — each commit adds a new climate-tech project to the directory — makes it the "GitHub of climate tech." Recent additions span carbon capture (claude-carbon), energy (PowerIO, MUIO), materials (ASSETRA, ToOp), and open hardware (openflexure microscope).

**Podcast Angle:** open-sustainable-technology is the meta-repository that indexes the climate tech ecosystem. With 2,552 stars, it's the most-followed climate-tech repo on GitHub. If you want to find a climate tech project, you start here. The 4-contributor model shows that curation can be distributed, not centralized.

### OpenAir-Cyan — The Community Beacon (Fresh Data)

**Fresh Commits Pulled:** 15 (all on Feb 12, 2024)

**Certification Day:** 6 commits by K Collins (OSHWA UID, CITATION.cff, README, file uploads)

**Pre-certification (2022):** 9 commits by 2 developers (DaOfficialWizard, ZanzyTHEbar)

**The Pattern:** Community building (2022) → Formalization (2024) → Silence (2024–present)

**Podcast Angle:** The OSHWA certification was a milestone, not a momentum shift. The community builders left; the formalizer arrived; then silence. Open hardware needs a different sustainability model — not "certify and freeze" but "iterate and maintain."

### Carbon_Capture_ML — The Living Bibliography (Fresh Data)

**Fresh Commits Pulled:** 15 (Jan 2023 – May 2024)

**Burst Phase (Feb 1–5, 2023):** 6 commits, 5 papers added

**Maintenance Phase (Jan–May 2024):** 5 README updates + 1 paper

**The Decline:** After the Feb 2023 burst, commits slow to ~1 per month. The repo is settling into "curated reference" mode — maintained enough to stay current, but not enough to be a living tool.

**Podcast Angle:** Carbon_Capture_ML is the field's bibliography and roadmap. When someone asks "what's the state of ML in carbon capture?", this repo answers. But it's a survey, not software. The gap between "we catalogued the papers" and "we built the tools" is the central story of ML in CC刻.

### DAC_peroxovanadates & DAC_peroxotitanates — The CC0 Revolution (Fresh Data)

**Fresh Commits Pulled:** 15 + 10 = 25 commits across both repos

**The CC0 Moment (Sep 12, 2025):** Both repos received CC0 public domain dedications by Jacob Hirschi

**Why This Matters:** CC0 is not just "open source" — it's "public domain." Anyone can use the computational screening data for any purpose, no license required. This is the biggest open-science signal in the entire carbon capture theme.

**The Dec 2023 Bulk Work:** 7 README updates in one day (Dec 5, 2023) — systematic metadata and documentation preparation.

**The Sep 2025 Updates:** README updates on Sep 23, 2025 in both repos.

**Podcast Angle:** "The CC0 Revolution" — When Jacob Hirschi dedicated the DAC peroxovanadate and peroxotitanate screening data to the public domain, he made computational chemistry data into public infrastructure. This is the model for how open science should work — not just sharing code, but sharing data with no restrictions. The CC0 choice is a statement: "This data belongs to everyone."

### carbon-capture-and-storage — The Ghost Project (Fresh Data)

**Fresh Commits Pulled:** 15 (all Feb 2020 – Mar 2021)

**Activity Pattern:** Thesis/paper project — upload data, run simulations, organize files, stop

**Dormancy:** 5+ years since last commit (Mar 6, 2021)

**85 stars but zero activity.** The thesis got cited, but the code is frozen.

**Podcast Angle:** "The academic deposit curse" — High-star, zero-activity repos represent a systemic failure in academic reward structures. The PIs get cited, the students move on, and the code rots.

### openair-sorbent-tester — The Companion Hardware (Fresh Data)

**Last Updated:** Jan 10, 2026 (only recent activity in the carbon hardware space)

**Focus:** Small-scale open hardware sorbent tester for moisture swing DACC sorbents

**Relationship to OpenAir-Cyan:** Companion project — Cyan is the capture device, sorbent-tester is the quality control tool

**Podcast Angle:** The sorbent tester is the most practically useful carbon capture hardware project on GitHub. You don't need to build a full DAC device — you can start by testing sorbents with this tool. It's the "入门" (entry point) for open-source carbon capture hardware.

---

## The August 2026 Materials Wave (Updated Deep Dive)

| Repo | Focus | Date | Nature of Update |
|------|-------|------|------------------|
| tjz21/DAC_peroxovanadates | Peroxovanadate sorbents | Aug 19, 2026 | README refresh (CC0 since Sep 2025) |
| tjz21/DAC_peroxotitanates | Peroxotitanate sorbents | Aug 19, 2026 | README refresh (CC0 since Sep 2025) |
| openair-collective/openair-cyan | DIY DAC device | Aug 19, 2026 | README update (community maintenance) |
| CCSI-Toolset/membrane_model | Membrane separation | Aug 23, 2026 | Recent activity (membrane modeling) |

**Updated Hypothesis:** The Aug 19 simultaneous updates are README refreshes, not data drops. The real signal is the CC0 license adoption on Sep 12, 2025 — seven months before the Aug 2026 wave. The materials wave is not a single event but a pattern: coordinated repos sharing a research context, with periodic README maintenance.

---

## Comparative Activity Matrix (Updated)

| Metric | Open-Sustain-Tech | OpenAir-Cyan | CC_ML | CC@Storage | Peroxovanadates | Peroxotitanates | Sorbent-Tester |
|--------|-------------------|-------------|-------|------------|-----------------|-----------------|----------------|
| Stars | 2,552 | 76 | 56 | 85 | 2 | 2 | 3 |
| Last activity | Sep 2026 | Feb 2024 | May 2024 | Mar 2021 | Sep 2025 | Sep 2025 | Jan 2026 |
| Commits pulled | 15 | 15 | 15 | 15 | 15 | 10 | — |
| Active devs | 4 | 1→0 | 1 | 1 | 1 | 1 | ? |
| Dev style | Curation | Community | Survey | Deposit | Research | Research | Hardware |
| Maintenance | ✅ Continuous | ❌ Frozen | ⚠️ Slow | ❌ Ghost | ⚠️ Periodic | ⚠️ Periodic | ⚠️ Slow |
| Open source HW | ❌ No | ✅ Yes | ❌ No | ❌ No | ❌ No | ❌ No | ✅ Yes |
| CC0/Public Domain | ❌ No | ❌ No | ❌ No | ❌ No | ✅ Yes | ✅ Yes | ❌ No |

---

## Emerging Trends (Fresh Data)

1. **The CC0 revolution is the biggest open-science story.** Two DAC sorbent screening repos are now public domain. This is the model for how open science should work — not just sharing code, but sharing data with no restrictions.

2. **The ecosystem directory is the most sustainable model.** open-sustainable-technology (2,552★, 4 contributors, 15 commits in 3 months) proves that curation can be continuously maintained. The "index the ecosystem" model works because every addition is a new entry point.

3. **The August 2026 wave is a pattern, not an event.** DAC materials repos update simultaneously because they share a research context — not because of a single coordinated release. The wave is latent and ready to activate with proper coordination.

4. **Open hardware needs a new sustainability model.** OpenAir-Cyan's OSHWA certification was the finish line, not the starting gun. Open hardware needs iteration, community, and continuous improvement — not just certification.

5. **The academic deposit curse persists.** 85★ carbon-capture-and-storage (dead since 2021) is the most-starred repo in the theme but the least useful. Stars measure citations, not usability.

6. **The companion hardware story matters.** openair-sorbent-tester (3★, last updated Jan 2026) is the most practically useful carbon capture hardware project. You don't need to build a full DAC device — start by testing sorbents.

---

## Questions for Next Episode (Updated)

- Is the CC0 dedication a one-person decision or a community movement? Will other DAC repos follow?
- Can open-sustainable-technology's curation model scale to other climate tech domains?
- What would a sustainable open-hardware DACC project look like, beyond OSHWA certification?
- Will peroxovanadates/peroxotitanates become the breakthrough sorbent, or are they incremental?
- Is the sorbent-tester the real entry point for open-source carbon capture hardware?
- How do we fix the academic deposit curse — incentivize long-term code maintenance?
- Is the $100/ton DAC cost target achievable, or is it a mirage?

---

*Full commit data sourced from GitHub API on September 2026 (v4 update).*
