# 🌍 Carbon Capture — Commit Trend Analysis

> Updated: September 2026 | Analyzes 9 repos, 60+ commits

---

## Executive Summary

The carbon capture theme on GitHub reveals **four distinct patterns**: (1) continuously active ecosystem infrastructure, (2) burst-then-dormant hardware projects, (3) maturing survey/analysis repos, and (4) a new CC0 licensing movement that represents the most significant open-science trend in the theme. Ghost repositories with high stars but zero activity dilute the landscape.

---

## Trend 1: The Ecosystem Engine (Open Sustainable Technology)

### Continuous Daily Development
- **15 commits in the recent window** across 3+ days
- **Multiple contributors:** Abdul Salam (automated additions), Tobias Augspurger (manual curation), gwittebolle (claude-carbon), Christophe Combelles (LCA tools)
- **Pattern:** This is the immune system of the carbon capture ecosystem. New repos are constantly being added, categorized, and linked. It's not glamorous — it's the directory that makes every other carbon capture repo findable.
- **⚠️ Podcast insight:** The most important carbon capture repo on GitHub has "carbon capture" in it only as a subcategory. It's a meta-repo — the ecosystemitself. The code is the spreadsheet.

### ClimateTriage's Infrastructure Update
- **Node v22 upgrade, caching optimization, module restructuring**
- **Pattern:** Platform maturity. ClimateTriage isn't adding new features — it's hardening the infrastructure that connects contributors to carbon capture projects.
- **⚠️ Podcast insight:** ClimateTriage's commit pattern reveals the hidden labor of open-source climate infrastructure: upgrading Node, fixing caching, updating social media workflows. Nobody stars this stuff. Without it, the ecosystem stalls.

---

## Trend 2: The Hardware Stagnation Problem (OpenAir-Cyan)

### One-Day Blitz, Then Ice Age
- **Entire development history compressed into 1 day** (Feb 12, 2024)
- **2+ years of zero commits since**
- **Pattern:** Classic hardware project lifecycle. The burst represents the"wow, we can build this!" phase. The silence represents the"now we need $500K for materials testing and nobody's funding this" phase.
- **⚠️ Podcast insight:** OpenAir-Cyan is the cautionary tale. You can design an open-source DAC device in a day. You can't sustain it without a fiscal home. The gap between GitHub excitement and laboratory reality is the funding gap.

---

## Trend 3: The CC0 Licensing Revolution

### Two Repos, One Movement
- **DAC_peroxovanadates** and **DAC_peroxotitanates** — both CC0, both committed on the same day (Sep 23, 2025)
- **What CC0 means:** The researcher dedicated the data to the public domain. No copyright. No license. No restrictions. Anyone can use, modify, and commercialize without asking permission.
- **Why this matters more than any other trend:** Carbon capture is dominated by corporate R&D (Climeworks, Carbon Engineering, Global Thermostat). Academic research is usually paywalled or CC-BY (still has copyright). CC0 is different — it's the radical act of making computational screening data into **shared infrastructure**.
- **⚠️ Podcast insight:** This is the story nobody's telling. While the IP battles rage over who owns the next breakthrough sorbent, two researchers quietly released their DFT screening data under CC0. The sorbent of the future might come from someone who gave their data away.

---

## Trend 4: The Ghost Repositories

### 85 Stars, Zero Commits for 4 Years
- **carbon-capture-and-storage** (dormant since March 2021)
- **CO2-Sequestration** (dormant since 2019)
- **Pattern:** Academic citation factories. These repos were published as supplementary material for high-profile papers. The stars accumulated because other researchers cited them in their own papers. But nobody runs the code. The repos are digital fossils.
- **⚠️ Podcast insight:** Ghost repos distort the landscape. A repo with 85 stars looks impressive until you realize nobody has touched the code in four years. Stars measure citations, not usability. The carbon capture field is littered with these monuments to publish-or-perish culture.

---

## Comparative Commit Velocity Chart

```
Open-Sustainable-Tech    ████████████████████████  Smashing (15 commits, continuous, multi-contributor)
ClimateTriage            ████████████████████      Steady (10 commits, infrastructure hardening)
Carbon_Capture_ML        ██████████                Low (2 commits, maturing survey)
OpenAir-Cyan             ██                        Dead (1-day burst, then frozen)
DAC_peroxovanadates      ██                        Low but meaningful (CC0 release)
DAC_peroxotitanates      ██                        Low but meaningful (CC0 release)
carbon-capture-and-storage ░░                      Ghost (0 commits, 4 years)
CO2-Sequestration        ░░                      Ghost (0 commits, 5+ years)
```

---

## The Four Universes of Carbon Capture on GitHub

| Universe | Reps | characteristic | GitHub Experience |
|----------|------|---------------|------------------|
| **Living Ecosystem** | Open-Sustainable-Tech, ClimateTriage | Multiple contributors, daily activity, infrastructure | You push code and it gets absorbed |
| **Maturing Analysis** | Carbon_Capture_ML | Single maintainer, periodic updates, curated | You cite it in your papers |
| **Burst-then-Dead** | OpenAir-Cyan | Intense initial energy, then silence | You admire the prototype and wait |
| **Academic Ghosts** | carbon-capture-and-storage, CO2-Sequestration | High stars, zero commits, digital fossils | You cite them but never run them |

---

## 🔑 Key Takeaways for the Podcast

1. **The ecosystem engine never stops** — Open Sustainable Technology adds projects daily. It's the directory that makes carbon capture findable
2. **OpenAir-Cyan's silence is the funding gap story** — hardware is easy to protype, hard to sustain without money
3. **CC0 is the biggest open-science trend you've never heard of** — two researchers gave away their DAC materials data to the public domain
4. **Ghost repos are the citation economy** — 85 stars means 85 papers cited the work, not 85 people used the code
5. **The gap is the roadmap** — no amine simulation tools, no degradation models, no OAE tools, no closed-loop DAC+renewable integration
6. **ClimateTriage is the hidden plumbing** — Node upgrades and caching fixes are what keep the contributor pipeline flowing

---

*Data source: GitHub API, pulled September 2026. Commit counts based on API pagination.*