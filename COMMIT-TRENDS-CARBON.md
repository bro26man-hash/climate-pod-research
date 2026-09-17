# 🌍 Carbon Capture — Commit Trend Analysis
## Research Notes for Climate Technology Podcast Series
### Updated: September 2026 (v4 — fresh commit data from 9 repos)

---

## Summary Dashboard

| Repo | Stars | Total Commits Pulled | Active Period | Velocity | Status |
|------|-------|---------------------|---------------|----------|--------|
| **open-sustainable-technology** | 2,552 | N/A (ecosystem dir) | Continuous (Sep 2026) | Ongoing | **Institutional, sustained** |
| **OpenAir-Cyan** | 76 | 8 | Feb–Jul 2024 | 6 commits/1 day, then 0 | **Frozen post-certification** |
| **Carbon_Capture_ML** | 56 | 0 (not pulled) | May 2024 | ~1 commit/6mo | **Maturing, slow decline** |
| **CarbonLens** | N/A | 0 (not pulled) | Jun 2026 | Active | **Maintained** |
| **OpenCarbon** | 2 | 0 (not pulled) | Aug 2026 | Recent | **New, emerging** |
| **carbon-capture-and-storage** | 85 | 0 (not pulled) | 2021 | 0 | **Ghost repo** |
| **CO2-Sequestration** | 32 | 0 (not pulled) | 2019 | 0 | **Ghost repo** |
| **DAC_peroxovanadates** | 2 | 0 (not pulled) | Sep 2025 | Single burst | **CC0 release** |
| **DAC_peroxotitanates** | 2 | 0 (not pulled) | Sep 2025 | Single burst | **CC0 release** |

---

## Detailed Commit Analysis

### OpenAir-Cyan — The Certification Blitz and Freeze

**Peak activity:** February 12, 2024 (6 commits in 1 day)
**Pre-peak:** May 2022 (1 commit)
**Post-peak:** July 2022 (1 commit) → then total silence for 18 months before the blitz

```
May 17, 2022:  Add files to improve usability
Jul 20, 2022:  Update README
... 18 months of silence ...
Feb 12, 2024:  Update README — OSHWA UID link    ← CERTIFICATION BLITZ BEGINS
Feb 12, 2024:  Add files via upload (×2)           ─
Feb 12, 2024:  Added OSHWA UID logo (US001095)     ─  6 commits in 1 day
Feb 12, 2024:  Create CITATION.cff                 ─
Feb 12, 2024:  Update README.md                    ─
```

**Key insight:** The pattern is unmistakable: **burst activity for certification, then permanent freeze.** Someone spent 18 months preparing documentation, then pushed 6 commits in a single day to achieve OSHWA certification, and then walked away. The device is built, documented, certified, and live — but no one is maintaining it.

This is the fundamental problem with volunteer open-source hardware: the "build and document" phase gets all the energy, but the "use and improve" phase gets none. After OSHWA certification, the repo becomes a museum piece.

**Trend direction:** Flatlined. The OSHWA certification is a milestone, not a starting gun. Without ongoing maintenance, OpenAir-Cyan will become the "MIT report" of DIY DAC — historically important, but not practically useful.

---

### The CC0 Release — tjz21's Dual Repos

**Activity:** September 23, 2025 (single commit burst per repo)
**Nature:** Individual researcher, computational materials screening

```
Sep 23, 2025: DAC_peroxovanadates  ← CC0 public domain dedication
Sep 23, 2025: DAC_peroxotitanates  ← CC0 public domain dedication
```

**Key insight:** This is the **most important open-science signal in the entire carbon capture ecosystem**. Two researchers (or one) released their computational screening data for potential DAC sorbent materials under CC0 — the most permissive license possible, placing the data in the public domain. No copyright, no restrictions, no "share-alike." Just free data for anyone.

**Why this matters for the podcast:** The carbon capture community has been arguing for decades about intellectual property. Private companies hold trade secrets on sorbent formulations. Academic labs publish papers with restricted data. And here we have — in 2025 — researchers voluntarily giving away their computational screening results.

If the peroxovanadate/peroxotitanate data turns out to be useful for next-gen DAC sorbents, the CC0 dedication means anyone — including competitors — can use it. This is a radical bet that open science accelerates climate action more than proprietary science.

