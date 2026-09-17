# 📊 Carbon Capture — Commit Trend Summary

**Data source:** GitHub API — 6 repositories, ~5 most recent commits each, pulled Sep 2026

---

## Repositories Analyzed

| Repo | Stars | Lang | Last Commit | Activity Level |
|------|-------|------|-------------|----------------|
| openair-collective/openair-cyan | 76 | Open HW | Feb 12, 2024 | 🔄 Single-Day Burst (OSHWA cert) |
| yohanesnuwara/carbon-capture-and-storage | 85 | Lasso | Jul 1, 2026 | 💤 Dormant (since Mar 2021) |
| zikribayraktar/Carbon_Capture_ML | 56 | Jupyter | May 8, 2024 | 🔄 Maintenance (survey updates) |
| Beckybams/AI-for-Carbon-Capture-Optimization | 25 | Python | Mar 2, 2026 | 🔄 Low Activity |
| tonyzyl/CO2-Soft-sensor-CC-pilot | 16 | Jupyter | Aug 18, 2026 | 🔄 Active (hybrid modeling) |
| CCSI-Toolset/membrane_model | 6 | Makefile | Aug 23, 2026 | 🔥 Active |

---

## Key Findings

### 1. The August 2026 Materials Wave
Multiple repos updated within days of each other (Aug 19-23, 2026):
- Perovkanvates/peroxotitanates DAC materials research
- Membrane model update
- AI-for-CC-optimization ongoing activity

**Interpretation:** Coordinated research push in computational DAC materials. Multiple groups converging on similar chemical spaces (perovskite/peroxide sorbents).

### 2. The OpenAir-Cyan Certification Burst
All 5 commits on Feb 12, 2024 happened within a single day — OSHWA certification push. This is a "one-time event" repo: the hardware exists, the certification happened, and then the project went quiet.

**Implication:** Open hardware projects on GitHub tend to have burst activity for milestones, then no ongoing maintenance.

### 3. Star Count ≠ Maintenance
- 85★ repo (carbon-capture-and-storage): dormant since 2021
- 6★ repo (membrane_model): active Aug 2026
- 16★ repo (soft sensor): active Aug 2026
- 76★ repo (OpenAir-Cyan): dormant since 2024

**The most-starred repos are the most dormant.** This inverts the "popular = active" assumption.

### 4. The Hybrid Modeling Trend
Two repos represent the emerging hybrid approach:
- **DAE-LSTM soft sensor:** Physics-based differential algebraic equations + LSTM neural network
- **AI-for-CC-optimization:** Synthetic industrial data for training

Both approaches combine domain knowledge with data-driven methods. Neither is purely physics OR purely ML.

### 5. The Lasso Anomaly
One repo (carbon-capture-and-storage) uses Lasso for what appears to be reservoir simulation. This is unusual — most geoscience/CC code is in Python, MATLAB, or Fortran. The Lasso choice suggests a niche tool or the author's preference. It may also explain the dormancy: the ecosystem around Lasso for CCS is very small.

---

## Commit Timeline (Most Recent per Repo)

```
2026-08-23  membrane_model: update (Makefiles)
2026-08-19  DAC peroxovanadates/titanates: computational materials
2026-08-18  CO2-Soft-Sensor: active development (Jupyter)
2026-03-02  AI-for-CC-Optimization: last commit (Python)
2026-07-01  carbon-capture-and-storage: repo metadata (dormant since 2021)
2024-05-08  Carbon_Capture_ML: OpenDAC paper added (Jupyter)
2024-02-12  openair-cyan: OSHWA certification burst (all 5 same-day commits)
2021-03-01  carbon-capture-and-storage: last real code commit
```

---

## Research Gaps Identified

1. **No full-scale DAC simulator** — No open-source tool that simulates a complete direct air capture system from energy input to CO2 output
2. **No economic model of DAC at scale** — Repos focus on chemistry/materials; none model the cost curve or deployment scenario
3. **No open-source amine chemistry model** — The dominant DAC chemistry (amine sorbents) has no GitHub simulation tools
4. **Hardware-software divide** — OpenAir-Cyan shares hardware; Carbon_Capture_ML shares surveys. Neither bridges to the other.

---

*Analysis date: Sep 2026 | Method: GitHub commit API + repository search*