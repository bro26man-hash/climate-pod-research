# 🌊 Ocean Intervention — Project Index

Quick-reference companion to `episodes/ocean-intervention/research-notes.md` for the ocean-intervention episode.

| # | Project | Repo | ⭐ | Lang | Last Active | Relevance |
|---|---------|------|----|------|-------------|-----------|
| 1 | open-sustainable-technology | [protontypes/open-sustainable-technology](https://github.com/protontypes/open-sustainable-technology) | 2,546 | — | Sep 2026 | Umbrella OSS directory for climate/energy/natural-resources tech |
| 2 | NebuGrid-OpenSource | [Team50-Labs/NebuGrid-OpenSource](https://github.com/Team50-Labs/NebuGrid-OpenSource) | 0 | C++ | Aug 2026 | Smart fog-harvesting + autonomous drip irrigation (conceptual analog to ocean-atmosphere flux manipulation) |
| 3 | Codes-RFG-Arctic-Impacts | [RhondaMueller/Codes-RFG-Arctic-Impacts](https://github.com/RhondaMueller/Codes-RFG-Arctic-Impacts) | 1 | — | Apr 2024 | Radiative-forcing code; Arctic ocean-ice/permafrost implications (tangential) |
| 4 | pmip_p2fvar_analyzer | [pmip4/pmip_p2fvar_analyzer](https://github.com/pmip4/pmip_p2fvar_analyzer) | 4 | — | Sep 2025 | CMIP6 palaeo-climate data analysis (ocean-forcing context) |

**Dedicated ocean-geoengineering repos: none found.** See the "Ocean-Intervention Gap" analysis in the research notes.

## 🧱 What OCEAN-INTERVENTION OPEN-SOURCE SHOULD LOOK LIKE (Wishlist)

| Capability | What it would model | Status on GitHub |
|------------|--------------------|------------------|
| Ocean Alkalinity Enhancement (OAE) codes | Dispersive nucleation, carbonate chemistry, alkalinity spreading | ❌ Essentially absent |
| Iron-fertilization simulators | Phytoplankton bloom dynamics, particle flux, sediment carbon burial | ❌ Essentially absent |
| Seaweed / blue-carbon trackers | Farm monitoring, carbon accounting, growth modeling | ❌ Essentially absent |
| Ocean circulation / upwelling models | MITgcm / NEMO configured for geoengineering scenarios | ⚠️ Only via general ocean models (not geo-specific) |
| Legal / governance tools | UNCLOS compliance, LFJL tracking, permitting | ❌ Absent |

## 📈 Commit Trend Takeaway

**The ocean-intervention gap is the defining finding.** GitHub's open-source climate-tech ecosystem has almost ZERO repositories specifically focused on ocean geoengineering, compared with a handful of solar and carbon-capture efforts:

| Theme | # Repos Found | Top Repo Stars |
|-------|--------------|----------------|
| Solar Geoengineering | 4 | 4 |
| Carbon Capture | 4 | 2 |
| Ocean Intervention | 1–2 (tangential) | 0 |

**Why the gap persists:**
1. **Experimental complexity** — ocean experiments need ships, permits, and massive logistics; harder to open-source than a DAC schematic or an atmospheric model.
2. **Governance sensitivity** — ocean fertilization (e.g., LOHAWEX, SO2020) triggered international legal challenges; researchers avoid public code.
3. **Institutional siloing** — work concentrates at a handful of institutions (GEOMAR Kiel, MIT, WHOI, Princeton) on internal tools.
4. **Media/political risk** — ocean interventions are perceived as riskier by funders, discouraging open publication.

**Podcast angle:** Ocean intervention is the "empty quadrant" of open climate tech — not because the science is trivial, but because the combination of experimental cost, regulatory fear, and institutional gatekeeping keeps it out of the open. The most promising open contribution isn't a giant ocean model; it's tractable, governance-aware tooling (alkalinity-dispersion toy models, carbon-accounting for kelp farms, UNCLOS compliance checkers) that lowers the cost of *thinking* out loud about ocean interventions.
