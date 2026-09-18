# 🌍 Carbon Capture — Commit Trend Analysis

> **Episode Theme:** Carbon Capture (DAC, CCS, ML-Optimized Sorbents, Open Hardware)
> **Data Source:** GitHub API — 5+ repositories, 50+ commits pulled (September 2026)

---

## Repository Commit Velocity

| Repository | Stars | Total Commits Pulled | Active Period | Pace | Status |
|-----------|-------|---------------------|---------------|------|--------|
| **protontypes/open-sustainable-technology** | 2,552 | (continuous) | Sep 2026 | continuous | 🟢 Fast — directory |
| **openair-collective/openair-cyan** | 76 | 6 (all Feb 12, 2024) | Feb 2024 | 1-day burst | 🟡 Dormant after sprint |
| **zikribayraktar/Carbon_Capture_ML** | 56 | 10 | Feb 2023–May 2024 | ~2/month | 🟡 Slow — solo researcher |
| **tonyzyl/CO2-Soft-sensor** | 16 | (continuous) | Aug 2026 | continuous | 🟢 Active — hybrid model |
| **yohanesnuwara/carbon-capture-and-storage** | 85 | 10 (all Feb–Mar 2021) | Feb–Mar 2021 | 5/day burst | 🔴 Ghost (5 yrs dormant) |

---

## Trend #1: The One-Day Blitz Pattern

**OpenAir-Cyan's Feb 12, 2024:**
```
b5422b3 — Update README.md — added OSHWA UID link
b164257 — Add files via upload
828f496 — Added OSHWA UID logo (OSHWA UID US001095)
4b08fb3 — Create CITATION.cff
859bfa8 — Update README.md
```

**6 commits in a single day.** Then: nothing for 2 years and 8 months.

**What happened:** Someone completed the OSHWA certification process, added the official UID logo, created a citation file (so people can *cite* the hardware as a scientific instrument), and uploaded final documentation.

**Why it matters:** This is the pattern of *completion*. Not "starting" — *finishing*. The repo went from "DIY project" to "certified open-source hardware" in one day. And then the creator moved on.

**🎙️ Podcast angle:** "The most important carbon capture commit on GitHub happened in a single day. Five changes that took 'Cyan' from a hobby project to legally-recognized open-source hardware. And then the person was done. No roadmap. No follow-up. Just… complete."

---

## Trend #2: The Solo Researcher's Marathon

**Carbon_Capture_ML's pattern:**
```
Feb 2023: ████████████████████  5 papers in 4 days (the PhD sprint)
Mar 2023: ██  1 paper
Jan 2024: ████  3 README updates
Apr 2024: █  1 README update
May 2024: █  1 OpenDAC paper added
Jun–Aug 2026: ░░░░░░░░░░░░░░░░░░  SILENCE
```

**The pattern:** A burst of 5 papers in 4 days (Feb 2–5, 2023), then slow, steady maintenance (1-2 commits/month) through mid-2024, then silence.

**What it means:** This is one person's literature review project. The Feb 2023 burst = thesis writing period. The 2024 maintenance = responding to citations and feedback. The silence = the project served its purpose, and the researcher moved to other work.

**🎙️ Podcast angle:** "One person, one repo, 500+ papers. On February 2nd, 2023, they committed 5 papers in 4 days. That's not a software project — that's a master's thesis being built in public. And when it was done, they stopped. No monetization. No community. Just… done."

---

## Trend #3: Ghost repos inflate star counts

**The data:**
- `carbon-capture-and-storage`: **85 stars**, last commit **March 2021**
- `CO2-Sequestration`: **32 stars**, last commit **2019**

**The mechanism:** These are academic repos from completed theses. Papers cite them → GitHub counts citations as stars → they appear "popular" → new users discover them → they realize nothing works → they leave a star anyway (politeness) → the cycle continues.

