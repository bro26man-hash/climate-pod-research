# ☀️ Solar Geoengineering — Commit Trend Analysis

**Last updated:** September 2026
**Data source:** GitHub List Commits API, 4 repos, 40+ commits analyzed

---

## Velocity Pages

### 🔴 Fast Universe (Institutional)
**PCMDI/pcmdi_metrics** — 133★

- **10 commits in 14 days** (Sep 3–17, 2026)
- Pattern: PR-driven, version-bump cadence (v4.2.1 released Sep 4)
- Contributors: 2 active (Jiwoo Lee, James Goodnight)
- Signal: **Continuous integration with quarterly release cycle**
- Episode note: PCMDI's velocity suggests SRM evaluation is treated as production software, not a research afterthought

### 🟡 Slow Universe (Academic Burst)
**Sustainable-Solutions-Lab/regional-geo** — 0★

- **10 commits in 3 days** (Feb 13–15, 2026) — then 7+ months dormant
- Pattern: Single-author analysis sprint, tied to paper preparation
- Contributor: Ken Caldeira (sole author)
- Signal: **Code ships with the paper; maintenance ends**
- Episode note: This is the typical lifecycle of geoengineering simulation code — born to publish, not to maintain

**eabarnes1010/actm-sai-csu** — 6★

- **10 commits in 3 months** (Jan–Mar 2023) — then 3+ years dormant
- Pattern: Paper-driven, multi-author relay (Mamalakis → Hueholt → Labe)
- Signal: **Each author adds code supporting their own publication**
- Episode note: DARPA-funded, but code is a means to papers, not a platform

### ⚫ Empty Universe (Governance Frontier)
**Zereo0317/climate-intervention-governance** — 0★

- **2 commits in 1 day** (Aug 23, 2026)
- Pattern: Initial release, then stabilization
- Signal: **Brand new; governance-as-software is an emerging idea**
- Episode note: The first governance-tracking repo for SRM — is this the beginning of a new category?

---

## Modeling vs. Detection Split

A critical pattern emerges in solar geoengineering code:

| Category | Repos | Pattern | Governance Implication |
|----------|-------|---------|----------------------|
| **Simulation** (modeling SRM effects) | regional-geo | Low-star, single-author, burst lifecycle | Who maintains the models that predict SRM outcomes? |
| **Detection** (attributing SRM deployments) | actm-sai-csu | Paper-driven, intelligence-funded, dormant after publication | If SRM is deployed, will the detection tools be ready? |
| **Evaluation** (quantifying model skill) | PCMDI/pcmdi_metrics | Institutional, fast, continuous | PCMDI defines what counts as "good" SRM modeling |
| **Governance** (tracking SRM policy) | climate-intervention-governance | Newborn, 2 commits | Governance code doesn't exist yet at scale |

---

## Episode 1 Architecture

### Opening question
*Why is solar geoengineering code inside climate models, not in SRM-specific repos?*

### Three act structure
1. **Act 1 — The Simulation Gap:** regional-geo shows that SRM code is niche, low-visibility, and tied to publication cycles. Ken Caldeira's WRF-Chem analysis is brilliant but has 0 stars and no community.
2. **Act 2 — The Evaluation Monopoly:** PCMDI has 133 stars and institutional momentum. If PCMDI defines how SRM is evaluated, that's a governance leverage point most people don't know exists.
3. **Act 3 — The Detection Problem:** actm-sai-csu (DARPA-funded) asks: if someone deploys SRM, how would you know? The code is dormant after its papers. The governance repo (Zereo0317) is brand new.

### Closing question
*If the models are in the hands of a few institutions, the detection tools are paper-dependent, and governance code barely exists — who's actually steering solar geoengineering research?*

---

## Trend Lines (watch for these in future episodes)

1. **PCMDI release cadence** — if v4.2.x becomes a quarterly rhythm, SRM evaluation is maturing into infrastructure
2. **regional-geo data pipeline** — the data_loader module could become a communityStandard if someone adopts it
3. **actm-sai-csu DARPA renewal** — new funding could trigger a new commit burst and updated detection methods
4. **climate-intervention-governance growth** — whether it stays at 2 commits or becomes a real governance-as-code platform
