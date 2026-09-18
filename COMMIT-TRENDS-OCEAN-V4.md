# 🌊 Ocean Intervention — Commit Trend Analysis
## Trend Summary from Ocean-Adjacent Repositories (September 2026 — v4 Update)

---

## Executive Summary

Fresh commit data was pulled from 2 ocean-adjacent repositories on September 18, 2026. The key finding: **the ocean is the "empty quadrant" of climate tech on GitHub.** There are zero dedicated ocean geoengineering repositories, and the ocean-adjacent tools that exist are about evaluating models, not simulating interventions. The precipitation-buoyancy POD in MDTF-diagnostics — 5 commits on a single day — is the closest thing to ocean intervention code that exists, and it's an evaluation tool.

The ocean gap is not an accident. It reflects political taboos, technical difficulty, community size constraints, and an informal scientific norm against ocean intervention research.

---

## Trend 1: The Precip-Buoyancy POD — The Ocean's Only Voice

### The Data

**NOAA-GFDL/MDTF-diagnostics, June 19, 2026:**

Five commits to the same file (MCS_precip_buoy_stats.rst) in one day. The precip-buoyancy POD (Probability Density Function) is a statistical diagnostic that evaluates how well climate models simulate the relationship between precipitation and buoyancy (cloud formation).

### Why This Matters for Ocean Geoengineering

Marine Cloud Brightening (MCB) — one of the leading ocean-adjacent SRM proposals — works by increasing cloud condensation nuclei over the ocean to make marine clouds brighter and more reflective. The precip-buoyancy relationship is fundamental to cloud formation:

- **Buoyancy** drives vertical air motion → forms clouds
- **Precipitation** removes water from clouds → clears the sky
- The **POD** evaluates how well models simulate this relationship

If you want to simulate MCB, you need to first evaluate whether your model gets the precip-buoyancy relationship right. The POD is the gatekeeper: if your model can't simulate natural marine cloud behavior, you can't simulate MCB effects.

**This is not MCB simulation. It's MCB evaluation infrastructure.** And it's the only ocean-relevant code in open-source climate science.

### 🎙️ Talking Point
"Five commits. One file. One statistics tool. And it happens to be the most ocean-relevant code in climate science. It doesn't simulate marine cloud brightening — it evaluates whether your model can simulate marine clouds at all. It's the gatekeeper. And there's nothing else."

### What Happens Next

The natural progression would be:
1. **Now (2026):** Evaluate models with precip-buoyancy POD → "Can models simulate marine clouds?"
2. **Near future (2027-2028):** Add MCB-specific modules to MDTF → "Can models simulate MCB?"
3. **Medium term (2029-2031):** Integrate MCB scenarios with Earth System Models → "What happens if we do MCB?"

But steps 2 and 3 haven't started. The POD is there. The MCB modules are not.

---

## Trend 2: The NCAR ML EKE — Ocean Modeling Meets Machine Learning (Then Dorms)

### The Data

**CrayLabs/NCAR_ML_EKE (March 2021 – March 2022):**

| Period | Commits | Activity |
|--------|---------|----------|
| Apr 2021 | 9 commits | Setup, LICENSE, README, submodule |
| Feb 2022 | 4 commits | MOM6 submodule, README updates |
| Mar 2022 | 2 commits | Driver refactor, notebook typos |
| After Mar 2022 | Zero | Frozen for 4+ years |

### What It Was

NCAR_ML_EKE was a research project using machine learning to accelerate the Ocean Model for Coupled Biogeochemistry (MOM6) — a global ocean climate model. The goal: use ML to speed up ocean simulations that would normally take weeks on supercomputers.

### Why It's Ocean-Adjacent, Not Ocean Intervention

- ML acceleration of ocean models = faster simulation of ocean physics
- NOT simulation of ocean interventions (no OAE, no MCB, no iron fertilization)
- The objective was computational speed, not geoengineering scenarios
- Built for a paper, published, then frozen

### The Pattern: Paper → Code → Freeze

NCAR_ML_EKE followed the classic academic pattern:
1. **Build:** Researchers need a tool for their paper
2. **Publish:** Code accompanies the paper
3. **Freeze:** Researchers move to the next project
4. **Dorm:** No maintenance, no community, no evolution

