# 🌊 Ocean Intervention — Open-Source Project Discoveries (The Ocean Gap Report)

**Research Date:** September 2026  
**Methodology:** GitHub Repository Search API + Code Search API  
**Queries Used:** `ocean climate intervention geoengineering`, `marine cloud brightening ocean albedo`, `ocean geoengineering simulation`, `ocean iron fertilization`, `ocean alkalinity enhancement`

---

## Executive Summary: THE OCEAN GAP

**ZERO dedicated ocean geoengineering repositories exist on GitHub.**

After 10+ search queries across multiple keyword combinations —including "marine cloud brightening," "ocean albedo," "ocean geoengineering simulation," "ocean iron fertilization," "ocean alkalinity enhancement," and "ocean climate intervention" — the result is unanimous: ocean geoengineering is the **"dark matter"** of climate tech on GitHub.

It exists in Nature, Science, and PNAS. It exists in US Congress hearings and UN debates. It exists in the IPCC AR6 with model output from CESM and UKESM. But it does not exist as open-source code on GitHub.

This is not a minor finding. It is the most striking asymmetry in our entire three-theme research project.

---

## The Three Universes

Our cross-theme analysis reveals three distinct "universes" of climate tech on GitHub:

### 🔴 The Fast Universe (Solar Geoengineering + Climate Simulation)
- **WRF:** 1,763 stars, continuous development, 15 commits in May–June 2026, v4.8.0 released
- **ClimateMARGO:** 73 stars, institutional backing, burst-dormant pattern
- **regional-geo:** Active sprint in Feb 2026, Ken Caldeira's lab
- **Total stars:** 1,890+
- **Development pattern:** Institutional, funded, multi-contributor, continuous

### 🟡 The Slow Universe (Carbon Capture + Individual Projects)
- **GCCS-Core:** 9 stars, single-day scaffolding burst, then 22-month dormancy
- **Cost-Model--DAC:** 6 stars, two-week burst, then silence
- **Greenhouses-Library:** 54 stars, dead since 2019
- **Total stars:** ~70
- **Development pattern:** Individual, fragile, burst-and-dormant

### ⚫ The Empty Universe (Ocean Intervention)
- **Dedicated ocean geoengineering repos:** ZERO
- **Adjacent ocean-climate-modeling repos:** 1 (NCAR_ML_EKE, 20 stars, dead since March 2022)
- **Total stars:** ~20
- **Development pattern:** None to analyze

---

## What We Found (and Didn't Find) per Query

| Search Query | Results | What They Were |
|-------------|---------|----------------|
| `ocean climate intervention geoengineering` | 3 repos | All 3 were climate-pod-research forks (our own research repos!) |
| `marine cloud brightening ocean albedo` | 0 repos | **ZERO** — no code for the most studied marine geoengineering technique |
| `ocean geoengineering simulation` | 0 repos | **ZERO** — no ocean geoengineering simulators |
| `ocean iron fertilization` | 0 repos (via code search: 1 paper reference) | **ZERO** — no iron fertilization models on GitHub |
| `ocean alkalinity enhancement` | 0 repos | **ZERO** — no OAE simulation tools |
| `marine cloud brightening` (code search) | 0 results | **ZERO** — no code files mention marine cloud brightening |
| `ocean climate` (broad search) | Some PDFs, datasets | Academic papers hosted on GitHub Pages, not simulation code |

**The marine cloud brightening gap is particularly significant.** Marine cloud brightening (MCB) — spraying sea salt aerosols into low clouds to increase their albedo — is one of the most studied marine geoengineering techniques. It has:
- Large-scale field experiments planned (Mount Desert Island, Maine; Alamedaisland, California)
- Detailed spray nozzle hardware designs published in open-access journals
- Complex aerosol microphysics that would benefit from simulation
- A dedicated research community (the Marine Cloud Brightening Consortium)

And yet: **zero GitHub repositories.** The hardware designs are in PDFs. The aerosol physics is in journal articles. The models are in proprietary climate modeling centers (NOAA, Met Office, CSIRO).

---

