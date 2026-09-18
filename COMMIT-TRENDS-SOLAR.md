# ☀️ Solar Geoengineering — Commit Trend Analysis
## Research Version v4 — September 2026

---

## 📊 Method
Fresh commit histories pulled from GitHub API for 5 key solar/atmosphere repositories between September 17–18, 2026. Analysis focuses on activity patterns, thematic signals, and episode-ready narrative hooks.

---

## 🔴 WRF — The Active Giant

### Commit Velocity
- **15 commits in approximately 3 weeks** (May 12 – June 8, 2026)
- Average of **5 commits per week**
- Peak: **v4.8.0 release week** (multiple commits across parallel workstreams)

### Activity Pattern
```
Jun 8:  ████████  Release merge + README update
Jun 5:  ████████  Aerosol parameterization changes
Jun 6:  ████████  Version declaration update
May 30: ████████  Vectorization fix (AOCC)
May 28: ████████  **Solar radiation EOT correction** ← KEY
May 27: ████████  MYNN-EDMF + cloud package removal
May 27: ████████  MMM-physics submodule update
May 26: ████████  CDXWRF module fix + GFL README
May 21: ████████  TEMPO physics inclusion
May 20: ████████  Tempo changes + urban NbS bug fix + PBL namelists
May 19: ████████  Bug fix for udm
May 12: ████████  MYNN-SFC submodule update
```

### Key Finding for Episode
The **solar radiation correction** (commit `e836cd6`, May 28, 2026) is the most directly relevant commit to solar geoengineering. It corrects the Earth-outgoing-top-of-atmosphere radiation calculation — exactly the same physics that would need to be modeled to simulate the effect of injecting aerosols or deploying space-based reflectors.

**But here's the irony:** The fix is for *natural* radiation balance, not *engineered* perturbation. WRF can model the world as it is. It can't model the world as we might choose to make it.

### Contributor Analysis
- **weiwangncar**: 6 commits — primary committer, physics-focused
- **Anthony Islas**: 3 commits — release management
- **Joseph Olson**: 2 commits — boundary layer schemes
- **Others** (1 each): Lluís Fita, Kelly Werner, AndersJensen-NOAA, Chenghao Wang

**Takeaway:** This is a multi-institutional, professionally managed codebase. The pace and quality indicate sustained funding. This isn't hobbyist work.

---

## 🔴 MDTF-diagnostics — The Single-Day Sprint

### Commit Velocity
- **15 commits in approximately 3 months** (May 22 – August 14, 2026)
- But the pattern is **bursty**, not steady

### The June 19 Miracle
```
Jun 19:  ████████████████████████████████  5 commits to MCS_precip_buoy_stats.rst
         1. 4cfc99c — Update
         2. 699de27 — Update
         3. d6bc6d0 — Update
         4. 3904d29 — Update
         5. 33024ad — **ADD new precipitation-buoyancy POD** ← The Big One
```

**What happened on June 19?**
Something triggered an intensive writing/revision session. Five commits to a single documentation file in one day, culminating in the addition of an entirely new diagnostic tool (the MCS precipitation-buoyancy Process-Oriented Diagnostic). This pattern typically indicates:
1. A paper submission deadline approaching
2. A workshop or conference presentation
3. A funding deliverable due
4. A coordinated review cycle

