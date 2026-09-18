# 🌊 Episode 3 Outline: "The Ocean Has 71% of the Codebase and 0% of the Geoengineering"
## Ocean Intervention GitHub Research | Climate Pod Research | September 2026

---

## Episode Metadata
- **Title:** "The Ocean Has 71% of the Codebase and 0% of the Geoengineering"
- **Theme:** Ocean Geoengineering (OAE, Iron Fertilization, Marine Cloud Brightening)
- **Duration target:** 45-50 minutes
- **Research basis:** 10+ GitHub search queries (0 results), 3 ocean-adjacent repos analyzed, Oceananigans.jl (1,413★)
- **Key insight:** Zero ocean geoengineering repositories exist on GitHub

---

## Act 1: The Thriving Ocean Physics (12 min)

### Opening Image
> "We searched GitHub for every ocean geoengineering term we could think of. Marine cloud brightening. Ocean alkalinity enhancement. Artificial upwelling. Ocean iron fertilization. Zero repositories. Not one. Meanwhile, the atmospheric model WRF gets 3 commits a week. Oceananigans.jl gets 4 commits a day. The ocean covers 71% of the Earth's surface and has 0% of the geoengineering codebase."

### Oceananigans.jl — The World's Best Ocean Model That Doesn't Do Interventions
- **1,413★** — the most active ocean code on GitHub
- 15 commits in 4 days (September 15-18, 2026) — ~4 commits/day
- 5+ contributors from UC Berkeley's CliMA project
- **Latest feature:** Lagrangian particle tracking (bouncing off immersed boundaries)
- **What it simulates:** Ocean fluid dynamics — nothing else
- **What it doesn't simulate:** Any ocean intervention whatsoever

### MDTF's Precipitation-Buoyancy POD — The Ocean's Only Advocate
- **80★** — the most ocean-relevant diagnostic tool in open source
- **5 commits on June 19, 2026** — all on one file (MCS_precip_buoy_stats.rst)
- Evaluates whether climate models correctly simulate ocean-atmosphere coupling
- **The closest thing to ocean geoengineering code on GitHub** — and it's a diagnostic, not an intervention

### WRF — The Atmospheric Model with an Ocean Boundary
- **1,763★** — gets better solar radiation correction (May 28) while deprecating aerosol physics (Jun 5)
- Can be coupled to ocean models, but no one has built an SRM or ocean intervention module
- The aerosol deprecation is a double-edged sword for ocean chemistry modeling

### Act 1 Key Insight
> "The most active code in this entire research project is about ocean physics. And not a single line of it is about what we'd do to the ocean."

---

## Act 2: The Intervention Vacuum (15 min)

### The Search Results
| Search Term | Repos Found |
|-------------|-------------|
| `"ocean geoengineering"` | **0** |
| `"marine cloud brightening"` | **0** |
| `"ocean alkalinity enhancement"` | **0** |
| `"artificial upwelling"` | **0** |
| `"ocean iron fertilization"` | **0** |
| `"marine geoengineering"` stars:>10 | **0** |
| `topic:geoengineering ocean` | **0** |

**Total: ZERO ocean geoengineering repositories.**

### The Hypotheses (Ranked)
1. **Governance chill** — London Protocol deters code publication
2. **Complexity curse** — Physics + chemistry + biology = 3x SRM complexity
3. **Funding gap** — Ocean interventions underfunded vs. SRM and DAC
4. **Biology barrier** — No repo models ecosystem response to interventions
5. **Oceananigans paradox** — Tool too sophisticated for intervention use

### The Governance Thesis
The most compelling explanation: **When the London Protocol debated ocean fertilization, they weren't just regulating experiments. They were regulating the question.** Because code is speech, and a repository is a declaration.

- A repo that simulates upwelling could be used to argue "someone has already modeled this, it's safe"
- A repo that simulates alkalinity enhancement could be used to argue "the technology exists, why not deploy it"
- The absence of code creates an **information asymmetry** that governance frameworks prefer

### Act 2 Key Insight
> "The silence on GitHub isn't accidental. It's a governance artifact. The legal community may have won the ocean debate by making the code community too afraid to write it."

---

## Act 3: The Connection That Doesn't Exist Yet (15 min)

### The Cross-Theme Triangle
The three themes of this podcast series actually share ocean tools:

