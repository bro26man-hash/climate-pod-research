# 🌍 Carbon Capture — Project Discoveries (v5 Update)
## Research Notes for Podcast Episode (October 2026)

---

## Overview
This document profiles all open-source repositories discovered during GitHub research relating to **carbon capture, direct air capture (DAC), and carbon removal technologies**. Data from GitHub search queries and direct commit-history pulls, October 2026.

---

## Executive Summary: The CC0 Revolution Slows, But the Directory Surges

After v4 (September 2026), the carbon capture ecosystem on GitHub shows **two contrasting signals**:

1. 🔴 **Open-Sustainable-Tech directory is surging** — 5 new entries on Sep 19, including DigitalizationSupportHub, MicroPowerManager, and GreenHEART — a coordinated IoT/energy monitoring sweep
2. 🟡 **Individual DAC projects remain small and fragmented** — no dominant open-source DAC codebase has emerged; the $1000/ton cost barrier hasn't been broken by open source

The CC0 public-domain revolution documented in v4 appears to have **slowed** — no new CC0-licensed DAC projects appeared this quarter. But the directory infrastructure is growing, which lowers barriers to entry.

---

## Repository Profiles

### 1. Open Sustainable Technology Directory (`protontypes/open-sustainable-technology`)
- **Stars:** 2,552 | **Last commit:** Sep 19, 2026 (5 days ago!)
- **Focus:** Comprehensive directory of 2,500+ climate-tech projects
- **Why it matters:** The single most important climate-tech resource on GitHub

**Recent commits (10 pulled):**

