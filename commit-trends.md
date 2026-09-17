# ☀️ Solar Geoengineering — Commit Trend Analysis

## Overview

Five repositories were analyzed for commit patterns across the solar geoengineering domain. The findings reveal a stark contrast between institutional infrastructure projects and dormant research tools.

## Individual Repo Histories

### 1. PCMDI/pcmdi_metrics (⭐133) — THE ONLY ACTIVE REPO

| Date | Commit | Author |
|------|--------|--------|
| Sep 4, 2026 | Merge PR #1428 (patch-1) | Jiwoo Lee |
| Sep 4, 2026 | Bump version to 4.2.1 | Jiwoo Lee |
| Sep 4, 2026 | Merge PR #1429 (patch-2) | Jiwoo Lee |
| Sep 4, 2026 | Update version in CITATION.cff | Jiwoo Lee |
| Sep 4, 2026 | Prepare v4.2.1 | Jiwoo Lee |
| Sep 4, 2026 | Merge PR #1427 (roundoff fix) | Jiwoo Lee |
| Sep 4, 2026 | Prevent roundoff to 1.00 in extremes | James Goodnight |
| Sep 3, 2026 | Merge PR #1425 (extremes chunking) | Jiwoo Lee |
| Sep 3, 2026 | Merge branch main into PR | Jiwoo Lee |
| Sep 3, 2026 | Merge PR #1423 (dask/SVD memory) | Jiwoo Lee |

**Pattern:** 10 commits in 2 days — a pure institutional release burst. All commits by Jiwoo Lee at LLNL, with PRs from James Goodnight (LLNL) and Jared Lewis (LLNL). This is well-funded, coordinated institutional development, not organic community contribution.

**Episode Insight:** This is what a mature climate-software institution looks like. The SRM community needs equivalent infrastructure — a dedicated SRM evaluation toolkit — but the funding and coordination to produce it doesn't exist in the geoengineering space.

---

### 2. FMS-ESM/AM3 (⭐4)

| Date | Commit | Author |
|------|--------|--------|
| Mar 2015 | Last commit (legacy Fortran atmospheric model) | GFDL staff |

**Pattern:** Complete dormancy since 2015. 4 stars total. This is a legacy model that was never designed for open-source collaboration — it's a research artifact.

---

### 3. pmip4/pmip_p2fvar_analyzer (⭐4)

| Date | Activity | Notes |
|------|----------|-------|
| Sep 2025 | Last update | CMIP6 paleoclimate data analysis tool |

**Pattern:** Sparse, infrequent updates. Paleoclimate specialist tool — not directly SRM-focused but provides the natural variability baseline that SRM research needs.

---

### 4. RhondaMueller/Codes-RFG-Arctic-Impacts (⭐1)

| Date | Activity | Notes |
|------|----------|-------|
| Apr 2024 | Last update | SRM radiative forcing calculations for Arctic region |

**Pattern:** Dormant since 2024. Research-specific code for calculating Arctic impacts of SRM — a critical topic that has almost no open-source tooling.

---

### 5. hausfath/srm-forever (⭐0)

| Date | Activity | Notes |
|------|----------|-------|
| Aug 26, 2026 | Last update | Interactive single-page SRM economics model |

**Pattern:** The only interactive, open-source SRM tool found. Updated as recently as Aug 26, 2026. Solo author. Educational rather than research-grade.

---

## Cross-Cutting Patterns

### The Big Picture: Two Tiers of Existence

| Tier | Repos | Characteristics |
|------|-------|-----------------|
| **Institutional Infrastructure** | PCMDI/pcmdi_metrics | Well-funded, multi-contributor, rapid release cycles, 133 stars |
| **Legacy/Dormant** | AM3, PMIP analyzer, Arctic Impacts | Single-author, Fortran or obscure languages, years without commits |
| **Nascent/Educational** | srm-forever | Recent activity but 0 stars, solo author, educational focus |

### What This Tells Us About SRM on GitHub

1. **No middle ground exists** — There is nothing between institutional infrastructure (PCMDI, 133★) and dormancy (AM3, 0★). The SRM community lacks the "small team maintaining a useful tool" tier that other climate-tech domains have.

2. **The institutional model works for evaluation but not for simulation** — PCMDI can evaluate models, but no one is building SRM scenarios. The gap between "evaluation infrastructure" and "scenario simulation infrastructure" is the key missing piece.

3. **Legacy Fortran is a barrier** — AM3 (2015) can theoretically be used for SRM experiments, but it's in Fortran with no modern front-end. The Python revolution in climate science has bypassed geoengineering simulation entirely.

4. **The August 2026 uptick in srm-forever** — The only solo-authored, interactive tool was updated recently. This suggests individual researchers are starting to build accessible SRM tools, but they're not yet institutionalized.

### The Governance Infrastructure Gap

The most important finding is not that SRM simulation code is scarce — it's that **the evaluation and governance infrastructure for SRM is also scarce.** PCMDI metrics is the closest thing to governance infrastructure for climate models, and it evaluate whole ESMs, not SRM-specific processes. The SRM community lacks:

- An SRM-specific evaluation toolkit (equivalent to PCMDI but for radiation management)
- A scenario comparison framework (how do you compare different SRM strategies?)
- A risk assessment standard (how do you evaluate unintended consequences?)
- An open-source general circulation model configured for SRM experiments

This infrastructure gap is the governance gap. Without these tools, the SRM policy debate operates without the computational infrastructure needed to test claims — a situation that has enormous implications for how the conversation unfolds.

## Key Episode Talking Points

1. **The Scarcity Story**: Why does the most controversial climate technology have so little open-source simulation code? The answer is partly about funding, partly about governance sensitivity, and partly about the legacy Fortran problem.

2. **The Governance Angle**: PCMDI's metrics toolkit is the unsung infrastructure of climate model evaluation. What does it mean that SRM lacks an equivalent? The policy debate is happening without the computational tools to test claims.

3. **The Democratization Question**: Can lightweight interactive models (like srm-forever) bring SRM discourse to a broader audience, or do they oversimplify? The gap between educational models and research-grade simulations is vast.

4. **The Arctic Risk**: RhondaMueller's code is the only tool specifically designed to calculate SRM's impacts on the Arctic — the region most sensitive to both warming and SRM side effects. Its dormancy (since 2024) is a warning sign.

5. **The August 2026 Cluster**: srm-forever was updated on Aug 26, 2026 — is this a sign of renewed interest in accessible SRM modeling? What would it take to turn a solo educational project into a community-maintained tool?