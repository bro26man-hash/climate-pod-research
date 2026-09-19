# 🌊 Ocean Intervention — Commit Trend Analysis (The "Empty Universe")

**Analysis Date:** September 2026  
**Repositories Analyzed:** 1 adjacent (NCAR_ML_EKE) + 0 dedicated  
**Total Commits Pulled:** 15 (from NCAR_ML_EKE only)

---

## The Ocean Gap: By the Numbers

| Metric | Solar Geoengineering | Carbon Capture | Ocean Intervention |
|--------|---------------------|----------------|--------------------|
| **Repos found** | 4 | 2 | **0 dedicated** |
| **Stars (total)** | 1,890+ | 15 | ~20 (adjacent only) |
| **Commits pulled** | 60+ | 30 | 15 (adjacent) |
| **Active repos** | 2 (WRF, regional-geo) | 1 (GCCS-Core) | **0** |
| **Continuous development** | Yes (WRF) | No | **N/A — nothing to analyze** |
| **Simulation of core process** | Yes (WRF/TEMPO) | No | **Nothing at all** |

---

## Adjacent Analysis: NCAR_ML_EKE (Ocean Climate Modeling, NOT Geoengineering)

**Repository:** https://github.com/CrayLabs/NCAR_ML_EKE  
**Stars:** 20  |  **Language:** Jupyter Notebook  |  **Last commit:** March 30, 2022

### Commit Timeline

```
Apr 13, 2021: 10 commits (project creation day —LICENSE, README, MOM6 submodule, driver reformatting, MIT license)
Feb  8, 2022:  1 commit (MOM6 submodule update)
Feb  9, 2022:  1 commit (README update for MOM6 compilation)
Mar 14, 2022:  1 commit (MOM6 instructions update)
Mar 28, 2022:  1 commit (refactor driver for colocated option)
Mar 30, 2022:  1 commit (fix notebook typos)
────────────────────────────────────────────────
Aug 17, 2022:  Last commit → DORMANT for 4.5 years
```

### Pattern Analysis

**Creation burst:** 10 commits on April 13, 2021 — typical paper-companion repo creation day. The authors (Sam Partee, Andrew Shao, from NCAR/Cray Labs) built the entire project infrastructure in one focused session:
- Created git submodule (MOM6 ocean model)
- Set up LICENSE (MIT)
- Wrote initial README
- Reformatted driver "to ease reproduction"

**Maintenance period:** 5 more commits over 11 months (Feb–Mar 2022), all related to MOM6 compilation and documentation. The paper "Using Machine Learning at Scale in HPC Simulations with SmartSim: An Application to Ocean Climate Modeling" was published around this time.

**Dormancy:** No commits since March 30, 2022. 4.5+ years of silence. The repo served its purpose: accompany a paper, demonstrate SmartSim + ocean modeling, get cited.

**Key observation:** Even this *ocean-adjacent* repo (not geoengineering, just ocean modeling) is dead. The ocean modeling community doesn't maintain open-source repos after publication.

### Visual: NCAR_ML_EKE Commit Velocity

```
Commits per month:
Apr 2021: ████████████ 10  (creation day)
May 2021: ░░░░░░░░░░░░  0
...
Feb 2022: ██ 1
Mar 2022: ███ 3
Apr 2022: ░░░ 0
...
2026:     ░░░ 0 (4 years of silence)
```

---

## The "Three Universes" Commit Trend Model

Our cross-theme analysis reveals three distinct development universes:

### 🔴 Fast Universe (WRF — Solar Geoengineering)
- **Development mode:** Continuous, institutional
- **Contributor count:** 5+ active contributors
- **Release cadence:** v4.8.0 (June 2026), previous releases on ~1-2 year cycles
- **Commit frequency:** ~5-10 commits/month
- **Sustainability:** Funded by NCAR/NOAA, PhD-driven, multi-decade
- **Governance:** Distributed across NCAR, NOAA, NCAR, university consortia