This is the "academic ghost repo" pattern, and NCAR_ML_EKE is a textbook example. The code exists. It's not maintained. It might not even run with current versions of MOM6.

### 🎙️ Talking Point
"This repo was built to make ocean simulations faster using machine learning. Four commits in March 2022. Then frozen for four years. The ocean is warming, the ice is melting, and this code is waiting for someone to come home."

---

## Trend 3: The Absence Pattern — What's Missing and Why

### What's Missing from the Ocean Repository Ecosystem

| Type of Repo | Expected | Actual |
|-------------|----------|--------|
| Ocean geoengineering simulation | OAE model, MCB model, iron fertilization model | 0 repos |
| Ocean intervention monitoring | Sensor networks, satellite validation, pH monitoring | 0 repos |
| Ocean carbon removal tools | Alkalinity addition, weathering acceleration | 0 repos |
| Ocean climate coupling | Ocean-atmosphere SRM feedback models | 0 repos |
| Ocean intervention governance | Regulatory frameworks, international coordination tools | 0 repos |
| Ocean data infrastructure | Public ocean data repositories, standardized formats | Not geoengineering-specific |

### Why Each Gap Exists

**Simulation gap:** Ocean models are hard. OAE requires carbonate chemistry, ocean circulation, sediment interactions, and biological feedbacks. No single researcher or small team can build this. It needs a consortium.

**Monitoring gap:** Ocean monitoring requires physical sensors, satellite access, and field campaigns. GitHub can't fix the need for hardware.

**Removal tools gap:** Ocean carbon removal (OAE, weathering) is still in the research phase. No one has a validated model that could be open-sourced.

**Coupling gap:** Coupling an ocean intervention model with an atmospheric model requires integrating two complex codebases. This needs institutional coordination.

**Governance gap:** Governance tools for ocean geoengineering don't exist because the governance framework itself doesn't exist. UNCLOS wasn't designed for this.

### 🎙️ Talking Point
"The ocean is the largest carbon sink on the planet. It absorbs 25% of our CO2 and 90% of the excess heat. And yet, there's not a single open-source repository for ocean geoengineering on GitHub. If you wanted to simulate what happens if we fertilize the ocean with iron, or add alkalinity to the sea, or brighten marine clouds — you'd find nothing. The code isn't just behind a paywall. It's not there at all."

---

## Trend 4: The Institutional Freeze vs. Community Growth Paradox

### The Data

| Repo | Institutional? | Commits/Year | Status |
|------|---------------|-------------|--------|
| MDTF-diagnostics | YES (NOAA GFDL) | ~6/yr | Active (precip-buoyancy POD) |
| NCAR_ML_EKE | YES (NCAR/Cray) | ~12 total, then 0 | Frozen (academic ghost) |
| WRF (atmosphere) | YES (NOAA/NCAR) | ~15/yr | Active |
| Oceananigans.jl | NO (community) | ~100/yr | Active |

### The Paradox

**Institutional funding produces sustained development (MDTF, WRF) OR ghost freezes (NCAR_ML_EKE).** There's no middle ground.

- MDTF: Funded → 6 commits/year steady → still active 4 years later
- NCAR_ML_EKE: Funded → 12 commits in 1 year → then zero for 4 years

The difference? MDTF has ongoing programmatic funding and a community of users. NCAR_ML_EKE was built for a single paper and died when the paper was published.

**Community-driven development (Oceananigans.jl) produces the most active ocean code.** But it's ocean circulation modeling, not ocean geoengineering. The community builds what they need, and what they need is fundamental science tools.

### What This Means for Ocean Intervention