```
         WRF (Solar)
         /        \
        /          \
       /            \
      /              \
MDTF -------- Oceananigans.jl
(Precipitation-\  (Ocean Physics)
buoyancy POD)

WRF's solar radiation → accurate SST → drives ocean convection
MDTF's POD → evaluates precipitation-buoyancy coupling
Oceananigans.jl → simulates ocean physics → provides boundary conditions

THE MISSING LINK: Nobody connects these for intervention scenarios.
```

### The 7 of 8 Pieces (Oceananigans.js Already Has)
1. ✅ **Lagrangian particle tracking** — Track dispersal of intervention materials
2. ✅ **Immersed boundaries** — Model artificial seafloor structures
3. ✅ **Time-dependent forcings** — Apply solar radiation or upwelling scenarios
4. ✅ **Differentiable programming** — Optimize intervention strategies
5. ✅ **GPU acceleration** — Fast enough for ensemble scenario runs
6. ✅ **Output diagnostics (TimeDerivative)** — Assess intervention impacts
7. ✅ **Robust column solving** — Handle extreme conditions
8. ❌ **Intervention Module** — Nobody has written this

### What Would a Cross-Theme Episode Look Like?
**Act 1:** The Thriving Ocean Physics (Oceananigans, MDTF, WRF)
**Act 2:** The Intervention Vacuum (Zero repos, governance chill)
**Act 3:** The Connection (Oceananigans + MDTF + WRF = intervention capability)

### Act 3 Key Insight
> "Oceananigans.jl already has 7 of the 8 tools needed for ocean intervention modeling. The 8th tool is a click in a GitHub Issues page: 'We should build an ocean intervention module.'"

---

## Closing Segment (5 min)

### The Empty Shelves Metaphor
> "GitHub is a library of climate solutions. The atmospheric section is packed. The carbon section is filling up. But the ocean section? Empty shelves. A single sign: 'Unfortunately, this section is not yet written.' The ocean covers 71% of the Earth's surface and 0% of the geoengineering codebase."

### The Final Question
> "Did the legal community win the ocean debate by making the code community too afraid to write it? Or is the silence simply the natural state of a field that hasn't yet decided it's ready?"

### The Call to Action
> "The ocean doesn't need more models. It needs one person who wants to use an existing model — Oceananigans.jl — to ask a question nobody's asked in code. The precip-buoyancy POD was built on June 19, 2026, by one person in one day. That's the closest thing to ocean geoengineering code on GitHub. And it's a diagnostic. The intervention tools don't exist. The evaluation tools do. The gap isn't technical. It's moral."

### Final Image
> "On June 19, 2026, Wei-Ming Tsai made 5 commits to a documentation file. Not code — documentation. But it was about the precipitation-buoyancy POD, the tool that tells you whether your climate model gets ocean-atmosphere coupling right. That's the ocean's closest friend in the geoengineering codebase. And it's a diagnostic. The ocean models are thriving. The intervention tools are nonexistent. The evaluation infrastructure is the only bridge between the two — and it was built to measure, not to change."

---

## Production Notes

### Sound Design
- **Cold Open:** Deep ocean ambience, sonar pings, then silence (the gap)
- **Oceananigans montage:** GPU humming, water simulation visuals, typing
- **The Search:** Keyboard sounds fading to silence — query after query, then silence
- **The POD:** Rain sounds, then ocean waves — the precipitation-buoyancy connection
- **The Connection:** Three instruments playing together — WRF, MDTF, Oceananigans in harmony
- **Closing:** A single wave, then quiet

### Guest Suggestions
- **Oceananigans.jl maintainer:** "Has anyone suggested adding intervention modules?"
- **London Protocol observer:** "Does the governance framework discourage code publication?"
- **MDTF developer:** "How would the precip-buoyancy POD evaluate ocean interventions?"
- **Marine geoengineering researcher (off-GitHub):** "What ocean intervention code exists that's not on GitHub?"

### Visual Aids
- Ocean coverage (71%) vs. code coverage (0%) — the shocking contrast
- Oceananigans.jl commit heat map (September 2026 — daily activity)
- The 5-commit June 19 blitz on MCS_precip_buoy_stats.rst
- The cross-theme triangle (WRF + MDTF + Oceananigans)
- Proposed Ocean Intervention Module architecture diagram

---

*Last updated: September 2026 (v4) | Search queries: 10+ | Ocean geoengineering repos: 0 | Ocean-adjacent repos analyzed: 3*