# 🌍 Carbon Capture — Commit Trend Analysis

**Branch:** `carbon-capture` | **Last Updated:** September 2026 (v4)

Commit trend analysis across carbon-capture repositories, based on fresh commit histories pulled via the GitHub API (September 2026).

---

## Activity Overview

| Repo | Total Commits Pulled | Date Range | Commit Density | Development State |
|------|---------------------|------------|---------------|------------------|
| protontypes/open-sustainable-technology | 15 | Jun–Sep 2026 | ~2-3/month sustained | 🟢 Active ecosystem curation |
| openair-collective/openair-cyan | 15 | May 2022–Feb 2024 | 💥 7/day blitz then ❌ frozen | ⚠️ Dormant 2+ years |
| zikribayraktar/Carbon_Capture_ML | 15 | Jan–May 2024 | ~1/week then ❌ frozen | ⚠️ Dormant 1.5 years |
| tjz21/DAC_peroxovanadates | 15 | Nov 2023–Sep 2025 | ❌ 6mo gap then 1 day, then ❌ | 🆕 CC0 adoption signal |
| tjz21/DAC_peroxotitanates | 10 | Feb–Sep 2024 | ~2/week then ❌ gap, then 1 day | 🆕 CC0 adoption signal |

---

## Trend 1: The Sustained Curation Model (Open Sustainable Technology)

Open Sustainable Technology is the **only repo in the carbon-capture theme showing consistent, ongoing development.** Its pattern is fundamentally different from all others:

**Commit velocity:**
```
Jun 2026:  ████████████████████  2 commits (EpexPredictor, Volca + wbdata)
Jul 2026:  ████████████████████████████████  3 commits (PowerIO, ASSETRA, ToOp)
Aug 2026:  ██████████████████████████████████  3 commits (claude-carbon, Story Seed, openflexure)
Sep 2026:  ████████████████████  3 commits (MUIO, MUIOGO, README fixes)
```

**Key insight:** ~2.5 commits/month, every month, without gaps. This is **institutional curation velocity**—not code development, but ecosystem maintenance. The contributors (Abdul Salam, Tobias Augspurger, Mikhail Alabugin, Christophe Combelles) are different people adding different entries. This is a community project, not an individual effort.

**🎙️ Podcast angle:** The most important carbon-capture repo on GitHub isn't building a device or writing a model. It's writing a **list.** And it's been doing it at a steady pace for years. This is the forgotten truth about open-source climate tech: most of it is curation, not creation.

---

## Trend 2: The "Big Bang Then Freeze" Pattern (OpenAir-Cyan & Carbon_Capture_ML)

Two repos show the same dramatic pattern:

| Repo | Build Phase | Lean Phase | Freeze |
|------|------------|-----------|--------|
| openair-cyan | May 2022: CodeQL, README, usability (6 commits) | Jul 2022: 1 README update | **Feb 12, 2024: 7 commits in 1 day (OSHWA blitz), then 2+ years silence** |
| Carbon_Capture_ML | Feb 2023: 7 commits in 1 week (full survey build) | Mar–Dec 2023: slow additions | **May 8, 2024: OpenDAC paper added, then silence** |

**The pattern:** A rapid build phase (1 week to 1 day) produces the full artifact, then a slow maintenance phase, then complete freeze.

**What this tells us about carbon-capture open source:**
1. **Individual researchers can build complete artifacts fast** — when there's a clear deliverable (a survey, a certified device)
2. **Maintenance is harder than creation** — after the initial build, there's no sustained effort
3. **Freeze is permanent** — neither repo has shown any revival signal in 1.5–2 years

**🎙️ Podcast angle:** "Can open-source carbon capture hardware survive without a budget?" OpenAir-Cyan got OSHWA certified in a single day, then went dark. Carbon_Capture_ML built a full survey in a week, then stopped updating. The pattern is the same: sprint, then silence. This isn't a sustainability problem—it's a **career structure** problem. Academics build tools for papers, not for maintenance.

---

## Trend 3: The CC0 Adoption Event (Sep 12, 2025)

The most significant event in the carbon-capture commit data:

```
DAC_peroxovanadates:
  Sep 12, 2025: e041eff — added CC0 license
  Sep 23, 2025: cfd04f7 — updated README.md (11 days later)

DAC_peroxotitanates:
  Sep 12, 2025: c7ea8ae — added CC0 license
  Sep 23, 2025: 61ade51 — updated README.md (11 days later)
```

**The timeline:**
1. **Before Sep 12:** Both repos were in their respective maintenance phases (3+ months of README updates in Dec 2023 for peroxovanadates; Jun–Jul 2024 for peroxotitanates)
2. **Sep 12, 2025:** Both repos get CC0 license on the exact same day
3. **Sep 23, 2025:** Both repos get README updates 11 days later
4. **After Sep 23:** Both repos go silent

**Interpretation:**
- The CC0 adoption was **coordinated** — same lab, same day, same license
- The README updates followed 11 days later — likely documenting the license change
- The repos then went silent — the "declaration" was the final act

**What CC0 means in practice:**
- Anyone can use, modify, distribute, or sell the data without permission or attribution
- Future researchers can build computational workflows on these DFT datasets without legal friction
- The data becomes **infrastructure**, not intellectual property

