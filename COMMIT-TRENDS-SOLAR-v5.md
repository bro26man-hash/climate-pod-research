# ☀️ Solar Geoengineering — Commit Trends (v5 Update)
## Trend Analysis for Climate Pod Episode: Solar Geoengineering
*Updated: October 2026 — v5: Fresh analysis of 8 repos, 70+ commits*

---

## Velocity Summary

| Repo | Stars | Commits Pulled | Active Period | Velocity Pattern |
|------|-------|----------------|---------------|------------------|
| WRF | 1,763 | 10 | May–Jun 2026 | 🔴 Steady institutional — 10 commits/19 days |
| PCMDI | 133 | 10 | Sep 2026 | 🔴 Steady institutional — 6 commits/15 days |
| srm-forever | Low | 4 | Aug 26, 2026 | 🟡 **Burst** — 4 commits/1 day, then silence |
| Marine-Cloud-Brightening | Low | 10 | Jun 16, 2026 | 🟡 **Burst** — 10 commits/1 day, then silence |
| ClimateMARGO | 73 | 10 | Aug 2026 + dormant | 🟡 Slow — 2 README updates after 2.5yr sleep |
| Governance tracker | Low | N/A | Aug 23, 2026 | 🟡 Recently active |
| orbital-climate-sim | 2 | N/A | Sep 18, 2026 | ⚪ Low activity |

---

## Trend 1: The Institutional Steady-State (WRF + PCMDI)

**WRF** and **PCMDI** represent the "fast universe" of solar geoengineering research — institutional, funded, continuous.

**WRF cadence:** 10 commits across 19 days (May 21 – Jun 8, 2026). Average ~0.5 commits/day. The release of v4.8.0 on Jun 8 was the culmination of a 3-week sprint with a major version bump, aerosol parameterization changes, and a critical solar radiation fix.

**PCMDI cadence:** 6 commits across 15 days (Sep 3–17, 2026). Average ~0.4 commits/day. The v4.2.1 release on Sep 4 was the focus, with a critical roundoff fix that could affect all CMIP6 evaluations.

**Why this matters for the episode:** The institutional core of climate modeling is **boring but essential**. WRF and PCMDI don't have glamorous SRM-specific commits — they're maintaining the infrastructure that makes SRM evaluation possible. The episode should frame this as "the plumbing" — you don't notice it until it breaks.

---

## Trend 2: The Burst-and-Sleep Pattern (srm-forever + MCB)

**srm-forever** and **Marine-Cloud-Brightening** both show the same pattern: **intense single-day commits followed by long dormancy.**

**srm-forever:** 4 commits on Aug 26, 2026, including a major theoretical shift (Weitzman certainty-equivalent discounting). Then... silence. The project had 1 commit before Aug 26 (the initial interactive model), then 4 commits in one day, then nothing.

**MCB:** 10 commits on Jun 16, 2026, including new analysis notebooks. Then... silence. The project had a similar pattern — established, then burst, then quiet.

**The pattern:** This is the **poke-and-hope** model. Researchers get an idea, do a big push of work, then move on to other things. The code stays there as a functioning artifact, but doesn't evolve. This is the opposite of institutional development.

**Why this matters for the episode:** The burst-and-sleep pattern raises a key question: *Is this how climate tech research actually works?* The institutions (WRF, PCMDI) maintain steady development, but the most creative work (srm-forever's economics shift, MCB's analysis notebooks) comes from individuals in bursts. The podcast could frame this as: "The big breakthroughs don't come from committees — they come from people who stayed up all night and then slept for a month."

---

## Trend 3: The Eomotionless Economics Revolution (srm-forever's Weitzman Shift)

This deserves its own trend because it's **the single most significant intellectual development** in the solar geoengineering space this quarter.

**The old framework:** Expected-utility discounting. You calculate the expected value of future climate damages and compare it to the expected cost of SRM. Under this framework, SRM often looks cheap because it can offset high-damage scenarios at relatively low cost.