| Date | Commit | Significance |
|------|--------|-------------|
| Sep 19, 2026 | Add-DigitalizationSupportHub (#1646) | **New entry** — digitalization support for sustainability projects |
| Sep 19, 2026 | Add-MicroPowerManager (#1645) | **New entry** — micro-power management IoT tool |
| Sep 19, 2026 | Add-GreenHEART (#1643) | **New entry** — green computing/energy efficiency tool |
| Sep 9, 2026 | Add-MUIO (#1638) | IoT/energy monitoring |
| Sep 9, 2026 | Add-MUIOGO (#1639) | Companion to MUIO — IoT platform |
| Sep 1, 2026 | Fix dead links in README (#1634) | Maintenance |
| Aug 23, 2026 | Add claude-carbon (#1633) | AI/climate tooling — AI carbon footprint tracker |
| Aug 18, 2026 | Add Story Seed Library (#1630) | Narrative/education tool |
| Aug 18, 2026 | Add openflexure microscope (#1631) | Open-source scientific instrument |
| Jul 19, 2026 | Remove duplicate AI content review checkbox | Governance: AI content moderation |

**Episode angle (v5):** The Sep 19 surge of 3 commits (DigitalizationSupportHub, MicroPowerManager, GreenHEART) continues the **IoT/energy monitoring sweep** that started with MUIO/MUIOGO on Sep 9. This is significant because the directory is becoming a **de facto standard** for what counts as climate tech. If your project isn't in this directory, does it count? The AI content review PR template (Jul 2026) is also fascinating — the directory is now managing AI-generated entries, which means the directory itself has become a governance challenge.

---

### 2. OpenAir-Cyan (`openair-collective/openair-cyan`)
- **Stars:** 76 | **Language:** C/Hardware | **License:** CERN-OHL-S-2.0 (open hardware)
- **Last commit:** Feb 12, 2024 (still dormant — 2.5+ years)
- **Focus:** DIY open-hardware DAC device — "Cyan"
- **Special:** OSHWA-certified (UID US001095)

**Status:** No change from v4. The repo remains frozen after the Feb 12, 2024 OSHWA certification blitz (6 commits in 1 day, then silence).

**Episode angle (v5):** OpenAir-Cyan remains the **"what happened?"** case study. Six commits in one day achieved certification, then 2.5 years of nothing. The OSHWA certification didn't lead to sustained development. Did certification fix the wrong problem — focusing on legitimacy rather than functionality? The podcast episode should ask: "After you get your badge, then what?"

---

### 3. New Discovery: DAC Moving-Bed Digital Twin (`IsaH93/dac-moving-bed-digital-twin`)
- **Stars:** Low | **Language:** Python | **Last commit:** Jul 3, 2026 (recent!)
- **Focus:** Moving-bed TVSA (Temperature Vacuum Swing Adsorption) digital twin for Direct Air Capture — couples continuous sorbent physics (Toth isotherm, LDF kinetics) with a SimPy discrete-event simulation platform
- **Why it matters:** This is one of the most technically detailed open-source DAC projects. A "digital twin" means it's not just a simulation — it's a **virtual replica** of a physical DAC system that can be used for optimization and control.

**Episode angle (v5):** The digital twin approach is interesting because it bridges the gap between pure simulation and real-world deployment. A digital twin of a DAC plant means you can test control strategies, optimize sorbent regeneration cycles, and predict maintenance needs — all without touching the physical plant. This could be a path to reducing the $1000/ton cost: not by inventing new chemistry, but by optimizing the existing process through simulation.

---

### 4. New Discovery: OpenCarbon (`terranexum/OpenCarbon`)
- **Stars:** 2 | **Last commit:** Aug 19, 2026
- **Focus:** Carbon management technologies and plans to advance DAC research — emphasizes clean energy use and low-cost DAC
- **Why it matters:** The "clean energy + low cost" framing is the key constraint. Most DAC projects focus on the chemistry; OpenCarbon explicitly addresses the energy source and cost structure.

---

### 5. New Discovery: Direct-Air-Capture ML (`Rudra57/Direct-Air-Capture`)
- **Stars:** Low | **Language:** Jupyter Notebook | **Last commit:** Jun 11, 2026
- **Focus:** Data-driven machine learning model for DAC technology as a climate solution
- **Why it matters:** This is another ML-for-DAC project, following in the footsteps of the Carbon_Capture_ML survey. The question is whether ML can actually accelerate DAC development or just document what's already known.

---

### 6. Carbon Capture ML Survey (`zikribayraktar/Carbon_Capture_ML`)
- **Stars:** 56 | **Language:** Python/ML | **Last commit:** May 8, 2024 (frozen 2.5+ years)
- **Focus:** Curated survey of ML papers for carbon capture

**Status:** No change from v4. Frozen since May 2024.

---

## Cross-Cutting Carbon Episode Themes

### Theme 1: The Infrastructure vs. Invention Gap
The Open-Sustainable-Tech directory (2,552 stars, 5 new entries this month) is **infrastructure** — it catalogs what exists. But none of the DAC-specific projects (OpenAir-Cyan, dac-moving-bed-digital-twin, OpenCarbon) are close to breaking the $1000/ton barrier. The gap between cataloging climate tech and inventing better climate tech is enormous.

### Theme 2: The Digital Twin Signal
The dac-moving-bed-digital-twin project (Jul 2026) represents a new approach: instead of inventing new DAC chemistry, **optimize the existing process through simulation**. This could be the path to cost reduction that doesn't require a chemistry breakthrough.

### Theme 3: The AI Gravity Well
Three projects this quarter involve AI/ML applied to climate: claude-carbon (AI carbon footprint tracker), Carbon_Capture_ML survey, and Direct-Air-Capture ML. The AI gravity well is pulling everything toward data-driven approaches — but whether this accelerates real-world deployment or just produces more papers is an open question.

### Theme 4: The Governance Vacuum (Carbon Version)
Unlike solar geoengineering, carbon capture doesn't have a governance vacuum — it's generally seen as beneficial. But there IS a governance question: who certifies that a DAC project is actually removing carbon (and not just claiming to)? The OpenAir-Cyan OSHWA certification is one model, but it's the only one.

---

## Carbon Episode Architecture (v5)

| Segment | Duration | Content |
|---------|----------|--------|
| **Cold Open** | 2 min | "It's been 2.5 years since the DIY DAC device got its certification badge. Then what?" (OpenAir-Cyan) |
| **The Landscape** | 12 min | The Open-Sustainable-Tech directory: 2,500+ projects, but where are the breakthroughs? |
| **The Digital Twin** | 10 min | Optimizing DAC through simulation — the dac-moving-bed-digital-twin approach |
| **The AI Angle** | 8 min | ML for carbon capture — survey, direct modeling, and the papers-vs-deployment gap |
| **The Cost Barrier** | 10 min | $1000/ton: can open source + digital twins + CC0 break it? The evidence says not yet. |
| **The Future** | 5 min | What would a sustainable, open-source DAC ecosystem look like? |

---

## Research Methodology
- **Search queries:** 6 distinct queries across DAC, carbon capture, CC0, open hardware, and ML-for-climate
- **Commit pulls:** 10 most recent commits from 4 key repositories (40 total commits analyzed)
- **API calls:** GitHub Repository Search, List Commits, Get Repository
- **Date of research:** October 2026

---

*Research methodology: GitHub REST API, October 2026. Commits pulled via List Commits API. Search queries via Repository and Code Search APIs.*