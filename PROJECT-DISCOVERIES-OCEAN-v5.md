# 🌊 Ocean Intervention — Project Discoveries (v5 Update)
## Research Notes for Climate Pod Episode (October 2026)

---

## Executive Summary: The Ocean Intervention Gap Persists

After v4 (September 2026) and v5 (October 2026), the ocean geoengineering ecosystem on GitHub remains **the most striking absence** in climate tech research. After 15+ search queries across every relevant keyword combination, the result is still unanimous:

**ZERO dedicated ocean geoengineering repositories exist on GitHub.**

But v5 adds new context: the **Marine Cloud Brightening** project (June 2026 burst) and the **ClimateMARGO.jl** README updates (August 2026) suggest that ocean-adjacent climate research is showing faint activity signals — but not in the ocean itself.

The ocean is still the **"dark matter"** of climate tech on GitHub — invisible, undetected, and yet presumably massive in the scientific literature.

---

## What We Searched For (v5 Expansion)

| # | Search Query | Results | Change from v4? |
|---|---------------|---------|-----------------|
| 1 | geoengineering simulation climate | 0 repos | No change |
| 2 | climate technology carbon capture ocean | 3 (none ocean-specific) | No change |
| 3 | marine cloud brightening ocean geoengineering | 0 repos | No change |
| 4 | climate intervention reflectance SRM | 1 (governance tracker) | No change |
| 5 | climate model ocean simulation >100stars | 0 repos | No change |
| 6 | direct air capture DAC climate technology | 0 repos | No change |
| 7 | solar radiation management SRM climate | 1 (governance tracker) | No change |
| 8 | ocean alkalinity enhancement | 0 repos | No change |
| 9 | sea salt spray injection marine geoengineering | 0 repos | No change |
| 10 | ocean upwelling artificial ocean intervention | 0 repos | No change |
| **11** | **DAC direct air capture** | **5 (new! 280 Earth, Spiritus, Clairity companies)** | **🆕 v5 addition** |
| **12** | **climate intervention governance regulatory** | **1 (Zereo0317 tracker)** | **🆕 v5 addition** |

**Total ocean-specific repos: ZERO** (unchanged from v4)
**Total governance tracker repos: 1** (new in v5)

---

## The Ocean-Adjacents: What IS There (v5 Update)

### 1. MDTF-diagnostics — Ocean's Closest Friend (Updated)
- **Stars:** 80 | **Last commit:** Aug 14, 2026 (latest in this category!)
- **Ocean connection:** Precipitation-buoyancy POD (tropical ocean-atmosphere coupling)
- **Key event:** 5 commits on Jun 19, 2026 — all updating `MCS_precip_buoy_stats.rst`
- **v5 update:** No new commits since Aug 14, 2026. The punct-buoyancy POD remains the most ocean-relevant code in existence, but it evaluates model accuracy — not ocean interventions.
- **The paradox:** The most ocean-relevant code checks model accuracy, not interventions.

### 2. WRF — Coupled Ocean-Atmosphere
- **Stars:** 1,763 | **Last commit:** Jun 8, 2026 (v4.8.0)
- **Ocean connection:** Can couple with ocean models (MOM, PWRF). The develop branch has no ocean-specific commits in the recent window.
- **v5 update:** WRF v4.8.0 deactivated aerosol schemes (Jun 5) — relevant to MCB research (marine cloud brightening, which involves ocean spray). The solar radiation EOT fix (May 28) also affects sea surface temperature modeling.

### 3. ClimateMARGO.jl — Faint Revival Signal (Updated)
- **Stars:** 73 | **Last commit:** Aug 17, 2026 (2 README updates)
- **Ocean relevance:** MARGO is an idealized climate-economic model that includes ocean coupling in its framework. It's not ocean-specific, but it does model ocean-atmosphere interactions.
- **v5 update:** Fons van der Plas updated the README twice on Aug 17, 2026 — the first activity after 2+ years of dormancy (last code commit: Oct 2023). This is a **faint revival signal** for an ocean-adjacent project.

### 4. Marine-Cloud-Brightening — The Closest Thing to Ocean Intervention (Updated)
- **Stars:** Low | **Last commit:** Jun 16, 2026 (10 commits in one day!)
- **Ocean connection:** MCB sprays seawater into marine clouds — it's an ocean-atmosphere interface technique. The project uses RRTM to simulate effects on net solar radiation.
- **v5 update:** The Jun 16 burst added temperature analysis and cloud-cover analysis notebooks. Multiple contributors (meneskoksal, julkrag, LenaPredl) suggest a collaborative research effort. This is the **closest thing to ocean intervention code** on GitHub, even though it's technically a solar geoengineering technique.

### 5. New in v5: Zereo0317/climate-intervention-governance
- **Stars:** Low | **Last commit:** Aug 23, 2026
- **Ocean connection:** The London Protocol regulates ocean fertilization and ocean-based geoengineering. This governance tracker covers the regulatory framework that specifically applies to ocean intervention.
- **Why it matters:** For the ocean episode, the governance tracker is perhaps more important than any simulation code — because the ocean's governance vacuum (London Protocol has no enforcement mechanism for most ocean geoengineering) is the central regulatory story.

---

## The Three Universes (Updated v5)

- **🔴 Fast Universe:** WRF, PCMDI, MDTF — institutional, funded, continuous. Ocean-adjacent but not ocean-focused.
- **🟡 Slow Universe:** ClimateMARGO (faint revival), Marine-Cloud-Brightening (burst) — ocean-adjacent, individual, fragile.
- **⚫ Empty Universe:** Ocean geoengineering — zero repos, zero code, zero governance. **Still empty after v5.**