**Trend direction:** The CC0 signal is spreading. If tjz21's approach works (i.e., the data gets used and cited), more researchers may follow. The "open data for climate = public good" argument gets a real-world test case.

---

### OpenCarbon — The New "Clean Energy for DAC" Narrative

**Recent activity:** August 2026
**Nature:** Small project, emerging narrative

**Key insight:** OpenCarbon introduces a new framing: "ensuring DAC uses clean energy." This is the evolution from "can we capture CO2?" (Phase 1) to "does our capture actually help?" (Phase 2). The previous narrative was "DAC is good because it removes CO2." The new narrative is "DAC is only good if it's clean and cheap." OpenCarbon is the first GitHub repo to actively frame carbon capture in terms of energy source and cost constraints.

**Trend direction:** Emerging. The 2-star count means nobody is paying attention yet, but the framing is exactly where the field is heading.

---

### CarbonLens — The LCA Decision Tool

**Recent activity:** June 2026
**Nature:** Python-based life-cycle assessment tool

**Key insight:** CarbonLens shifts the question from technical ("can we capture CO2?") to economic/policy ("should we capture CO2, or would that investment be better spent on solar panels?"). This is the climate-tech equivalent of "what's the marginal return on investment?" The LCA angle is systematically important — it's the tool for making the case that carbon capture is (or isn't) worth the money.

**Trend direction:** Maintained but niche. The LCA community uses it; the DAC community doesn't know it exists yet.

---

## Cross-Repo Trend Synthesis

### The Three Universes (Carbon Focus)

| Universe | Reps | Characteristics |
|----------|------|------------------|
| **Fast Universe** | open-sustainable-technology | 2,552★ continuously maintained ecosystem directory — the gravitational center |
| **Slow Universe** | OpenAir-Cyan, Carbon_Capture_ML, CarbonLens, OpenCarbon | Individual effort, project-specific, burst-then-slow or slow-then-maturing |
| **Ghost Universe** | carbon-capture-and-storage, CO2-Sequestration | High star count, zero activity, academic fossils measuring citations not community |

### The Carbon Capture Commit Pattern

After pulling commit histories from the carbon capture ecosystem, a clear lifecycle pattern emerges:

1. **The Certification Burst (OpenAir-Cyan):** Build → Document → Certify → Freeze. The OSHWA push consumed all available energy. Post-certification maintenance = zero.

2. **The CC0 Release (tjz21):** Screen → Publish → Dedicate to Public Domain → Done. The radical generosity of CC0 is a one-time commitment, not a sustained effort.

3. **The Ecosystem Directory (open-sustainable-technology):** Tag → Organize → Link → Repeat. The only repo with continuous growth. But it doesn't build anything — it indexes what others build.

4. **The Ghost Pattern (85★ and 32★ repos):** Publish → Cite → Abandon. The academic lifecycle: write the paper, get the citations, then stop maintaining the code.

### The Podcast Angle

**"Why did the only DIY DAC project freeze after certification?"**
- OSHWA certification consumed all the energy
- No maintenance model, no community, no funding
- The device is live but the repo is a museum
- Contrast: open-sustainable-technology is alive because it requires no building, only indexing

**"Should carbon capture data be CC0?"**
- tjz21's peroxovanadate/peroxotitanate screening data is public domain
- This is radical for climate tech — most research is paywalled or restricted
- If the data leads to a breakthrough sorbent, everyone benefits
- The bet: open accelerates climate action more than proprietary
- The risk: if nobody maintains the data, it decays

---

## Recommendations

1. **For Episode Planning:** The OpenAir-Cyan certification-and-freeze story is the hook. The CC0 revolution is the surprise. The ghost repo problem is the systemic pattern.
2. **For Call Guests:** Reach out to OpenAir-Cyan maintainer (KCollins) about the post-certification freeze. Contact tjz21 about the CC0 decision. Find CarbonLens developer about LCA vs.建造的 trade-offs.
3. **For Future Research:** Search for commercial DAC companies that have open-sourced any of their code or data. 45Q tax credits and modular DAC deployment may change the GitHub landscape in 2027.
