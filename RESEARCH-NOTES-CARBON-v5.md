# 🌍 Carbon Capture — Research Notes
**Podcast Episode: Carbon Capture & Direct Air Capture | Last updated: September 2026**

---

## 📋 Episode Anchor Question
**Can open source + CC0 licensing break the $1,000/ton DAC cost barrier?**

---

## 🔬 Project Discoveries

### 1. dac-moving-bed-digital-twin — `IsaH93/dac-moving-bed-digital-twin`
- **Stars:** Low (niche) | **Language:** Python | **Updated:** 2026-07-03
- **Description:** Moving-bed TVSA (Temperature-Vacuum Swing Adsorption) digital twin for Direct Air Capture. Couples continuous sorbent physics (Toth isotherm, LDF kinetics) with a SimPy discrete-event simulation platform.
- **Why it matters for the episode:** This is the most technically sophisticated DAC code we found — a *digital twin* that models real sorbent physics. 8 commits all landed on a single day (2026-07-03), suggesting a research paper submission push. The code bridges the gap between lab-scale chemistry and systems-level optimization.
- **Link:** https://github.com/IsaH93/dac-moving-bed-digital-twin

### 2. OpenCarbon — `terranexum/OpenCarbon`
- **Stars:** 2 | **Language:** (unspecified) | **Updated:** 2026-08-19
- **Description:** Carbon management technologies and plans to advance research and innovation in direct air capture, ensuring it uses clean energy and achieves low cost.
- **Why it matters:** This is explicitly a *planning* and *roadmapping* project, not a simulation. It reflects the community's desire for coordinated DAC research. Dormant since mid-2023 — the initial burst of interest may have fizzled.
- **Link:** https://github.com/terranexum/OpenCarbon

### 3. Direct-Air-Capture — `Rudra57/Direct-Air-Capture`
- **Stars:** Low (niche) | **Language:** Jupyter Notebook | **Updated:** 2026-06-11
- **Description:** Explores DAC technology as a climate solution for removing CO₂ directly from the atmosphere. Uses data-driven modeling approaches.
- **Why it matters:** All 4 commits landed on a single day (2026-06-11). This is a classic "exploratory notebook" project — created for a specific analysis, not designed for ongoing community use.
- **Link:** https://github.com/Rudra57/Direct-Air-Capture

### 4. ClimateMARGO.jl (cross-listed)
- **Stars:** 73 | **Language:** Julia
- **Why it appears here too:** ClimateMARGO's economic optimization framework explicitly models carbon capture as one of the mitigation/adaptation/geoengineering trade-off levers. It's the economic modeling side of the carbon capture conversation.

### 5. wrf-model/WRF (cross-listed)
- **Stars:** 1,763 | **Language:** Fortran
- **Why it appears here too:** WRF includes atmospheric transport modeling that's essential for understanding CO₂ dispersion from point-source DAC sites. The 2026 solar radiation fix commits are also relevant to atmospheric modeling generally.

---

## 📊 Commit Trend Analysis

### Commit Velocity by Repo

| Repo | 12-mo Commits | Pattern | Last Commit |
|------|---------------|---------|-------------|
| dac-moving-bed-digital-twin | 8 | Single-day burst (paper push) | 2026-07-03 |
| Direct-Air-Capture | 4 | Single-day burst | 2026-06-11 |
| OpenCarbon | 0 | Dormant since 2023 | 2023-07-18 |
| ClimateMARGO.jl | 2 | Burst-then-dormant | 2026-08-17 |
| WRF | 10+ | Institutional, continuous | 2026-06-08 |

### Key Observations

1. **The "paper push" pattern is overwhelming.** 6 of the 8 commits in the most active DAC repo landed on a single day. This is the dominant development pattern in carbon capture open source: someone does the research, writes the paper, pushes the code to GitHub as supplementary material, then walks away.

2. **No continuous DAC codebase exists.** Unlike climate modeling (WRF) or solar geoengineering (ClimateMARGO), there is no actively maintained, community-governed open-source DAC simulation platform. The field is entirely paper-driven.

3. **OpenCarbon's dormancy is telling.** A project explicitly about coordinating DAC research, with a clean mission and a .org-style name, lasted about a year of activity then died. The coordination problem is real.

4. **The CC0 / open-source question is unresolved.** None of the repos we found explicitly use CC0 or permissive licenses as a cost-reduction strategy. The DAC cost barrier isn't just an engineering problem — it's a *licensing and collaboration infrastructure* problem.

5. **WRF is the hidden backbone.** The most active carbon-relevant code is happening inside WRF — atmospheric transport, radiation physics, aerosol chemistry. If you want to understand where DAC research is *actually* happening in code, you have to look inside the general climate modeling repos, not the DAC-specific ones.

---

## 🎙️ Episode Talking Points

- **The $1,000/ton problem:** Current DAC costs are $100-$600/ton for the best systems. Open source could reduce the *engineering* cost through collaboration, but the chemical cost of sorbents and the energy cost of regeneration remain physical constraints no license can fix.
- **The paper-push pattern:** Every DAC repo we found follows the same pattern: burst of commits for a paper, then silence. Is this a governance failure, or is it the right incentive structure for early-stage research?
- **The missing middle:** There are lots of small DAC *experiments* (notebooks, single analyses) and one big climate model (WRF) that contains DAC-relevant physics, but there's nothing in between — no shared simulation platform, no community benchmarks, no open datasets.
- **CC0 as a strategy:** Could releasing DAC designs under CC0 (public domain) accelerate the field the way open-source software did for AI? The evidence from GitHub so far is: not yet, because the field is too small.

---

## 🔗 Cross-References
- See `main/CROSS-THEME-ANALYSIS-v4.md` for the unified dashboard across all three themes.
- See `solar-geoengineering/RESEARCH-NOTES-SOLAR-v5.md` for the solar comparison.
- See `ocean-intervention/RESEARCH-NOTES-OCEAN-v5.md` for the ocean intervention gap analysis.

*Methodology: GitHub Repository & List Commits APIs, September 2026. Search queries: "carbon capture climate tech", "direct air capture DAC climate", "carbon capture simulation", "CC0 climate".*