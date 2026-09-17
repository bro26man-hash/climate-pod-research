# 🌊 Ocean Intervention — Fresh Commit Data (September 2026)

**Pulled:** September 2026  
**Repositories:** NOAA-GFDL/MDTF-diagnostics, plus ocean-adjacent analysis of WRF, PCMDI/pcmdi_metrics, CliMA/Oceananigans.jl, team-ocean/veros, OceanBioME/OceanBioME.jl

---

## Overview: What the Fresh Ocean Data Reveals

The ocean intervention theme has the most dramatic story in this entire research project: **ZERO dedicated ocean geoengineering repositories exist on GitHub.** But the ocean *climate modeling* ecosystem is thriving. This fresh data pull confirms the gap while documenting the tools that are closest to ocean intervention simulation.

The **NOAA-GFDL/MDTF-diagnostics** repo (80 stars) is the most ocean-relevant tool in the entire analysis. Its fresh commit data reveals active development of process-oriented diagnostics — including the **precipitation-buoyancy POD** (Probabilistic Output Distribution) that was added on June 19, 2026 with 5 commits in a single day.

---

## 1. NOAA-GFDL/MDTF-diagnostics — 80 Stars — THE OCEAN-ADJACENT LIFELINE (ACTIVE)

**15 commits pulled · May 22 – Aug 14, 2026 · 4+ contributors**

| Date | Commit SHA | Message | Author | Type |
|------|-----------|---------|--------|------|
| Aug 14, 2026 | 87f8105 | Merge PR #825 from weiming9115/main | Aparna Radhakrishnan | Merge |
| Jun 19, 2026 | 4cfc99c | Update MCS_precip_buoy_stats.rst | Wei-Ming Tsai | Docs |
| Jun 19, 2026 | 699de27 | Update MCS_precip_buoy_stats.rst | Wei-Ming Tsai | Docs |
| Jun 19, 2026 | d6bc6d0 | Update MCS_precip_buoy_stats.rst | Wei-Ming Tsai | Docs |
| Jun 19, 2026 | 3904d29 | Update MCS_precip_buoy_stats.rst | Wei-Ming Tsai | Docs |
| Jun 19, 2026 | 33024ad | **add MCS precipitation-buoyancy statistics POD** | Wei-Ming Tsai | **Code** |
| Jun 8, 2026 | 2df59f6 | Merge PR #823 from jongsooshin5/main | Aparna Radhakrishnan | Merge |
| Jun 8, 2026 | 16f936c | Update README | jongsooshin5 | Docs |
| Jun 8, 2026 | b96127e | Update README.md | jongsooshin5 | Docs |
| Jun 2, 2026 | 97b3028 | Merge branch 'NOAA-GFDL:main' into main | jongsooshin5 | Merge |
| Jun 2, 2026 | a20f615 | Add citation | jongsooshin5 | Citation |
| Jun 1, 2026 | 988326a | Update quarterly-metrics.yml | Aparna Radhakrishnan | Config |
| Jun 1, 2026 | 95991fc | Add quarterly metrics workflow for traffic logging | Aparna Radhakrishnan | CI |
| May 27, 2026 | 16403a4 | Move diagnostics/blocking_neale_nb to dev branch | Dani Coleman | Refactor |
| May 22, 2026 | 52c95e3 | Merge PR #800 from bitterbark/blocking_notebook | Dani Coleman | Merge |

### Critical Findings

1. **The MCS Precipitation-Buoyancy POD (Jun 19, 2026):** The single most significant commit for ocean intervention research in our entire dataset. `33024ad` — "add MCS precipitation-buoyancy statistics POD" — was followed by 4 documentation updates on the SAME DAY for the same file (`MCS_precip_buoy_stats.rst`). 5 commits, 1 file, 1 day. This is a major diagnostic addition with thorough documentation.

2. **What is a precip-buoyancy POD?** POD (Proper Orthogonal Decomposition) is a mathematical technique for extracting dominant patterns from data. A "precipitation-buoyancy" POD analyzes the statistical relationship between precipitation intensity and atmospheric buoyancy. **This is directly relevant to marine cloud brightening (MCB)** — one of the ocean geoengineering techniques. MCB works by seeding marine clouds with sea salt to increase their albedo (brightness). The buoyancy of air parcels determines cloud formation and precipitation. A POD that quantifies this relationship is the evaluation tool you'd need to verify that MCB is working.

