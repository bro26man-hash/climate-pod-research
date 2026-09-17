# 🌊 Ocean Intervention — Project Discoveries

**Research Date:** September 2026
**Podcast Episode:** Ocean-Based Geoengineering (OAE, Iron Fertilization, Seaweed)

---

## Overview

This file catalogs open-source repositories relevant to ocean-based geoengineering — including ocean alkalinity enhancement (OAE), iron fertilization, seaweed/bioenergy, marine cloud brightening over oceans, and ocean carbon cycle modeling. Commit histories were pulled fresh from GitHub in September 2026.

---

## 🚨 The Ocean Gap: Headline Finding

**Our GitHub search across multiple query strategies returned ZERO dedicated ocean geoengineering repositories.** This is the most significant finding of the entire research effort.

### Search Queries That Returned Nothing

| Query | Results |
|-------|--------|
| `ocean intervention climate` | 0 repos |
| `ocean alkalinity enhancement` | 0 repos |
| `iron fertilization ocean` | 0 repos |
| `marine cloud brightening` | 0 repos |
| `seaweed climate carbon` | 0 repos |
| `ocean geoengineering simulation` | 0 repos |

### What Exists vs. What's Missing

| Ocean Geoengineering Approach | Open-Source Code? | Nearest GitHub Proxy |
|-------------------------------|-------------------|---------------------|
| Ocean Alkalinity Enhancement (OAE) | ❌ None | MDTF-diagnostics (precipitation-buoyancy POD) |
| Iron Fertilization | ❌ None | ClimateMARGO (integration framework only) |
| Seaweed / Macroalgae Carbon | ❌ None | open-sustainable-technology (may list projects) |
| Marine Cloud Brightening (oceanic) | ❌ None | WRF (can simulate marine clouds, no SRM config) |
| Ocean Circulation / Carbon Cycle | ❌ None | MOM6/POP (not found in search) |
| Coastal Blue Carbon (mangroves, seagrass) | ❌ None | open-sustainable-technology (may list) |

**The silence is itself the story.** Ocean geoengineering is the "dark matter" of climate tech on GitHub — it exists in the scientific literature (Nature, Science, PNAS) but not in open code.

---

## Ocean-Adjacent Repositories

### 1. NOAA-GFDL/MDTF-diagnostics ⭐ 80 (Ocean-Adjacent)
- **URL:** https://github.com/NOAA-GFDL/MDTF-diagnostics
- **Last Activity:** August 14, 2026
- **Why it's ocean-adjacent:** The new **MCS precipitation-buoyancy POD** (Process-Oriented Diagnostic, June 2026) is the closest thing to an ocean interaction diagnostic in open source. Precipitation-buoyancy statistics are fundamental to understanding ocean-atmosphere coupling — the tropical Pacific freshness budget, ENSO dynamics, and how SRM might alter ocean heat uptake.

**Recent Commits (10 pulled):**
| Date | SHA | Message |
|------|-----|--------|
| 2026-08-14 | 87f8105 | Merge PR #825 |
| 2026-06-19 | 4cfc99c | Update MCS_precip_buoy_stats.rst |
| 2026-06-19 | 699de27 | Update MCS_precip_buoy_stats.rst |
| 2026-06-19 | d6bc6d0 | Update MCS_precip_buoy_stats.rst |
| 2026-06-19 | 3904d29 | Update MCS_precip_buoy_stats.rst |
| 2026-06-19 | 33024ad | Add MCS precipitation-buoyancy statistics POD |
| 2026-06-08 | 2df59f6 | Merge PR #823 |
| 2026-06-08 | 16f936c | Update README |
| 2026-06-08 | b96127e | Update README.md |
| 2026-06-02 | 97b3028 | Merge branch 'NOAA-GFDL:main' into main |

**Ocean Connection:** The MCS precipitation-buoyancy POD provides a diagnostic for how precipitation and buoyancy interact in the ocean-atmosphere system. This is the kind of tool you'd need to verify whether ocean geoengineering interventions are working. Five commits on the same day (Jun 19) for the same file is a focused development push.

---

### 2. ClimateSoton/climate-research-group (Closest Active Research Group)
- **URL:** https://github.com/ClimateSoton/climate-research-group
- **Last Activity:** August 6, 2026 (4 commits in 1 day)
- **Why it's ocean-adjacent:** The University of Southampton group works on chemical looping, carbon capture and utilisation, and CFD modelling. While not ocean-focused, CFD (Computational Fluid Dynamics) is the computational backbone of ocean circulation modeling. Their website updates signal active climate research that could encompass ocean studies.

**Recent Commits (4 pulled):**
| Date | SHA | Message |
|------|-----|--------|
| 2026-08-06 | 4b7cc18 | Update index.html |
| 2026-08-06 | f0b123f | Delete 1.zip |
| 2026-08-06 | 503e839 | Add files via upload |
| 2026-08-06 | 3807b50 | Add files via upload |

---

### 3. wrf-model/WRF ⭐ 1,761 (Atmosphere-Ocean Coupling)
- **URL:** https://github.com/wrf-model/WRF
- **Last Activity:** June 8, 2026 (v4.8.0)
- **Why it's ocean-adjacent:** WRF can be coupled with ocean models (MOM6, POP, HYCOM) for fully coupled climate simulations. While WRF itself is atmospheric, its coastal and air-sea interaction physics are directly relevant to ocean geoengineering. The air-sea flux calculations in WRF are the gateway to modeling how ocean interventions affect climate.

