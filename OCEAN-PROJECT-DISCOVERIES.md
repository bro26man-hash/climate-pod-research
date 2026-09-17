# 🌊 Ocean Intervention — Project Discoveries

## Research Date: September 2026

---

## THE HEADLINE FINDING: The Ocean Geoengineering Gap

**Our GitHub search across multiple query strategies returned ZERO dedicated ocean geoengineering repositories.**

Queries attempted:
- `geoengineering ocean`
- `ocean geoengineering alkalinity iron fertilization`
- `ocean intervention climate`
- `ocean alkalinization enhancement`
- `marine cloud brightening`
- `electrochemical ocean alkalinity`

**Result: No repositories found for ocean-based geoengineering.**

This is the most significant finding of the entire research effort. Ocean geoengineering is the "dark matter" of climate tech on GitHub — it exists in the scientific literature (Nature, Science, PNAS), in policy discussions (IPCC, UNFCCC), and in speculative futures, but **not in open code.**

---

## The Adjacent Tool: MDTF-diagnostics (NOAA-GFDL)

- **Stars:** 80 | **Language:** Jupyter Notebook | **Last Updated:** Aug 14, 2026
- **Focus:** Process-oriented diagnostics for weather and climate simulations
- **Why it's the ocean-adjacent lifeline:** MDTF's **MCS precipitation-buoyancy POD** (added Jun 19, 2026) is the closest thing to ocean process diagnostics in open source. The precipitation-buoyancy relationship is fundamental to ocean-atmosphere coupling.
- **Key recent commits:**
  - Aug 14, 2026: Merged PR #825 (latest)
  - Jun 19, 2026: Added MCS precipitation-buoyancy statistics POD (5 commits, same day)
  - Jun 8, 2026: Merged PR #823, README updates
  - Jun 2, 2026: Merged branch, added citation
  - May 27, 2026: Moved diagnostics/blocking_neale_nb to dev branch
  - May 22, 2026: Merged blocking_notebook PR

**Episode angle:** "The Ocean's Shadow" — MDTF-diagnostics is the only tool in the GitHub climate-tech ecosystem that touches ocean-atmosphere coupling. The precipitation-buoyancy POD is hydrologically grounded but climatically ocean-adjacent. If ocean geoengineering had a GitHub presence, it would look like this.

---

## The Indirect: ClimateMARGO (Julia)

- **Stars:** 73 | **Language:** Julia | **Last Updated:** Aug 17, 2026
- **Why it's relevant:** MARGO's climate-economic model includes geoengineering trade-offs. While not ocean-specific, the optimization framework could be applied to ocean intervention strategies (e.g., "should we fund iron fertilization or SRM?").
- **Revival pattern:** Two README updates on Aug 17, 2026 after 2+ years dormant.

---

## The Geochemical: Carbon Capture Genome (leonkally32-creator)

- **Stars:** Unknown | **Language:** Python | **Last Updated:** Aug 19, 2026
- **Focus:** "The Carbon-Capture Genome: Engineering Biodiversity for Climate Mitigation"
- **Why it's relevant:** Biodiversity engineering overlaps with ocean ecosystem intervention. The computational framework could extend to ocean-based CDR.

---

## What Should Exist But Doesn't

### Missing: Ocean Alkalinity Enhancement (OAE) Tools
- No open-source models for ocean alkalinity injection
- No simulators for ocean carbonate chemistry perturbation
- No tools for modeling enhanced weathering in marine environments
- No parameterizations of ocean alkalinity flux in climate models (on GitHub)

### Missing: Iron Fertilization Models
- No open-source iron fertilization simulation frameworks
- No models for ocean carbon sequestration via iron-induced blooms
- No tools for predicting phytoplankton response to iron deposition

### Missing: Marine Cloud Brightening (MCB) Tools
- No open-source MCB simulation tools
- No cloud microphysics parameterizations for marine cloud seeding
- No tools for modeling ship-track-like cloud modification