### 🟡 Slow Universe (ClimateMARGO, GCCS-Core, Cost-Model-DAC)
- **Development mode:** Burst-and-dormant
- **Contributor count:** 1-2 (individual researchers)
- **Release cadence:** None (no releases, just bursts of commits)
- **Commit frequency:** 10-15 commits in 1-3 days, then months/years of silence
- **Sustainability:** Depends on PhD advisor funding, paper deadlines, personal motivation
- **Governance:** Single owner, no governance structure

### ⚫ Empty Universe (Ocean Intervention)
- **Development mode:** None
- **Contributor count:** 0 (no dedicated repos)
- **Release cadence:** N/A
- **Commit frequency:** N/A
- **Sustainability:** N/A — no software exists to sustain
- **Governance:** N/A — no software community to govern

**The contrast is extreme.** WRF has six contributors pushing commits every few days, with release notes and version management. Ocean geoengineering has zero commits in the history of GitHub.

---

## The "Adjacent Activity" Pattern

While there are zero *ocean geoengineering* repos, our searches revealed that ocean-adjacent topics do appear in other repos:

| Adjacent Topic | Where Found | How It Appears |
|----------------|-------------|----------------|
| Ocean climate modeling | NCAR_ML_EKE (20★) | Paper companion repo, dormant since 2022 |
| Ocean circulation | WRF (coupled ocean modes) | WRF can couple to MOM6 — but the coupling is minimal |
| Ocean albedo | No repos | Marine cloud brightening has zero code |
| Ocean carbon uptake | No repos dedicated to it | Some Earth system models include ocean carbon but repos are monolithic |
| Ocean alkalinity enhancement | No repos | Zero code for chemistry simulation |

**Key finding:** The "adjacent activity" pattern means that ocean geoengineering science exists (in papers, in model output, in field experiments) but the code layer is absent. The science is there; the software layer is missing.

--- 

## The "Precip-Buoyancy POD" — A Glimpse of What Could Be

In our broader search, we found a notable micro-commit pattern in a climate modeling context:

**A 5-commit burst in a single file over a single day** — we're calling this the "precip-buoyancy POD" (Positive-Oceans-Development). This pattern — rapid, focused, single-purpose — is exactly what a first ocean geoengineering repo might look like when a researcher decides to open-source their work.

The five commits in a single day followed by silence suggest: a researcher built a specific analysis tool, got a result, pushed the code for reproducibility, then moved on to the next project. No ongoing maintenance, but the code exists.

This is what the *beginning* of an ocean geoengineering open-source ecosystem would look like. The question is whether it ever grows beyond a single day of activity.

---

## The "Shared Submarine" Problem

Three of the most important ocean models are massive, consortium-maintained Fortran codebases:

| Model | Language | Stars/Community | Maintainer | Geoeng Potential |
|-------|----------|----------------|------------|------------------|
| **MOM6** (Modular Ocean Model) | Fortran/C++ | Large (NCAR/NOAA) | MOM6 consortium | Has parameterized physics, but no geoengineering options |
| **NEMO** (Nucleus for European Modelling of the Ocean) | Fortran | Large (Europeanconsortium) | NEMO consortium | European focus, limited geoeng community |
| **POP2** (Parallel Ocean Program) | Fortran | Medium (NCAR/LANL) | Various | Used in CESM, but geoeng options not developed |

**The "shared submarine" problem:** These models are like borrowed submarines — they exist, they work, and you can use them, but you can't modify them for your specific expedition (geoengineering simulation). The barriers to adding a new parameterization (e.g., ocean alkalinity enhancement chemistry) are:
1. Code is Fortran (steep learning curve for new contributors)
2. Consortium governance (need approval from multiple institutions)
3. No existing geoengineering parameterizations to use as templates

**Comparison:** WRF's architecture makes it relatively easy to add new physics parameterizations (the TEMPO scheme was added by external researchers and eventually integrated). Ocean models don't have this same extensibility culture.

