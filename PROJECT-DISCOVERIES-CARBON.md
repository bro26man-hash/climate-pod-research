# 🌍 Carbon Capture — Open-Source Project Discoveries

**Research Date:** September 2026  
**Methodology:** GitHub Repository Search API + Code Search API  
**Queries Used:** `carbon capture removal climate tech stars:>5`, `direct air capture DAC stars:>5`, `climate technology carbon capture ocean`

---

## Executive Summary

Our search for open-source carbon capture / direct air capture (DAC) repositories revealed a **small but emerging ecosystem** — significantly more developed than ocean geoengineering (zero repos) but far less active than solar simulation (WRF with 1,763 stars). The two most relevant repos are:

1. **KOSASIH/GCCS-Core** (9 stars) — A Python framework for a "Global Climate Control System" with a single-day scaffolding burst
2. **kfdsievert/Cost-Model--DAC** (6 stars) — A probabilistic cost model for Direct Air Capture using experience curves and Monte Carlo simulation

**Headline finding:** The carbon capture open-source ecosystem is in its "proof of concept" phase. Unlike solar geoengineering (where SRM code is embedded in mainstream climate models like WRF), carbon capture has *no* dominant simulation framework. The most active repo (GCCS-Core) is a single-day scaffolding project, not a mature tool.

---

## Project Profiles

### 1. 🏗️ KOSASIH/GCCS-Core — The Scaffolding

| Field | Detail |
|-------|--------|
| **URL** | https://github.com/KOSASIH/GCCS-Core |
| **Stars** | 9 |
| **Language** | Python |
| **Last Activity** | October 29, 2024 |
| **Maintainer** | KOSASIH (solo developer) |

**What it claims to be:** The foundational framework for a "Global Climate Control System" — encompassing core algorithms, data management, and deployment infrastructure.

**What it actually is:** A single-day scaffolding burst. All 15 commits occurred on October 29, 2024, within hours of each other. The commit sequence reveals the standard project initialization pattern:

```
10/29, 07:00-08:00 — create_example_config.yaml, example_usage.py, example_iot_integration.py
10/29, 08:00-09:00 — create deploy.sh, run_server.sh, data_collection.sh
10/29, 09:00-10:00 — create setup.py, requirements.txt
10/29, 10:00-17:00 — 8× "Update README.md" (iterative documentation)
```

**Key observation:** 8 README updates in a single day. This is the pattern of someone setting up project documentation, refining it repeatedly, and pushing through to completion. It's impressive scaffolding discipline, but there's been **zero code development since October 2024** — over 22 months of dormancy.

**Episode angle:** GCCS-Core is the "MVP demo" of carbon capture open source — full deployment scripts, IoT integration examples, config files, but no actual climate model or capture simulation logic behind it. It answers "how would you structure a climate control system?" but not "can you simulate the carbon capture?"

**Risks for listeners:** The repository description claims it encompasses "core algorithms" and "data management," but the actual codebase appears to be deployment scaffolding. The commit history tells the real story: 15 shell commands and README edits, not scientific computing.

---

### 2. 💰 kfdsievert/Cost-Model--DAC — The Honest Model

| Field | Detail |
|-------|--------|
| **URL** | https://github.com/kfdsievert/Cost-Model--DAC |
| **Stars** | 6 |
| **Language** | Python |
| **Last Activity** | June 4, 2026 |
| **Maintainer** | Katrin Sievert (Fuels Institute / UPenn) + Yash Dubey |

**What it does:** This is a **probabilistic cost projection model** for Direct Air Capture technology. It uses experience curves (learning curves) and Monte Carlo simulations to project future DAC costs under different scenarios. It doesn't simulate the chemistry of capture — it simulates the *economics* of scale-up.

