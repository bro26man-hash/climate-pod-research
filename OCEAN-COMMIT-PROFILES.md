# 🌊 Ocean Intervention — Repository Profiles (Updated Sep 2026)

**Branch:** ocean-intervention
**Last Updated:** September 17, 2026
**New commits sourced:** September 2026

---

## The Ocean Quadrant: Still Empty

Our September 2026 commit pull across three major climate repos (WRF, PCMDI, ClimateMARGO) confirms the same finding from our initial search: **there are zero ocean geoengineering repositories on GitHub.** But the adjacent tools tell us what's missing.

---

## Adjacent Tools (Not Ocean-Specific, but Relevant)

### WRF Model — Ocean Coupling Capability
- **Stars:** 1,761 | **Active:** Yes (v4.8.0, June 2026)
- **What it does:** Coupled atmosphere-ocean modeling with WOF (Wave Ocean Foundation)
- **What's missing:** No geoengineering scenario modules. No alkalinity addition. No artificial upwelling parameterization. No iron fertilization response. The ocean is a boundary condition, not an intervention target.
- **What would be needed:** A modular add-on package — something like "WRF-OAE" (Ocean Alkalinity Enhancement) or "WRF-IF" (Iron Fertilization) — that adds intervention scenarios to the existing coupled model

### PCMDI Metrics — Ocean Evaluation Tools
- **Stars:** 133 | **Active:** Yes (v4.2.1, Sep 2026)
- **What it does:** Evaluates CMIP6 models on ENSO, MJO, monsoon, cloud feedback, sea ice, and ocean metrics
- **What's missing:** No verification metrics for ocean interventions. PCMDI can tell you if a model reproduces observed sea surface temperatures. It cannot tell you if an alkalinity injection produced the expected pH change.
- **What would be needed:** An "Intervention Verification" module — analogous to the "Stratospheric Aerosol" metrics that would measure SRM effectiveness. For ocean: pH change metrics, alkalinity transport tracking, marine ecosystem impact indicators.

### ClimateMARGO.jl — Economic Modeling
- **Stars:** 73 | **Active:** Revival (Aug 2026 README updates)
- **What it does:** Idealized climate-economic optimization — trades off mitigation, adaptation, and geoengineering
- **What's missing:** Ocean intervention scenarios in the optimization. Currently configured for solar geoengineering and emissions only.
- **What would be needed:** Ocean alkalinity enhancement and iron fertilization scenarios in the cost-benefit framework.

---

## What an Open-Source Ocean Intervention Stack Would Look Like

If the ocean geoengineering gap were filled, here's the stack we'd expect:

| Layer | Current State | What'sNeeded |
|-------|--------------|--------------|
| **Ocean circulation model** | MOM6, NEMO, WRF-ocean — exist but not intervention-focused | Add alkalinity/iron pumping modules |
| **Ocean chemistry model** | PISCES, MARBL — describe carbonate system | Add OAE and IF scenario modules |
| **Verification metrics** | PCMDI for CMIP6 | Create intervention verification metrics (pH change, alkalinity tracking, ecosystem impact) |
| **Economic modeling** | ClimateMARGO (solar geo only) | Add ocean intervention cost-benefit scenarios |
| **Open data** | Some cruise data, Argo floats | Standardized OAE/IF experiment data format (like LETSI for SRM))
| **Community protocol** | SCI for materials science | Open Ocean Geoengineering Protocols (analogous to SRM Exterior Repository) |

---

## 🎙️ Episode Angle: The Ocean as the Empty Quadrant

**The September 2026 commit pull confirms what our initial search found: the ocean is the one quadrant of climate tech where open source has produced nothing.** Not zero — the adjacent tools exist. But zero ocean-specific intervention models, metrics, or data platforms.

**The podcast narrative arc:**

1. **The finding:** WRF models the atmosphere over the ocean. PCMDI evaluates how well it does. ClimateMARGO costs out the trade-offs. But nowhere in this stack can you ask: "What happens if we change the ocean?"

2. **The hypothesis:** The absence isn't about technical difficulty — ocean alkalinity enhancement is just dissolution chemistry. It's about governance. The London Protocol restricts ocean fertilization research. The absence on GitHub mirrors the absence in the regulatory framework.

3. **The opportunity:** Unlike atmospheric SRM (which requires complex radiative transfer codes) or DAC (which requires high-temperature sorbent processes), ocean intervention is chemistry done in the wild. A modular, open-source OAE model wouldn't need a supercomputer — it needs carbonate chemistry equations, ocean circulation data, and a community willing to build it.

4. **The question for the next episode:** If we built the first open-source ocean intervention model, what would it look like? And who would build it?

**Potential interview subjects:**
- Scientists working on ocean alkalinity enhancement experiments (e.g., at GEOMAR, WHOI, Scripps)
- Legal scholars studying the London Protocol and ocean governance
- The Earth System Modelers who'd open-source an OAE module if someone gave them a clean interface
- The citizen science community that already builds ocean sensors (think OpenArduino for pH)