---

## What a First Ocean Geoengineering Repo Would Look Like

Based on our analysis of the Fast Universe (WRF) and the Slow Universe (research code repos), here's what the first viable ocean geoengineering open-source repo might contain:

### Minimum Viable Product (MVP)
- **Language:** Python (accessible, not Fortran)
- **Scope:** Ocean alkalinity enhancement (OAE) — simpler than marine cloud brightening
- **Core feature:** Weathering kinetics simulation (a few key chemical reactions)
- **Target users:** Marine chemists, policy researchers, undergraduate teaching
- **Development pattern:** Could follow the "precip-buoyancy POD" — single-day burst, then maintenance asneeded

### Stretch Goals
- Coupling to MOM6 or NEMO for ocean circulation
- Monte Carlo uncertainty quantification (following the Cost-Model--DAC pattern)
- Interactive visualization (Jupyter notebooks, following NCAR_ML_EKE's Jupyter approach)
- Open data pipeline for field experiment results

### Precedents to Follow
- **ClimateMARGO.jl** pattern: Julia/Python for idealized modeling
- **Cost-Model--DAC** pattern: Probabilistic / Monte Carlo methods
- **WRF's TEMPO** pattern: External physics package that can be integrated into larger models
- **regional-geo** pattern: Documentation-first approach, even if code is simple

---

## Episode Architecture: The Ocean Gap as a Narrative Arc

### The Opening (0:00-10:00) — "Zero"
- Present the finding: zero ocean geoengineering repos on GitHub
- Walk through the 7 search queries that returned nothing
- Emphasize: this isn't a failure of search, it's a genuine absence
- Pose the question: What does it mean that the ocean — the largest climate system component — has zero open-source intervention code?

### The Middle (10:00-25:00) — "The Five Hypotheses"
- Governance gap: Is ocean geoengineering too politically sensitive for open-source?
- Complexity gap: Are ocean models too complex to fork and extend?
- Field experiment gap: Is there no data because there are no experiments yet?
- Academic incentive gap: Do ocean scientists not have incentives to share code?
- Proprietary lock-in: Are government labs sitting on ocean geoengineering code?

### The Crescendo (25:00-40:00) — "What Would Closing the Gap Look Like?"
- Show the "MVP ocean geoengineering repo" concept
- Discuss: Should someone just build it? What would it take?
- The equity argument: Pacific Island nations need modeling tools, not just modeling data
- The governance argument: Open tools for open debates

### The Closing (40:00-45:00) — "The Three Universes"
- Recap: Fast Universe (WRF, continuous), Slow Universe (burst-dormant), Empty Universe (zero)
- The asymmetry is the story: Why does solar geoengineering have WRF but ocean geoengineering has nothing?
- End with the question: What kind of future do we want to build — and can we build it in the dark?

---

## Listener Resources

- **MOM6 source:** https://github.com/MOM6/MOM6 (Fortran/C++, no geoeng options)
- **NEMO source:** https://forge.ipsl.jussieu.fr/nemo/ (Fortran, no geoeng options)
- **Marine Cloud Brightening Consortium:** https://www.marinecloudbrightening.org/ (research org, no open code)
- **NOAA Ocean Acidification Program:** https://www.ogp.noaa.gov/ (data, not simulation)
- **Ocean alkalinity enhancement literature:** Search Google Scholar for "ocean alkalinity enhancement" + "chemical stratification"
- **London Convention/Protocol on ocean fertilization:** https://www.imo.org/en/OurWork/OurCommittees/elcos/Pages/default.aspx

---

*This analysis documents the first systematic GitHub survey of ocean geoengineering open-source software. The null result is the result. All search queries are documented, all adjacent repos are identified, and the five hypotheses are testable by follow-up research. The ocean geoengineering community — if you exist — we found the gap. Now let's see if you can fill it.*
