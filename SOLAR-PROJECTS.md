# ☀️ Solar Geoengineering — Project Discoveries

**Last Updated:** September 2026
**Research Round:** Second pass — commit histories from 10 repositories

---

## Repository Catalog

### Tier 1 — Institutional / High-Impact

| Repo | Stars | Language | Focus | Last Activity |
|------|-------|----------|-------|---------------|
| **wrf-model/WRF** | 1,761 | Fortran | Foundational atmospheric model (v4.8.0) | Jun 8, 2026 |
| **PCMDI/pcmdi_metrics** | 133 | Python | ESM evaluation toolkit (v4.2.1) | Sep 4, 2026 |
| **NOAA-GFDL/MDTF-diagnostics** | 80 | Jupyter | Process-oriented climate diagnostics | Aug 14, 2026 |

### Tier 2 — Active Research / Modeling

| Repo | Stars | Language | Focus | Last Activity |
|------|-------|----------|-------|---------------|
| **ClimateMARGO/ClimateMARGO.jl** | 73 | Julia | Climate-economic modeling (MarGO framework) | Aug 17, 2026 |
| **KOSASIH/GCCS-Core** | 9 | Python | Global Climate Control System core algorithms | Sep 2025 |
| **cjcarlson/geomalaria** | 3 | R | Malaria risk under solar geoengineering scenarios | 2024 |

### Tier 3 — Conceptual / Dormant

| Repo | Stars | Language | Focus | Last Activity |
|------|-------|----------|-------|---------------|
| **PSLmodels/Geo-DICE** | 2 | MATLAB | Modified DICE model with geoengineering | Sep 2018 |
| **jlehtomaa/OOCC_2021** | 2 | Python | Solar geoengineering governance model | Nov 2021 |
| **brandonhimpfen/awesome-geoengineering** | 4 | Python | Curated list of geoengineering resources | Sep 2026 |
| **hausfath/srm-forever** | 0 | HTML | Interactive SRM economics model | Aug 26, 2026 |
| **prashaant1926/open-earth-digital-twin-simulation** | 0 | TeX | Distributed Earth system simulation manifesto | Oct 2025 |

---

## Deep Dives

### 1. wrf-model/WRF — The Atmospheric Foundation (1,761 stars)

**Why it matters for SRM:** WRF is the de facto atmospheric model for climate simulation. Its aerosol-aware physics modules are the building blocks for any SRM simulation pipeline.

**Recent commit highlights (May-Jun 2026):**
- v4.8.0 release (Jun 8) — major institutional milestone
- Tempo aerosol/hail options disabled in Registry (Jun 5) — experimental features being finalized
- Solar radiation EOT correction (May 28) — radiative transfer precision improvements
- MYNN-EDMF update (May 27) — boundary layer physics refinements
- 10 commits over 18 days with 6+ contributors (Islas, weiwangncar, Olson, Fita, Werner)

**Podcast angle:** "The atmospheric modeling infrastructure for SRM exists — NCAR and NOAA maintain it as a core climate tool. But no one has built an SRM-specific configuration on top of it. Why?"

### 2. ClimateMARGO/ClimateMARGO.jl — The Policy Model Awakens (73 stars)

**What it is:** Julia implementation of MARGO, an idealized climate-economic modeling framework for optimizing trade-offs between emissions Mitigation, Adaptation, and Geoengineering.

**Why it matters:** This is the closest thing to an open-source SRM policy model. It models the optimal deployment of geoengineering relative to mitigation and adaptation strategies.

**Commit pattern:** Dormant from Nov 2023 to Aug 2026. Two README updates on Aug 17, 2026 by Fons van der Plas after 2+ years of silence. Code commits stopped in Oct 2023.

**Podcast angle:** "A climate-economic model that optimizes geoengineering deployment went dormant for two years, then suddenly someone updated the README. Is the policy-modeling community waking up — or is it another false start?"

### 3. PSLmodels/Geo-DICE — The DICE-with-SRM (2 stars)

**What it is:** Modified DICE (Dynamic Integrated Climate-Economy) model that includes geoengineering as a control variable.

**Commit history:** Only 4 commits total, all from Aug-Sep 2018. Soheil Shayegh uploaded the code and it's been frozen since.

**Podcast angle:** "The DICE model is the most influential climate-economics model ever built. Making it include geoengineering was a landmark — but the code has been dead for 7 years. The model works in papers; it doesn't work in open source."

### 4. jlehtomaa/OOCC_2021 — The Governance Model (2 stars)

**What it is:** A simple model for solar geoengineering governance, published alongside a 2021 paper.

**Commit pattern:** All 10 commits happened in Sep-Nov 2021 — a paper-driven burst. BibTeX and citation updates continued through Nov 2021, then complete silence.

**Podcast angle:** "This repo is a tutorial in how academic geoengineering code works: paper comes out, code goes up, citations get updated, then nobody touches it for years."

### 5. KOSASIH/GCCS-Core — The Ambitious Framework (9 stars)

**What it is:** "Foundational framework for the Global Climate Control System" — encompassing core algorithms, data management, and simulation components.

**Concern:** The name "Global Climate Control System" is alarmist. The actual technical content appears to be a climate model orchestration framework, not a real-world climate control system.

**Podcast angle:** "One repo called its project the 'Global Climate Control System.' That name tells you half the story: the technical ambition is real, but the framing reveals the governance gap."

### 6. hausfath/srm-forever — The Transparency Model (0 stars)

**What it is:** Interactive single-page SRM economics model using Weitzman certainty-equivalent discounting. Published alongside an essay on discount rates and geoengineering economics.

**Why it matters:** Proves that simple, transparent models can make SRM economics accessible without running a GCM. It's a pedagogical and governance tool, not a simulation tool.

---

## The Solar Geoengineering Gap Matrix

| Layer | What Exists | What's Missing |
|-------|-------------|----------------|
| **Atmospheric modeling** | WRF (1,761 stars), active | SRM-specific configurations |
| **Model evaluation** | PCMDI (133 stars), active | SRM-specific metrics |
| **Economic modeling** | Geo-DICE (2 stars, dead), srm-forever (0 stars) | Modern, maintained policy models |
| **Policy/governance** | OOCC (2 stars, dead), MARGO (73 stars, dormant) | Interactive governance tools |
| **Impact assessment** | geomalaria (3 stars), Arctic impacts code | Multi-impact integrated assessment |
| **Resource lists** | awesome-geoengineering (4 stars) | Living, community-maintained catalogs |

---

## Episode Talking Points

1. **The infrastructure exists but the application doesn't.** WRF and PCMDI are world-class. But there's no open-source SRM simulation pipeline on top of them. The building blocks are there; the house hasn't been built.

2. **ClimateMARGO's revival is the sleeper story.** An idealized climate-economic model that optimizes geoengineering deployment, dormant for 2 years, suddenly showing README activity. What does it mean when a policy model wakes up?

3. **The naming problem.** GCCS-Core calls itself the "Global Climate Control System." That name reveals more about the governance gap than any commit message ever could.

4. **The DICE-with-SRM paradox.** Geo-DICE modified the most influential climate-economics model to include geoengineering — then froze for 7 years. The model lives in citations; it doesn't live in code.

5. **srm-forever proves transparency is possible.** A single HTML file that makes SRM economics interpretable. It's not a simulation, but it's democratic. Is that enough?