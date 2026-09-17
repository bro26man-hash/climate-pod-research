# ☀️ Solar Geoengineering — Research Branch

## Theme Overview

Solar Radiation Management (SRM) is the controversial family of climate geoengineering approaches designed to reflect a small fraction of incoming solar radiation back into space, thereby cooling the Earth. This branch catalogs open-source simulation tools, Earth-system model components, and interactive models relevant to SRM research and discourse.

## Key Questions for Episode Planning

- Why is SRM simulation code so scarce on GitHub compared to other climate-tech domains?
- Can interactive, open-source models democratize the SRM discourse beyond a handful of specialized institutions?
- What are the Arctic-specific risks and feedback dynamics that SRM simulations must capture?
- Is CMIP6 ESM evaluation infrastructure (like PCMDI metrics) the governance backbone that the SRM community lacks?

## Top Repositories Discovered

| # | Repository | Stars | Language | Last Updated | Focus |
|---|-----------|-------|----------|-------------|-------|
| 1 | [PCMDI/pcmdi_metrics](https://github.com/PCMDI/pcmdi_metrics) | 133 | Python | Sep 4, 2026 | ESM evaluation toolkit (CMIP6 metrics) |
| 2 | [FMS-ESM/AM3](https://github.com/FMS-ESM/AM3) | 4 | Fortran | Mar 2015 | GFDL atmospheric model (legacy) |
| 3 | [pmip4/pmip_p2fvar_analyzer](https://github.com/pmip4/pmip_p2fvar_analyzer) | 4 | — | Sep 2025 | CMIP6 paleoclimate data analysis |
| 4 | [RhondaMueller/Codes-RFG-Arctic-Impacts](https://github.com/RhondaMueller/Codes-RFG-Arctic-Impacts) | 1 | — | Apr 2024 | SRM radiative forcing on Arctic |
| 5 | [hausfath/srm-forever](https://github.com/hausfath/srm-forever) | 0 | — | Aug 26, 2026 | Interactive single-page SRM economics model |

## Gaps Identified

- **No dedicated SRM simulation frameworks** — No open-source general-circulation model (GCM) or Earth-system model (ESM) designed specifically for SRM scenario simulation exists on GitHub.
- **Legacy Fortran dominates** — The most relevant code (AM3) dates to 2015 and uses Fortran. The Python/data-science revolution has not reached geoengineering-specific simulation.
- **PCMDI metrics as governance infrastructure** — PCMDI's 133-star toolkit is the closest thing to an active, maintained analysis platform, but it evaluates whole ESMs rather than SRM-specific processes.
- **Interactive models are nascent** — The `srm-forever` project is a single-page economics model, not a physical simulation. The gap between "interactive educational tool" and "research-grade simulator" is vast.

## Commit Trend Summary

See [`commit-trends.md`](./commit-trends.md) for detailed analysis.

### Quick Takeaways

1. **Institutional bursts, not sustained community effort** — PCMDI's v4.2.1 release saw 10 commits in 2 days (Sep 3–4, 2026), all by Jiwoo Lee at LLNL with PRs from James Goodnight and Jared Lewis. This is a well-funded institutional pattern, not organic community development.
2. **Dormancy is the norm** — 3 of 4 other SRM-related repos have had no meaningful activity in over a year. AM3 hasn't been touched since 2015.
3. **The August 2026 cluster** — `srm-forever` was updated on Aug 26, 2026, suggesting some renewed interest in interactive SRM modeling, but it's a solo effort.

## Episode Angles

- **The Scarcity Story**: Why does the most controversial climate technology have so little open-source simulation code?
- **The Governance Angle**: PCMDI's metrics toolkit is the unsung infrastructure of climate model evaluation — what does it mean that SRM lacks equivalent infrastructure?
- **The Democratization Question**: Can lightweight interactive models (like srm-forever) bring SRM discourse to a broader audience, or do they oversimplify?