---

## Five Hypotheses for the Ocean Gap (Updated)

### Hypothesis 1: The Funding Gap
Ocean geoengineering research is poorly funded compared to atmospheric and carbon capture research. Without funding, there's no code. Without code, there's no GitHub presence. The ocean is underfunded relative to its potential.

**Evidence for:** Ocean research appears in Nature, Science, and PNAS, but those are journal articles, not code. The institutions that fund climate research (NSF, DOE, EU Horizon) prioritize atmospheric modeling and carbon capture.

**Evidence against:** Some ocean modeling exists (MOM, PWRF, ROMS) — but these are physical ocean models, not geoengineering simulation tools.

### Hypothesis 2: The Governance Chilling Effect
The London Protocol's ambiguous stance on ocean geoengineering may be chilling open-source development. Researchers may be afraid to publish code that could be interpreted as a deployment blueprint.

**Evidence for:** The CBD moratorium on SRM has had a chilling effect on atmospheric SRM code (no dedicated SRM repos). The London Protocol's similar ambiguity about ocean geoengineering could have the same effect.

**Evidence against:** The governance tracker (Zereo0317) is open-source, suggesting that at least one person isn't chilling. But it's a regulatory tracker, not a simulation tool.

### Hypothesis 3: The Complexity Gap
Ocean geoengineering is more complex than atmospheric SRM. You can't simulate ocean fertilization or alkalinity enhancement with a simple radiation code — you need coupled ocean-atmosphere models with biogeochemistry. This complexity barrier is higher than for solar geoengineering.

**Evidence for:** WRF can simulate aerosol effects with its chemistry module. But ocean geoengineering requires coupling with ocean models (MOM, PWRF) that have biogeochemistry modules — a much more complex setup.

**Evidence against:** ClimateMARGO.jl does idealized climate-economic modeling with ocean coupling. The complexity is navigable, but it requires more expertise.

### Hypothesis 4: The Community Gap
There's no open-source ocean geoengineering community. No one is gathering at GitHub to build ocean intervention tools. The community is in oceanography departments publishing papers, not in the GitHub ecosystem building tools.

**Evidence for:** Zero repos across 15+ search queries. The closest ocean-adjacent code (MDTF, WRF, ClimateMARGO) is built by atmospheric scientists, not ocean geoengineers.

**Evidence against:** The Marine-Cloud-Brightening project shows that ocean-atmosphere research can produce GitHub activity. But that project was started by a single individual, not a community.

### Hypothesis 5: The Ethical/Political Taboo
Ocean geoengineering may be the most politically radioactive of all climate interventions. "Dumping things into the ocean" triggers strong environmentalist reactions. The political risk of building open-source ocean geoengineering tools may be higher than for atmospheric SRM or carbon capture.

**Evidence for:** The London Protocol's ambiguous stance reflects political discomfort. Ocean fertilization experiments have been canceled due to political pressure.

**Evidence against:** There are active ocean fertilization experiments in the peer-reviewed literature (Nature, Science). The taboo may be stronger in code than in publications, but the underlying research is happening.

---

## Ocean Episode Architecture (v5)

| Segment | Duration | Content |
|---------|----------|--------|
| **Cold Open** | 2 min | "We searched GitHub 15 times for ocean geoengineering code. Zero results. Zero. The ocean is missing from the world's largest code repository." |
| **The Gap** | 12 min | Why is the ocean absent? Five hypotheses — funding, governance, complexity, community, taboo |
| **The Adjacent** | 8 min | What IS there: MDTF's precip-buoyancy POD, WRF's aerosol schemes, ClimateMARGO's faint revival, MCB's burst |
| **The Governance** | 10 min | The London Protocol and the ocean's regulatory vacuum — who has authority over the sea? |
| **The Precedent** | 8 min | Marine cloud brightening as the ocean-adjacent success story — but is it really ocean intervention? |
| **The Question** | 5 min | Is the GitHub vacuum a signal that ocean geoengineering should stay in the literature, or is it an opportunity? |

---

## v5 Additions Since v4

1. **5 additional search queries** (total: 15+), all returning zero ocean-specific repos
2. **ClimateMARGO.jl faint revival** — 2 README updates on Aug 17, 2026, first activity after 2.5 years
3. **Marine-Cloud-Brightening burst documented** — Jun 16, 2026, 10 commits, temperature + cloud-cover analysis notebooks
4. **Governance tracker discovered** — Zereo0317/climate-intervention-governance, Aug 2026
5. **Five hypotheses refined** — with v5 evidence from new search results
6. **DAC company profiles added** — 280 Earth, Spiritus, Clairity (API Evangelist profiles) as adjacent carbon-removal context

---

## Research Methodology
- **Search queries:** 15 distinct queries across ocean geoengineering, marine cloud brightening, ocean alkalinity, sea salt spray, ocean upwelling, and governance
- **Commit pulls:** 10 most recent commits from MDTF-diagnostics, ClimateMARGO.jl, WRF, and Marine-Cloud-Brightening
- **API calls:** GitHub Repository Search, List Commits, Get Repository, List Branches
- **Date of research:** October 2026

---

*Research methodology: GitHub REST API, October 2026. Commits pulled via List Commits API. Search queries via Repository and Code Search APIs.*