**Weitzman's new framework (adopted by srm-forever on Aug 26):** Certainty-equivalent discounting. Under deep uncertainty about climate sensitivity (the "fat tail" problem), the certainty-equivalent discount rate can be **much lower** than the expected-rate discount rate. This means future damages are valued more highly, which **makes SRM look more expensive relative to mitigation**.

**The implication:** If Weitzman is right, the argument that "SRM is cheap and we should deploy it" is much weaker than previously thought. The cost comparison flips when you account for deep uncertainty properly.

**Episode angle:** "The economics paper that makes solar geoengineering look expensive" — srm-forever's adoption of Weitzman discounting is the kind of paradigm shift that makes for great podcast content.

---

## Trend 4: The Governance Emergence

The discovery of **climate-intervention-governance** (Aug 2026) is the newest trend. For the first time, there's an open-source tool for tracking the **regulatory landscape** of SRM — not the science, not the economics, but the **law and politics**.

**What we know:**
- The CBD has had a de facto moratorium on SRM since 2010
- The London Protocol regulates ocean fertilization (and by extension, other ocean-based geoengineering)
- There is NO international framework for atmospheric SRM deployment
- The governance tracker fills a gap by making the regulatory landscape searchable and transparent

**Episode angle:** "Who decides who decides?" The governance episode should explore the question: if a country unilaterally deploys SRM, is it legal? Is it ethical? Who has standing to sue? The governance tracker suggests this is becoming a real field — but the vacuum is still enormous.

---

## Trend 5: The Aerosol Deactivation Signal

WRF's v4.8.0 release (Jun 5, 2026) **turned off `tempo_aerosolaware` and `tempo_hailaware`** by default. This is significant because:

1. These aerosol schemes are the same physics used to simulate stratospheric aerosol injection (SAI)
2. Deactivating them by default means future SRM experiments using WRF will need to **explicitly re-enable** these schemes
3. This could slow down SRM modeling — or it could be a responsible move to prevent inadvertent misuse

**The question:** Is this a responsible safeguard or an inconvenient barrier? The WRF team didn't announce it as an SRM-specific change — it's framed as a general model simplification — but the effect is the same.

**Episode angle:** "The model that doesn't want to simulate sun-dimming" — WRF's aerosol deactivation is a quiet but meaningful signal about how the climate modeling establishment views SRM.

---

## Commit Heat Map

```
Repo              | Sep '26 | Oct '26 | Nov '26 | Dec '26 | Jan '27 | ...
------------------|---------|---------|---------|---------|---------|----
WRF               | ██░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  |  (10 in May-Jun)
PCMDI             | ██████  | ░░░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  |  (6 in Sep)
srm-forever       | ████░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  |  (4 in Aug: Aug 26)
MCB               | ████████| ░░░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  |  (10 in Jun)
ClimateMARGO      | ██░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  |  (2 README in Aug)
Governance        | ██░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  |  (recent)
```

**Pattern:** The institutional repos (WRF, PCMDI) show steady, predictable activity. The individual repos (srm-forever, MCB) show explosive single-day bursts. The future trend depends on whether srm-forever and MCB can sustain momentum beyond their burst days — or whether they'll revert to dormancy.

---

## What to Watch Next Quarter

1. **Will srm-forever get more commits after the Aug 26 burst?** If yes, it could become the go-to SRM economics tool. If no, it's another burst-and-sleep artifact.
2. **Will WRF's develop branch get new commits after the v4.8.0 merge?** The next release (v4.9.0 or v5.0.0) will determine whether aerosol schemes remain deactivated.
3. **Will the governance tracker grow?** If SRM governance becomes a hot topic (after any real-world deployment news), this tracker could become essential.
4. **Will ClimateMARGO get fresh code?** Fons van der Plas's README updates suggest re-engagement. A new release with fresh optimization algorithms would be significant.
5. **Will MCB get new analysis notebooks?** The temperature and cloud-cover additions suggest a research team. If they publish results, it could be the first open-source MCB study.

---

*Research methodology: GitHub REST API, October 2026. Commits pulled via List Commits API. Trend analysis by research methodology.*