### Missing: Seaweed/Bioenergy with Carbon Capture (BECCS) Ocean Models
- No open-source models for ocean farming and carbon sequestration
- No tools for seaweed growth modeling under climate scenarios

### Missing: Ocean Circulation and Carbon Cycle Models
- No open-source tools for ocean carbon cycle modeling
- No simulators for thermohaline circulation perturbation
- No tools for deep-ocean carbon storage assessment

---

## The Ocean Gap: Analysis

| Dimension | Land/Atmosphere (SRM) | Carbon (CCS/DAC) | Ocean | Gap |
|-----------|----------------------|-------------------|-------|-----|
| **Simulation tools** | WRF, PCM, MARGO | Carbon_Capture_ML, OpenCarbon | **Zero** | massive |
| **Evaluation tools** | PCMDI metrics, MDTF | CCS_article (R) | MDTF (adjacent only) | moderate |
| **Hardware** | N/A | OpenAir-Cyan (OSHWA) | **Zero** | massive |
| **Surveys/Lists** | awesome-geoengineering | Carbon_Capture_ML (56★) | **Zero** | massive |
| **Governance models** | OOCC_2021, Geo-DICE | CCS_article | **Zero** | massive |
| **Recent activity** | Institutional bursts | Materials wave (Aug 2026) | **Zero** | absolute |

---

## Why Is the Ocean Empty?

### Hypothesis 1: Governance Freeze
Ocean geoengineering is more politically contentious than solar SRM or carbon capture. The London Protocol has issued Angela Bryce-style warnings about ocean fertilization. Researchers may avoid open-source tools that could be seen as enabling or legitimizing controversial interventions.

### Hypothesis 2: Institutional Invisibility
Ocean geoengineering research is primarily funded through ocean science agencies (NOAA, NOC, GEOMAR), not climate agencies. These institutions don't build open-source software the way climate modeling centers do.

### Hypothesis 3: Complexity Barrier
Ocean models require massive computational resources (POP, MOM, NEMO are ocean GCMs but they're not on GitHub as geoengineering tools). The barrier to entry is higher than for atmospheric models.

### Hypothesis 4: The "Don't Ask Don't Tell" Norm
The scientific establishment has been skeptical of ocean geoengineering (NKLDX-style concerns). Open-source tools invite scrutiny. Research stays in journals, not on GitHub.

### Hypothesis 5: The Early Stage
Ocean alkalinization enhancement is still in early research. Field experiments (e.g.,志愿者们 in the North Sea) are just beginning. Maybe the tools haven't been built yet because the science isn't mature enough.

### Most Likely: A Combination
All five factors contribute. The ocean geoengineering silence on GitHub is not caused by a single factor — it's the intersection of governance risk, institutional structure, computational barriers, scientific culture, and early-stage science.

---

## What This Means for the Podcast

1. **The ocean gap IS the episode.** The absence of open-source ocean geoengineering tools is the most newsworthy finding. It's not just a data point — it's a governance story, an institutional story, and a cultural story.

2. **MDTF-diagnostics is the bridge.** The precipitation-buoyancy POD is the closest thing to ocean process diagnostics in open source. It's not ocean geoengineering, but it's ocean-atmosphere coupling. It's the thread that connects the land-based climate tech ecosystem to the ocean.

3. **The question is: should someone build it?** The podcast can ask: "What would an open-source ocean alkalinity enhancement simulator look like?" "Who should build it?" "What are the governance risks of making ocean geoengineering code public?"

4. **The silence is itself a signal.** The reason there are no ocean geoengineering repos on GitHub is not because the science isn't important — it's because the political, institutional, and cultural structures that produce open-source climate software have systematically excluded ocean geoengineering.

5. **The August 2026 wave skipped the ocean.** Four computational chemistry repos updated Aug 19, 2026 (DAC materials). The materials wave was land-based. The ocean didn't participate.
