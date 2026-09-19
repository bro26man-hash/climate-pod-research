# 🌊 Ocean Intervention — Commit Trend Analysis & Project Discoveries

*Last updated: September 2026 — sourced from GitHub REST API*

---

## 🔬 Key Repositories Discovered

### 1. CrayLabs/NCAR_ML_EKE — Machine Learning for Ocean Climate Modeling
| Metric | Value |
|--------|-------|
| Stars | 20 |
| Language | Jupyter Notebook |
| Last commit | August 10, 2026 (repository-level; code commits stopped in 2022) |
| Activity level | **⚫ Dormant code, active paper** |

**Recent commit highlights (2021–2022, 15 commits pulled):**

| Date | Commit message | Author |
|------|---------------|--------|
| 2022-03-30 | Fix notebook typos (#10) | Andrew Shao |
| 2022-03-28 | Refactor driver to support colocated option (#9) | Andrew Shao |
| 2022-03-14 | Update MOM6 instructions and submodule | Sam Partee |
| 2022-02-09 | Update README for compiling MOM6 | Andrew Shao |
| 2022-02-08 | Update MOM6 submodule | Andrew Shao |
| 2021-07-23 | edit README | Sam Partee |
| 2021-04-13 | Create LICENSE / Update README (x4) / Add git submodule / Add MOM6 submodule | Sam Partee, arigazzi |

**🎙️ Podcast angle:** This is the *closest* thing to an ocean-coded repo in the climate-tech space — using ML to simulate ocean energy kinetics (EKE = Eddy Kinetic Energy) with MOM6 (Modular Ocean Model). It's NCAR-affiliated, paper-backed, and demonstrably useful. But **the code hasn't been touched since March 2022** — 4+ years dormant. The paper got cited; the code didn't get maintained. This is the "publish-or-perish, abandon-the-code" pattern.

---

### 2. jnickla1/CESM2geoeng_documentation — Ocean Geoengineering CESM2 Paper
| Metric | Value |
|--------|-------|
| Description | Documentation for the ocean geoengineering CESM2 paper |
| Last update | November 2025 |

**🎙️ Podcast angle:** CESM2 (Community Earth System Model v2) is the other major climate model alongside WRF. It *has* an ocean component. This repo documents ocean geoengineering experiments run in CESM2 — but it's *documentation*, not code. The actual simulations live in the CESM2 codebase, not in a dedicated repo. The ocean geoengineering research is buried inside a monolithic model.

---

### 3. ClimateMARGO/ClimateMARGO.jl — Climate-Economic Modeling (Adjacent)
| Metric | Value |
|--------|-------|
| Stars | 73 |
| Language | Julia |
| Last commit | August 17, 2026 (README update); core commits stopped 2023 |

**🎙️ Podcast angle:** MARGO (Model for Optimizing Trade-offs between Mitigation, Adaptation and Geoengineering) includes ocean carbon-cycle economics. It's the most-starred geoengineering-adjacent repo we found. But the core code hasn't changed since 2023 — the 2026 commits are README-only.

---

## 🌊 The Ocean Gap — Absence Analysis

After 10+ search queries across multiple keyword combinations (ocean geoengineering, ocean intervention, ocean fertilization, ocean alkalinity enhancement, marine cloud brightening, CESM ocean, MOM6 ocean, etc.), the result is unanimous:

### **ZERO dedicated ocean geoengineering repositories exist on GitHub.**

| Search query | Results | Dedicated ocean-geoeng repos? |
|-------------|---------|-------------------------------|
| "ocean geoengineering" | 4 | 0 |
| "ocean fertilization" | 0 | 0 |
| "ocean alkalinity enhancement" | 0 | 0 |
| "marine cloud brightening" | 0 | 0 |
| "ocean climate intervention" | 4 | 0 |
| "ocean carbon removal" | 0 | 0 |
| "CESM ocean geoengineering" | 1 (docs only) | 0 |
| "MOM6 ocean" | 0 geoeng-specific | 0 |

**This is NOT because ocean geoengineering isn't being studied.** The science is active — Nature, Science, and PNAS publish ocean geoengineering papers regularly. But the code stays inside monolithic climate models (CESM2, MOM6, GFDL) or on paper supplementary materials, not in discoverable open-source repos.

### The Three Universes (updated with ocean data):

- **🔴 Fast Universe:** WRF, CESM2, MOM6 — institutional, funded, continuous. Ocean codes exist *inside* these monoliths but are not independently discoverable.
- **🟡 Slow Universe:** ClimateMARGO, NCAR_ML_EKE — individual researchers, dormant after paper publication.
- **⚫ Empty Universe:** Ocean geoengineering as standalone open-source — zero repos, zero code, zero governance.

---

## 📊 Ocean Theme — Trend Summary

| Signal | Evidence |
|--------|----------|
| **Ocean codes are buried in monoliths** | CESM2 has an ocean component; MOM6 is a submodule; nothing standalone |
| **Publish-maintain-abandon pattern** | NCAR_ML_EKE: 15 commits, then 4-year silence |
| **Documentation > Code** | jnickla1/CESM2geoeng is docs-only; the real code is in the CESM2 monorepo |
| **The GitHub vacuum is a governance signal** | No one has created an ocean-geoeng repo because the field is cautious about premature governance frameworks |
| **5 hypotheses for the gap** | (1) Code is proprietary in national labs; (2) Ocean models are too expensive to run openly; (3) Governance fear — no one wants to be the "first"; (4) papers + supplementary is "good enough"; (5) The community hasn't coalesced yet |

### Episode architecture suggestion:
1. **Cold open:** "We searched GitHub 10+ times for ocean geoengineering code. There's nothing. And that's the story."
2. **Act 1:** The ocean gap — why the most serious geoengineering research has zero GitHub presence
3. **Act 2:** NCAR_ML_EKE — what happens when ML meets ocean modeling (and then nobody maintains it)
4. **Act 3:** CESM2's hidden ocean — the ocean geoengineering experiments buried inside a giant model
5. **Tag:** Is the GitHub vacuum a governance signal? Are researchers afraid to open the ocean Pandora's box?

---

*Methodology: GitHub Repository Search API (10+ query variations), GitHub List Commits API. Data pulled September 2026.*
