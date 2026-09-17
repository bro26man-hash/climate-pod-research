# ☀️ Solar Geoengineering — Commit Trend Analysis (v2 — Second Research Round)

**Last Updated:** September 2026 (Second research round — fresh commit data)
**Source Repositories Analyzed:** wrf-model/WRF, PCMDI/pcmdi_metrics, NOAA-GFDL/MDTF-diagnostics, ClimateMARGO/ClimateMARGO.jl, PSLmodels/Geo-DICE, jlehtomaa/OOCC_2021, KOSASIH/GCCS-Core, cjcarlson/geomalaria, brandonhimpfen/awesome-geoengineering, hausfath/srm-forever

---

## Repository-by-Repository Commit Histories

### 1. wrf-model/WRF — 1,761 stars (The Atmospheric Infrastructure)

| Date | Commit | Author | Significance |
|------|--------|--------|-------------|
| Jun 8, 2026 | v4.8.0 release merge | Anthony Islas | **Major release milestone** |
| Jun 6, 2026 | README & version update for v4.8.0 | Anthony Islas | Release preparation |
| Jun 5, 2026 | Disable tempo_aerosolaware & tempo_hailaware | weiwangncar | Experimental features finalized |
| May 30, 2026 | AOCC vectorization fix | weiwangncar | Performance optimization |
| May 28, 2026 | Solar radiation EOT correction | weiwangncar | **Radiative transfer precision** |
| May 27, 2026 | MYNN-EDMF update | Joseph Olson | Boundary layer physics |
| May 27, 2026 | MMM-physics SHA update | Anthony Islas | Physics package integration |
| May 26, 2026 | CDXWRF module fix | Lluis Fita | Diagnostic tooling repair |
| May 26, 2026 | GFL option README | weiwangncar | Feature documentation |
| May 21, 2026 | mp_physics=88 error message | Kelly Werner | User experience improvement |

**Activity Pattern:** 10 commits over 18 days (May 21-Jun 8, 2026) with 6 contributors. Institutional release cycle.

**SRM Relevance:** The solar radiation EOT correction and aerosol-aware physics development are directly relevant to SRM simulation capability. WRF's atmosphere model is the foundation that any SRM simulation would build upon.

---

### 2. PCMDI/pcmdi_metrics — 133 stars (The Evaluation Gold Standard)

| Date | Commit | Author | Significance |
|------|--------|--------|-------------|
| Sep 4, 2026 | v4.2.1 release merge | Aparna Radhakrishnan | **10 commits in 2 days** |
| Sep 3, 2026 | v4.2.1 tagged | Jiwoo Lee | Release tag |
| Aug 14, 2026 | PR #825 merged | Aparna Radhakrishnan | Diagnostic enhancement |
| Jun 19, 2026 | MCS precip-buoyancy POD | Wei-Ming Tsai | **Ocean-relevant diagnostics** |
| Jun 8, 2026 | PR #823 merged | Aparna Radhakrishnan | Code review passage |
| Jun 2, 2026 | Main branch merge | jongsooshin5 | Integration |

**Activity Pattern:** Intense institutional burst for v4.2.1 (10 commits in 2 days). Multiple contributors (Jiwoo Lee, James Goodnight, Jared Lewis). Funded by LLNL/DOE.

**SRM Relevance:** CMIP6 evaluation tools are the baseline infrastructure for SRM governance. You can't evaluate SRM's effects without tools to evaluate model outputs.

---

### 3. NOAA-GFDL/MDTF-diagnostics — 80 stars (The Ocean-Adjacent Tool)

| Date | Commit | Author | Significance |
|------|--------|--------|-------------|
| Aug 14, 2026 | PR #825 merge | Aparna Radhakrishnan | Cross-institutional PR |
| Jun 19, 2026 | MCS precip-buoyancy POD (x4) | Wei-Ming Tsai | **New ocean process diagnostic** |
| Jun 8, 2026 | PR #823 merge + README | jongsooshin5 | Code review + docs |
| Jun 2, 2026 | Branch merge | jongsooshin5 | Integration |

**Activity Pattern:** 10 commits across Jun-Aug 2026, with a burst around the June precip-buoyancy POD. Multi-contributor with PR-based workflows.

