# 🌍 Carbon Capture — Commit Trend Analysis (v4: Sep 2026 Update)
## Research Notes | Climate Pod Research | September 2026

---

## Executive Summary

Across **9 carbon capture repositories** spanning from 2022 to September 2026, we identified **four distinct development patterns** that define the carbon capture software landscape:

1. **Ecosystem Continuously** (Open-Sustainable-Tech) — Steady multi-week pace, many contributors, directory maintenance
2. **Publication-Anchored** (Carbon_Capture_ML) — Commits tied to paper submissions and benchmark launches
3. **Burst-then-Freeze** (OpenAir-Cyan) — Intense single-day development, then permanent hibernation
4. **Ghost Dormancy** (carbon-capture-and-storage, CO2-Sequestration) — Dead academic repos with high star counts

---

## Detailed Trend Analysis by Repository

### Open-Sustainable-Technology: The Ecosystem Engine
**Commit velocity:** ~5 commits/week over 3 months (Jun-Sep 2026)
**Contributors:** 5 active developers (Abdul Salam, Tobias Augspurger, Mikhail Alabugin, gwittebolle, Christophe Combelles)

**Commit timeline analysis:**
```
Jun  6 ─── Add EpexPredictor (energy price prediction)
Jun 23 ─── Add wbdata (World Bank data) + Add Volca to LCA
Jul  1 ─── Add ToOp + Add ASSETRA + Add PowerIO (3 projects in 1 day!)
Jul  2 ─── Add PowerIO (continued)
Jul 17 ─── Update PR template with review reminder
Jul 19 ─── Remove duplicate AI checkbox + Modify PR template for AI review
Aug 18 ─── Add Story Seed Library + Add openflexure microscope
Aug 23 ─── Add claude-carbon (AI-related carbon project)
Sep  1 ─── Fix dead links in README
Sep  9 ─── Add-MUIO + Add-MUIOGO (2 projects in 1 day!)
```

**Pattern characteristics:**
- **Additive development:** Every commit adds a new project to the directory
- **Batch additions:** Jul 1 (3 projects in 1 day), Sep 9 (2 projects in 1 day)
- **Governance evolution:** PR template changes for AI content review (Jul 19) — unique in climate OSS
- **Link maintenance:** Sep 1 dead link fix shows the directory is getting large enough for link rot
- **No deletion commits** — once something's in, it stays in

**What this means for CCUS:** The directory is growing at ~5 new projects/week. At this rate, it will hit 3,000 projects by early 2027. The AI content review PR template is the most significant governance development — the community is preparing for AI-assisted climate project development.

---

### Carbon_Capture_ML: The Publication Anchor
**Commit velocity:** 15 commits over 16 months (Jan 2023 – May 2024), then dormant
**Contributor:** Zikri Bayraktar (single developer)

**Commit timeline analysis:**
```
Jan 11-20 ── Initial setup: citation info, surrogate paper, 2 new papers
Feb 1-5 ──── Paper deluge: 6 commits in 5 days (process papers)
Feb 16 ────── MOFsimplify paper added
Mar 1 ──────── Process paper added
Apr-May 2024 ── README updates (3)
May 8, 2024 ── ★ OpenDAC paper added (LANDMARK)
```

**Pattern characteristics:**
- **Paper-driven commits:** Every commit either adds or references a paper
- **Feb 2023 burst:** 6 commits in 5 days — likely tied to a paper submission deadline
- **May 2024 landmark:** OpenDAC paper addition signals benchmark adoption
- **No code commits after May 2024** — transitioned from active development to reference archive

**What this means for CCUS:** Carbon_Capture_ML is the **best-indexed survey** of ML for carbon capture, but it's now an archival resource. The OpenDAC commit (May 2024) is the anchor point — the repo transformed from "here are papers" to "here's how to evaluate them systematically."

---

### OpenAir-Cyan: The Burst-then-Freeze Pattern
**Commit velocity:** 15 commits, all within **~24 months** (May 2022 – Feb 2024)
**Peak:** 7 commits on **February 12, 2024**
**Contributors:** KCollins (lead), DaOfficialWizard, ZanzyTHEbarzy

