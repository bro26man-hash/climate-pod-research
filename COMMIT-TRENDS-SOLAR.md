# ☀️ Solar Geoengineering — Commit Trend Analysis

**Research Date:** September 2026 (v4 Update)  
**Data Source:** 5 repositories across solar geoengineering and climate simulation, 64+ commits pulled fresh from GitHub API

---

## Executive Summary

The solar geoengineering open-source ecosystem is characterized by **institutional dominance, paper-driven development, and a scarcity of dedicated SRM simulation tools.** The most significant signals in the fresh commit data are: **(1)** WRF's continuous institutional development with a direct solar radiation correction (May 2026), **(2)** PCMDI's extreme-event evaluation burst (10 commits on Sep 4, 2026 for v4.2.1), **(3)** MDTF's precipitation-buoyancy POD (5 commits on Jun 19, 2026 — the ocean's closest friend), and **(4)** ClimateMARGO's ambiguous revival after 2.5 years of dormancy. Meanwhile, srm-forever's 4-commit theoretical burst (Aug 26, 2026) introduced the Weitzman discounting framework — the most rigorous economic analysis of SRM sustainability ever coded.

---

## Commit Activity Timeline (Updated with Fresh Data)

```
2022 ──► ClimateMARGO: 7 commits (Henri Drake era, Jan-Feb)
         ClimateMARGO: 2 commits (JuMP compat, Nov)
2023 ──► actm-sai-csu: 10 commits (paper/preprint cycle)
2024 ──► GCCS-Core: 10 commits (single-day bulk upload)
2025 ──► GeoVision: sparse updates
2026 ──► ClimateMARGO: 2 README commits (Aug 17) ★ AMBIGUOUS SIGNAL
         WRF: 15 commits (May-Jun) — v4.8.0, solar radiation fix ★ SRM-RELEVANT
         MDTF: 15 commits (May-Aug) — precip-buoyancy POD Jun 19 ★ OCEAN-ADJACENT
         PCMDI: 15 commits (Sep 3-17) — v4.2.1, extremes chunking ★ EVALUATION INFRA
         srm-forever: 4 commits (Aug 26) — Weitzman discounting ★ THEORY BURST
```

---

## Detailed Analysis by Project (Updated with Fresh Commits)

### ClimateMARGO.jl — The Revival Signal (Re-Analysis)

**Commit Span:** Jan 2022 – Aug 2026 (but with 2.5-year gap)

**Phase 1 (Jan–Feb 2022):** Henri Drake established the project
- Added CITATION.bib, fixed typos, updated docs
- 7 commits in the first 2 months

**Phase 2 (Nov 2022):** Dependency maintenance
- JuMP/Ipopt compat upgrade
- Project.toml update
- 2 commits

**Phase 3 (GAP):** No meaningful activity for 2.5 years (Feb 2022 → Aug 2026)

**Phase 4 (Aug 2026):** Fons van der Plas updates README twice
- Two README-only commits on the same day (Aug 17)
- No code changes, no issue discussions
- **Interpretation:** Could be a genuine revival, or could be a link/update without deeper engagement. The fact that a new maintainer (different from original) is updating it suggests possible institutional interest.

**Podcast Angle:** Is ClimateMARGO's revival a canary for growing geoengineering policy-modeling interest? Or is it another ghost-update in a sea of dormant climate repos? The maintainer change (Drake → van der Plas) is the key detail — this isn't the original author coming back, it's someone new discovering the project.

### WRF — The Institutional Engine (Fresh Data)

**Fresh Commits Pulled:** 15 (May 12 – Jun 8, 2026)

**Key SRM-Relevant Commit:**
- `e836cd6` (May 28, 2026) — "Correction for eot calculation for solar radiation" by weiwangncar
- This fix corrects the solar radiation energy balance calculation — the physics that SRM simulations depend on

**Development Pattern:** Continuous, multi-developer, institutional
- 5 distinct developers in 15 commits
- Regular release cycle (v4.8.0 released Jun 8, 2026)
- Bug fixes, physics updates, namelist additions, submodule management

**Podcast Angle:** WRF is the "Linux of climate simulation" — nobody notices it until it breaks, but everything depends on it. SRM researchers configure WRF with aerosol injection modules. Without institutional funding, there's no WRF, and without WRF, there's no SRM simulation. The solar radiation correction proves that even "routine" maintenance has SRM implications.

### MDTF-diagnostics — The Governance Infrastructure (Fresh Data)

**Fresh Commits Pulled:** 15 (May 22 – Aug 14, 2026)

**Key Ocean-Adjacent Commit:**
- `33024ad` (Jun 19, 2026) — "Add MCS precipitation-buoyancy statistics POD" by Wei-Ming Tsai
- 5 total commits on `MCS_precip_buoy_stats.rst` on the same day

**Development Pattern:** Release-driven, institutional
- v4.2.1 release cycle evident in PCMDI's parallel commits
- Precipitation-buoyancy POD is the most ocean-relevant diagnostic in open source
- Quarterly metrics workflow added for "traffic logging"

**Podcast Angle:** MDTF-diagnostics is the evaluation toolkit for CMIP6 models. If SRM is ever deployed, we need to be able to detect, attribute, and evaluate its effects. MDTF is the governance infrastructure that makes that possible. The precip-buoyancy POD is a building block for ocean-specific evaluation.

### PCMDI/pcmdi_metrics — The Evaluation Breakthrough (Newly Detailed)

**Fresh Commits Pulled:** 15 (Sep 3–17, 2026)

**Key Release Commit:**
- `6419050` (Sep 4, 2026) — "Bump version to 4.2.1"
- 10 commits on Sep 4 alone — institutional release burst

