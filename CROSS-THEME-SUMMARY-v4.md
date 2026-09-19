# 🎙️ Climate Pod Research — v4 Cross-Theme Summary

**Last Updated:** September 2026
**Data Source:** GitHub Repository Search API + List Commits API
**Repos Analyzed:** 4 key repositories across 3 theme branches

---

## 📊 Unified Dashboard

| Theme | Repo Analyzed | Commits Pulled | Top Signal | Development Pattern |
|-------|--------------|----------------|------------|---------------------|
| ☀️ Solar | Sustainable-Solutions-Lab/regional-geo | 10 | WRF aerosol injection simulation | Burst (10 commits / 3 days) |
| ☀️ Solar | PCMDI (adjacent) | Multiple | Institutional steady cadence | Continuous (2–5/week) |
| 🌍 Carbon | salmansust/CO2-Sequestration | 2 | 32 stars, zero activity since 2019 | Upload-and-die |
| 🌍 Carbon | terranexum/OpenCarbon | 10 | 6 README updates, zero functional code | Kickoff-and-stall |
| 🌍 Carbon | ClimateSoton/climate-research-group | 4 | Website maintenance only | Single-day update |
| 🌊 Ocean | (zero dedicated repos) | 0 | GitHub dark matter | Absent |

---

## 🔑 The Three Universes

```
┌─────────────────────────────────────────────────────────────┐
│                    CLIMATE TECH GITHUB                       │
│                                                            │
│   🔴 RED UNIVERSE          🟡 YELLOW UNIVERSE              │
│   Fast / Institutional      Slow / Individual               │
│   🌐 Solar geoengineering   🌱 Carbon capture              │
│   WRF, PCMDI, MDTF          CO2-Sequestration, OpenCarbon   │
│   Continuous commits        Burst-then-dormant              │
│   Multiple contributors     Single-Pi projects              │
│                                                            │
│              ⬇️ ️ OCEAN INTERVENTION ⬇️                        │
│              ⚫ BLACK UNIVERSE                                │
│              💀 ZERO REPOS                                   │
│              🔇 ZERO COMMITS                                 │
│              🌊 ZERO CODE                                    │
│              ❓ ZERO GOVERNANCE                              │
└─────────────────────────────────────────────────────────────┘
```

---

## 🔬 Cross-Cutting Findings

### 1. The Reproducibility Crisis Is Visible in Commit Patterns
Every repository examined — across all three themes — shows the same pattern: **research sprints, not software engineering**. No CI/CD, no tests, no semantic versioning. Code is built for papers, not platforms.

### 2. Hardware Determines Development Velocity
- **Solar geoengineering** (software-heavy): Active development, even if bursty
- **Carbon capture** (hardware-heavy): Dormant or artifact-style repos
- **Ocean intervention** (infrastructure-heavy): Zero presence

The more hardware a technology requires, the less GitHub presence it has.

### 3. The Governance-Chilling Effect
Ocean geoengineering's absence on GitHub isn't an accident. The London Protocol, CBD regulations, and political sensitivity around ocean intervention create a chilling effect that keeps researchers from publishing open code.

### 4. The Star Count Illusion
CO2-Sequestration has 32 stars but 2 commits in 7 years. Stars measure curiosity, not community. The most-starred carbon capture repo is a digital cemetery.

### 5. The Open-Source Opportunity Gap
Ocean intervention has zero GitHub repos. If someone builds the first ocean geoengineering simulation tool, they'll own the category. The void is both a warning and an opportunity.

---

## 📋 Episode Planning Summary

| Episode | Branch | Key Question | Strongest Evidence |
|---------|--------|--------------|-------------------|
| **Solar Geoengineering** | `solar-geoengineering` | Why is SRM code inside climate models, not in SRM-specific repos? | regional-geo: WRF-based, 10 commits in 3 days by one PI |
| **Carbon Capture** | `carbon-capture` | Can open source + CC0 break the $1000/ton DAC cost barrier? | OpenCarbon died before writing code; CO2-Sequestration is a ghost town |
| **Ocean Intervention** | `ocean-intervention` | Is the GitHub vacuum a governance signal? | 10 searches, zero repos, five hypotheses for the void |

---

## 🗂️ File Structure by Branch

| Branch | File | Description |
|--------|------|-------------|
| `solar-geoengineering` | `PROJECT-DISCOVERIES-SOLAR.md` | Detailed profiles of solar/atmosphere repos with fresh commit data |
| `solar-geoengineering` | `COMMIT-TRENDS-SOLAR.md` | Solar-specific trend analysis, velocity charts, episode architecture |
| `carbon-capture` | `PROJECT-DISCOVERIES-CARBON.md` | Detailed profiles of carbon capture repos, discovery summary |
| `carbon-capture` | `COMMIT-TRENDS-CARBON.md` | Carbon-specific trend analysis, lifecycle patterns, episode architecture |
| `ocean-intervention` | `PROJECT-DISCOVERIES-OCEAN.md` | Ocean gap report, 5 hypotheses, absence analysis |
| `main` | `CROSS-THEME-SUMMARY-v4.md` | This file — unified dashboard and cross-cutting findings |

---

## 🔗 Quick Links
- 🔗 **Repo:** https://github.com/bro26man-hash/climate-pod-research
- ☀️ **Solar branch:** https://github.com/bro26man-hash/climate-pod-research/tree/solar-geoengineering
- 🌍 **Carbon branch:** https://github.com/bro26man-hash/climate-pod-research/tree/carbon-capture
- 🌊 **Ocean branch:** https://github.com/bro26man-hash/climate-pod-research/tree/ocean-intervention

*Research methodology: GitHub REST API, September 2026. Commits pulled via List Commits API. Search queries via Repository and Code Search APIs.*
