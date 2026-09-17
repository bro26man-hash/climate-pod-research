# ☀️ Solar Geoengineering — Commit Trend Analysis

**Research Date:** September 2026  
**Data Source:** 6 repositories across solar geoengineering and climate simulation

---

## Executive Summary

The solar geoengineering open-source ecosystem is characterized by **institutional dominance, paper-driven development, and a scarcity of dedicated SRM simulation tools.** The most significant signal in the commit data is the **August 2026 revival of ClimateMARGO**, a 2+ year dormant climate-economic modeling framework, which may indicate growing policy interest. Meanwhile, WRF (1,761 stars) and MDTF-diagnostics (80 stars) show steady institutional maintenance.

---

## Commit Activity Timeline

```
2022 ──► ClimateMARGO: 6 commits (Henri Drake era)
2023 ──► actm-sai-csu: 10 commits (paper/preprint cycle)
2024 ──► GCCS-Core: 10 commits (single-day bulk upload)
2025 ──► GeoVision: sparse updates
2026 ──► ClimateMARGO: 2 commits (README revival) ★ SIGNAL
         WRF: continuous institutional commits
         MDTF-diagnostics: Jun-Aug burst (v4.2.1 release cycle)
```

---

## Detailed Analysis by Project

### ClimateMARGO.jl — The Revival Signal

**Commit Span:** Jan 2022 – Aug 2026 (but with 2.5-year gap)

**Phase 1 (Jan–Feb 2022):** Henri Drake established the project
- Added CITATION.bib, fixed typos, updated docs
- 4 commits in the first month

**Phase 2 (Nov 2022):** Dependency maintenance
- JuMP/Ipopt compat upgrade
- Project.toml update
- 2 commits

**Phase 3 (GAP):** No meaningful activity for 2.5 years

**Phase 4 (Aug 2026):** Fons van der Plas updates README twice
- Two README-only commits on the same day
- No code changes, no issue discussions
- **Interpretation:** Could be a genuine revival, or could be a link/update without deeper engagement. The fact that a new maintainer (different from original) is updating it suggests possible institutional interest.

**Podcast Angle:** Is ClimateMARGO's revival a canary for growing geoengineering policy-modeling interest? Or is it another ghost-update in a sea of dormant climate repos?

### WRF — The Institutional Engine

**Commit Span:** Continuous (1,761 stars)

WRF doesn't show individual commits in our pull — it's maintained by NCAR/NOAA with regular release cycles. v4.8.0 was released June 2026. This is the infrastructure that the entire SRM simulation community depends on.

**Podcast Angle:** WRF is the "Linux of climate simulation" — nobody notices it until it breaks, but everything depends on it. SRM researchers configure WRF with aerosol injection modules. Without institutional funding, there's no WRF, and without WRF, there's no SRM simulation.

### MDTF-diagnostics — The Governance Infrastructure

**Commit Span:** Jun–Aug 2026 (release-driven)

The August 2026 burst of commits accompanies the v4.2.1 release. This is classic institutional release-cycle behavior.

**Podcast Angle:** MDTF-diagnostics is the evaluation toolkit for CMIP6 models. If SRM is ever deployed, we need to be able to detect, attribute, and evaluate its effects. MDTF is the governance infrastructure that makes that possible.

### GCCS-Core — The "Kitchen Sink" Project

**Commit Span:** Oct 29, 2024 (single day)

7 README updates + 3 infrastructure commits = bulk upload. No visible modeling code in the commit history.

**Podcast Angle:** GCCS-Core aspires to be the "God mode" climate control system. But the commit pattern reveals it's more aspiration than implementation. The scaffolding (requirements.txt, setup.py, data_collection.sh) exists, but the physics doesn't yet.

### actm-sai-csu — Paper-Only Development

**Commit Span:** Jan–Mar 2023 (10 commits in 3 months)

Every commit maps to a paper or preprint event. The code is supplementary to research papers, not a standalone tool.

**Podcast Angle:** DARPA-funded SRM attribution research is producing papers, but not tools. This is typical of defense-funded research — the output is publications, not software. The open-source community doesn't inherit anything when the funding ends.

---

## Comparative Activity Matrix

| Metric | ClimateMARGO | WRF | MDTF | GCCS-Core | actm-sai |
|--------|-------------|-----|------|-----------|----------|
| Stars | 73 | 1,761 | 80 | 9 | 6 |
| Last activity | Aug 2026 | Sep 2026 | Aug 2026 | Oct 2024 | Mar 2023 |
| Commits pulled | 10 | — | — | 10 | 10 |
| Active devs | 2 | Multi/org | Multi | 1 | 3 |
| Development style | Individual | Institutional | Institutional | Bulk upload | Paper-driven |
| Code maturity | Framework | Production | Production | Scaffolding | Supplementary |
| Revival potential | Medium | N/A | N/A | Low | Low |

---

## Emerging Trends

1. **Policy-modeling renaissance?** ClimateMARGO's revival could signal that climate economists are returning to geoengineering trade-off modeling after a long pause.

2. **The evaluation bottleneck** — MDTF-diagnostics' activity shows that the community is investing in evaluation infrastructure, not just simulation. This is a governance-first approach.

3. **Paper-only tools** — actm-sai-csu exemplifies a pattern where DARPA-funded research produces papers but no maintainable software. When funding ends, the code dies.

4. **The scarcity signal** — The total number of dedicated SRM simulation repos is tiny. The field relies on general-purpose climate models. This is both a strength (robust tools) and a weakness (no SRM-specific innovation).

---

## Questions for Next Episode

- Is ClimateMARGO's revival real, or just a README edit without follow-through?
- What would a community-driven SRM simulator look like?
- Can the governance infrastructure (MDTF, CMIP evaluation) keep pace with potential SRM deployment?
- How does the DARPA funding of SRM attribution (actm-sai-csu) affect the open-source ecosystem?

---

*Full commit data sourced from GitHub API on September 2026.*