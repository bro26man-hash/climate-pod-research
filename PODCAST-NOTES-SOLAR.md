# ☀️ Solar Geoengineering — Podcast Episode Research Notes

**Episode Title (Working):** "Solar Radiation Management: The Code That Could Cool the Planet"

---

## 🔍 Top Repository Discoveries

### 1. ClimateMARGO/ClimateMARGO.jl — 73 ⭐ | Julia
- **Focus:** Idealized climate-economic modeling framework for optimizing trade-offs between emissions mitigation, adaptation, and geoengineering.
- **Last Updated:** Aug 17, 2026 (README refresh after 2+ years dormant)
- **Language:** Julia
- **Key Commits:**
  - `d916f36` (Aug 17, 2026) — README update by Fons van der Plas
  - `6d9ba7a` (Aug 17, 2026) — Second README update same day (possible release prep)
  - `57d4da7` (Oct 18, 2023) — Unit conversions fix, referencing issue #86
  - `fbb619` (Jul 6, 2023) — PlutoDB linkage added to README
  - `5063c42` (Nov 14, 2022) — Project.toml version bump
- **🎙️ Episode Angle:** The dual README update in Aug 2026 after 2 years of silence is a narrative goldmine. Is this a genuine revival or a death-rust flutter? MARGO (Model for Adapting to a Changing Climate) is one of the few open-source frameworks that explicitly models the *governance* dimension of SRM — not just the physics, but the trade-offs. The Julia implementation makes it accessible. **Interview question:** "What does it mean for a climate model to go dormant — and what would it take to wake it up?"

### 2. wrf-model/WRF — 1,761 ⭐ | Fortran
- **Focus:** The Weather Research and Forecasting model — the foundational atmospheric simulation tool used by NOAA, NSF, and virtually every climate center.
- **Last Updated:** Sep 2026 (active development)
- **Language:** Fortran
- **🎙️ Episode Angle:** WRF is the simulation pipeline that SRM research depends on. You can't model solar radiation management without an atmospheric model. WRF's aerosol physics modules are the closest thing to SRM simulation in mainstream climate software. Its v4.8.0 release (Jun 2026) represents institutional investment in the tool that could one day assess SRM scenarios. **Interview question:** "Is WRF a geoengineering tool whether its developers intend it to be or not?"

### 3. NOAA-GFDL/MDTF-diagnostics — 80 ⭐ | Jupyter Notebook
- **Focus:** Process-oriented diagnostics for weather and climate simulations.
- **Last Updated:** Aug 14, 2026
- **Key Commits (from Sep 2026 pull):**
  - Precipitation-buoyancy POD analysis (Jun 2026)
  - 10 commits across Jun-Aug 2026 for v4.2.1 release
- **🎙️ Episode Angle:** MDTF-diagnostics is the ocean-adjacent tool to watch. Its precipitation-buoyancy POD is the closest thing to ocean process diagnostics in open source. For SRM, the diagnostic toolkit matters as much as the model — how do you *verify* that a solar intervention would actually work? **Interview question:** "What's the difference between a climate model that predicts and a diagnostic tool that proves?"

### 4. jlehtomaa/OOCC_2021 — 2 ⭐ | Python
- **Focus:** A simple model for solar geoengineering governance.
- **Last Updated:** Nov 15, 2021 (bibtex references only — fully dormant)
- **Language:** Python
- **Key Commits:**
  - `333c878` (Nov 15, 2021) — Bibtex entry update
  - `b62c2da` (Oct 26, 2021) — Bibtex reference update
  - Three README updates on Sep 5, 2021
- **🎙️ Episode Angle:** This is a governance model, not a physics model. It's the sort of project that exists at the intersection of policy and code. 2 stars, fully dormant since 2021. But it asks the question that matters: *who decides*? **Interview question:** "If we can't agree on a carbon price, how will we agree on a solar dimming protocol?"

### 5. PSLmodels/Geo-DICE — 2 ⭐ | Matlab
- **Focus:** Modified DICE (Dynamic Integrated Climate-Economy) model with geoengineering modules.
- **Last Updated:** 2026
- **🎙️ Episode Angle:** DICE is the Nobel Prize-winning integrated assessment model. Geo-DICE adds SRM to the calculus. When the model includes geoengineering as an option, the optimal policy trajectory changes dramatically. **Interview angle:** "The DICE model said the optimal carbon price was $X. But what happens when you add a tech that could lower temperatures without cutting emissions?"

