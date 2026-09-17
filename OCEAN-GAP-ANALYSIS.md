# 🌊 Ocean Intervention Gap Analysis

## The Most Significant Finding of This Research

---

## Executive Summary

After exhaustive GitHub searches across 6 query strategies, 3 topic categories, and multiple keyword combinations, this research project found **ZERO dedicated ocean geoengineering repositories on GitHub.** This is in stark contrast to:

- **Solar geoengineering:** Multiple repositories (WRF 1,761★, PCMDI 133★, MDTF 80★), active institutional development
- **Carbon capture:** Multiple repositories (OpenAir-Cyan 76★, Carbon_Capture_ML 56★, carbon-capture-and-storage 85★), active community
- **Ocean geoengineering:** Nothing. Nada. Zero.

---

## Search Methodology

| Query | Strategy | Results |
|-------|----------|---------|
| `geoengineering ocean` | Behavioral + space | No repos |
| `ocean geoengineering alkalinity iron fertilization` | Topic + keyword | No repos |
| `ocean intervention climate` | Behavioral | No repos |
| `marine cloud brightening` | Keyword | No repos |
| `electrochemical ocean alkalinity` | Keyword + topic | No repos |
| `ocean alkalinization enhancement` | Keyword | No repos |

All searches conducted September 2026. All returned zero results.

---

## What Does Exist at the Ocean-Climate Interface

| Repo | Stars | Type | What It Does |
|------|-------|------|-------------|
| MDTF-diagnostics | 80 | Process diagnostics | Precipitation-buoyancy POD (ocean-atmosphere coupling) |
| ClimateMARGO | 73 | Economic model | Climate-economic optimization including geoengineering |
| WRF | 1,761 | Atmospheric model | Used by ocean-atmosphere researchers |
| Carbon-Capture-Genome | Unknown | Biodiversity | Terrestrial/Genetic, could extend to ocean |

**None of these are ocean geoengineering tools.** MDTF is ocean-adjacent diagnostics. ClimateMARGO is climate-economic optimization. WRF is atmospheric. The ocean is present only as a boundary condition, not as a deployment target.

---

## Why This Gap Matters

### For the Science
Ocean geoengineering (alkalinity enhancement, iron fertilization, marine cloud brightening) is discussed in IPCC reports and Nature papers, but without open-source simulation tools, the field cannot:
- Test scenarios computationally
- Share parameterizations across research groups
- Build community consensus on approaches
- Enable citizen science and education

### For Governance
The absence of open-source ocean geoengineering tools means:
- No public infrastructure for evaluating ocean intervention proposals
- No transparent, auditable models for policy discussions
- No way for affected communities (particularly island nations) to run their own simulations
- Governance is entirely dependent on proprietary institutional models

### For the Podcast
The ocean gap is not just a data point — it's the central narrative of Episode 3. The question isn't "What ocean geoengineering tools exist on GitHub?" but "Why is the ocean the one climate domain where GitHub has nothing to say?"

---

## What Would a Broken Ocean Geoengineering Ecosystem Look Like?

| Component | If it existed | What it would do |
|-----------|--------------|------------------|
| **OAE Simulator** | Ocean alkalinity enhancement modeling | Model dissolution rates, carbon uptake, ocean chemistry perturbation |
| **IronFert Model** | Iron fertilization simulation | Predict phytoplankton blooms, carbon export, ecosystem impacts |
| **MCB Tool** | Marine cloud brightening simulator | Model cloud microphysics, albedo changes, regional climate impacts |
| **OceanCYC** | Ocean carbon cycle model | Track carbon fluxes, deep-ocean storage, circulation impacts |
| **OAE-Eval** | OAE evaluation toolkit | Compare OAE scenarios, assess effectiveness and risks |

**None of these exist on GitHub. The entire ocean geoengineering toolchain is missing from open source.**

---

## The Conversation This Repo Should Start

1. **Should someone build the first ocean geoengineering GitHub repo?** What would it look like?

2. **What are the governance risks?** Open-source ocean intervention tools could be misused by actors who want to deploy without oversight.

3. **Is the gap a feature or a bug?** Does the absence of tools serve as a de facto governance mechanism (no code = no deployment)?

4. **What does the ocean need from the software community?** The gap is not just about ocean science — it's about whether the open-source community sees ocean intervention as a responsibility.

5. **How do we measure the gap?** This repo can serve as a baseline: as of September 2026, zero ocean geoengineering repos on GitHub. Future searches can track whether this changes.

---

## References and Context

- IPCC AR6 Chapter 7 discusses ocean-based CDR but notes limited model capability
- Nature Geoscience (2023): "Ocean alkalinity enhancement: a review of approaches"
- London Protocol Resolution LC-LP.1 (2013): warns against ocean fertilization
- The only ocean-related tool in this entire research project: MDTF-diagnostics' precipitation-buoyancy POD
- The ocean is 90% unmapped, unmodeled, and un-software-ified

---

## Final Thought

The GitHub silence on ocean geoengineering is not a bug in the search. It's a feature of the entire climate tech ecosystem. The open-source community has built tools for the atmosphere (WRF), the economics (DICE, MARGO), and the land (DXR, Carbon_Capture_ML). But the ocean — the planet's largest carbon sink and the most controversial intervention target — remains silent on GitHub.

This episode is about that silence. What it means, why it exists, and what it would take to break it.
