# ☀️ Solar Geoengineering — Project Discoveries

## 1. PCMDI/pcmdi_metrics (⭐133)

**Full Name:** PCMDI Metrics Package  
**URL:** https://github.com/PCMDI/pcmdi_metrics  
**Language:** Python  
**License:** MIT  
**Last Activity:** Sep 4, 2026 (v4.2.1 release)  

### What It Does

The PCMDI Metrics Package (PMP) is a comprehensive toolkit for evaluating Earth System Models (ESMs) against observations and historical records. It provides CMIP6-compliant metrics for analyzing model performance across variables like temperature, precipitation, sea ice, and extremes. While not SRM-specific, it is the de facto evaluation infrastructure for any climate model experiment — including those involving solar radiation management.

### Why It Matters for SRM

Any SRM simulation needs to be evaluated against observed climate. PMP provides the standard metrics (RMSE, correlations, extreme-value statistics) that would be used to assess whether an SRM scenario actually produces the intended cooling without unwanted side effects. It is the **governance infrastructure** that the SRM community currently lacks an equivalent of.

### Recent Commits (Sep 3–4, 2026)

- **v4.2.1 release** — 10 commits in 2 days by Jiwoo Lee (LLNL)
- PRs from James Goodnight (roundoff fix in extremes) and Jared Lewis (dask/SVD memory optimization)
- Version bump, CITATION.cff update, bug fixes

### Episode Potential

This is a story about **institutional capacity** — the SRM debate happens at a scale where evaluation infrastructure matters enormously, and PMP represents the kind of coordinated, well-funded effort that informal or community-driven projects cannot match. It also raises the question: should there be an SRM-specific equivalent of PMP?

---

## 2. FMS-ESM/AM3 (⭐4)

**Full Name:** GFDL AM3 Atmospheric Model  
**URL:** https://github.com/FMS-ESM/AM3  
**Language:** Fortran  
**Last Activity:** March 2015  

### What It Does

AM3 (Modular Ocean Model / Earth System Model Component) is the atmospheric component of GFDL's ESM. It has been used in CMIP experiments and can be configured for various scenarios. Being legacy Fortran, it is not accessible to most modern researchers.

### Why It Matters for SRM

AM3 is one of the few actual GCM components available on GitHub that could theoretically be used for SRM experiments. However, its legacy status and Fortran implementation make it practically unusable for most researchers. It represents the **pre-open-source era** of climate simulation.

### Episode Potential

A story about how the **Fortran-to-Python transition** has left geoengineering simulation behind. The tools that exist are either legacy or inaccessible, and the modern open-source climate modeling ecosystem (mostly Python) has not extended to SRM-specific simulations.

---

## 3. pmip4/pmip_p2fvar_analyzer (⭐4)

**Full Name:** PMIP4 Past2Future Variability Analyzer  
**URL:** https://github.com/pmip4/pmip_p2fvar_analyzer  
**Last Activity:** Sep 2025  

### What It Does

Part of the Paleoclimate Modeling Intercomparison Project (PMIP), this tool analyzes climate variability from paleoclimate data and model outputs. It can be used to understand natural climate variability, which is critical context for SRM (since SRM aims to counteract anthropogenic warming against a backdrop of natural variability).

### Episode Potential

The PMIP tools are relevant because they provide the **natural variability baseline** that SRM discussions need. Without understanding natural variability, it's impossible to attribute changes to SRM interventions.

---

## 4. RhondaMueller/Codes-RFG-Arctic-Impacts (⭐1)

**Full Name:** RFG Arctic Impacts — SRM Radiative Forcing Code  
**URL:** https://github.com/RhondaMueller/Codes-RFG-Arctic-Impacts  
**Last Activity:** Apr 2024  

### What It Does

Code associated with research on the radiative forcing impacts of SRM specifically on the Arctic region. This is one of the few repos that directly addresses SRM's regional effects — a critical concern given that the Arctic is disproportionately sensitive to both warming and potential SRM cooling.

### Episode Potential

The **Arctic SRM risk story**: What happens to Arctic ice if we start reflecting sunlight? The research is sparse and the code is dormant, but the implications are enormous.

---

## 5. hausfath/srm-forever (⭐0)

**Full Name:** SRM Forever — Interactive SRM Economics Model  
**URL:** https://github.com/hausfath/srm-forever  
**Last Activity:** Aug 26, 2026  

### What It Does

A single-page, interactive web-based model for exploring SRM economics. Users can adjust parameters and see cost implications. It's designed for education and public engagement, not research.

### Why It Matters

This is the **only interactive, open-source SRM tool** found in the search. It represents the democratization angle — can lightweight models bring SRM discourse to a broader audience? But it's a sola

### Episode Potential

The **Democratization vs. Oversimplification** debate: Is an interactive economics model enough to inform public discourse, or does it risk trivializing a complex geoengineering approach?
