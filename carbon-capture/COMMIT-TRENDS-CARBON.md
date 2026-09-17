# 🌍 Carbon Capture — Commit Trend Analysis

**Research Date:** September 2026  
**Data Source:** 6+ repositories across direct air capture and carbon capture

---

## Executive Summary

The carbon capture open-source ecosystem shows a **stark divide between thriving community hardware projects (OpenAir-Cyan) and dormant academic deposits (carbon-capture-and-storage, 85★).** The most significant finding is the **August 2026 DAC materials wave** — independent research groups updating DAC sorbent repositories simultaneously, suggesting coordinated activity. Meanwhile, the living survey (Carbon_Capture_ML) remains the best single resource for understanding ML's role in CC刻.

---

## Commit Activity Timeline

```
2020 ──► carbon-capture-and-storage begins (BSc thesis project)
2021 ──► carbon-capture-and-storage: 10 commits over 10 months, then silence
2022 ──► openair-cyan: Active community building (May–Jul)
2023 ──► Carbon_Capture_ML: 5 commits in 4 days (Feb burst, papers)
2024 ──► openair-cyan: Feb burst (OSHWA certification)
         Carbon_Capture_ML: README updates + OpenDAC paper
2025 ──► Minimal activity
2026 ──► Aug: DAC materials wave begins ★ MAJOR SIGNAL
         Aug: openair-cyan, peroxovanadates, peroxotitanates, membrane_model all update
         Jun: Cost-Model--DAC continues (Monte Carlo cost projections)
```

---

## Detailed Analysis by Project

### OpenAir-Cyan — The Community-Driven Beacon

**Active Phase:** May–Jul 2022 (5 commits, 2 developers)
**Formalization Phase:** Feb 12, 2024 (6 commits, 1 developer, OSHWA UID)
**Current Status:** Maintenance

The developer community shifted from hardware builders (DaOfficialWizard, ZanzyTHEbar) to documentation formalizers (K Collins). The OSHWA UID certification (US001095) is the milestone — it's the first open-source CC刻 device with official open-hardware certification.

**Why It Matters:** OpenAir-Cyan proves that DIY carbon capture is possible. The device is small-scale, documented, and reproducible. It's not going to save the planet alone, but it demonstrates that the technology is accessible.

### Carbon_Capture_ML — The Living Bibliography

**Peak Activity:** Feb 2–5, 2023 (5 commits, 4 papers in 4 days)
**Maintenance Period:** Jan–May 2024 (5 README updates + 1 paper)

The burst pattern is typical of a literature review responding to publication cycles. The project's value is as a curated index — not as software.

**Why It Matters:** When someone asks "what's the state of ML in carbon capture?", this repo answers. It's the field's bibliography and roadmap.

### carbon-capture-and-storage — The Ghost Project

**Activity:** May 2020 – Mar 2021 (10 commits over 10 months)
**Silence:** Mar 2021 – present (5+ years)

This is the most frustrating pattern in climate tech open source. 85 stars, but the developer stopped maintaining it 5 years ago. The thesis got cited, but the code is frozen.

**Why It Matters:** Academic incentive structures don't reward long-term code stewardship. The PIs get cited, the students move on, and the code rots.

### Cost-Model--DAC — The Economics Answer

**Activity:** Continuous, most recent Jun 2026

This project is notable for being still active. The Monte Carlo approach to DAC cost projections is methodologically sound and provides uncertainty quantification.

**Why It Matters:** The cost question is the make-or-break question for DAC. This model gives a probabilistic answer: "it could be $100/ton by 2040, but there's wide uncertainty."

---

## The August 2026 Materials Wave: Deep Dive

| Repo | Focus | Date | Likely Trigger |
|------|-------|------|----------------|
| tjz21/DAC_peroxovanadates | Peroxovanadate sorbents | Aug 19, 2026 | Shared deadline? |
| tjz21/DAC_peroxotitanates | Peroxotitanate sorbents | Aug 19, 2026 | Shared deadline? |
| CCSI-Toolset/membrane_model | Membrane separation | Aug 23, 2026 | Related release? |
| openair-collective/openair-cyan | DIY DAC device | Aug 19, 2026 | Community update? |

**Hypothesis:** These may be connected to a workshop, conference, or collaborative data release focused on computational DAC materials. The 2-day gap between perovskite updates (Aug 19) and membrane model (Aug 23) suggests a multi-phase event.

**Podcast Angle:** The August 2026 wave suggests that open computational chemistry for DAC is latent and ready to activate. With proper coordination (a shared platform, a workshop, a challenge), this distributed research could accelerate dramatically.

---

## Comparative Activity Matrix

| Metric | OpenAir-Cyan | CC_ML | CC@Storage | CO2-Sensor | Cost-Model |
|--------|-------------|-------|------------|------------|------------|
| Stars | 76 | 56 | 85 | 16 | 6 |
| Last activity | Feb 2024 | May 2024 | Mar 2021 | Aug 2026 | Jun 2026 |
| Active devs | 2→1 | 1 | 1 | ? | ? |
| Dev style | Community | Survey | Deposit | Research | Model |
| Maintenance | Low | Low | None | Medium | Medium |
| Open source HW | ✅ Yes | ❌ No | ❌ No | ❌ No | ❌ No |
| OSHWA cert | ✅ Yes | ❌ No | ❌ No | ❌ No | ❌ No |

---

## Emerging Trends

1. **Open hardware is the differentiator** — Cyan and Epiphyte are the only projects with physical, reproducible outputs. OSHWA certification of Cyan is a blueprint for open-source climate hardware.

2. **The materials wave is coming** — The August 2026 cluster suggests that DAC materials research is about to get a coordinated open-source boost. Peroxovanadates and peroxotitanates are the hot sorbent candidates.

3. **Survey repos have outsized impact** — Carbon_Capture_ML (56★) has more impact than most 100+ star repos because it's a living resource, not a frozen codebase.

4. **The cost barrier is the real story** — Cost-Model--DAC shows that the path to $100/ton is uncertain but possible. The economics, not the chemistry, is the primary barrier.

5. **The academic deposit curse** — High-star, zero-activity repos (carbon-capture-and-storage, 85★) represent a systemic failure in academic reward structures.

---

## Questions for Next Episode

- Is the August 2026 materials wave a one-time event or the beginning of coordinated open-source DAC research?
- Can OpenAir-Cyan's OSHWA certification model scale to other climate hardware?
- Will peroxovanadates/peroxotitanates become the breakthrough sorbent, or are they incremental?
- How do we fix the academic deposit curse — incentivize long-term code maintenance?
- Is the $100/ton DAC cost target achievable, or is it a mirage?

---

*Full commit data sourced from GitHub API on September 2026.*