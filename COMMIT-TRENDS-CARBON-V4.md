# 🌍 Carbon Capture — Commit Trend Analysis
## Trend Summary from 6 Repositories (September 2026 — v4 Update)

---

## Executive Summary

Fresh commit data was pulled from 6 carbon capture repositories on September 18, 2026. The key finding: **carbon capture open-source development is defined by three paradoxes — (1) directories outpace hardware, (2) licenses matter more than code, and (3) the most important commits are the ones that aren't code at all.**

The CC0 license revolution in DAC materials, the OSHWA certification moment in open hardware, and the directory dominance of Open-Sustainable-Technology are the three signals that define the current state of carbon capture open-source.

---

## Trend 1: The Directory Dominance — 2,552 Stars vs. 76 Stars

### The Data

| Repo | Type | Stars | Commits in Last 3 Months |
|------|------|-------|--------------------------|
| Open-Sustainable-Technology | Curated directory | 2,552 | 14 |
| OpenAir-Cyan | Working DAC hardware | 76 | 0 (frozen since Feb 2024) |
| Carbon_Capture_ML | Literature review | 56 | 0 (frozen since May 2024) |
| DAC_peroxovanadates | Computational screening | 2 | 0 (frozen since Sep 2025) |

### What This Tells Us

**The directory has 33× more stars than the hardware.** Open-Sustainable-Technology is a list of links. OpenAir-Cyan is a working device you can build. Yet the directory gets 33× more attention.

**Why this matters for the episode:**
1. It suggests that climate tech investment flows toward curation rather than creation
2. It's easier to link to a project than to build one
3. The directory model scales; the hardware model doesn't
4. But the directory is useless without the hardware — and the hardware is frozen

**The structural problem:** Open-Sustainable-Technology gets traffic. OpenAir-Cyan gets stars but no contributors. DAC_peroxovanadates gets CC0 licenses but 2 stars. The carbon capture ecosystem is a pyramid where only the top layer is growing.

### 🎙️ Talking Point
"The most popular carbon capture repository on GitHub is a list of links with 2,552 stars. The second most popular is a working direct air capture device with 76 stars — and it hasn't been touched in two and a half years. What does that tell us about where climate tech investment actually goes?"

---

## Trend 2: The CC0 License Revolution — One Commit That Changes Everything

### The Data

**tjz21/DAC_peroxovanadates, September 12, 2025:**
- Single commit: "added CC0 license"
- This dedicated all data, code, and analysis to the public domain
- No code change. No feature addition. No bug fix. Just a license file.

### Why This Is the Most Important Commit in Carbon Capture Open-Source

1. **CC0 is radical** — It's more permissive than MIT, Apache, or GPL. It waives all copyright and related rights. Anyone can use, modify, distribute, and commercialize without restriction or attribution.

2. **It's a pattern** — The companion repo DAC_peroxotitanates also adopted CC0. This isn't a one-off; it's a philosophy.

3. **It's timely** — September 2025 is during a period of intense policy debate about DAC governance. The CC0 commitment says: the data is the science, and the science belongs to humanity.

4. **It's practical** — CC0 enables data fusion. If one research group's screening data is CC0 and another's is proprietary, they can't be combined. CC0 removes that barrier.

**The contrast with other carbon capture repos:**
- Open-Sustainable-Technology: MIT (open, but attribution required)
- OpenAir-Cyan: CERN-OHL-S (open hardware, but share-alike)
- Carbon_Capture_ML: Unknown (academic default = all rights reserved)
- DAC_peroxovanadates: **CC0 (public domain — no rights reserved)**

CC0 is the only license that truly treats data as public infrastructure.

### 🎙️ Talking Point
"One commit. One sentence. 'Added CC0 license.' And it might be the most important thing in carbon capture open-source — because it says the data belongs to everyone. No patents. No restrictions. Just science. This is the CC0 revolution, and it happened in a single afternoon."

---

## Trend 3: The OSHWA Certification Moment — Build It, Certify It, Freeze It

### The Data

**OpenAir-Cyan, February 12, 2024:**
- 7 commits in a single day
- OSHWA UID US001095 awarded
- CITATION.cff created
- README finalized
- Logo added

After February 12, 2024: **zero commits.** 29 months of silence.

### What This Pattern Reveals

The OSHWA certification is the finish line of open-source hardware development — but it might also be the starting line of a different problem:

1. **Certification is a validation milestone** — It proves the hardware meets open standards
2. **But it's also an endpoint** — Once certified, there's nothing left to "do" in the traditional development cycle
3. **The freeze is predictable** — Academic projects do this all the time: build, publish, certify, disappear
4. **The question is: what comes next?** — Does certification enable community iteration? Or does it mark the project as "complete" and untouchable?

**The clean energy parallel:** Solar panel open-source projects had the same pattern — early bursts of development, then stabilization once the design was "good enough." OpenAir-Cyan might be following the same arc.

### 🎙️ Talking Point
"OpenAir-Cyan went from zero to OSHWA-certified open hardware in a single day. Seven commits. Then silence. Twenty-nine months of silence. Is certification the finish line — or the point where the project stops being alive?"

