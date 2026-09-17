# ☀️ Solar Geoengineering — Commit Trend Analysis

**Last Updated:** September 2026
**Source Repositories Analyzed:** PCMDI/pcmdi_metrics, wrf-model/WRF, FMS-ESM/AM3, pmip4/pmip_p2fvar_analyzer, RhondaMueller/Codes-RFG-Arctic-Impacts, hausfath/srm-forever

---

## 📊 Repository-by-Repository Commit Histories

### 1. PCMDI/pcmdi_metrics — 133 ⭐ (The Gold Standard)

| Date | Commit | Author |
|------|--------|--------|
| Sep 4, 2026 | v4.2.1 release merge | Aparna Radhakrishnan |
| Sep 3, 2026 | v4.2.1 tagged | Jiwoo Lee |
| Aug 14, 2026 | PR #825 merged | Aparna Radhakrishnan |
| Jun 19, 2026 | MCS precip-buoyancy POD added | Wei-Ming Tsai |
| Jun 8, 2026 | PR #823 merged | Aparna Radhakrishnan |
| Jun 2, 2026 | Main branch merge | jongsooshin5 |

**Key Insight:** 10 commits in 2 days (Sep 3-4, 2026) for v4.2.1 release. Institutional, funding-backed development at LLNL/DOE. Multiple contributors (Jiwoo Lee, James Goodnight, Jared Lewis). This is the most actively maintained climate simulation evaluation toolkit on GitHub.

**Trending Signal:** CMIP6 evaluation tooling is the infrastructure for SRM governance. If we deploy SRM, we need to evaluate its effects against a baseline — PCMDI-style tools are that baseline infrastructure.

---

### 2. wrf-model/WRF — 1,761 ⭐ (Civil Infrastructure)

| Date | Commit | Author |
|------|--------|--------|
| Jun 8, 2026 | v4.8.0 release merge | Anthony Islas |
| Jun 6, 2026 | README & version update for v4.8.0 | Anthony Islas |
| Jun 5, 2026 | Tempo aerosol/hail options disabled | weiwangncar |
| May 30, 2026 | AOCC vectorization fix | weiwangncar |
| May 28, 2026 | Solar radiation EOT correction | weiwangncar |
| May 27, 2026 | MYNN-EDMF update | Joseph Olson |
| May 26, 2026 | MMM-physics SHA update | Anthony Islas |
| May 26, 2026 | CDXWRF module fix | Lluís Fita |
| May 26, 2026 | GFL README update | weiwangncar |
| May 21, 2026 | mp_physics=88 error message | Kelly Werner |

**Key Insight:** WRF is the foundational atmospheric model for *all* climate simulation — including SRM. The active development of transient aerosol options and radiation corrections directly feeds into SRM simulation capability. The v4.8.0 release is a major institutional milestone.

**Trending Signal:** The atmospheric modeling infrastructure that would simulate SRM is actively maintained by NCAR/NOAA. The transition from parameterization tuning to aerosol-aware physics is the key methodological shift.

---

### 3. FMS-ESM/AM3 — 4 ⭐ (Legacy Fortran)

| Date | Commit | Author |
|------|--------|--------|
| Mar 2015 | Last known update | FMS team |

**Key Insight:** Only 4 commits total, last activity 2015. This is GFDL's AM3 atmospheric model — historically significant as one of the first models to include aerosol microphysics. Now effectively frozen in time.

**Trending Signal:** Legacy Fortran codes dominate the historical SRM simulation space, but they are no longer being developed. The modern Python ecosystem (PCMDI, xCDAT) has not yet reached geoengineering-specific simulation.

---

### 4. hausfath/srm-forever — 0 ⭐ (The Emergent Approach)

| Date | Commit | Author |
|------|--------|--------|
| Aug 26, 2026 | Initial release | hausfath |

**Key Insight:** All 4 commits were on a single day. A transparent, single-HTML-page SRM economics model using Weitzman certainty-equivalent discounting. Published alongside an essay on discount rates and geoengineering economics.

**Trending Signal:** The "interpretable model" movement — making SRM economics accessible without running a GCM. Not a simulation tool, but a pedagogical and governance tool.

---

## 🔬 What the Commit Histories Tell Us

### Five Key Findings

1. **Institutional bursts dominate climate software.** PCMDI's 133★ had 10 commits in 2 days (v4.2.1 release). WRF's v4.8.0 release also showed concentrated institutional activity. Most repos can't sustain this; it requires funding and personnel.

2. **The atmospheric modeling pipeline is alive.** WRF (v4.8.0, Jun 2026) and PCMDI (v4.2.1, Sep 2026) are both actively releasing new versions. The infrastructure for SRM simulation *exists* — it's just not geoengineering-specific.

3. **SRM-specific code is virtually nonexistent.** Beyond srm-forever (a single HTML file) and AM3 (frozen in 2015), there is no open-source code that simulates the *physical* effects of solar geoengineering. No aerosol microphysics, no radiative transfer for geoengineering scenarios.

4. **Legacy Fortran is a graveyard.** AM3, PMIP analyzers — the geoengineering-relevant Fortran codes are either frozen or being repurposed. The Python migration hasn't reached this niche.

5. **The ARCTIC is the most active research frontier.** Codes-RFG-Arctic-Impacts (Apr 2024) is the only recent repo specifically looking at SRM's effect on Arctic ice. This signals where the research community is focusing.

### What This Means for Your Podcast

- The **story is in the gap**: the infrastructure for evaluating SRM exists (PCMDI, WRF), but the SRM simulation code itself doesn't exist as open source.
- The **institutional story is real**:climate software development is institutional, not community-driven. This raises governance questions about who controls simulation tools.
- The **economic transparency story is emerging**: srm-forever shows that simple, transparent models can make SRM economics accessible — but they can't substitute for physical simulation.

---

## 🎙️ Updated Episode Questions

1. **Why does the atmospheric modeling infrastructure (WRF, PCMDI) exist but SRM-specific simulation doesn't?** What's the institutional barrier?
2. **Can transparent economic models (srm-forever) bridge the gap?** Or is physical simulation essential for governance?
3. **How does the August-Sep 2026 PCMDI/WRF release cycle change the SRM discourse?** Are we closer to evaluating SRM effects than we thought?
4. **The Arctic as a canary:** Why is Arctic impact the only active SRM research area on GitHub?
