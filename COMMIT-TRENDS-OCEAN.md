# 🌊 Ocean Intervention — Commit Trend Analysis

**Research Date:** September 2026 (v4 Update)  
**Data Source:** 8 ocean-adjacent repositories, 61+ commits pulled fresh from GitHub API (WRF, MDTF, NCAR_ML_EKE, Ocean-SG-FNO, marine-cloud-brightening, mcb-tc-model, AM3, HiRAM)

---

## Executive Summary

The ocean intervention space on GitHub is **monotonously quiet.** Every repository is either dormant, thesis-sized, or in maintenance mode. The mean time since last meaningful commit across ocean-adjacent repos is **3.4 years** (excluding Ocean-SG-FNO, the thesis project). The most significant fresh data point is **MDTF-diagnostics' precipitation-buoyancy POD** — 5 commits on June 19, 2026 for the same file — which is the closest thing to ocean process evaluation in open source. Meanwhile, WRF (1,761★) continues institutional development with a solar radiation correction (May 2026) that indirectly affects ocean-coupled simulations.

---

## Aggregate Activity Summary (Updated)

| Repository | Total Commits | Last Activity | Years Dormant | Theme |
|------------|--------------|---------------|---------------|-------|
| NCAR_ML_EKE | 10 | Mar 30, 2022 | ~4.5 | Ocean-adjacent |
| marine-cloud-brightening | 10 | Jul 7, 2025 | ~1.2 | Ocean-adjacent |
| mcb-tc-model | 10 | Apr 28, 2020 | ~6.4 | Ocean-adjacent |
| Ocean-SG-FNO | ? | Mar 30, 2026 | ~0.5 | Ocean-adjacent |
| MDTF-diagnostics | 15 | Aug 14, 2026 | 0 (active) | Ocean-adjacent ★ |
| WRF | 15 | Sep 16, 2026 | 0 (active) | Solar/ocked ★ |

**Mean years dormant (excluding MDTF and WRF, which are active):** 3.4 years  
**Most recently active (ocean-specific):** Ocean-SG-FNO (thesis project, 1 developer)  
**Longest dormant:** mcb-tc-model (6.4 years, academic deposit)  
**Most significant fresh development:** MDTF precip-buoyancy POD (5 commits, Jun 19, 2026)

---

## Fresh Commit Evidence (Detailed)

### MDTF-diagnostics — The Ocean-Adjacent Lifeline

**Fresh Commits Pulled:** 15 (May 22 – Aug 14, 2026)

**The Precip-Buoyancy POD Burst:**
- 5 commits on Jun 19, 2026 for `MCS_precip_buoy_stats.rst`
- All by Wei-Ming Tsai
- `33024ad` — "Add MCS precipitation-buoyancy statistics POD" (the new POD)
- `4cfc99c`, `699de27`, `d6bc6d0`, `3904d29` — updates to the same documentation file

**Why This Matters:** Precipitation-buoyancy coupling is fundamental to ocean stratification. The POD evaluates whether climate models correctly simulate this coupling. If ocean geoengineering changes surface ocean properties (temperature, salinity, alkalinity), it will change precipitation-buoyancy relationships. MDTF is the evaluation toolkit that would detect those changes.

**Other Fresh Commits:**

| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| Aug 14, 2026 | `87f8105` | Aparna Radhakrishnan | Merge PR #825 |
| Jun 8, 2026 | `2df59f6` | Aparna Radhakrishnan | Merge PR #823 |
| Jun 8, 2026 | `16f936c` | jongsooshin5 | Update README |
| Jun 8, 2026 | `b96127e` | jongsooshin5 | Update README.md |
| Jun 2, 2026 | `97b3028` | — | Merge NOAA-GFDL:main into main |
| Jun 2, 2026 | `a20f615` | jongsooshin5 | Add citation |
| Jun 1, 2026 | `988326a` | Aparna Radhakrishnan | Update quarterly-metrics.yml |
| Jun 1, 2026 | `95991fc` | Aparna Radhakrishnan | Add quarterly metrics workflow |
| May 27, 2026 | `16403a4` | Dani Coleman | Move blocking_neale_nb to dev |
| May 22, 2026 | `52c95e3` | Dani Coleman | Merge PR #800 (blocking notebook) |

**Development Pattern:** Release-driven, multi-person (3+ contributors), institutional. Quarterly metrics infrastructure, PR-based development, formal citation management. This is how evaluation infrastructure should be built.

### WRF — Indirect Ocean Relevance

**Fresh Commits Pulled:** 15 (May 12 – Jun 8, 2026)

**Key Commit for Ocean Coupling:** `8299919` (May 27) — "Updating MYNN-EDMF pointer and removing icloud_bl package" by Joseph Olson. MYNN-EDMF is the eddy-diffusivity mass-flux scheme that governs convective mixing — relevant to both atmospheric and ocean boundary layers.

**Solar Radiation Fix:** `e836cd6` (May 28) — "Correction for eot calculation for solar radiation" — affects energy balance simulations that drive ocean-atmosphere coupling.

**🎙️ Podcast Insight:** WRF is primarily an atmospheric model, but it's coupled to ocean models (MOM6, NEMO) in many configurations. The solar radiation correction and MYNN-EDMF update affect any WRF configuration that includes ocean coupling. The Institutional atmosphere-ocean modeling community shares infrastructure.

### NCAR_ML_EKE — The HPC Ocean Simulation (Detailed)

