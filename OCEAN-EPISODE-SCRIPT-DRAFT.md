# 🌊 Ocean Intervention — Episode Script Draft
## Git Evidence-Based Script Outline
### v4 — September 2026

---

## Cold Open (2 min)

*"We searched GitHub ten different ways for ocean geoengineering code. Ten searches. Zero results. While solar has atmospheric models and carbon has DIY hardware, the ocean has nothing — not a single repository. This isn't a GitHub problem. It's a mirror. The code tells us what the community thinks is possible. And for ocean geoengineering, the code is silent. This episode, we chase that silence."*

---

## Segment 1: The Empty Quadrant (8 min)

### The Zero Result
- 10+ search queries across GitHub: `ocean climate intervention`, `marine geoengineering simulation`, `ocean fertilization climate`, `artificial upwelling`, `ocean alkalinization`, etc.
- Every query returns zero repos
- Compare: 8+ solar geoengineering repos, 9+ carbon capture repos
- The ocean is the missing theme in open-source climate tech

### The Scale of the Void
- Solar: ClimateMARGO (73★), WRF (1,761★), awesome-geoengineering (4★), GeoVision (0★)
- Carbon: open-sustainable-technology (2,552★), OpenAir-Cyan (76★), Carbon_Capture_ML (56★), tjz21 CC0 repos (2★ each)
- Ocean: **nothing**

### Talking Point
- *"We found zero repositories for ocean geoengineering on GitHub. Not a few. Not a handful. Zero. After searching ten different ways, the GitHub vacuum is the biggest finding in this research. The silence is the signal."

### Evidence
- All 10+ search queries returned 0 results
- GitHub is the world's largest code hosting platform — if the code existed, it would be here

---

## Segment 2: The Tool That Came Close (6 min)

### The Precip-Buoyancy POD
- MDTF-diagnostics: NOAA's process-oriented diagnostic framework
- Jun 19, 2026: 5 commits for the same file in one day — a burst of development
- The precip-buoyancy POD is the most ocean-relevant tool in open source
- But it's for **evaluating models**, not **simulating interventions**

### The Critical Distinction
- MDTF tells you if your model correctly simulates precipitation-buoyancy relationships
- It doesn't tell you what happens if you add iron to the ocean (fertilization)
- It doesn't tell you what happens if you brighten marine clouds
- It doesn't tell you what happens if you pump cold water to the surface
- **Gap: between evaluation and intervention**

### Talking Point
- *"The closest thing to an ocean geoengineering tool on GitHub is a diagnostic that checks if your climate model is right. It evaluates. It doesn't simulate. It's the world's most sophisticated 'is your model for the ocean correct?' tool — but it can't answer 'what should we do to the ocean?' That's the gap."

### Evidence
- https://github.com/NOAA-GFDL/MDTF-diagnostics/commit/33024ad30f39b05a473a8e3613bc5aed8b6cc176 (Jun 19, 2026 — new POD)
- 5 commits on Jun 19 for MCS_precip_buoy_stats.rst

---

## Segment 3: Why the Void Exists (6 min)

### Four Hypotheses
1. **Funding Invisibility:** Ocean geoengineering has no dedicated funding program. NOAA has no geoengineering line. The Radcliffe program focuses on solar. Ocean alg geoengineering is at the fringe of oceanographic institutions.

2. **Governance Taboo:** The London Protocol prohibits ocean fertilization. No country has a regulatory framework for ocean intervention. Unlike carbon capture (45Q) or solar (some intelligence community interest), ocean geoengineering has zero policy tailwinds.

3. **Technical Difficulty:** You can't test ocean geoengineering in a lab. MCB requires ships, monitors, and ocean campaigns. The cost of entry is millions, not thousands. You need a research vessel to do what OpenAir-Cyan did in someone's garage.

4. **Public Good Problem:** Ocean interventions have global benefits and concentrated costs. Nobody has incentive to fund them. "The ocean belongs to everyone" means "nobody's responsible for funding ocean geoengineering research."

### Talking Point
- *"Solar geoengineering has the intelligence community interested. Carbon capture has 45Q tax credits and ESG money. Ocean geoengineering has... nobody. The void isn't an accident. It's an equilibrium."

### Evidence
- London Protocol explicitly prohibits ocean fertilization
- No national ocean geoengineering program exists
- Project costs: MCB requires ships ($50K+ per day), ocean fertilization requires thousands of tonnes of iron

---

## Segment 4: The Blueprint (4 min)

### What Would Open-Source Ocean Geoengineering Look Like?

| Concept | Analog in Existing Ecosystem | Ocean Equivalent? |
|---------|-------------------------------|---------------------|
| Simulator | WRF (solar) | Marine Cloud Brightening LES tool |
| Decision tool | CarbonLens (carbon) | Fertilization LCA tool |
| DIY hardware | OpenAir-Cyan (carbon) | Upwelling pump open hardware |
| Data release | tjz21 CC0 repos (carbon) | Alkalinity enhancement experiments dataset |
| Resource list | awesome-geoengineering (solar) | Ocean geoengineering bibliography |

### The Blueprint is Complete — The Code is Missing
Every analog exists in solar or carbon. None has been built for ocean. The blueprint is sitting in other people's repos.

### Talking Point
- *"We know how to build an open-source SRM simulator. We know how to build an open-source DAC device. We know how to curate a resource list. We just haven't done it for the ocean. The blueprint is already in the solar and carbon repos. It just hasn't been copied over."

### Evidence
- Cross-reference: WRF, OpenAir-Cyan, awesome-geoengineering (all analyzed in solar/carbon episodes)

---

## Segment 5: Silence as Signal (2 min)

### The Core Argument
The GitHub vacuum is not neutral. It's a governance signal. Just as WRF's aerosol scheme changes tell a story about institutional avoidance of SRM simulation, the zero-repo result for ocean geoengineering tells a story about **which interventions the tech community won't even code.**

### Talking Point
- *"If ocean geoengineering were considered viable, fundable, and permissible, someone would have written a marine cloud brightening simulator by now. The fact that no one has — after a decade of scientific papers — is the most honest metric in this entire research project. The code says what the funding can't."

---

## Closing (2 min)

*"We searched ten ways for ocean geoengineering code on GitHub. Zero results. The closest ocean tool is a diagnostic that evaluates models, not one that simulates interventions. The ocean is the forbidden quadrant of climate tech — where the sun gets models, carbon gets hardware, and the ocean gets nothing. The silence isn't an oversight. It's a signal. And the question this episode has to ask: is the silence correct? Or is it a self-fulfilling prophecy — because we can't model it, we can't deploy it, because we can't deploy it, we won't model it? The code is missing. But maybe that's the point."*

---

## Production Notes

| Element | Detail |
|---------|--------|
| **Total runtime** | ~24 min (5 segments + cold open + closing) |
| **Key evidence links** | 4 GitHub commit URLs, 10+ search query log |
| **Guest candidates** | MDTF-diagnostics developer (Wei-Ming Tsai), ocean geoengineering researcher from中叶 omitted, London Protocol expert |
| **Topics to handle carefully** | London/or-Moscow Protocol implications (geopolitical), iron fertilization (controversial), marine cloud brightening (visual impact concern) |
| **Recommended pre-listen** | Solar episode first (contrast: solar has models but no hardware; ocean has neither) |