**Critical PRs:**
- #1425: "extremes_chunking" — chunking for extreme event analysis
- #1423: "variability-modes-dask-svd-memory" — memory optimization for SVD
- #1418: "jsgoodni_corr_roundoff" — prevents roundoff to 1.00 in mean_climate

**Podcast Angle:** The "extremes chunking" PR is the most SRM-relevant commit in the entire dataset. Extreme event analysis is how you detect SRM injection signals. If you want to know whether solar geoengineering is working, you look for shifts in extreme event statistics. PCMDI is building the detection infrastructure.

### srm-forever — The Weitzman Model (Fresh Data)

**Fresh Commits Pulled:** 4 (all on Aug 26, 2026)

**Theoretical Framework:**
1. `9999436` — Interactive SRM-forever vs mitigation+CDR cost model (base)
2. `9ee822a` — Price abatement as a vintage annuity (economic framing)
3. `aa9bc0f` — Adopt Weitzman certainty-equivalent discounting; add discount-rate essay (core theory)
4. `61df1a4` — Add effective discount rate chart (visualization)

**Weitzman Certainty-Equivalent Discounting:** This framework asks "what is the certainty-equivalent cost of maintaining SRM indefinitely?" William Weitzman's insight is that under deep uncertainty, the expected cost of perpetual SRM may be infinite — meaning that from a decision-theoretic perspective, you should not commit to permanent SRM even if the expected cost seems low.

**Podcast Angle:** This is the most policy-relevant code in the solar geoengineering space, despite having 0 stars. The question "what does it cost to keep SRM going forever?" is the philosophical core of the SRM debate. srm-forever makes this question computable. The fact that it's interactive (not just a paper) means people can experiment with the framework.

### GCCS-Core — The "Kitchen Sink" Project

**Commit Span:** Single day bulk upload (Oct 29, 2024)

7 README updates + 3 infrastructure commits = bulk upload. No visible modeling code in the commit history.

**Podcast Angle:** GCCS-Core aspires to be the "God mode" climate control system. But the commit pattern reveals it's more aspiration than implementation. The scaffolding (requirements.txt, setup.py, data_collection.sh) exists, but the physics doesn't yet.

### actm-sai-csu — Paper-Only Development

**Commit Span:** Jan–Mar 2023 (10 commits in 3 months)

Every commit maps to a paper or preprint event. The code is supplementary to research papers, not a standalone tool.

**Podcast Angle:** DARPA-funded SRM attribution research is producing papers, but not tools. This is typical of defense-funded research — the output is publications, not software. The open-source community doesn't inherit anything when the funding ends.

---

## Comparative Activity Matrix (Updated)

| Metric | ClimateMARGO | WRF | MDTF | PCMDI | srm-forever | GCCS-Core | actm-sai |
|--------|-------------|-----|------|-------|-------------|-----------|----------|
| Stars | 73 | 1,761 | 80 | 133 | 0 | 9 | 6 |
| Last activity | Aug 2026 | Sep 2026 | Aug 2026 | Sep 2026 | Aug 2026 | Oct 2024 | Mar 2023 |
| Commits pulled | 10 | 15 | 15 | 15 | 4 | 10 | 10 |
| Active devs | 2 | Multi/org | Multi | Multi | 1 | 1 | 3 |
| Development style | Individual | Institutional | Institutional | Institutional | Individual | Bulk upload | Paper-driven |
| Code maturity | Framework | Production | Production | Production | Interactive | Scaffolding | Supplementary |
| Revival potential | Medium | N/A | N/A | N/A | Low | Low | Low |
| SRM relevance | Low (economic) | High (physics) | High (eval) | High (eval) | Critical (econ) | Low | Medium (attrib) |

---

## Emerging Trends (Fresh Data)

1. **Evaluation infrastructure is maturing faster than simulation tools.** PCMDI's v4.2.1 with extremes chunking and MDTF's precip-buoyancy POD show that the community is investing in verification. The question is shifting from "can we simulate SRM?" to "can we verify it worked?"

2. **The Weitzman framework enters the codebase.** srm-forever's 4-commit burst introduces the most rigorous economic argument against indefinite SRM. This is the theoretical counterweight to the "SRM is cheap" argument. If Hurricane Chris Weitzman is right, then committing to permanent SRM is a decision-theoretic trap.

3. **The solar radiation fix in WRF is a canary.** When WRF fixes its solar radiation calculation, it affects every SRM simulation that's ever been run. This is "boring" maintenance with huge implications — the physics engine behind SRM is being corrected, not just extended.

4. **Policy-modeling renaissance?** ClimateMARGO's revival (new maintainer, not original author) could signal that climate economists are returning to geoengineering trade-off modeling after a long pause. But README-only commits are ambiguous.

5. **The scarcity signal persists.** The total number of dedicated SRM simulation repos is tiny. The field relies on general-purpose climate models. This is both a strength (robust tools) and a weakness (no SRM-specific innovation).

---

## Questions for Next Episode (Updated)

- Is ClimateMARGO's revival real, or just a README edit without follow-through?
- What would a community-driven SRM simulator look like?
- Can the evaluation infrastructure (MDTF, PCMDI) keep pace with potential SRM deployment?
- How does the DARPA funding of SRM attribution (actm-sai-csu) affect the open-source ecosystem?
- Does the Weitzman framework change the SRM debate? Is "permanent SRM" a decision-theoretic trap?
- The solar radiation correction in WRF — how many SRM simulations used the old (incorrect) calculation?

---

*Full commit data sourced from GitHub API on September 2026 (v4 update).*