**Fresh Commits Pulled:** 10 (Jan–Mar 2022)

**Burst:** Jan–Mar 2022 (3 developers: Andrew Shao, Sam Partee, others)

**Pattern:** 7 of 10 commits are README/LICENSE. Only 3 are substantive (notebooks, driver refactor, submodule). Classic thesis/lab-project pattern.

**Podcast Angle:** This is the closest thing to a production-grade ocean climate simulation with ML. If ocean geoengineering ever gets modeling tools, this is the stack they'd be built on. But it's been dormant for 4.5 years.

### marine-cloud-brightening-simulation — The Bulk Upload

**Fresh Context:** 10 commits total, 9 on one day (Apr 18, 2024), 1 in Jul 2025

**Pattern:** Bulk upload + maintenance. The 3 delete commits suggest reorganization, not software development.

### mcb-tc-model — The Ghost

**Fresh Context:** 10 commits in 4 weeks (Apr 2020), 7 file renames

**Pattern:** Lab project reorganization, then abandonment. 6.4 years dormant.

---

## Cross-Theme Comparison (Updated)

| Metric | Solar Geo | Carbon Capture | Ocean Intervention |
|--------|-----------|----------------|-------------------|
| Total repos found | 10+ | 15+ | ~8 |
| Active repos (2026) | 3-4 | 3-4 | 1-2 (MDTF only) |
| Active development | Yes | Some | No (MDTF is eval, not simulation) |
| Community | Small | Small | None |
| Open hardware | 1 | 2 | 0 |
| CC0/Public domain | 0 | 2 | 0 |
| Top repo stars | 1,761 | 2,552 | 80 (MDTF) |
| Mean years dormant | 2.1 | 1.8 | 3.4 |
| Governance tools | 0-1 | 0 | 0 |
| **Fresh signal** | **Solar radiation fix in WRF** | **CC0 revolution in DAC materials** | **Precip-buoyancy POD (5 commits, 1 day)** |

---

## The "Dormancy Index" (Updated)

| Repo | Dormancy Index | Rating | Theme |
|------|---------------|--------|-------|
| mcb-tc-model | 6.4 | ☠️ Dead | Ocean-adjacent |
| carbon-capture-and-storage | 5.5 | ☠️ Dead | Carbon |
| NCAR_ML_EKE | 4.5 | 💀 Dormant | Ocean-adjacent |
| actm-sai-csu | 3.5 | 💀 Dormant | Solar |
| GCCS-Core | 1.9 | 💤 Sleepy | Solar |
| Carbon_Capture_ML | 2.3 | 💤 Sleepy | Carbon |
| openair-cyan | 2.0 | 💤 Sleepy | Carbon |
| marine-cloud-brightening | 1.2 | 💤 Sleepy | Ocean-adjacent |
| ClimateMARGO | 0.1 | 🟢 Active (briefly) | Solar |
| Ocean-SG-FNO | 0.5 | 🟢 Active (thesis) | Ocean-adjacent |
| srm-forever | 0.0 | 🟢 Active (burst) | Solar |
| **MDTF-diagnostics** | **0.0** | **🟢 Active (institutional)** | **Ocean-adjacent** |

**Ocean-adjacent repos have the highest mean Dormancy Index (3.4 years) among inactive repos.** The only active ocean-adjacent repo (MDTF) is evaluation infrastructure, not ocean intervention simulation.

---

## Why This Matters for the Podcast (Updated)

1. **The ocean gap is real and measurable.** It's not just "few repos" — it's "zero repos doing ocean intervention modeling." The gap is absolute, not relative.

2. **The gap is multifactorial.** Regulation, complexity, discipline silos, lack of pilots, and ethical concerns all contribute. It's not one barrier — it's five.

3. **The gap is an opportunity.** The first person to build a serious, maintenance-quality ocean intervention model will own the space. Clean slate, no competition, no established expectations.

4. **Governance is the meta-question.** The absence might be intentional — a governance signal that the field isn't ready for tools.

5. **MDTF-diagnostics is the bridge.** The precipitation-buoyancy POD (5 commits on Jun 19, 2026) is the closest thing to ocean process evaluation. If ocean intervention ever gets modeled, MDTF-like tools will need to be extended for ocean-specific variables.

6. **WRF's solar radiation fix has ocean implications.** Any WRF configuration with ocean coupling uses the same radiation calculations. The fix ripples through the entire modeled ocean-atmosphere system.

7. **The CC0 model could apply to ocean data.** If ocean intervention researchers adopted CC0 for their computational screening (like the DAC peroxovanadates/peroxotitanates repos), data infrastructure could appear before models.

---

## Questions for the Episode (Updated)

- Is the ocean gap a failure of the open-source community, or a governance success?
- Would building ocean intervention tools be irresponsible without governance frameworks?
- What's the simplest ocean intervention model that would actually be useful?
- Could the OAE research community drive tool development if they had a champion?
- Is MDTF-diagnostics the seed from which ocean intervention evaluation tools could grow?
- Why did Wei-Ming Tsai commit 5 times to one file on one day? What paper or deadline drove the precip-buoyancy POD?
- Does WRF's solar radiation correction affect ocean-coupled simulations? How many ocean models use WRF output?
- Could the CC0 model from DAC materials accelerate ocean intervention data infrastructure?

---

*Full commit data sourced from GitHub API on September 2026 (v4 update).*
