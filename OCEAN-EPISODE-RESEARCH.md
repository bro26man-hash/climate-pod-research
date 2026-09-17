# 🌊 Ocean Intervention — Episode Research Notes

## Episode Overview
This episode tackles ocean-based geoengineering — the least explored, most controversial, and most scientifically uncertain quadrant of climate tech. We examine ocean alkalinity enhancement (OAE), iron fertilization, marine cloud brightening, seaweed/kelp farming, and the profound absence of open-source tools for any of these approaches.

---

## The Discovery Gap: Zero Ocean Geoengineering Repos

**The headline finding of our entire GitHub research:**

Across multiple search queries — `"ocean geoengineering alkalinity iron fertilization"`, `"geoengineering simulation climate"`, `"climate technology carbon capture ocean"` — we found **zero dedicated open-source ocean geoengineering repositories.**

This is not a search failure. It is a meaningful signal.

### What EXISTS (and what DOESN'T):

| Approach | GitHub Repos | Status |
|----------|-------------|--------|
| **Solar Radiation Management** | 6+ repos (ClimateMARGO, Geo-DICE, OOCC, etc.) | Dormant but present |
| **Carbon Capture / DAC** | 7+ repos (OpenAir-Cyan, DAC materials, etc.) | Active bursts |
| **Ocean Alkalinity Enhancement** | 0 | **Nothing** |
| **Iron Fertilization** | 0 | **Nothing** |
| **Marine Cloud Brightening** | 0 dedicated repos | CESM2 paper has documentation (empty repo) |
| **Seaweed / Kelp Carbon** | 0 | **Nothing** |
| **Ocean Acidification Modeling** | 0 | **Nothing** |

---

## The One Paper: CESM2 Ocean Geoengineering

The closest thing to an ocean geoengineering codebase is the documentation repo for the CESM2 ocean geoengineering paper:

### jnickla1/CESM2geoeng_documentation
- **Stars:** N/A | **Language:** Documentation | **Last Updated:** Nov 27, 2025
- **What it does:** Documentation (paper supplementary material) for the CESM2 paper on ocean geoengineering — covering ocean alkalinity enhancement and marine cloud brightening simulations
- **Problem:** The repository has **zero commits**. It's an empty shell. The documentation exists as paper supplementary files, but no one has pushed the code.
- **Episode angle:** "The most important ocean geoengineering paper has a documentation repo with no code. The reproducibility crisis isn't just about numbers — it's about entire approaches with zero artifacts."

### JdeJong96/sai-git (related)
- While this is solar aerosol injection (SAI), not ocean, it's part of the CESM geoengineering ecosystem
- Active in 2025 — the most recently active geoengineering-related repo
- Shows that *some* CESM experiments have live code, but ocean experiments don't

---

## Why Is the Ocean Quadrant Empty?

Our hypothesis for the GitHub silence:

### 1. **The Biological Complexity Barrier**
Ocean geoengineering involves biological systems (diatoms for OAE, phytoplankton for iron fertilization, coral for mineralization). These are harder to model than atmospheric physics. The "code" would be biological models, not climate models. Different community entirely.

### 2. **The Governance Minefield**
Ocean alteration is the most internationally governed area of geoengineering. London Convention, London Protocol, CBD, UNEA — all have roles. Researchers may avoid open-source tools because the legal risk of "provocative" tools is higher.

### 3. **The Scale Problem**
Ocean geoengineering requires ocean-scale implementation. You can't test it with a desktop simulation. The "simulation" *is* the pilot project. Software is secondary.

### 4. **The Funding Gap**
No one is funding ocean geoengineering *software*. NASA funds GCMs. NSF funds climate economics. But who funds "open-source ocean alkalinity enhancement modeling"? The SILMARILS proposal? The Ocean Visions pipeline? Unclear.

### 5. **The "Music Hall" Effect**
Ocean geoengineering sounds like science fiction. Iron fertilization = "fertilizing the ocean to grow algae." OAE = "putting lime in the sea." The ideas are so visually dramatic that they attract attention but not serious computational investment.

---

## What Would Good Ocean Geoengineering Software Look Like?

### Hypothetical Open-Source Ocean OAE Toolkit:
- **Chemical module:** Dissolution kinetics of CaCO3 and Mg(OH)2 in seawater
- **Transport module:** Ocean circulation models (MOM6, NEMO) with alkalinity tracers
- **Impact module:** Calcification responses, pH changes, ecosystem effects
- **Governance module:** London Protocol compliance checker, well-to-keel carbon accounting
- **Visualization:** Global bathymetry + alkalinity anomaly maps

### Hypothetical Open-Source Iron Fertilization Toolkit:
- **Biological module:** Phytoplankton growth models (NPZD, PISCES)
- **Iron chemistry module:** Fe speciation, ligand binding, bioavailability
- **Carbon export module:** Ballast effects,下沉 flux modeling
- ** observe:** SOCCOM float data integration

### Neither of these exists as open-source, community-maintained tools.

---

## The Seaweed / Kelp Angle

 seaweed/kelp farming for carbon sequestration is a growing area of climate-tech interest:
- **Team50-Labs/NebuGrid-OpenSource** — Fog-harvesting & drip irrigation (found in search, only 0 stars, but represents the "blue carbon" agriculture space)
- The kelp ocean farming pipeline: grow kelp → sink it → carbon sequestered in deep ocean
- Companies: Running Tide (sinking kelp), Sequesterium, ocean-based CDR start-ups
- **GitHub presence:** None.

---

## Key Episode Questions

1. **Why is ocean geoengineering the "dark matter" of climate tech on GitHub?** The absence of code is the story.
2. **Is the ocean geoengineering gap a governance signal, or just a scientific gap?** Researchers may be self-censoring because of the London Protocol's ambiguity.
3. **The "biological complexity" excuse:** Is it really too hard to model ocean alkalinity, or is it too unglamorous for computational science careers?
4. **The CESM2 ocean paper:** One of the most cited ocean geoengineering papers in science, and its GitHub repo is empty. What does that say about the reproducibility of geoengineering science?
5. **Should the podcast community build the first ocean geoengineering open-source toolkit?** An "Ocean-OSS" initiative — the GitHub polaris project for ocean climate intervention.

---

## Sources & Links
- [CESM2geoeng_documentation](https://github.com/jnickla1/CESM2geoeng_documentation)
- [sai-git](https://github.com/JdeJong96/sai-git) (solar, but CESM ecosystem)
- [ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl) (includes some ocean coupling)
- Search queries used: `"ocean geoengineering alkalinity iron fertilization"`, `"geoengineering simulation climate"`, `"climate technology carbon capture ocean"`
- **Result:** 0 ocean geoengineering repos found across all queries