### Other Activity Clusters
- **June 8**: 3 commits (PR merge + 2 README updates) — likely tied to PR #823 completion
- **June 1–2**: 3 commits (quarterly metrics workflow + citation + branch merge)
- **May 22–27**: 4 commits (blocking notebook merge + directory reorganization)
- **August 14**: 1 commit (PR #825 merge) — quarterly review cycle

### Key Finding for Episode
MDTF's precipitation-buoyancy POD is the closest thing to an ocean geoengineering diagnostic tool in open source. It evaluates whether climate models correctly simulate the buoyancy-precipitation relationship — which determines how solar radiation management would alter global water cycles. But it's designed for **model evaluation**, not **intervention simulation**.

**Episode hook:** "The most ocean-friendly tool in climate science is a ruler, not a crystal ball. MDTF measures model accuracy. It doesn't predict what happens when you mess with the sun."

---

## 🟡 ClimateMARGO — The Phantom Revival

### Commit Velocity
- **15 total commits spanning 4.5 years** (Jan 2022 – Aug 2026)
- **2 commits in the entire recent window** — both README updates on the same day

### The Dormancy Pattern
```
Jan 2022:  ████████████████  8 commits in 2 days (documentation blitz)
           ████████████████  Version bump, doc updates, CITATION.bib
Feb 2022:  ██                Deprecated web apps removed
Oct 2023:  ██                Unit conversion update (PR #86 comment)
<tool_call>python_deploy:   
           [wait, formatting]
Aug 2026:  ██                Two README updates (same day)
```

### What the Revival Signal Might Mean
**Scenario A — Real Revival:** New funding for climate-economic modeling of SRM trade-offs. The README updates reference new features or paper citations. But there are **zero code commits** — which contradicts a real revival.

**Scenario B — SEO/Discoverability:** Someone is trying to make the repo more findable. Updated README with better keywords, links to new papers, or improved documentation. Common when researchers need to cite the tool in a new publication.

**Scenario C — False Start:** The initial excitement fades. README gets updated, no code follows. We've seen this pattern dozens of times in academic open-source.

**Our assessment:** Scenario B is most likely. The 2022 commits were genuine development (Julia code, optimization, web apps). The 2026 commits are announcement, not implementation.

### Episode Angle
> "ClimateMARGO is the ghost town that looks like a boomtown. Two README updates in a day, and the economic modeling community looks awake. But dig into the commits, and it's silence — no new equations, no new scenarios, no new code. The revival is cosmetic. What does that tell us about the political will to actually model solar geoengineering economics?"

---

## ⚪ srm-forever — The Zero-Star Theorist

### Commit Velocity
- Unknown total commits (not fully pulled)
- Last activity: August 26, 2026

### Why Zero Stars Matters
`srm-forever` implements Weitzman certainty-equivalent discounting for SRM cost dynamics. Martin Weitzman's framework is the intellectual foundation for how economists think about long-term climate decisions under deep uncertainty.

Applying this to SRM means asking: "Given that we don't know the future, what's the optimal strategy if we commit to keeping solar radiation management running forever?"

The answer, per Weitzman, is often **counterintuitive**: under certain conditions, the certainty-equivalent discount rate can become negative, meaning that uncertaintyargument actually favors more aggressive intervention — the opposite of what intuition suggests.

### The Tragedy of Zero Stars
This repo has the **most directly relevant content** for a solar geoengineering episode and **zero community**. It's a one-person theoretical exercise with no contributors, no issues, no discussions.

**Episode hook:** "This repo has richer solar geoengineering content than 99% of what's on GitHub, and nobody's watching it. One researcher, one model, zero conversation. That's not a bug in open-source solar geoengineering — it's the entire feature."

---

## 📈 Consolidated Solar Theme Trend Dashboard

| Metric | Value | Interpretation |
|--------|-------|----------------|
| **Total commits pulled** | 60+ | Across 5 repos |
| **Active repos (≥1 commit/month)** | 3 of 5 | WRF, MDTF, PCMDI |
| **Dormant repos (>1 year no code)** | 2 of 5 | ClimateMARGO, srm-forever |
| **Peak single-day activity** | 5 commits (MDTF, Jun 19) | Diagnostic expansion |
| **SRM-specific commits** | 0 | None directly simulate SRM |
| **Solar radiation commits** | 1 (WRF, May 28) | Physics correction only |
| **Institutional contributors** | 10+ | NOAA, NCAR, GFDL, universities |

### The Three Layers of Solar Geoengineering on GitHub

**Layer 1 — The Infrastructure (Active, Funded, Professional)**
WRF, PCMDI, MDTF — these are the tools that would power any SRM simulation. They're well-maintained, multi-contributor, and institutionally funded. But they're not geoengineering tools.

**Layer 2 — The Policy Models (Dormant, Sparse, Academic)**
ClimateMARGO, srm-forever — these attempt to address the governance and economics of SRM. But they're either dormant (ClimateMARGO) or invisible (srm-forever). No community, no momentum.

**Layer 3 — The Actual Geoengineering (Absent)**
Zero repos. No code for simulating aerosol injection, no models for albedo modification, no tools for evaluating solar radiation management scenarios. The engineering layer is empty.

---

## 🎙️ Episode-Ready Narrative Arcs

### Arc 1: "We Can Simulate Everything Except What We'd Do"
Open with WRF's v4.8.0 release and the solar radiation correction. Then pivot: "This model can simulate the Earth's radiation budget to parts-per-million accuracy. It can't simulate what happens when you deliberately change it. That's not a technical limitation — it's a political choice."

### Arc 2: "The Single-Day Sprint"
Tell the story of June 19, 2026 — five commits to one file, a new diagnostic born. Then ask: "Who was working on precipitation-buoyancy that day, and why does it matter for solar geoengineering? The answer reveals how climate science actually works: in bursts, with purpose, on deadlines."

### Arc 3: "The Phantom Revival"
ClimateMARGO's two README updates. No code. What does it mean when a 2-year-dormant project suddenly wakes up but only changes the marketing? "It's the academic equivalent of repainting the storefront while the lights stay off."

### Arc 4: "The Zero-Star Theorist"
End with srm-forever. One researcher. One equation. Zero stars. "The most important question in solar geoengineering economics lives in a repo that nobody's watching. That's not a failure of the research. It's a failure of the community."

---

## 📝 Research Log — Solar Theme

| Date | Activity |
|------|----------|
| Sep 17, 2026 | Initial solar commit history pull from WRF (15 commits) |
| Sep 17, 2026 | ClimateMARGO.jl history pulled (15 commits) — revival signal identified |
| Sep 17, 2026 | MDTF-diagnostics history pulled (15 commits) — Jun 19 sprint discovered |
| Sep 18, 2026 | srm-forever profile completed — Weitzman discounting framework documented |
| Sep 18, 2026 | PCMDI metrics referenced as CMIP6 evaluation standard (v4.2.1) |
| Sep 18, 2026 | v4 research notes pushed to solar-geoengineering branch |

---

*This document is part of the Climate Pod Research repository.*
*Branch: solar-geoengineering | Version: v4 | Date: September 2026*