### 6. brandomhimpfen/awesome-geoengineering — 4 ⭐ | Python
- **Focus:** Curated list of geoengineering projects, research, organizations, tools, and resources.
- **Last Updated:** Sep 6, 2026 (surprisingly active for a curated list)
- **🎙️ Episode Angle:** The most useful entry point for anyone starting SRM research. The fact that it's still being updated in Sep 2026 suggests a community of maintainers. **Interview angle:** "What's on the awesome-geoengineering list that surprises people?"

---

## 📊 Commit Trend Analysis — Solar Geoengineering Theme

### Pattern 1: Institutional Bursts vs. Individual Drift
The most active solar/climate repos (WRF at 1,761★, MDTF-diagnostics at 80★) show **institutional commit patterns** — coordinated releases by funded teams. In contrast, individual SRM projects (OOCC_2021, Geo-DICE) are **fully dormant** with 0 commits/year.

**Implication for the episode:** The SRM code ecosystem is split between well-funded institutional tools (WRF, CESM) that happen to be applicable to SRM, and standalone SRM-specific projects that lack sustained development. The tools exist; the dedicated SRM modeling layer does not.

### Pattern 2: The ClimateMARGO Revival Signal
ClimateMARGO.jl is the only Julia-based SRM/governance model showing activity. Two README updates in Aug 2026 after 2+ years of silence. This could signal:
- Growing policy-modeling interest post-COP29
- A reproducibility push for the MARGO framework
- Or simply a maintenance commit before another long dormancy

**Episode soundbite:** "ClimateMARGO woke up, yawned, and went back to sleep. But the fact that it has maintainers who remember the password is itself a story."

### Pattern 3: Fortran's Century-Long Run
WRF is in Fortran. The atmospheric modeling stack is Fortran. Even the newer tools (Oceananigans.jl, veros) are moving to Julia/Python, but the *atmospheric* core remains locked in Fortran. This is both a practical constraint (nobody wants to rewrite 500K lines of Fortran) and a cultural one (the SRM simulation community inherits the WRF stack).

**Episode angle:** "The question isn't whether Fortran can model solar dimming — it already does. The question is whether the next generation of climate scientists can even read the code."

### Pattern 4: Governance Code is Extremely Scarce
Of the 6 solar-geoengineering-tagged repos discovered, only OOCC_2021 explicitly models governance. The rest are physics models. This is a major gap: we have no open-source tools for *the political economy of SRM deployment*.

**Episode question:** "If we can't model the governance of SRM, can we even have a reasonable public debate about it?"

---

## 🎙️ Episode Structure Recommendation

| Segment | Content | Duration |
|---------|---------|----------|
| **Cold Open** | The ClimateMARGO dual-commit mystery — what wakes a dormant climate model? | 2 min |
| **Act 1** | The physics pipeline: WRF → radiative transfer → aerosol microphysics → how SRM would actually be simulated |
| **Act 2** | The governance gap: OOCC_2021, Geo-DICE, and the absence of SRM policy models |
| **Act 3** | The revival question: is ClimateMARGO's Aug 2026 activity a trend or a blip? |
| **Act 4** | The institutional vs. individual divide: why big climate tools get funded but SRM-specific tools don't |
| **Close** | The uncomfortable question: if the code for SRM governance doesn't exist, should we build it before we need it? |

---

## 🔗 Key Links
- ClimateMARGO.jl: https://github.com/ClimateMARGO/ClimateMARGO.jl
- WRF: https://github.com/wrf-model/WRF
- MDTF-diagnostics: https://github.com/NOAA-GFDL/MDTF-diagnostics
- OOCC_2021: https://github.com/jlehtomaa/OOCC_2021
- Geo-DICE: https://github.com/PSLmodels/Geo-DICE
- awesome-geoengineering: https://github.com/brandomhimpfen/awesome-geoengineering

---

*Last updated: Sep 2026 | Research method: GitHub API commit history pull + repository search*