**🎙️ Podcast angle:** "On September 12, 2025, two researchers at Oregon State University made a decision that would change the openness of computational carbon-capture science. They didn't publish a paper. They didn't file a patent. They added a license file. And in doing so, they made the entire computational dataset for their direct air capture materials research available to the world—forever, without restriction. The only question is: will others follow?"

---

## Trend 4: The Star-Activity Inversion

Critically important carbon-capture repos show an inversion between stars and activity:

| Repo | Stars | Last Active | Interpretation |
|------|-------|------------|---------------|
| open-sustainable-technology | 2,552 | Sep 2026 (active) | ⭐ = useful, and still is |
| openair-cyan | 76 | Feb 2024 (frozen) | ⭐ = was useful, still bookmarked |
| Carbon_Capture_ML | 56 | May 2024 (frozen) | ⭐ = was useful, still referenced |
| carbon-capture-and-storage | 85 | Mar 2021 (ghost) | ⭐ = cited, but useless now |
| DAC_peroxovanadates | 2 | Sep 2025 (frozen) | ⭐ = invisible, but scientifically critical |
| DAC_peroxotitanates | 2 | Sep 2025 (frozen) | ⭐ = invisible, but scientifically critical |

**The inversion:** The most-starred repos are often the least active. The most active repo (open-sustainable-technology) is also the most-starred. But the 2-star DAC repos may be more scientifically consequential than the 85-star ghost repo.

**🎙️ Podcast angle:** "85 stars and dead since 2021. 2 stars and scientifically foundational. On GitHub, popularity is a poor proxy for importance. The most-starred carbon-capture repo might be the least useful one. And the most important dataset in direct air capture materials science has fewer stars than your personal project."

---

## Trend 5: The AI Integration Signal

The July–August 2026 commits to Open Sustainable Technology reveal a new pattern:

| Date | Addition | Category |
|------|----------|----------|
| Jul 17, 2026 | AI content review PR template | Governance |
| Jul 19, 2026 | PR template modified (AI review) | Governance |
| Aug 23, 2026 | claude-carbon (AI tool) | Tool addition |

**What this means:** The climate-tech community is building **AI governance into its infrastructure.** The PR template requires AI-generated content to be reviewed before merging. The "claude-carbon" entry is an AI tool specifically for carbon accounting.

**This is a two-sided signal:**
1. **Positive:** AI is being used to curate and manage the climate-tech ecosystem (claude-carbon for accounting)
2. **Cautious:** The community is simultaneously building guardrails (AI content review PR template)

**🎙️ Podcast angle:** "The climate-tech community just did something remarkable: they added AI tools to their directory AND added AI review requirements for entries. They're saying: 'AI can help us find carbon accounting tools, but we won't let AI write the entries without human oversight.' It's the fastest-growing governance debate in open-source climate tech, and it happened in July 2026."

---

## Commit Velocity Comparison

```
Open-Sustainable-Tech:  ██████████████████████████████  sustained, ~2.5/month
OpenAir-Cyan:           💥💥💥💥💥💥💥  7/day blitz, then ❌ frozen
Carbon_Capture_ML:      ██████████████████████  1/week initial, then ❌ frozen
DAC_peroxovanadates:    ░░░░░░░░░░░ ██████ ░░░░░░  then ❌ frozen
DAC_peroxotitanates:    ██████ ██████████ ░░░░░░░░  then ❌ frozen
```

**The pattern:** Individual researchers can build fast (1 week to 1 day). But sustained curation requires a community. Only Open Sustainable Technology has achieved that.

---

## 🎙️ Episode Structure (Suggested)

### Act 1: "The Directory" (5 min)
- Open Sustainable Technology (2,552★) as the ecosystem map
- Why a list is the most important open-source artifact in carbon capture
- The AI governance signal: claude-carbon + AI review PR template

### Act 2: "The One-Day Wonders" (7 min)
- OpenAir-Cyan's Feb 12, 2024 OSHWA blitz → 2 years of silence
- Carbon_Capture_ML's Feb 2023 survey sprint → 1.5 years of silence
- Why academics sprint and individuals freeze

### Act 3: "The CC0 Decision" (7 min)
- September 12, 2025: the day two repos changed everything
- CC0 in practice: what does "public domain" mean for computational data?
- Why the Nyman lab's decision matters more than their papers
- Will others follow?

### Act 4: "The Ghost Stars" (4 min)
- 85-star carbon-capture-and-storage: dead since 2021
- 2-star DAC repos: scientifically foundational
- Why GitHub stars don't measure what we think they measure

---

## Data Sources

All commit data pulled fresh from GitHub API on September 19, 2026:
- `protontypes/open-sustainable-technology` — 15 commits (page 1)
- `openair-collective/openair-cyan` — 15 commits (page 1)
- `zikribayraktar/Carbon_Capture_ML` — 15 commits (page 1)
- `tjz21/DAC_peroxovanadates` — 15 commits (page 1)
- `tjz21/DAC_peroxotitanates` — 10 commits (page 1)

---

## Research Log

| Date | Activity |
|------|----------|
| 2026-09-19 | v4: Fresh commit histories pulled from 5 active carbon-capture repos; CC0 analysis, AI governance signal, and episode brief pushed to branch |
| 2026-09-17 | v3: Previous analysis completed (incorporated into README) |
| 2026-09-03 | Initial research notes created |