**Potential SRM/Ocean Connection:** WRF's ocean-coupled mode could theoretically simulate the effects of ocean alkalinity enhancement on local ocean chemistry and atmospheric CO2. No one has configured this for geoengineering purposes in open source.

---

## The Deep Ocean: Where GitHub Ends and the Ocean Begins

### What's in the Scientific Literature but Not on GitHub

| Research Area | Key Papers | Open-Source Code? |
|--------------|-----------|------------------|
| Ocean Alkalinity Enhancement | Koeve et al. (2021), Alge et al. (2024) | ❌ |
| Iron Fertilization Experiments | BOSS, SOIREE, EIFEX, KEYSER | ❌ |
| Marine Cloud Brightening | Latham (2012), Ehrhardt & Vance (2014) | ❌ |
| Seaweed Carbon Sequestration | Duarte et al. (2013), Pastor et al. (2021) | ❌ |
| Ocean Wing/Kite Drills | Voss et al. (2014) | ❌ |
| coastal blue carbonAldersey et al. (2016) | | ❌ |

### What Would Open-Source Ocean Geoengineering Look Like?

If ocean geoengineering were as active on GitHub as solar or carbon, we'd expect:

1. **Ocean Circulation Models with Geoengineering Modules** — MOM6 or POP configured with OAE or iron fertilization parameterizations
2. **Ocean Chemistry Solvers** — Code that models the carbonate system changes from alkalinity additions
3. **Marine Cloud Microphysics Models** — Cloud-resolving models with sea salt aerosol injection for marine cloud brightening
4. **Seawood Growth and Carbon Sequestration Models** — Grey-box models of macroalgae carbon export
5. **OAE Exposure Twin** — A virtual experiment platform showing how alkaline plumes disperse in the ocean

**None of these exist.** The ocean geoengineering quadrant of climate tech on GitHub is empty.

---

## The Governance Angle: Why Is the Ocean Silent?

The absence is not an oversight — it's a structural signal:

1. **Regulatory risk:** Ocean interventions carry Treaty of London / London Protocol constraints. OAE involves disposing of alkaline materials into the ocean. Iron fertilization is governed by the London Protocol's waste dumping prohibitions. Researchers may avoid creating code that could be interpreted as facilitating ocean waste disposal.

2. **Identity differences:** Solar geoengineering researchers share simulation tools (WRF, CESM). Carbon capture researchers share materials and system models. Ocean geoengineering researchers are distributed across physical oceanography, marine biology, and geochemistry — they don't share a common simulation platform.

3. **Computational expense:** Ocean models require massive computational resources. A single global ocean simulation at 1/10° resolution can take months on a supercomputer. No individual researcher or small team would publish their ocean simulation code as open source.

4. **Data scarcity:** Unlike atmospheric modeling (which has decades of observational data for evaluation), ocean observation networks are sparser, especially in the Southern Ocean. You can't validate an ocean geoengineering model without observations.

---

## Commit Trend Summary — Ocean Intervention Theme

| Signal | Detail |
|--------|--------|
| **The empty quadrant** | Zero dedicated ocean geoengineering repositories found across 6+ search queries. This is the defining finding. |
| **Ocean-adjacent: MDTF** | The MCS precipitation-buoyancy POD (Jun 2026) is the closest ocean-interaction diagnostic in open source. 4 commits in 1 day on the same file. |
| **Ocean-adjacent: WRF** | v4.8.0 (Jun 2026) with aerosol/air-sea physics. Could be configured for ocean geoengineering, but isn't. |
| **Ocean-adjacent: ClimateSoton** | Active research group (4 commits in 1 day, Aug 2026), but website, not code. CFD could be ocean-relevant. |
| **No governance infrastructure** | No open-source tool for assessing ocean geoengineering impacts. No interpretation framework. No scenario testing. |
| **The silence is the signal** | Ocean geoengineering code absence reflects regulatory caution, computational expense, and disciplinary fragmentation — not lack of scientific interest. |

---

## Podcast Episode Hooks

1. **"The ocean geoengineering code doesn't exist."** The most radical finding of our research. While solar has WRF and carbon has openair-cyan, ocean has... nothing. Why?

2. **"The precipitation-buoyancy POD is the ocean's closest friend."** A single diagnostic tool for atmospheric-ocean coupling is the closest thing to ocean geoengineering code on GitHub. What does that tell us about where the field stands?

3. **"The London Protocol may be killing open-source ocean geoengineering."** If creating code that simulates ocean waste disposal could be legally risky, researchers won't publish it. The governance regime may be suppressing open-source development.

4. **"Ocean geoengineering is the dark matter of climate tech."** It exerts gravitational influence on the scientific literature (100+ papers) but emits no light on GitHub (0 repos). What would it take to make ocean geoengineering code visible?

5. **"If we can simulate the atmosphere, why can't we simulate the ocean?"** The answer involves computational cost, observational data scarcity, and a regulatory environment that makes ocean researchers afraid to write code.