# 🌍 Carbon Capture — Commit Trends (v5 Update)
## Trend Analysis for Climate Pod Episode (October 2026)

---

## Velocity Summary

| Repo | Stars | Commits Pulled | Active Period | Velocity Pattern |
|------|-------|----------------|---------------|------------------|
| Open-Sustainable-Tech | 2,552 | 10 | Jul–Sep 2026 | 🔴 Steady institutional — 10 commits/64 days |
| OpenAir-Cyan | 76 | 10 | Feb 2024 (frozen) | ⚪ Dormant — 6 commits/1 day, then 2.5yr sleep |
| Carbon_Capture_ML | 56 | N/A | May 2024 (frozen) | ⚪ Dormant — survey frozen |
| dac-moving-bed-digital-twin | Low | N/A | Jul 2026 | 🟡 Recent activity — single project, uncertain sustainability |
| OpenCarbon | 2 | N/A | Aug 2026 | 🟡 Recent activity — new project, uncertain direction |
| Direct-Air-Capture ML | Low | N/A | Jun 2026 | 🟡 Recent activity — academic project |

---

## Trend 1: The Directory Machine (Open-Sustainable-Tech)

**Open-Sustainable-Tech** is the **highest-velocity project** in the carbon capture space — not because it invents technology, but because it **catalogs what exists.**

**Cadence:** 10 commits across 64 days (Jul 19 – Sep 19, 2026). Average ~0.16 commits/day. The burst pattern: 3 commits on Sep 19, 2 on Sep 9, 1 on Sep 1. This is a **sweep pattern** — someone is systematically adding projects to the directory.

**Why this matters:** The directory is becoming a **de facto registry** of what counts as climate tech. If your project isn't indexed here, it's invisible to the climate-tech community. But the directory doesn't evaluate — it just lists. This means the quality bar is low: anyone can submit, and the AI content review template (Jul 2026) is the first attempt at quality control.

**Episode angle:** "The world's biggest climate tech directory doesn't build anything — it just lists. But who decides what gets listed?"

---

## Trend 2: The Dormancy Problem (OpenAir-Cyan + Carbon_Capture_ML)

**OpenAir-Cyan** and **Carbon_Capture_ML** both show the same pattern: **a big burst of activity followed by permanent dormancy.**

**OpenAir-Cyan:** 6 commits on Feb 12, 2024 (OSHWA certification blitz), then 2.5 years of silence. The project achieved legitimacy (OSHWA certification) but didn't achieve sustainability (continued development).

**Carbon_Capture_ML:** 10 commits in Jan-Feb 2023 (survey construction), then 5 single-paper additions through May 2024. Frozen since. The survey is comprehensive but outdated — new papers appear weekly in this field.

**The pattern:** This is the **"publish and perish"** problem in climate tech. Researchers build things, get temporary recognition (certification, citations), then move on. The projects don't sustain because they're personal projects, not community efforts.

**Episode angle:** "Why do climate tech projects have such short half-lives? The OpenAir-Cyan story — 6 commits, then silence — is the cautionary tale."

---

## Trend 3: The Digital Twin Signal (dac-moving-bed-digital-twin)

**The newest and most interesting trend** in carbon capture is the **digital twin** approach — not inventing new DAC chemistry, but simulating the existing process in detail to find optimization opportunities.

**Why this matters:** The $1000/ton DAC cost barrier is a **process optimization problem**, not just a chemistry problem. A digital twin that couples sorbent physics (Toth isotherm, LDF kinetics) with discrete-event simulation can:
- Optimize sorbent regeneration cycles
- Predict maintenance needs
- Test control strategies without physical experiments
- Identify bottlenecks in the process

This is the **optimization-first** approach to DAC cost reduction — as opposed to the **invention-first** approach (try new chemistry, try new materials).

**Episode angle:** "Instead of inventing better DAC chemistry, why not just simulate the existing process better? The digital twin approach."

---

## Trend 4: The AI Gravity Well

Three carbon-capture-related projects this quarter involve AI/ML:
1. **claude-carbon** (Aug 2026): AI carbon footprint tracker — added to Open-Sustainable-Tech
2. **Carbon_Capture_ML survey** (May 2024, frozen): Curated ML-for-CC papers
3. **Direct-Air-Capture ML** (Jun 2026): Data-driven ML model for DAC

The AI gravity well is pulling everything toward data-driven approaches. But the question remains: **does ML accelerate real-world deployment, or just produce more papers?** The Carbon_Capture_ML survey, frozen for 2.5 years, suggests the papers don't lead to deployed systems.

---

## Trend 5: The CC0 Revolution Slowing?

In v4, we documented a "CC0 public-domain revolution" — projects releasing carbon capture technology into the public domain. But this quarter, **no new CC0 DAC projects appeared**.

**Possible explanations:**
1. The CC0 movement had its moment (v4), and the wave has passed
2. DAC is too complex for individual projects — it needs industrial-scale labs, not bedroom coders
3. The CC0 licensing model doesn't work for hardware-intensive projects (which need physical fabrication, not just code)
4. The Open-Sustainable-Tech directory is replacing the CC0 approach — instead of releasing everything to public domain, projects just get listed in the directory

**Episode angle:** "The public-domain revolution in carbon capture: did it fizzle, or did it transform into something quieter?"

---

## Commit Heat Map

```
Repo                      | Jul '26 | Aug '26 | Sep '26 | Oct '26 | Nov '26 | ...
--------------------------|---------|---------|---------|---------|---------|----
Open-Sustainable-Tech     | ██░░░░  | ██░░░░  | ██████  | ░░░░░░  | ░░░░░░  |  (sweep pattern)
OpenAir-Cyan              | ░░░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  |  (frozen)
Carbon_Capture_ML         | ░░░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  |  (frozen)
dac-moving-bed-digital    | ██░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  |  (single burst)
OpenCarbon                | ░░░░░░  | ██░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  |  (recent)
Direct-Air-Capture ML     | ██░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  | ░░░░░░  |  (recent)
```

**Pattern:** The directory (Open-Sustainable-Tech) is the only project with sustained activity. Everything else is either frozen (OpenAir-Cyan, Carbon_Capture_ML) or recently active but unproven (dac-moving-bed-digital-twin, OpenCarbon, Direct-Air-Capture ML). The carbon capture space on GitHub is **wide but shallow** — many projects, few that sustain.

---

## What to Watch Next Quarter

1. **Will Open-Sustainable-Tech keep its sweep pattern?** If yes, it's becoming the definitive climate-tech registry. If no, it's just another directory that stopped getting updated.
2. **Will dac-moving-bed-digital-twin get more commits?** A single project doesn't make a trend. But if more DAC groups adopt digital twins, it could be a paradigm shift.
3. **Will OpenAir-Cyan ever wake up?** The OSHWA certification gave it legitimacy. A new release with improved hardware designs would signal renewed community interest.
4. **Will the AI-for-CC pipeline produce deployed systems?** The frozen Carbon_Capture_ML survey suggests papers don't lead to deployments. But a working ML-optimized DAC process would be a counterexample.

---

*Research methodology: GitHub REST API, October 2026. Commits pulled via List Commits API. Trend analysis by research methodology.*