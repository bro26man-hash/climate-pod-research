# Climate Pod Research 🌍🎙️

Podcast research repository: climate technology and geoengineering — commit histories, project discoveries, and episode notes for **solar-geoengineering**, **carbon-capture**, and **ocean-intervention** themes.

---

## Episode Themes & Research Files

| Episode Theme | Research File | Branch |
|--------------|---------------|--------|
| ☀️ Solar Geoengineering (SRM) | [solar-geoengineering-projects.md](https://github.com/bro26man-hash/climate-pod-research/blob/solar-geoengineering/research/solar-geoengineering-projects.md) | [`solar-geoengineering`](https://github.com/bro26man-hash/climate-pod-research/tree/solar-geoengineering) |
| 🏭 Carbon Capture (CDR) | [carbon-capture-projects.md](https://github.com/bro26man-hash/climate-pod-research/blob/carbon-capture/research/carbon-capture-projects.md) | [`carbon-capture`](https://github.com/bro26man-hash/climate-pod-research/tree/carbon-capture) |
| 🌊 Ocean Intervention | [ocean-intervention-projects.md](https://github.com/bro26man-hash/climate-pod-research/blob/ocean-intervention/research/ocean-intervention-projects.md) | [`ocean-intervention`](https://github.com/bro26man-hash/climate-pod-research/tree/ocean-intervention) |

---

## Open-Source Projects Discovered

### Solar Geoengineering
| Project | Stars | Language | Last Active | Focus |
|---------|-------|----------|-------------|-------|
| [NorESM](https://github.com/NorESMhub/NorESM) | 51 | Python | Aug 2026 | Full Earth System Model (atmosphere, ocean, land, sea ice) |
| [C-ESM-EP](https://github.com/jservonnat/C-ESM-EP) | 7 | Jupyter/Python | Jul 2026 | Climate model evaluation platform (ORCHIDEE mapper) |

### Carbon Capture
| Project | Stars | Language | Last Active | Focus |
|---------|-------|----------|-------------|-------|
| [Carbon-Climate Box Model](https://github.com/lnnrtrmm/Carbon-Climate-Box-Model) | 6 | Python | Jun 2025 | Box-model CDR simulation (1→2→3 box configurations) |

### Ocean Intervention
| Project | Stars | Language | Last Active | Focus |
|---------|-------|----------|-------------|-------|
| [ACCESS-ESM1.6](https://github.com/ACCESS-NRI/ACCESS-ESM1.6) | 3 | Shell/Fortran | Aug 2026 | Australia's coupled ESM with biogeochemistry |
| [CMEW](https://github.com/MetOffice/CMEW) | 5 | Python | Sep 2026 | Climate model evaluation workflow (Cylc 8) |

---

## Commit Trend Summary (All Projects, Sep 2026)

| Repo | Primary Trend | Key Signal |
|------|--------------|------------|
| **NorESM** | Governance + docs maturity | CODE_OF_CONDUCT, US-language removal, submodule cleanup |
| **C-ESM-EP** | ORCHIDEE mapper overhaul + visualization | alb_mean (albedo!), Ctrl-click, rapid multi-contributor iteration |
| **Carbon-Climate Box Model** | Ocean carbon coupling + numerics | 2BoxOcean, spinup, thickness-dependent physics |
| **ACCESS-ESM1.6** | Release infrastructure | Monthly versions, spack dependency management, FMS/MOM5 updates |
| **CMEW** | Legacy cleanup + evaluation expansion | Recipe file removal, env var elimination, monsoon test, AutoAssess apps |

---

## Key Takeaways for the Podcast

1. **Albedo analysis is hot:** C-ESM-EP's alb_mean feature and NorESM's active development signal growing open-source capability for SRM reflectivity studies
2. **Carbon modeling is solo-developer territory:** The Carbon-Climate Box Model is entirely maintained by one person — ripe for community contribution
3. **Ocean intervention has the largest gap:** Almost no open-source parameterizations for iron fertilization or ocean albedo modification exist; most work is behind collaboration agreements at central modeling centers
4. **Infrastructure > Science:** ACCESS-ESM1.6 and CMEW show that even active repos spend most cycles on build systems and evaluation workflows, not new physics
5. **Reproducibility is a universal priority:** spack, tag-based versioning, and environment variable removal appear across ALL projects