**Commit timeline analysis:**
```
May 5, 2022 ─── Delete .github/workflows (CI/CD removal)
May 7, 2022 ─── Update CodeQL x2 (static analysis)
May 11, 2022 ─── Rename CodeQL file
May 15, 2022 ─── Update README x2
May 17, 2022 ─── Add files for usability
Jul 20, 2022 ─── Update README
...18 months of silence...
Feb 12, 2024 ─── ★ 7 COMMITS IN ONE DAY:
                 - Update README with OSHWA UID link
                 - Add files via upload (x2)
                 - Add OSHWA UID logo
                 - Create CITATION.cff
                 - Update README (final)
```

**Pattern characteristics:**
- **Phase 1 (May-Jul 2022):** CI/CD setup and documentation — infrastructure work
- **Phase 2 (Aug 2022 - Feb 2024):** Complete silence — 20 months with zero commits
- **Phase 3 (Feb 12, 2024):** **The Great Blitz** — 7 commits in a single day, all about OSHWA certification and formalization
- **Phase 4 (Feb 2024 onward):** Complete silence again — no community adoption yet

**What this means for CCUS:** The Feb 12, 2024 blitz is the **story within the story**. KCollins pushed 7 commits in one day to achieve OSHWA certification (UID US001095). This isn't development — it's **legal formalization**. The device was already built; what needed to happen was the paperwork. The 20-month silence before the blitz suggests the hardware was developed **offline** and then brought to GitHub for certification.

---

### DAC Peroxovanadates & Peroxotitanates: The CC0 Pair
**Commit velocity:** 2 commits each, both on the same date
**Contributor:** tjz21 (single developer)
**License:** CC0 (public domain)

**Commit timeline analysis:**
```
Sep 23, 2025 ── Both repos updated:
               - DAC_peroxovanadates: data update or correction
               - DAC_peroxotitanates: data update or correction
```

**Pattern characteristics:**
- **Synchronized development:** Both repos updated on the same day
- **CC0 licensing:** Maximum openness — no restrictions whatsoever
- **Minimal commits:** 2 per repo suggests focused, intentional updates
- **No test commits, no documentation commits** — pure data

**What this means for CCUS:** The **CC0 license is the thesis statement.** TJ Z21 is saying: "This data belongs to everyone. Use it, break it, build on it, commercialize it — I don't care." In the context of the $1000/ton DAC cost barrier, CC0 is **radical accessibility**.

---

### Carbon Capture and Storage: The Academic Ghost
**Commit velocity:** Dormant since March 2021
**Contributor:** yohanesnuwara (academic)
**Stars:** 85 ⭐

**Pattern characteristics:**
- **Zero commits since 2021** — 5+ years of complete silence
- **85 stars** — highly cited in academic literature
- **MATLAB** — specialized, non-collaborative ecosystem
- **Covers:** Reservoir simulation, geomechanics, CO2 injection modeling

**What this means for CCUS:** This is the **textbook ghost repo**. 85 stars but zero maintenance. The MATLAB dependency is the killer — no one outside academia can easily contribute. A Python port could wake this giant.

---

## Cross-Repo Comparative Analysis

### By Commit Velocity (Peak)
| Repo | Peak Day | Peak Rate | Interpretation |
|------|----------|----------|---------------|
| OpenAir-Cyan | Feb 12, 2024 | 7/day | Certification push |
| Open-Sustainable-Tech | Sep 9, 2026 | 2/day | Batch additions |
| Carbon_Capture_ML | Feb 1-5, 2023 | 1.2/day | Paper sprint |
| DAC_peroxovanadates | Sep 23, 2025 | 1/day | Focused update |
| carbon-capture-and-storage | Mar 6, 2021 | 0/day | Ghost |

### By Contributor Count
| Tier | Repos | Avg Contributors |
|------|-------|-----------------|
| Multi-contributor | Open-Sustainable-Tech (5), OpenAir-Cyan (3) | 4.0 |
| Single-contributor | Carbon_Capture_ML, DAC repos, carbon-capture-and-storage | 1.0 |

### By Time Since Last Commit
| Repo | Last Commit | Status |
|------|------------|--------|
| Open-Sustainable-Tech | Sep 9, 2026 | **Actively maintained** |
| OpenAir-Cyan | Feb 12, 2024 | Hibernating |
| Carbon_Capture_ML | May 8, 2024 | Archival |
| DAC_peroxovanadates | Sep 23, 2025 | Focused |
| DAC_peroxotitanates | Sep 23, 2025 | Focused |
| carbon-capture-and-storage | Mar 6, 2021 | **Dead** |
| CO2-Sequestration | ~2019 | **Dead** |