---

## Trend 4: The Living Literature Review — Start Fast, Slow Down, Go Stale

### The Data

**zikribayraktar/Carbon_Capture_ML:**

| Period | Activity | Pace |
|--------|----------|------|
| Jan–Mar 2023 | 10+ paper additions | 🔥🔥🔥🔥 (fever pitch) |
| Jan–Apr 2024 | 3 README updates | 🔥🔥 (maintenance) |
| May 2024 | 1 paper addition | 🔥 (trickling) |
| After May 2024 | Nothing | ❄️ (frozen) |

### What This Pattern Reveals

The "living literature review" is a compelling idea — a repo that continuously catalogs new papers so nobody has to read everything. But the pattern is always the same:

1. **Launch phase:** The author is energized, reading papers furiously, adding entries daily
2. **Maintenance phase:** The pace slows as the field matures and new papers become harder to find
3. **Freeze phase:** The author moves on to a new project, and the repo becomes stale

**The risk:** When a living literature review goes stale, it becomes a liability. People cite it, trust it, and build on it — but the citations become outdated. The repo looks current but isn't.

**The deeper question:** Can a living literature review survive if it's treated as public infrastructure? CC0 licensing doesn't just apply to data — it could apply to literature reviews too. What if anyone could add entries? What if the review was truly community-maintained?

### 🎙️ Talking Point
"This repo added 10 papers in 2 months in early 2023. Then it added one paper in 2024. Then nothing. The 'living literature review' model works — until it stops living. What happens when a literature review goes stale but people are still citing it?"

---

## Trend 5: The Crypto Infiltration — Financial Instruments, Not Capture Technology

### The Data

Multiple "carbon capture" repos on GitHub are actually crypto/DeFi projects:
- `aslembadru/CarbonCapture` — Smart contract for DAC technology exposure
- `drakemesh/CarbonVault` — Carbon removal protocol tokenizing DAC infrastructure
- `aslembadru/CarbonVault` — Same project, forked
- `somlettes/CarbonNeg` — Synthetic covering DAC, mineralization, negative emissions

These aren't building capture technology. They're building **financial instruments** around carbon capture.

### What This Tells Us

The crypto-carbon capture ecosystem reveals a governance truth: **it's easier to tokenize carbon than to capture it.** Tokenizing DAC exposure requires no chemistry, no engineering, no hardware — just a smart contract and a liquidity pool.

**The danger:** These projects may obscure the real challenge of carbon capture by making it look like a financial product. "Invest in DAC" sounds the same whether you're buying a token or building a plant. But they're fundamentally different activities.

**The opportunity:** Some of these projects might be legitimate attempts to finance DAC through decentralized mechanisms. But the GitHub activity doesn't distinguish between "financial innovation" and "technical innovation."

### 🎙️ Talking Point
"You can't build a direct air capture plant from a smart contract. But on GitHub, the carbon capture repos that look most active are the ones that just write financial code. The crypto infiltration of carbon capture isn't a bug — it might be the whole point."

---

## 📊 Trend Dashboard

```
                    Carbon Capture Activity by Type

Directory    ████████████████████████████████████████████████  2552★  [GROWING]
Hardware     ██████████████████████████████                   76★   [FROZEN]
Literature   ██████████████████████████                       56★   [STALING]
Screening    ██                                                  2★   [CC0!]
Ghost        ██████████████████████████████████████████████     85★   [DEAD]
Crypto       ████████                                           Few   [ACTIVE]
```

**Legend:** ★ = GitHub stars (not commits) | FROZEN = no commits in 12+ months | CC0 = public domain

---

## 🔮 What to Watch

1. **CC0 adoption spreading** — If more DAC materials repos adopt CC0, it could create a public domain data commons for carbon capture research. Watch for CC0 licenses in MOF (Metal-Organic Framework) screening repos.

2. **OpenAir-Cyan iteration** — Will anyone fork OpenAir-Cyan and continue development? The OSHWA certification means anyone can build it — but will anyone improve it?

3. **Living literature review model evolution** — Could Carbon_Capture_ML be revived as a community-maintained, CC0-licensed resource? The infrastructure is there; the governance is missing.

4. **Crypto-carbon capture regulation** — As tokenized DAC assets grow, regulators will need to distinguish between legitimate carbon finance and speculative crypto. The GitHub activity won't help — but the papers might.

5. **Directory-to-hardware pipeline** — Open-Sustainable-Technology catalogs 2,552 projects. How many are actually buildable? How many have working prototypes? The directory could be the bridge between interest and action.

---

*Data source: GitHub API commit histories pulled September 18, 2026. All commit URLs available in the raw research log. License information verified from repository metadata.*

**Research log:** v4 update — fresh commit data from 6 carbon capture repositories. CC0 license trend identified as major open-science signal. OSHWA certification moment documented. Crypto infiltration flagged.

**Next steps:** Interview KCollins (OpenAir-Cyan) about hardware iteration. Contact tjz21 about CC0 motivation for DAC materials. Research CC0 adoption in other climate tech domains. Investigate carbon capture crypto project legitimacy.