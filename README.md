# ☀️ Solar Geoengineering — Episode Research Notes

**Podcast Theme:** Solar Radiation Management (SRM) — Reflecting sunlight to cool the planet
**Branch:** `solar-geoengineering`
**Last Updated:** September 2026

---

## 🎙️ Episode Angle

The central tension for the solar geoengineering episode: **the most important climate intervention knows almost nothing about itself in open source.** The codebase for SRM simulation is sparse, siloed in closed academic labs (GFDL, NCAR, ETH Zürich), and dominated by legacy Fortran models from the 2000s. The gap between simulation ambition and open-source availability is the story.

---

## 🔍 Project Discoveries

### Tier 1 — Active & Most Important

| Repo | Stars | Forks | Language | Last Commit | Description |
|------|-------|-------|----------|-------------|-------------|
| **[PCMDI/pcmdi_metrics](https://github.com/PCMDI/pcmdi_metrics)** | 133 | 49 | Python | Sep 4, 2026 | The gold-standard open-source toolkit for evaluating Earth System Models. Uses CMIP6 data to compare model performance on ENSO, MJO, monsoon, cloud feedback, and more. Maintained by DOE/LLNL's PCMDI program. |
| **[hausfath/srm-forever](https://github.com/hausfath/srm-forever)** | 0 | 0 | HTML | Aug 26, 2026 | Interactive single-page model comparing SRM (stratospheric aerosol injection) vs. rapid mitigation + carbon removal to hold 1.5°C. Uses Weitzman certainty-equivalent discounting. Transparent, published in a single `index.html`. |
| **[prashaant1926/open-earth-digital-twin-simulation](https://github.com/prashaant1926/open-earth-digital-twin-simulation)** | 0 | 0 | TeX | Oct 10, 2025 |Distributed simulation platform modeling Earth's major environmental systems using real-time public data and agent-based modeling. Built via Co-Sci collaborative research. |

### Tier 2 — Legacy & Regional

| Repo | Stars | Forks | Language | Last Commit | Description |
|------|-------|-------|----------|-------------|-------------|
| **[FMS-ESM/AM3](https://github.com/FMS-ESM/AM3)** | 4 | — | Fortran | Mar 2015 | GFDL's AM3 atmospheric model — a legacy but historically significant climate simulation codebase. |
| **[pmip4/pmip_p2fvar_analyzer](https://github.com/pmip4/pmip_p2fvar_analyzer)** | 4 | — | — | Sep 2025 | CMIP6 climate data analysis tool for PMIP (Paleoclimate Model Intercomparison Project). |
| **[RhondaMueller/Codes-RFG-Arctic-Impacts](https://github.com/RhondaMueller/Codes-RFG-Arctic-Impacts)** | 1 | — | — | Apr 2024 | Simulates radiative forcing from geoengineering on Arctic climate impacts. |

---

## 📊 Commit Trend Analysis

### What the commit histories reveal:

**1. Peak activity is concentrated in a single institutional lab.** The PCMDI Metrics Package (133★) had a burst of 10 commits on Sep 3-4, 2026 — all tagged to Jiwoo Lee at LLNL, with PRs from multiple contributors (James Goodnight, Jared Lewis). This is institutional, funding-backed development, not community-driven open source. Each release (v4.2.1) carries months of coordinated work.

**2. SRM-specific open source is nearly empty.** The entire `srm-forever` repository has only 4 commits — all on a single day (Aug 26, 2026) by a single author (hausfath). This is a brilliant *intellectual exercise* (transparent assumptions, published discount-rate essay) but not a simulation tool. There is no open-source equivalent of the GFDL SAI model or NCAR's geoengineering module.

**3. Legacy Fortran dominates what exists.** The AM3 model (2015) and PMIP analyzers are Fortran-based, reflecting the era when climate simulation was dominated by institutional Fortran codes. The modern shift toward Python (PCMDI, xCDAT) hasn't yet reached the geoengineering-specific simulation space.

**4. The "digital twin" concept is nascent.** The Open Earth Digital Twin (TeX/LaTeX-based, 1 commit) is more of a research manifesto than a functioning codebase — but it represents where the field *wants* to go: agent-based, real-time data, collaborative.

### Trending Themes:
- ✅ **CMIP6 evaluation tooling** is the most active climate simulation code on GitHub (PCMDI, 133★)
- ✅ **Interactive financial/economic SRM models** are emerging asstandalone teaching tools (hausfath/srm-forever)
- ⚠️ **Physical SRM simulation** (aerosol microphysics, radiative transfer codes) has no significant open-source presence
- ⚠️ **Regional geoengineering impacts** (Arctic, monsoon) are under-represented
- 🔮 **Agent-based Earth system modeling** is a growing aspiration (Co-Sci, Open Earth Digital Twin)

---

## 🎙️ Key Episode Questions

1. **Why is there no "GitHub for SRM"?** The computational barriers, governance concerns, and institutional gatekeeping that keep geoengineering code off GitHub.
2. **Can interactive models like srm-forever democratize SRM discourse?** A single HTML file makes the economics transparent — but can it substitute for physical simulation?
3. **What role do CMIP6 evaluation tools play in SRM governance?** If we're going to deploy SRM, we need to evaluate its effects against a baseline — PCMDI-style tools are the infrastructure for that.
4. **The Arctic question:** How would SRM affect Arctic ice, and who decides? (Codes-RFG-Arctic-Impacts is the only codebase touching this.)

---

## 🔗 Related Resources
- **PCMDI Metrics Package docs:** http://pcmdi.github.io/pcmdi_metrics/
- **SRM Forever live tool:** https://hausfath.github.io/srm-forever/
- **Co-Sci Open Earth Digital Twin:** https://co-sci.org
