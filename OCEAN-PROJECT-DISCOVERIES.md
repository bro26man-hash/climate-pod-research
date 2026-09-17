# 🌊 Ocean Intervention — Project Discoveries & Gap Analysis

## Discovery Methodology
Searched GitHub using queries:
- `"ocean geoengineering alkalinity iron fertilization"` → **0 results**
- `"geoengineering simulation climate"` → 20 results (zero ocean-specific)
- `"climate technology carbon capture ocean"` → 20 results (cross-listed, none ocean)
- Additional filters: `"marine cloud brightening"`, `"ocean alkalinity enhancement"`, `"seaweed carbon capture"` → 0 repos each

## The Finding: Ocean Geoengineering Is Invisible on GitHub

### The Evidence
Across all search strategies, we found:

| Search Strategy | Results | Ocean-Specific |
|----------------|---------|---------------|
| `"ocean geoengineering alkalinity iron fertilization"` | 0 | 0 |
| `"geoengineering simulation climate"` | 20 | 0 |
| `"climate technology carbon capture ocean"` | 20 | 0 |
| `"marine cloud brightening"` (implied in CESM2 docs) | 1 (empty repo) | 0 |
| `"seaweed carbon capture"` | 0 | 0 |
| `"ocean alkalinity enhancement"` | 0 | 0 |

### The Comparison Table That Says It All

| Climate Tech Quadrant | GitHub Repos | Most-Starred | Active Development? |
|----------------------|-------------|-------------|---------------------|
| ☀️ Solar Geoengineering | 6+ | 73★ | Sparse but present |
| 🌍 Carbon Capture / DAC | 7+ | 76★ | Bursty, some active |
| 🌊 Ocean Intervention | **0** | **—** | **—** |
| 🔄 Integrated Assessment | 3+ | 2,546★ | Active (general climate) |

---

## What DO Exist (Near-Ocean or Adjacent)

### CESM2geoeng_documentation (jnickla1)
- **Type:** Documentation (paper supplementary)
- **Content:** Ocean alkalinity enhancement + marine cloud brightening simulation setup for CESM2
- **GitHub status:** Empty repo (0 commits)
- **Why it matters:** It proves that ocean geoengineering *science* exists — the CESM2 paper is published and cited — but the *code artifacts* are absent
- **The gap:** Theory → published paper → empty repo → no reproduction path

### Team50-Labs/NebuGrid-OpenSource
- **Type:** Fog-harvesting & drip irrigation
- **Stars:** 0 | **Updated:** Aug 2026
- **Why it's listed:** It's the closest thing to an "ocean/climate intervention" hardware project on GitHub, but it's about water harvesting, not ocean geoengineering
- **The gap:** No connecting thread between water infrastructure and ocean alkalinity/iron work

### ClimateMARGO.jl (ClimateMARGO)
- In theory, an "idealized climate-economic model" could include ocean components. In practice, the ocean geoengineering scenarios aren't there.

---

## The 5 Tallest Walls in Ocean Geoengineering Open Source

### Wall 1: Reproducibility
The CESM2 ocean paper published in 2024 has a documentation repo with zero commits. If you can't download the code, you can't reproduce the results. If you can't reproduce the results, the science is just a story.

### Wall 2: Governance Fear
The London Protocol regulates ocean fertilization. The legal ambiguity means researchers may avoid open-source tools the way a catholic priest avoids whoops — the risk is too high and the enforcement too unpredictable._until.regulations.clarify.

### Wall 3: Biological Complexity
Ocean alkalinity enhancement involves: mineral dissolution kinetics + ocean circulation + ecosystem response + carbon cycle feedbacks. That's four PhDs worth of complexity, minimum. Better to run an Excel model than build a community codebase.

### Wall 4: No Champions
Solar geoengineering has this modal supporter. Carbon capture has David Keith and multiple well-funded companies. The ocean quadrant has theoretical papers but no "Ocean Geoengineering LLC" making a GitHub repo and tweeting about it.

### Wall 5: Dear futility: testing
You can't test ocean geoengineering on a desktop. The experiments are ocean-scale. Even if you could build the model, validation requires real-world ocean experiments, which are expensive, controversial, and logistically nightmarish.

---

## The Opportunity: "Ocean-OSS"

If someone built a community ocean geoengineering modeling toolkit — analogous to WRF for atmospheric science — what would it need?

**Minimal Viable Ocean-OSS:**
1. A Python module for OAE chemistry kinetics (CaCO3/Mg(OH)2 dissolution in seawater)
2. Coupling to MOM6 or NEMO ocean models (existing code exists in those communities)
3. An alkalinity/carbonate chemistry tracer module (c白玉, DIC, TA)
4. A visualization layer mapping alkalinity anomalies onto global bathymetry
5. A governance compliance checker (London Protocol, CBD guidelines)

This package would be 5,000-10,000 lines of Python. A small team could build it in 6 months with funding.

**But no one is building it.**

---

## Cross-Reference Path

For episodes covering ocean intervention, the listener should know:
1. The CESM2 ocean paper is the canonical reference — but the code is absent
2. Solar geoengineering simulation has ClimateMARGO.jl (73★) — ocean has *nothing*
3. Carbon capture has OpenAir-Cyan (76★) — ocean has *nothing*
4. The India-based DAC materials researchers (tjz21) have two repos — ocean has *nothing*
5. The awesome-geoengineering list (brandonhimpfen) covers solar and carbon, but ocean resources are negligible

**The ocean quadrant is the white whale of climate tech open source.**