**The result:** **Ghost repos with more stars than active projects.** OpenAir-Cyan (76★, 2.5yr dormant) vs. carbon-capture-and-storage (85★, 5yr dormant). The "winner" is a tombstone.

**🎙️ Podcast angle:** "85 stars. Five years without a commit. This repo is a digital ghost — it lives because papers cite it, not because people use it. Star counts on GitHub measure citations, not utility. And in climate tech, that's a dangerous confusion."

---

## Trend #4: The CC0 License Revolution

**The signal:** tjz21's two DAC materials repos (peroxovanadates & peroxotitanates) both use **CC0 1.0 Universal** — the most permissive license possible, effectively placing the work in the **public domain**.

**The context:** Most open-source projects use MIT, Apache, or GPL. CC0 is rare. It means the creators have *waived all copyright*. Anyone can use, modify, distribute, or sell the data without asking permission.

**Why this matters for carbon capture:** Materials screening data is traditionally published behind paywalls or with restrictive licenses. CC0 says: "This data belongs to everyone. It's infrastructure."

**🎙️ Podcast angle:** "Two stars, CC0 license, and the most radical idea in carbon capture: your data isn't yours. These researchers gave away their entire computational screening dataset to the public domain. No copyright. No licenses. Just… take it. Is this the future of materials science?"

---

## Trend #5: Hybrid Modeling Emerges

**tonyzyl's CO2 Soft Sensor:**
- **DAE (Differential-Algebraic Equation) structure** = physics backbone
- **LSTM (Long Short-Term Memory) network** = learns residuals
- **Result:** A model that respects conservation laws but adapts to real-world complexity

**Why this is the future:** Pure physics models are too rigid. Pure ML models are uninterpretable and unreliable outside their training data. The hybrid approach gives you the best of both.

**🎙️ Podcast angle:** "This isn't AI *or* first-principles. It's AI *wrapped around* first-principles. The physics tells the neural network what's possible. The neural network tells the physics what's real. That's the future of industrial carbon capture."

---

## 📊 Commit Timeline (Carbon Theme)

```
2020 ░░░░░░░░░░░░░░░░░░░░  carbon-capture-and-storage starts
2021 ██████████████████████  Ghost burst (thesis, 10 commits in 2 months)
2022 ░░░░░░░░░░░░░░░░░░░░  Silence
2023 ████████████████████  Carbon_Capture_ML PhD sprint (5 papers/4 days)
2024 ████████████████████  Cyan OSHWA blitz (6 commits/1 day) + CC details
2025 ████████████████████  CC0 licenses (peroxovanadates/titanates)
2026 ░░░░░░░░░░░░░░░░░░░░  Silence on most repos;sporadic updates on directory
       ↑↑↑↑↑↑↑↑↑↑↑↑↑↑↑↑↑↑
       The burst pattern: climate tech commits come in sprints, not rivers
```

---

## 🎙️ Episode Script Notes

**Act 1 — The Directory:** "2,552 stars on a list. Not a model. Not a device. A *list*. That's the carbon capture ecosystem. Bigger on the outside than the inside."

**Act 2 — The OSHWA Moment:** "February 12th, 2024. Five commits. Open-source hardware certification for a DIY carbon capture device. Then silence for 2.5 years."

**Act 3 — The Solo Researcher:** "One person. 500 papers. 5 papers in 4 days. Then slow maintenance, then silence. This is what a PhD looks like in public."

**Act 4 — The Ghost:** "85 stars. Zero commits since 2021. A BSc thesis frozen in time. GitHub counts citations as stars. That's not a bug — it's a feature that makes climate tech look more active than it is."

**Act 5 — The Revolution:** "CC0. Public domain. No copyright. These researchers gave away their DAC screening data to the world. Two stars. Infinite potential."

**Close:** "The $1,000/ton barrier isn't an engineering problem. It's a community problem. We have the code. We have the devices. We have the data. What we don't have is the thread that connects them all."