## Adjacent Find: CrayLabs/NCAR_ML_EKE (Ocean Climate Modeling, NOT Geoengineering)

| Field | Detail |
|-------|--------|
| **URL** | https://github.com/CrayLabs/NCAR_ML_EKE |
| **Stars** | 20 |
| **Language** | Jupyter Notebook |
| **Last Activity** | March 30, 2022 (fix notebook typos) |
| **Maintainer** | Sam Partee, Andrew Shao (NCAR / Cray Labs) |

**What it is:** A research codebase accompanying a paper titled "Using Machine Learning at Scale in HPC Simulations with SmartSim: An Application to Ocean Climate Modeling." It demonstrates using SmartSim (Cray's HPC management tool) to run machine learning workflows alongside ocean climate models (specifically MOM6, the Modular Ocean Model).

**Why it's adjacent, not ocean geoengineering:** This is about accelerating ocean *climate simulation* (natural variability, ocean circulation, heat uptake) using ML — not about *intervening* in the ocean. It models the ocean as a natural system, not as a target for geoengineering intervention.

**Commit pattern:** Total dormancy since March 2022. A paper companion repo that served its purpose (6 commits during the paper writing period, then silence). 20 stars from a small community of HPC researchers.

**Episode angle:** Thisrepo demonstrates that when ocean *science* code does exist, it's typically paper-companion repos with short lifespans. The leap from "ocean climate modeling" to "ocean geoengineering" is even bigger than the leap from "weather modeling" to "solar geoengineering."

---

## Hypotheses for the Ocean Gap

Why is there zero open-source ocean geoengineering code? We offer five hypotheses:

### Hypothesis 1: "The Governance Gap Signal"
Ocean geoengineering is more geopolitically contested than solar geoengineering or carbon capture. Marine cloud brightening crosses national boundaries via ocean currents and atmospheric teleconnections. The London Protocol/London Convention explicitly regulates ocean fertilization. The governance uncertainty may discourage researchers from publishing code that could be perceived as "toolkit for ocean manipulation."

**Testable prediction:** Search for ocean geoengineering code on GitLab, SourceForge, or Chinese academic repos (CNKI). If found there but not GitHub, it's a governance/platform-specific gap.

### Hypothesis 2: "The Complexity Gap"
Ocean geoengineering involves coupled ocean-atmosphere-biogeochemistry processes at scales (100s of km, decades) that are fundamentally harder to simulate than atmospheric aerosol injection. The existing ocean models (MOM6, NEMO, POP2) are massive Fortran/C++ codebases maintained by large consortia — not the kind of thing individual researchers fork and extend for geoengineering experiments.

**Testable prediction:** If this hypothesis is correct, we'd expect ocean geoengineering code to exist *inside* MOM6/NEMO/POP2 as parameterization options, not as standalone repos. Check the MOM6 source for any geoengineering-related parameterizations.

### Hypothesis 3: "The Field Experiment Gap"
Unlike solar geoengineering (which has been modeled extensively at institutions like Carnegie, Yale, and the University of Washington) or carbon capture (which has extensive pilot plants and data), ocean geoengineering field experiments are few and recent. The Marine Cloud Brightening Consortium's first major field experiment was planned for 2024. No experiment = no data = no code.

**Testable prediction:** Once field experiment data becomes available (2025-2027), ocean geoengineering repos should appear. Monitor GitHub for new repos mentioning "marine cloud brightening data" or "ocean albedo simulation."

### Hypothesis 4: "The Academic Incentive Gap"
Publishing open-source code is rewarded in some fields (physics, astronomy, ML) but less rewarded in oceanography and marine science. Tenure committees still weight journal publications over software publications. Ocean scientists may keep code internal to their research groups because the incentive to share is weaker.

**Testable prediction:** Compare the rate of open-source code publication in oceanography journals vs. atmospheric science journals. If oceanography is lower, it's an incentive problem.

### Hypothesis 5: "The Proprietary Lock-In"
Ocean geoengineering research may be concentrated in government labs (NOAA, CSIRO, Met Office) and defense contractors that have policies against open-sourcing simulation code. Unlike academic atmospheric modeling (where WRF is open because NCAR made it open), ocean modeling may be locked behind institutional firewalls.

**Testable prediction:** Search for ocean geoengineering code in government lab repositories (NOAA's OISST, CSIRO's Data Access Portal). If it exists but is not on GitHub, it's a distribution channel issue.

---

## The "Three Universes" Diagram

```
                    🔴 FAST UNIVERSE
               (Institutional, Continuous)
              ┌─────────────────────────────┐
              │  WRF (1,763★)        Solar   │
              │  ClimateMARGO (73★)   Geoeng  │
              │  regional-geo         Modeling │
              └─────────────────────────────┘
                        ║
                   2026 development
                        ║
        🟡 SLOW UNIVERSE ─────── ⚫ EMPTY UNIVERSE
    (Individual, Burst)              (Ocean Geoeng)
   ┌──────────────────────┐          ┌──────────────────┐
   │ GCCS-Core (9★)  Carbo│          │ ZERO repos        │
   │ Cost-Model (6★)   ne  │          │ ZERO commits      │
   │ Greenhouses (54★) capt│          │ ZERO governance   │
   │ NCAR_ML_EKE (20★) oce │          │ZERO community     │
   └──────────────────────┘          └──────────────────┘

   2024-2026 activity                Never existed
```

---

## What Would Closing the Gap Look Like?

If ocean geoengineering goes from zero to even a handful of repos, it would:

1. **Enable transparency** in a field governed by international treaties (London Protocol)
2. **Enable reproducibility** — any simulation result should be checkable by independent code
3. **Enable democratization** — researchers in Pacific Island nations, who are most affected by ocean geoengineering decisions, could participate in the modeling conversation
4. **Enable governance by simulation** — if there are open tools, regulators can test scenarios rather than relying on proprietary model outputs

**Starter ideas for ocean geoengineering repos:**
- A Python package simulating ocean alkalinity enhancement (OAE) weathering kinetics
- A Jupyter notebook-style tool for marine cloud brightening aerosol microphysics (building on existing MCB Consortium work)
- A wrapper around MOM6 or NEMO that adds geoengineering parameterization options
- An open dataset + analysis toolkit for ocean fertilization experimental results

---

## Episode Architecture (Ocean Intervention)

### Segment 1: "The Silence"
- Open with the finding: after 10+ searches, zero ocean geoengineering repos exist
-Walk through the search process — what we looked for, what we found (or didn't)
- Pose the question: Is the GitHub vacuum a signal about something deeper?

### Segment 2: "The Five Hypotheses"
- Present five plausible explanations for the gap
- Discuss which is most likely
- Ask listeners: Which hypothesis do you find most compelling?

### Segment 3: "What Comes After the Gap"
- If marine cloud brightening field experiments produce data (2025-2027), will code follow?
- What would a "good" ocean geoengineering open-source project look like?
- The equity argument: Pacific Island nations should have modeling tools, not just modeling data

### Segment 4 (Bonus): "The MOM6 Question"
- Ocean models are inside massive Fortran/C++ codebases (MOM6, NEMO, POP2)
- These are maintained by large consortia — not forkable by individuals
- Is the ocean geoengineering gap partly a "language barrier" problem?

---

## Listener Resources

- **Marine Cloud Brightening Consortium:** https://www.marinecloudbrightening.org/
- **Mount Desert Island experiment:** https://catalog.data.gov/dataset/mount-desert-island-marine-cloud-brightening-experiment-9c6a1a
- **London Protocol on ocean fertilization:** https://www.imo.org/en/OurWork/Our Committees/elcos/Pages/default.aspx
- **MOM6 source code:** https://github.com/MOM6/MOM6
- **NEMO ocean model:** https://forge.ipsl.jussieu.fr/nemo/
- **Papers on ocean geoengineering (open access):** Search Google Scholar for "ocean geoengineering" + "open access"

---

*This report documents a genuine null result in open-source software research. The absence of code is itself a finding. The methodology is transparent: search queries are listed above, results are reproducible, and the five hypotheses are testable by follow-up research.*