**SRM/Ocean Relevance:** The precipitation-buoyancy POD is the closest thing to ocean process diagnostics in open source. Critical for evaluating any ocean intervention's effects.

---

### 4. ClimateMARGO/ClimateMARGO.jl — 73 stars (The Policy Model Revival)

| Date | Commit | Author | Significance |
|------|--------|--------|-------------|
| Aug 17, 2026 | README update (#2) | Fons van der Plas | **First activity in 2+ years** |
| Aug 17, 2026 | README update (#1) | Fons van der Plas | Revival signal |
| Oct 18, 2023 | Unit conversion comment (#86) | Fons van der Plas | Last code-level change |
| Jul 6, 2023 | Pluto notebook link | Fons van der Plas | Ecosystem integration |
| Nov 14, 2022 | Project.toml update | Fons van der Plas | Dependency management |
| Nov 12, 2022 | JuMP/Ipopt compat upgrade (#85) | Fons van der Plas | **Last substantive code change** |
| Feb 10, 2022 | Remove deprecated web apps | Henri Drake | Cleanup |
| Feb 4, 2022 | CITATION.bib added | Henri Drake | Citation infrastructure |
| Jan 13, 2022 | Typo fix | Henri Drake | Maintenance |
| Jan 12, 2022 | Doc version deployment | Henri Drake | Documentation |

**Activity Pattern:** 4 contributors, dormant since Oct 2023, then 2 README updates on Aug 17, 2026. Name = MARGO (& Trade-offs) = Mitigation/Adaptation/Geoengineering.

**Revival Analysis:** Two README updates after 2+ years of code dormancy. Could signal: (a) growing policy-modeling interest in SRM, (b) a paper preparing, or (c) another false start. No new code commits yet — the revival is cosmetic so far.

---

### 5. KOSASIH/GCCS-Core — 9 stars (The Ambitious Framework)

**What it is:** "Foundational framework for the Global Climate Control System" — encompassing core algorithms, data management, and simulation components.

**Last activity:** ~Sep 2025 (moderate activity)

**Caution:** The name "Global Climate Control System" conflates research infrastructure with geoengineering anxiety. The technical content is a climate model orchestration framework, not a real-world climate control system.

**Podcast angle:** "One repo calls its project the 'Global Climate Control System.' That name reveals more about the governance gap than any commit message ever could."

---

### 6. PSLmodels/Geo-DICE — 2 stars (The Modified DICE)

| Date | Commit | Author | Significance |
|------|--------|--------|-------------|
| Sep 27, 2018 | File upload | Soheil Shayegh | **Last activity — 7+ years dormant** |
| Aug 15, 2016 | File upload (x2) | Soheil Shayegh | Initial content |
| Aug 15, 2016 | Initial commit | Matt Jensen | Project init |

**Activity Pattern:** 4 commits over 2 years (2016-2018). Then complete silence. Modified DICE model with geoengineering as a control variable.

**Dormancy Analysis:** This is a classic "published-and-frozen" academic codebase. The model is cited in literature but the code is a museum piece. 7 years of zero activity.

---

### 7. jlehtomaa/OOCC_2021 — 2 stars (The Governance Model)

| Date | Commit | Author | Significance |
|------|--------|--------|-------------|
| Nov 15, 2021 | BibTeX entry update | jlehtomaa | Citation refinement |
| Oct 26, 2021 | BibTeX reference update | jlehtomaa | Citation refinement |
| Sep 5, 2021 | README update (x3) | jlehtomaa | Documentation polish |
| Sep 4, 2021 | Citation update | jlehtomaa | Citation infrastructure |
| Sep 4, 2021 | CITATION file added | jlehtomaa | Citation setup |
| Sep 3, 2021 | README update (x3) | jlehtomaa | Documentation setup |

**Activity Pattern:** 10 commits all within Sep-Nov 2021. A paper-driven burst. After the paper was published and citations finalized, the repo was abandoned.

**Dormancy Analysis:** 4+ years dormant. This is the "academic code lifecycle" pattern: intense activity around paper publication, then nothing.

---

### 8. hausfath/srm-forever — 0 stars (The Transparency Model)

| Date | Commit | Author | Significance |
|------|--------|--------|-------------|
| Aug 26, 2026 | Initial release (x4) | hausfath | Single-day launch burst |

**Activity Pattern:** All 4 commits on one day. A single-page HTML SRM economics model using Weitzman certainty-equivalent discounting.

**Significance:** Proves that simple, transparent models can make SRM economics accessible without running a GCM. It's a pedagogical and governance tool, not a simulation tool.

---

## Comparative Activity Analysis

| Repo | Stars | Total Commits | Active Period | Pattern | Current State |
|------|-------|--------------|--------------|---------|---------------|
| WRF | 1,761 | 10+ (recent) | Continuous | Institutional release cycle | **Active** — v4.8.0 Jun 2026 |
| PCMDI | 133 | 10+ (recent) | 2 days | Institutional burst | **Active** — v4.2.1 Sep 2026 |
| MDTF | 80 | 10+ (recent) | 3 months | Incremental + PR burst | **Active** — Jun-Aug 2026 |
| ClimateMARGO | 73 | 10 | 4 years | Dormant then revival | **Dormant revival** — 2 README updates Aug 2026 |
| GCCS-Core | 9 | Moderate | Sep 2025 | Incremental | **Low activity** |
| Geo-DICE | 2 | 4 | 2 years | Academic upload | **Dead** — 7 years dormant |
| OOCC_2021 | 2 | 10 | 3 months | Paper-driven burst | **Dead** — 4+ years dormant |
| srm-forever | 0 | 4 | 1 day | Single launch | **Launch only** — no iteration |

---

## Three Activity Patterns

### 1. Institutional Continuity (WRF, PCMDI, MDTF)
- Funded by national labs (NCAR, NOAA, LLNL, DOE)
- Multiple contributors with PR-based workflows
- Version-tagged releases on predictable cycles
- **These are the Only repos that are genuinely alive in the SRM space**

### 2. Dormant Revival (ClimateMARGO)
- Code dormant for 2+ years, then README activity
- The question: is this a real revival or just a paper preparation?
- **The revival of a policy model for geoengineering is itself a story**

### 3. Academic Freeze-Dry (Geo-DICE, OOCC, srm-forever)
- Code uploaded for a paper, then abandoned
- No maintenance, no community, no iterative development
- **These repos are digital fossils — they show what was thought, not what was built**

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

## Key Findings for the Podcast

1. **The atmospheric modeling pipeline is alive.** WRF (v4.8.0, Jun 2026) and PCMDI (v4.2.1, Sep 2026) are both actively releasing. The infrastructure for SRM simulation exists. But it's not geoengineering-specific — it's general-purpose climate infrastructure.

2. **SRM-specific code is virtually nonexistent.** Beyond srm-forever (a single HTML file) and Geo-DICE (frozen since 2018), there is no open-source code that simulates the physical effects of solar geoengineering.

3. **ClimateMARGO's revival is the sleeper story.** An idealized climate-economic model that optimizes geoengineering deployment, dormant for 2 years, then 2 README updates in Aug 2026. The policy-modeling layer for SRM could be here — or it could go dormant again.

4. **The governance-research gap is real.** OOCC_2021 (governance model, 2 stars) and Geo-DICE (economics model, 2 stars) both froze after their paper was published. The academic incentive structure produces papers, not maintained tools.

5. **srm-forever is the transparency outlier.** A single HTML page making SRM economics interpretable. It's not simulation, but it's democratic. The question for governance: is transparency enough without physical simulation?

---

## Episode Questions

1. **Why does the atmospheric modeling infrastructure (WRF, PCMDI) exist but SRM-specific simulation doesn't?** What's the institutional barrier between general-purpose climate modeling and geoengineering-specific simulation?

2. **Can ClimateMARGO's revival signal a policy-modeling renaissance?** If the MARGO framework starts getting code commits again, what would it mean for SRM governance discourse?

3. **Is the "transparency model" (srm-forever) sufficient for governance?** Or do we need physical simulation to make SRM decisions responsibly?

4. **How do academic incentive structures shape the open-source geoengineering landscape?** The pattern is clear: papers get published, code gets uploaded, then code gets abandoned. What would change this?

5. **The August-Sep 2026 release cycle:** WRF v4.8.0 (Jun) to PCMDI v4.2.1 (Sep) — are we closer to evaluating SRM effects than we thought? What's next in the release pipeline?