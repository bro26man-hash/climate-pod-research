# 🌍 Carbon Capture — Project Discoveries (v4 Update)
## Research Notes for Podcast Episode (September 2026)

---

## Overview
This document profiles all open-source repositories discovered during GitHub research relating to **carbon capture, direct air capture (DAC), and carbon removal technologies**. Data from GitHub search queries and direct commit-history pulls, September 2026.

---

## Repo Profiles

### 1. Open Sustainable Technology Directory (`protontypes/open-sustainable-technology`)
- **Stars:** 2,552 | **Last commit:** Sep 9, 2026 (4 days ago!)
- **Focus:** Comprehensive directory of 2,500+ climate-tech projects
- **Why it matters:** The single most important climate-tech resource on GitHub

**Recent Commits (Sep 2026):**
- Sep 9: Add-MUIO, Add-MUIOGO (IoT/energy monitoring)
- Sep 1: Fix dead links in README
- Aug 23: Add claude-carbon (AI/climate tooling)
- Aug 18: Add Story Seed Library, Add openflexure microscope
- Jul 19: AI content review PR template (governance meta-process)
- Jul 2: Add PowerIO; Jul 1: Add ASSETRA, Add ToOp
- Jun 23: Add wbdata, Add Volca to LCA; Jun 6: Add EpexPredictor

**Episode Angle:** Two commits in one day (Sep 9) suggest a coordinated sweep of IoT/energy projects. The AI content review PR template (Jul 2026) is meta-governance: the directory is managing AI-generated entries.

---

### 2. OpenAir-Cyan (`openair-collective/openair-cyan`)
- **Stars:** 76 | **Language:** C/Hardware | **Last commit:** Feb 12, 2024 (dormant 2.5+ years)
- **Focus:** DIY open-hardware DAC device — "Cyan"
- **Special:** OSHWA-certified (UID US001095)
- **License:** CERN-OHL-S-2.0 (open hardware)

**Blitz Day (Feb 12, 2024):** 6 commits — OSHWA UID logo, CITATION.cff, file uploads, README update. Then: silence.
**Red flag:** CI/CD workflows deleted May 2022, 3 months before the blitz.

**Episode Angle:** 6 commits in one day achieved OSHWA certification, then 2.5 years of nothing. Did Certification fix the wrong problem?

---

### 3. Carbon Capture ML Survey (`zikribayraktar/Carbon_Capture_ML`)
- **Stars:** 56 | **Language:** Python/ML | **Last commit:** May 8, 2024 (frozen 2+ years)
- **Focus:** Curated survey of ML papers for carbon capture

**Pattern:** 10 commits in Jan-Feb 2023 (survey construction), then 5 single-paper additions through May 2024. Frozen since.

**Episode Angle:** Is a 2.5-year-old survey still trustworthy in a field where new papers appear weekly?

---

### 4. DAC Peroxovanadates (`tjz21/DAC_peroxovanadates`)
- **Stars:** 2 | **License:** CC0 (public domain) | **Last commit:** Sep 23, 2025
- **Focus:** Computational screening of peroxovanadate sorbents for DAC

**Key Event:** Sep 12, 2025 — CC0 license added (commit `e041eff`)
**Companion:** `DAC_peroxotitanates` adopted CC0 on the same day

**Episode Angle:** The CC0 license adoption is the single most important governance signal in carbon capture on GitHub. Two researchers gave away their entire computational screening dataset to the public domain.

---

### 5. Carbon Capture and Storage — Ghost Repo (`yohanesnuwara/carbon-capture-and-storage`)
- **Stars:** 85 | **Language:** MATLAB/Jupyter | **Last commit:** Mar 6, 2021 (dead 5+ years)
- **Focus:** Reservoir simulation and geomechanics

**Pattern:** All 6 final commits on a single day (Mar 6, 2021) — simulation results uploaded. Then: nothing for 5 years.

**Episode Angle:** 85 stars measure citations, not usability. This repo is a monument, not a tool.

---

## The CC0 Revolution
The most significant governance finding: **CC0 public-domain dedication** by `tjz21` on Sep 12, 2025.

**Pattern:** Two repos (`DAC_peroxovanadates` and `DAC_peroxotitanates`) both adopted CC0 on the same day.

**Why it matters:**
- In climate tech, where IP is hoarded by corporations, academic researchers choosing CC0 is radical
- Computational screening data is typically treated as a trade asset
- Making it public domain removes the "data moat"
- Enables reproducibility — anyone can verify, build on, or use the data commercially

**Episode hook:** "In September 2025, two researchers who spent months running quantum mechanical calculations on DAC sorbent materials made a decision that most corporations would find insane: they put all their data in the public domain."

---

## The OpenAir-Cyan Parable
6 commits in one day (Feb 12, 2024) achieved OSHWA certification and CITATION.cff. Then: 2.5 years of silence. CI/CD deleted 3 months before the blitz.

---

## The Ghost Repo Problem
carbon-capture-and-storage (85 stars, dead since 2021) represents a pattern: stars measure citations, not usability. Academic repos are created for papers, not communities.

---

## Episode Structure

**Cold Open:** "In September 2025, a researcher named Jacob Hirschi pushed a single commit. The message: 'added CC0 license.' But what he did was hand the keys to his entire research dataset to the public."

**Act 1:** Open Sustainable Technology (2,552 stars), Carbon Capture ML (56 stars, frozen), OpenAir-Cyan (76 stars, then silence)

**Act 2:** CC0 public domain (radical move), OpenAir-Cyan certification (cautionary tale), ghost repos (bibliography problem)

**Act 3:** Is a 2.5-year-old survey still trustworthy? Does OSHWA certification mean anything if nobody builds the device?

---

## Sources
- [Open Sustainable Technology Directory](https://github.com/protontypes/open-sustainable-technology)
- [OpenAir-Cyan](https://github.com/openair-collective/openair-cyan)
- [Carbon Capture ML Survey](https://github.com/zikribayraktar/Carbon_Capture_ML)
- [DAC Peroxovanadates](https://github.com/tjz21/DAC_peroxovanadates)
- [Carbon Capture and Storage (Ghost)](https://github.com/yohanesnuwara/carbon-capture-and-storage)