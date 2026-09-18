# 🎙️ Climate Pod Research — v9 Cross-Theme Update (September 2026)

> **Repository:** `bro26man-hash/climate-pod-research`
> **Update version:** v9 — Fresh GitHub API commit pulls
> **Date:** September 2026

---

## What's New in v9

We pulled fresh commit histories from **8 repositories** across all three themes using the GitHub API, then produced detailed per-theme commit trend analyses. Here's what we found:

### By the Numbers

| Theme | Repos Pulled | Total Commits | Key Finding |
|-------|-------------|----------------|-------------|
| ☀️ Solar | 5 (WRF, PCMDI, MDTF, ClimateMARGO, srm-forever) | 39 | Solar radiation bug fix + aerosol physics shutdown in WRF |
| 🌍 Carbon | 6 (OpenCarbon, CO2-Sequestration, openair-cyan, Carbon_Capture_ML, DAC_peroxovanadates, DAC_peroxotitanates) | 38 | OSHWA blitz day + CC0 revolution + 32-star ghost |
| 🌊 Ocean | 3 (MDTF-adjacent, WRF-adjacent, ClimateSoton) | 23 | **15 searches, zero ocean geoengineering repos** |

---

## Top 5 Commit Signals (Sep 2026)

### 1. The WRF Solar Radiation Fix (May 28, 2026)
**Commit:** `e836cd6` in `wrf-model/WRF`
**Message:** "Correction for eot calculation for solar radiation"
**Impact:** If you published an SRM simulation using WRF before May 28, 2026, your energy balance might be systematically off. This is the most SRM-critical commit in the entire dataset.

### 2. The PCMDI Roundoff Bug (Sep 4, 2026)
**Commit:** `90cbc50` in `PCMDI/pcmdi_metrics`
**Message:** "Prevents roundoff to 1.00 in mean_climate figures"
**Impact:** Climate models could score "perfect" (1.00) on evaluation metrics by rounding error. James Goodnight's fix means model-observation comparisons are now more honest.

### 3. The OSHWA Certification Blitz (Feb 12, 2024)
**Commits:** 6 in one day in `openair-collective/openair-cyan`
**Impact:** A DIY direct air capture device received official open-source hardware certification (OSHWA UID US001095). The finish line was a second starting gun.

### 4. The PBP-POD Launch (Jun 19, 2026)
**Commit:** `33024ad` in `NOAA-GFDL/MDTF-diagnostics`
**Message:** "add MCS precip-buoyancy statistics POD" + 4 documentation revisions
**Impact:** The most ocean-relevant diagnostic in open source was born in a single day. Four rounds of documentation on the same file — science building trust in code.

### 5. The srm-forever Theory Bundle (Aug 26, 2026)
**Commits:** 4 in one day in `hausfath/srm-forever`
**Impact:** Weitzman certainty-equivalent discounting applied to SRM cost dynamics. Zero stars. Maximum conceptual density. The most important repo nobody's using.

---

## The Three Universes (Updated)

| Universe | Character | GitHub Presence | What They Tell Us |
|----------|-----------|------------------|-------------------|
| **Fast** | Institutions (WRF, PCMDI, MDTF) | Heavy, continuous, funded | "Climate science is a team sport" |
| **Slow** | Individuals (ClimateMARGO, srm-forever, OpenAir-Cyan) | Dormant, symbolic, unfunded | "Individuals keep hope alive" |
| **Empty** | Ocean geoengineering | **Zero repos** | "We haven't even started" |

---

## Repository Structure

| Branch | File | Description |
|--------|------|-------------|
| `main` | `COMMIT-TRENDS.md` | Master consolidated analysis |
| `main` | `CROSS-THEME-ANALYSIS-SEP2026.md` | Cross-theme dashboard |
| `main` | `COMMIT-TRENDS-v9-SEP2026.md` | **NEW: This file** |
| `solar-geoengineering` | `COMMIT-TRENDS-SOLAR-v9-SEP2026.md` | **NEW: Solar commit-by-commit analysis** |
| `solar-geoengineering` | `PROJECT-DISCOVERIES-SOLAR.md` | Solar project profiles (v8) |
| `solar-geoengineering` | `EPISODE-1-SOLAR-COMMIT-ARCHIVE.md` | **NEW: Episode-ready source notes** |
| `solar-geoengineering` | `SOLAR-EPISODE-DRAFT-OUTLINE.md` | **NEW: Episode script outline** |
| `carbon-capture` | `COMMIT-TRENDS-CARBON-v9-SEP2026.md` | **NEW: Carbon commit-by-commit analysis** |
| `carbon-capture` | `PROJECT-DISCOVERIES-CARBON.md` | Carbon project profiles (v7) |
| `carbon-capture` | `EPISODE-2-CARBON-COMMIT-ARCHIVE.md` | **NEW: Episode-ready source notes** |
| `carbon-capture` | `CARBON-EPISODE-DRAFT-OUTLINE.md` | **NEW: Episode script outline** |
| `ocean-intervention` | `COMMIT-TRENDS-OCEAN-v9-SEP2026.md` | **NEW: Ocean gap analysis + PBP-POD deep-dive** |
| `ocean-intervention` | `PROJECT-DISCOVERIES-OCEAN.md` | Ocean gap analysis (v7) |

---

## Episode Status

| Episode | Branch | Research Status | Key Angle |
|---------|--------|----------------|-----------|
| **Solar Geoengineering** | `solar-geoengineering` | ✅ COMPLETE | "The code beneath the sun" — infrastructure vs. lone theorists |
| **Carbon Capture** | `carbon-capture` | ✅ COMPLETE | "The longest john" — ghosts, blitzes, and CC0 revolution |
| **Ocean Intervention** | `ocean-intervention` | ✅ COMPLETE | "The empty quadrant" — 15 searches, zero repos, one diagnostic |

---

## Quick Links

- 🔗 **Repo:** https://github.com/bro26man-hash/climate-pod-research
- ☀️ Solar branch: https://github.com/bro26man-hash/climate-pod-research/tree/solar-geoengineering
- 🌍 Carbon branch: https://github.com/bro26man-hash/climate-pod-research/tree/carbon-capture
- 🌊 Ocean branch: https://github.com/bro26man-hash/climate-pod-research/tree/ocean-intervention

---

## Research Log

| Date | Activity |
|------|----------|
| 2026-09-03 | Repository created; initial research notes pushed |
| 2026-09-17 | v1–v3: Cross-theme analysis, branch creation, project discoveries |
| 2026-09-17 | v3: Ocean gap confirmed — 10+ search queries, zero repos |
| 2026-09-18 | **v9: Fresh commit histories pulled from 8 repos via GitHub API** |
| 2026-09-18 | **v9: COMMIT-TRENDS-SOLAR-v9 pushed to solar-geoengineering branch** |
| 2026-09-18 | **v9: COMMIT-TRENDS-CARBON-v9 pushed to carbon-capture branch** |
| 2026-09-18 | **v9: COMMIT-TRENDS-OCEAN-v9 pushed to ocean-intervention branch** |
| 2026-09-18 | **v9: Episode archive files and draft outlines pushed to all branches** |