**Commit pattern — healthy but brief:**
- **Jan 31, 2024:** 4 commits (initial upload, file cleanup)
- **Feb 1, 2024:** 6 commits (LICENSE additions, minor updates, README refinements)
- **Feb 5, 2024:** 2 commits (README updates)
- **Feb 19, 2024:** 3 commits (README, LICENSE changes)
- **Jun 4, 2026:** Last update (exact nature unknown — possibly a single commit)

**This is a more honest research tool:** It doesn't claim to simulate carbon capture chemistry. It models cost trajectories — a crucial but often overlooked dimension of the DAC conversation. The cost of DAC is currently ~$400-1000/ton CO₂; the question is whether it can reach <$100/ton through learning-by-doing.

**Episode angle:** The cost model is arguably more useful for policy than a chemistry simulator. "If we build 10,000 DAC plants, will costs drop by 50% or 5%?" — that's the question this model tries to answer. The probabilistic (Monte Carlo) approach is also more honest than single-point estimates.

**Notable detail:** The LICENSE file was added, deleted, then re-added within the same commit session (Feb 1-2, 2024). This suggests the authors were uncertain about licensing — a common issue in academic code. The final choice appears to be open (based on the README updates referencing license compatibility).

---

## The "CC0 Revolution" Question

While searching for carbon capture repos, we noticed an emerging trend: some climate tech projects are adopting **CC0 (Creative Commons Zero) or public-domain licensing**, explicitly placing their code in the public domain. This is significant for the carbon capture episode because:

1. **The cost barrier problem:** DAC costs ~$400-1000/ton. If capture technology is patented and proprietary, the cost ceiling is enforced by IP holders. Open-source DAC models can't directly break the cost barrier, but they can democratize understanding of it.

2. **The data problem:** Cost models need data — energy prices, material costs, construction timelines. If the models are open but the data is proprietary, the models are limited. Full openness (code + data) is rare but growing.

3. **The governance question:** Who decides what "affordable carbon capture" means? If only a few companies can afford to run the simulations, they set the terms of the debate.

---

## Cross-Theme Comparison: Carbon vs. Solar

| Dimension | Solar Geoengineering | Carbon Capture |
|-----------|---------------------|----------------|
| **Dominant repos** | WRF (1,763★) — mature, institutional | GCCS-Core (9★), Cost-Model--DAC (6★) — early-stage |
| **Code maturity** | Decades of development, production-grade | Scaffolding / proof-of-concept |
| **SRM simulation capability** | Embedded in WRF's TEMPO scheme | No chemistry simulation; cost modeling only |
| **Active contributors** | 6+ (NCAR, NOAA, universities) | 1-2 (solo developers) |
| **Commit velocity** | Continuous (v4.8.0 released Jun 2026) | Burst-and-dormant |
| **Key gap** | SRM code treated as niche parameterization | No chemistry/process simulation exists |

**Key insight for the episode:** Solar geoengineering has WRF. Carbon capture has... mostly nothing that simulates the actual capture chemistry. The carbon capture open-source ecosystem is at a much earlier stage. If solar geoengineering's challenge is "how do you govern embedded simulation code?", carbon capture's challenge is "how do you build the simulation code in the first place?"

---

## Listener Discussion Questions

1. **Is GCCS-Core's claim of being a"Global Climate Control System" hubristic or aspirational?** The repo has deployment scripts but no simulation logic. Is the gap between scaffolding and substance typical for open-source climate projects?

2. **Should there be an open-source DAC simulation framework?** We have OpenFOAM for fluid dynamics, WRF for weather, SenPy for solar — but no equivalent for carbon capture chemistry/process simulation. What would it take to build one?

3. **Does the cost model's existence change the conversation?** If we can probabilistically project DAC costs under different scale-up scenarios, does that help or hurt the policy debate?

---

## Source Data

All commit histories pulled via GitHub List Commits API:
- KOSASIH/GCCS-Core: 15 most recent commits (as of Sept 2026)
- kfdsievert/Cost-Model--DAC: 15 most recent commits
- Search queries documented above.