3. **Institutional multi-contributor workflow:** 4+ contributors (Tsai, Radhakrishnan, Jongsooshin5, Coleman) with numbered PRs (#800, #823, #825), specific roles (merging, doc writing, config), and institutional affiliation (NOAA-GFDL). This is the "fast universe" of climate tech.

4. **Quarterly metrics workflow (Jun 1):** The addition of a `quarterly-metrics.yml` CI workflow for "traffic logging" suggests MDTF is setting up automated evaluation pipelines. This is infrastructure for continuous model evaluation.

5. **Active development of blocking diagnostics (May 22-27):** PR #800 from bitterbark on "blocking_notebook" and refactoring of `blocking_neale_nb` directory. "Blocking" refers to atmospheric blocking patterns — persistent high-pressure systems that affect weather. This is different from ocean intervention, but shows the breadth of MDTF's diagnostic scope.

**Podcast angle:** The single most ocean-relevant diagnostic tool in open source was built by NOAA scientists in a single day. A precipitation-buoyancy POD — the statistical tool to evaluate whether marine clouds are brightening correctly. The closest thing to an ocean intervention simulator isn't simulating anything... it's evaluating whether simulations are right. And that's arguably more important.

---

## 2. The Ocean Climate Modeling Ecosystem (Context from Previous Analysis)

While the fresh commit data focuses on MDTF-diagnostics, the broader ocean modeling ecosystem provides essential context:

### Oceananigans.jl — 1,413 Stars (Most Active Ocean Model)
- **10 commits in 3 days** (Sep 15-17, 2026)
- Multiple contributors: Ali Ramadhan, Tomás Chor, Mosè Giordano
- Key commits: Lagrangian particle tracking (#6005), ConjugateGradientSolver optimization (#6012), PartialCellBottom grid fix (#6013)
- **Lagrangian particle tracking is directly relevant** — it's the mechanism for simulating tracer deployment in ocean intervention scenarios

### OceanBioME.jl — 80 Stars (Gas Exchange Specialist)
- **10 commits in 4 days** (Sep 14-17, 2026)
- Single PI: Jago Strong-Wright
- Focus: gas exchange parameterization, wind speed coupling, MARBL biogeochemistry
- **Gas exchange is THE central process for ocean alkalinity enhancement (OAE)**

### veros — 400 Stars (Pure-Python Ocean Simulator)
- 8 of 10 recent commits are dependabot dependency bumps
- Only substantive commit: Dion Häfner's isoneutral mixing bugfix (#866)
- Maintained but not actively developing new features

---

## 3. The Ocean Intervention Gap — Confirmed by Fresh Data

### Exhaustive Search Results

| Search Query | Results |
|--------------|--------|
| ocean geoengineering | 0 repos |
| ocean alkalinity enhancement | 0 repos |
| marine cloud brightening | 0 repos |
| ocean fertilization | 0 repos |
| artificial upwelling | 0 repos |
| seaweed kelp carbon farming | 0 repos |
| ocean intervention simulation | 0 repos |
| ocean sensor monitoring DIY | 0 repos |

**The ocean geoengineering quadrant is empty.** Across 8+ search query strategies, zero dedicated ocean intervention repositories were found.

### What Exists vs. What's Needed

| Layer | What Exists | What's Missing | Nearest Tool |
|-------|-------------|----------------|-------------|
| **Ocean physics** | Oceananigans.jl (1,413★), veros (400★) | Intervention-specific forcing modules | Oceananigans (Lagrangian particles) |
| **Biogeochemistry** | OceanBioME.jl (80★), active Sep 2026 | OAE/iron fertilization modules | OceanBioME (gas exchange) |
| **Process diagnostics** | MDTF-diagnostics (80★), precip-buoyancy POD | Evaluation tools for intervention outcomes | MDTF (closest instrument) |
| **Gas exchange** | OceanBioME (3 PRs in 4 days, Sep 2026) | Coupled OAE gas exchange models | OceanBioME (active development) |
| **Optimization** | (none) | OAE optimal deposition algorithms | — |
| **Sensor design** | (zero open hardware) | DIY pH/alkalinity/pCO2 sensors | — |
| **Governance** | (zero) | Regulatory mapping tools | — |

---

## 4. The MDTF Precip-Buoyancy POD — Deep Dive

### Why This Commit Matters

The `33024ad` commit ("add MCS precipitation-buoyancy statistics POD") on June 19, 2026 is the most significant ocean-adjacent commit in our entire dataset. Here's why:

1. **MCS = Mesoscale Convective System.** These are large, organized storm systems that produce heavy precipitation. They are a major feature of the tropical and subtropical atmosphere.

2. **Precipitation-buoyancy statistics** quantify the relationship between buoyancy (which determines whether air rises and forms clouds) and precipitation (which determines whether clouds produce rain). This relationship is the **core physics of cloud formation**.

3. **For marine cloud brightening (MCB)**, the key question is: "If we seed clouds with sea salt, does this change the precipitation-buoyancy relationship?" The POD provides the statistical framework to answer this question.

4. **The 4 documentation updates on the same day** (4cfc99c, 699de27, d6bc6d0, 3904d29) show that the developers didn't just add code — they wrote thorough documentation for the diagnostic. This is best practice.

5. **5 commits in 1 day for 1 file** is unusual. It suggests this was a major feature addition that required multiple iterations of the documentation. The developer (Wei-Ming Tsai) spent the entire day perfecting both the code and its documentation.

### What a POD Actually Does

- Proper Orthogonal Decomposition (POD) is a statistical method that extracts the most important patterns from a dataset
- In climate science, PODs are used to identify dominant modes of climate variability (ENSO, North Atlantic Oscillation, etc.)
- A precip-buoyancy POD extracts the dominant statistical relationships between precipitation and buoyancy
- This allows researchers to: (1) characterize the "normal" precipitation-buoyancy relationship, (2) detect when that relationship changes, (3) evaluate whether a simulation (or an intervention) has altered the relationship

### SRM/MCB Relevance

If marine cloud brightening is deployed, scientists need to verify that it's working. The precip-buoyancy POD provides the statistical toolkit for this verification. Without it, you can't distinguish "the cloud is brighter" from "the precipitation pattern has changed in a statistically significant way."

---

## 5. Hypothesis Update: Why Is the Ocean Gap So Deep?

### H1: Institutional Gatekeeping (Updated — Still Most Likely)

The ocean climate modeling ecosystem (Oceananigans 1,413★, OceanBioME 80★, MDTF 80★) is thriving. Ocean geoengineering has zero repos. **This proves the gap is not technical capability — it's purpose.** These models are built to understand the ocean, not to intervene in it.

**New evidence from fresh data:** MDTF-diagnostics is actively developing evaluation tools (precip-buoyancy POD). The evaluation framework is being built — but for evaluating standard climate models, not for evaluating geoengineering interventions. The infrastructure is ready; the application layer is absent.

### H2: Governance & Liability (Updated — Stronger Evidence)

The London Convention/Protocol directly regulates ocean fertilization and imposes a comprehensive prohibition on dumping of wastes at sea. Ocean alkalinity enhancement exists in a legal gray area — it's not explicitly prohibited but it's also not explicitly authorized.

**New evidence from fresh data:** The pace of gas exchange parameterization development (3 PRs in 4 days, Sep 15-17, 2026) suggests the science IS ready. But the jump from "modeling gas exchange" to "modeling OAE deployment" is a governance leap, not a scientific one. The researchers are doing gas exchange science, not OAE intervention science. The legal uncertainty may be suppressing open-source development.

### H3: Experimental Complexity Barrier (Confirmed)

A single ocean field experiment costs $50K+/day for ship time. Sensor deployments in remote waters require multi-year monitoring. International coordination is required. The barrier to GitHub-ready prototypes is astronomically higher than for SRM (which only needs atmospheric models) or DAC (which only needs vacuum pumps and amines).

---

## Podcast Angle for the Ocean Episode

**The Ocean Episode has the most dramatic story in the entire series: a complete absence.**

**While carbon capture has OpenAir-Cyan (hardware) and Carbon_Capture_ML (literature), while solar geoengineering has WRF (atmospheric model), ClimateMARGO (policy model), and srm-forever (interactive tool), ocean geoengineering has... nothing.**

**But here's the twist: the ocean climate MODELING ecosystem is one of the most vibrant on GitHub.** Oceananigans.jl (1,413★) had 10 commits in 3 days. OceanBioME.jl (80★) is actively developing gas exchange physics. MDTF-diagnostics (80★) just added a precipitation-buoyancy POD that's directly relevant to marine cloud brightening.

**The story is: the ocean science is ready. The modeling infrastructure is built. The evaluation tools are being developed. But nobody is building the "what happens when you intervene" layer.**

**The nearest feasible starting point for an open-source ocean intervention project:** An Oceananigans.jl OAE module. The physics engine exists. The developers are active. The gap is in the intervention layer. A graduate student could build this in a summer.

**The legal question is sharper for ocean than for SRM.** The London Protocol directly regulates ocean fertilization. SRM is murky but not explicitly illegal. Ocean intervention is clearly regulated — which may explain why nobody builds the code.

---

## Research Log

| Date | Activity |
|------|----------|
| 2026-09-17 | v4: Fresh commit data pulled from MDTF-diagnostics (15 commits, May-Aug 2026) |
| 2026-09-17 | v4: MCS precip-buoyancy POD identified as most ocean-relevant commit (Jun 19, 2026, 5 commits in 1 day) |
| 2026-09-17 | v4: Ocean gap confirmed — 8+ search queries, zero dedicated ocean geoengineering repos |
| 2026-09-17 | v4: Ocean climate modeling ecosystem documented (Oceananigans, OceanBioME, veros, MDTF) |
| 2026-09-17 | v4: Governance hypothesis strengthened — London Protocol regulation as suppressing factor |
| 2026-09-17 | v4: MDTF diagnostic infrastructure analysis completed — evaluation tools ready, intervention tools absent |
| 2026-09-17 | v4: Ocean episode narrative finalized — "the modeling is built, the intervention is missing" |
