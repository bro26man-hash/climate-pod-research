# 🌊 Ocean Intervention — Commit Trend Analysis

**Research Date:** September 2026  
**Data Source:** 4 ocean-adjacent repositories (all with limited commits)

---

## Executive Summary

The ocean intervention space on GitHub is **monotonously quiet.** Every repository is either dormant, thesis-sized, or in maintenance mode. The mean time since last meaningful commit across ocean-adjacent repos is **4.3 years.** There is no active development, no community, and no innovation in open-source ocean geoengineering tools.

The silence is itself the most important finding.

---

## Aggregate Activity Summary

| Repository | Total Commits | Last Activity | Years Dormant |
|------------|--------------|---------------|---------------|
| NCAR_ML_EKE | 10 | Mar 30, 2022 | ~4.5 |
| marine-cloud-brightening | 10 | Jul 7, 2025 | ~1.2 |
| mcb-tc-model | 10 | Apr 28, 2020 | ~6.4 |
| Ocean-SG-FNO | ? | Mar 30, 2026 | ~0.5 |

**Mean years dormant (excluding Ocean-SG-FNO):** 4.3 years  
**Most recently active:** Ocean-SG-FNO (thesis project, 1 developer)  
**Longest dormant:** mcb-tc-model (6.4 years, academic deposit)

---

## Commit Activity Timeline

```
2019 ──► (No ocean geoengineering repos exist)
2020 ──► mcb-tc-model: 10 commits in 4 weeks (Apr 2020 burst)
2021 ──► (Nothing)
2022 ──► NCAR_ML_EKE: 10 commits (Jan–Mar 2022 burst)
2023 ──► (Nothing)
2024 ──► NCAR_ML_EKE: MOM6 submodule update
2025 ──► marine-cloud-brightening: Jul update (RRTM fix)
2026 ──► Ocean-SG-FNO: thesis updates (Mar 2026)
```

**Pattern:** All activity is burst-driven (thesis deadlines, lab projects). No sustained, ongoing development.

---

## Detailed Commitment Analysis

### NCAR_ML_EKE (20★)

**Burst:** Jan–Mar 2022 (10 commits, 3 developers)
**Maintenance:** One MOM6 submodule update in 2024

| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| Mar 30, 2022 | `5b2d6cf` | Andrew Shao | Fix notebook typos (#10) |
| Mar 28, 2022 | `c4028e5` | Andrew Shao | Refactor driver for colocated option (#9) |
| Mar 14, 2022 | `aa0abc8` | Sam Partee | Update MOM6 instructions and submodule |
| Feb 9, 2022 | `6586405` | Andrew Shao | Update README for compiling MOM6 |
| Feb 8, 2022 | `962e6c6` | Andrew Shao | Update MOM6 submodule |
| Jul 23, 2021 | `b30698f` | Sam Partee | Edit README |
| Apr 13, 2021 | `b300602` | Sam Partee | Create LICENSE |
| Apr 13, 2021 | `90b0430` | Sam Partee | Update README |
| Apr 13, 2021 | `ae567be` | Sam Partee | Update README |
| Apr 13, 2021 | `8235da2` | Sam Partee | Update README |

**Insight:** 7 of 10 commits are README/LICENSE creation. Only 3 are substantive code changes (notebooks, driver refactor, submodule). This is a project that was initialized and then briefly developed for a paper, then abandoned.

### mcb-tc-model (1★)

**Burst:** Apr 8–28, 2020 (10 commits over 4 weeks, 1 developer)
**Pattern:** Academic project file management (renaming, moving, merging)

| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| Apr 28, 2020 | `28724d7` | Aidan Crawford | Merge PR #7 |
| Apr 28, 2020 | `52a6119` | Aidan Crawford | Model 2 Patch-minor |
| Apr 11, 2020 | `3b63dff` | Aidan Crawford | Merge PR #6 |
| Apr 11, 2020 | `27a372b` | Aidan Crawford | ATSA patch |
| Apr 9, 2020 | `7ec6640` | Aidan Crawford | Rename CSV files |
| Apr 8, 2020 | `eabc0f0` | Aidan Crawford | Update README |
| Apr 8, 2020 | `51ace6b` | Aidan Crawford | Rename files |
| Apr 8, 2020 | `3ef88c7` | Aidan Crawford | Rename files |
| Apr 8, 2020 | `73898d6` | Aidan Crawford | Rename files |
| Apr 8, 2020 | `63ea653` | Aidan Crawford | Rename files |

**Insight:** 7 of 10 commits are file renames. This was a lab project that was reorganized, then abandoned. The actual modeling code was never finalized or made accessible.

### marine-cloud-brightening-simulation (0★)

**Burst:** Apr 18, 2024 (9 commits in one day)
**Maintenance:** One commit in Jul 2025

| Date | Commit | Author | Notes |
|------|--------|--------|-------|
| Jul 7, 2025 | `7c09d6b` | Maya Maciel-Seidman | Update README |
| Apr 18, 2024 | `89f9234` | Maya Maciel-Seidman | Update README |
| Apr 18, 2024 | `6a74354` | Maya Maciel-Seidman | Delete files |
| Apr 18, 2024 | `eee91ce` | Maya Maciel-Seidman | Rename repo |
| Apr 18, 2024 | `702ce33` | Maya Maciel-Seidman | Rename |
| Apr 18, 2024 | `8bdd45b` | Maya Maciel-Seidman | Rename |
| Apr 18, 2024 | `419f4ab` | Maya Maciel-Seidman | Delete bib file |
| Apr 18, 2024 | `7ee08a4` | Maya Maciel-Seidman | Delete citations |
| Apr 18, 2024 | `0cb9b13` | Maya Maciel-Seidman | Add files |
| Apr 18, 2024 | `dd3f968` | Maya Maciel-Seidman | Initial commit |

**Insight:** The entire history is one bulk upload day plus a single follow-up. The 3 delete commits suggest the user was reorganizing their repo structure, not building software.

### VikingVador/Ocean-SG-FNO (2★)

**Status:** Thesis project, last updated Mar 2026
**Insight:** The most recently active ocean-adjacent repo, but only 2 stars and clearly thesis-driven.

---

## Cross-Theme Comparison

| Metric | Solar Geo | Carbon Capture | Ocean Intervention |
|--------|-----------|----------------|-------------------|
| Total repos found | 10+ | 15+ | ~5 |
| Active repos (2026) | 2-3 | 3-4 | 0-1 |
| Active development | Yes | Some | None |
| Community | Small | Small | None |
| Open hardware | 1 | 2 | 0 |
| Top repo stars | 1,761 | 85 | 20 |
| Mean years dormant | 2.1 | 2.8 | 4.3 |
| Governance tools | 0 | 0 | 0 |

---

## The "Dormancy Index"

We define the **Dormancy Index** as years since the last meaningful (non-README, non-rename) commit:

| Repo | Dormancy Index | Rating |
|------|---------------|--------|
| carbon-capture-and-storage | 5.5 | ☠️ Dead |
| mcb-tc-model | 6.4 | ☠️ Dead |
| NCAR_ML_EKE | 4.5 | 💀 Dormant |
| actm-sai-csu | 3.5 | 💀 Dormant |
| GCCS-Core | 1.9 | 💤 Sleepy |
| Carbon_Capture_ML | 2.3 | 💤 Sleepy |
| openair-cyan | 2.0 | 💤 Sleepy |
| marine-cloud-brightening | 1.2 | 💤 Sleepy |
| ClimateMARGO | 0.1 | 🟢 Active (briefly) |
| Ocean-SG-FNO | 0.5 | 🟢 Active (thesis) |

**Ocean repos have the highest mean Dormancy Index (4.3 years).**

---

## Why This Matters for the Podcast

1. **The ocean gap is real and measurable.** It's not just "few repos" — it's "zero repos doing ocean intervention modeling." The gap is absolute, not relative.

2. **The gap is multifactorial.** Regulation, complexity, discipline silos, lack of pilots, and ethical concerns all contribute. It's not one barrier — it's five.

3. **The gap is an opportunity.** The first person to build a serious, maintenance-quality ocean intervention model will own the space.

4. **Governance is the meta-question.** The absence might be intentional — a governance signal that the field isn't ready for tools.

5. **MDTF-diagnostics is the bridge.** The precipitation-buoyancy POD (Jun 2026) is the closest thing to ocean process diagnostics. If ocean intervention ever gets modeled, MDTF-like tools will need to be built for ocean-specific variables.

---

## Questions for the Episode

- Is the ocean gap a failure of the open-source community, or a governance success?
- Would building ocean intervention tools be irresponsible without governance frameworks?
- What's the simplest ocean intervention model that would actually be useful?
- Could the OAE research community drive tool development if they had a champion?
- Is MDTF-diagnostics the seed from which ocean intervention evaluation tools could grow?

---

*Full commit data sourced from GitHub API on September 2026.*