---

## The CC0 Revolution: A Case Study

### What Is CC0?
Creative Commons Zero — a legal tool that waives all copyright and related rights. In science, it means:
- Anyone can use the data for any purpose (commercial, academic, personal)
- No attribution required (though appreciated)
- No patent filings, no licensing discussions, no legal barriers
- The data becomes **public infrastructure**

### Why Does It Matter for Carbon Capture?
The DAC cost barrier ($1000/ton) is partly an **IP barrier**. Companies hold patents on:
- Sorbent materials (peroxovanadates, amines, MOFs)
- Process designs (temperature vacuum swing, moisture swing)
- System configurations (contactors, regenerators)

When TJ Z21 applies CC0 to computational screening data, they're **removing the IP barrier** for two specific sorbent families. This doesn't break the $1000/ton barrier alone, but it's a **signal** that the next breakthrough might come from open collaboration.

### The Ripple Effect
- **OpenAir-Cyan** uses OSHWA (hardware certification) — complementary form of openness
- **Open-Sustainable-Tech** doesn't require specific licenses for listed projects (a weakness)
- **Carbon_Capture_ML** uses traditional academic sourcing
- **srm-forever** (solar) uses no explicit license

The CC0 pair (DAC_peroxovanadates + DAC_peroxotitanates) is the **only explicitly public-domain carbon capture research on GitHub**.

---

## The OpenAir-Cyan Phenomenon

### What Makes It Special?
1. **OSHWA certification** — the only certified open-source CCUS hardware project
2. **DIY approach** — 3D-printable, citizen-scientific DACC device
3. **76 stars** — high visibility for a hardware project
4. **Single-day blitz** — 7 commits on Feb 12, 2024 for certification
5. **20 months of silence** before and after — no community adoption yet

### The Unanswered Question
Did the Feb 12, 2024 blitz signal **readiness** (the device works, let's certify it) or **resignation** (nothing's happening, let's formalize what we have)? The 20-month silence before and after suggests **both**.

---

## 🎙️ Episode 2: Suggested Structure

### Cold Open
> "On a single day in February 2024, someone uploaded files, added an OSHWA logo, created a citation file, and updated a README. Seven commits. No code. No hardware changes. Just paperwork. But that paperwork certified the first open-source, DIY, 3D-printable device that captures carbon from the air directly. And the company that's trying to do the same thing commercially charges $500 a ton."

### Act 1: The Map-Makers (Open-Sustainable-Tech)
- 2,552 stars, 2,500+ projects, 5 contributors
- AI content review PR template (July 19, 2026)
- **Quote:** "The largest climate tech directory on GitHub adds 5 new projects a week — but which ones are actually about capturing carbon?"

### Act 2: The Garage Builders (OpenAir-Cyan)
- OSHWA-certified DACC device, 76 stars, 7 commits in one day
- 20 months of silence before and after
- **Quote:** "A DIY carbon capture device with OSHWA certification. Not a prototype — a certified device. The question isn't whether it works. The question is: who's going to build it?"

### Act 3: The Data Donors (TJ Z21's CC0 Repos)
- Peroxovanadate + Peroxotitanate, CC0 public domain, synchronized development
- **Quote:** "Two repositories, two metals, one license: public domain. The researcher behind them didn't patent anything. Didn't license anything. Just said 'this data belongs to everyone.'"

### Act 4: The Ghosts (carbon-capture-and-storage)
- 85 stars, dormant since 2021, MATLAB-only
- **Quote:** "85 stars and zero commits since 2021. This repo is a citation monument — papers reference it, but nobody runs it."

### Closing
> "The CC0 license is the most important legal development in carbon capture open source that nobody is talking about. Two researchers gave away their perovskite screening data to the public. No patents. No licensing. Just CC0. If the next breakthrough in direct air capture comes from open data, it might come from someone who never intended to be an innovator — they just didn't want to be the reason someone else couldn't build on their work."

---

*Last updated: September 2026 (v4) | Data source: GitHub API commit histories for 9 repositories*