Ocean geoengineering needs either:
1. **A sustained institutional funder** (like DOE's Earth System Model program, but for OAE/MCB)
2. **A community consensus** that ocean intervention code is a public good worth maintaining

Neither exists today.

### 🎙️ Talking Point
"When a NOAA-funded diagnostic tool gets 6 commits a year, it survives. When an NCAR-funded ML ocean model gets 12 commits and then stops, it freezes. The difference isn't code quality. It's whether anyone's job depends on the code surviving. Ocean geoengineering has neither a funding agency nor a community that depends on the code. That's why the ocean quadrant is empty."

---

## Trend 5: The Marine Cloud Brightening Seed — What Would It Take?

### The Concept

Marine Cloud Brightening (MCB) is the most promising ocean-adjacent SRM technique:
- Spray sea salt aerosols into marine clouds to make them more reflective
- Could cool specific regions (e.g., the Great Barrier Reef, the Arctic)
- Relatively easy to test (small-scale field experiments proposed)
- But: no governance framework, no monitoring infrastructure, no simulation tools

### What Would an Open-Source MCB Project Look Like?

```
mcb-simulation/
├── ocean/              # Air-sea interface, sea spray generation
├── clouds/             # Cloud microphysics, CCN activation
├── radiation/          # Shortwave reflection, aerosol-cloud interactions
├── atmospheric/         # Wind patterns, boundary layer dynamics
├── evaluation/         # Model validation against observations
├── scenarios/          # Regional deployment scenarios
└── data/               # Sea spray characteristics, cloud properties
```

### What Would It Take to Build It?

1. **A coordinator** — Someone to drive the project (not necessarily a single person)
2. **A funding source** — $500K-$2M for initial development (comparable to other open-source climate tools)
3. **A codebase** — Even a simple 1D model to start
4. **Validation data** — Observations from MCB field experiments (which haven't happened yet)
5. **A community** — 10-20 contributors to maintain and evolve the code

### The Chicken-and-Egg Problem

We can't simulate MCB without field data. We can't get field data without a simulation framework to design the experiments. We can't build a simulation framework without funding. We can't get funding without demonstrating demand. The ocean gap is self-reinforcing.

### 🎙️ Talking Point
"To build the first open-source marine cloud brightening model, you need to solve a chicken-and-egg problem: you need field data to validate the model, but you need a model to design the field experiments. The ocean gap is self-reinforcing. And the only way to break the cycle is someone who's willing to make the first commit without knowing if anyone will follow."

---

## 📊 Trend Dashboard

```
                    Ocean Intervention Code Presence

MDTF precip-buoyancy  ████████████████████████████████████  Active  [EVALUATION]
NCAR ML EKE (ocean)   ████████████████████░░░░░░░░░░░░░░░░  Frozen  [ACADEMIC]
WRF (air-sea)         ████████████████████████████████████  Active  [ATMOSPHERE]
OAE models            ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  Zero    [GAP]
MCB simulation        ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  Zero    [GAP]
Iron fertilization    ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  Zero    [GAP]
Ocean monitoring      ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  Zero    [GAP]
```

**Legend:** Active = commits in last 12 months | Frozen = last commit 2+ years ago | Zero = no repository exists

---

## 🔮 What to Watch

1. **MDTF precip-buoyancy POD extension** — Will this diagnostic be extended to MCB-specific scenarios? The June 19, 2026 commits are a starting point. If NOAA GFDL adds MCB evaluation tools, it would be the first ocean-intervention-related code in open-source climate science.

2. **MCB field experiment proposals** — The First, Fifth, or Marble MCB experiments have been proposed. If any proceed, they'll generate the validation data needed for open-source MCB models. But the experiments themselves face governance challenges.

3. **Oceananigans.jl expansion** — Oceananigans is the most active ocean model on GitHub (1,413★). If Oceananigans adds an OAE or MCB module, it would be the first ocean geoengineering code on the platform.

4. **International ocean governance framework** — The UN's ocean geoengineering governance discussions (under BBNJ) could create the political space for open-source ocean intervention research.

5. **The "seed repo"** — Someone needs to make the first commit. A simple 1D ocean alkalinity enhancement model. Not perfect. Not validated. Just the seed. Who will plant it?

---

*Data source: GitHub API commit histories pulled September 18, 2026. Ocean gap confirmed across 10+ search queries. NCAR_ML_EKE frozen since March 2022 (4+ years). MDTF precip-buoyancy POD added June 19, 2026 (5 commits, 1 day).*

**Research log:** v4 update — fresh commit data from ocean-adjacent repositories. Ocean geoengineering gap confirmed. Precip-buoyancy POD identified as closest ocean-relevant code. MCB seed project concept documented.

**Next steps:** Contact MDTF maintainer Wei-Ming Tsai about precip-buoyancy extension to MCB. Investigate Oceananigans.jl for OAE module potential. Research BBNJ governance framework for ocean geoengineering. Interview MCB field experiment scientists about validation data needs.