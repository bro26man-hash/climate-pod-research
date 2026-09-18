# 📊 Cross-Theme Commit Trend Analysis — September 2026 (v4)
## Master Update: Pulling Fresh Data from 12 Repositories Across All Three Themes

---

## Summary of Fresh Data Pulled

We pulled recent commit histories from **12 repositories** across all three podcast themes in September 2026:

| Theme | Repositories Analyzed | Commits Pulled | freshest commit |
|-------|----------------------|----------------|-----------------|
| ☀️ Solar | WRF, PCMDI, ClimateMARGO, srm-forever, OOCC_2021, Geo-DICE, awesome-geoengineering | 50+ | Sep 17, 2026 (PCMDI) |
| 🌍 Carbon | open-sustainable-technology, openair-cyan, DAC_peroxovanadates, Carbon_Capture_ML, carbon-capture-and-storage | 30+ | Sep 9, 2026 (OST) |
| 🌊 Ocean | MDTF-diagnostics, WRF (coupled), NCAR_ML_EKE | 14+ | Aug 14, 2026 (MDTF) |

---

## The Three Universal finding (updated from v3)

### 1. ☀️ Solar: The Infrastructure Twins

**Key signal:** WRF and PCMDI are both in active development, but for fundamentally different reasons.

- **WRF (1,762★):** Active because it's *needed*. Weather forecasting and climate simulation require constant updates. v4.8.0 released June 2026 with a critical solar radiation correction (e836cd6).
- **PCMDI (133★):** Active because it's *funded*. The Program for Climate Model Diagnosis and Intercomparison is an institutional project with dedicated staff (Jiwoo Lee is maintaining at least 6 of the 10 recent commits).

**The governance implication:** Solar geoengineering evaluation depends entirely on institutional infrastructure that was never designed for SRM. WRF is a weather model. PCMDI evaluates models. Neither has an SRM mandate. Yet they are the *only* tools that can credibly evaluate whether SRM works.

**New finding in v4:** srm-forever's August 26 burst (4 commits, one day) represents the *theoretical* counterweight to WRF's *practical* infrastructure. If WRF provides the "how" and PCMDI provides the "whether," srm-forever asks the "what does it cost."

### 2. 🌍 Carbon: The CC0 Revolution and the Freeze-and-Burst

**Key signal:** Two DAC materials repos adopted CC0 public domain licenses (Sep 12, 2025), while OpenAir-Cyan froze after OSHWA certification (Feb 12, 2024). These are opposite strategies with the same root cause.

- **CC0 Adoption (tjz21/DAC_peroxovanadates + DAC_peroxotitanates):** The researcher gave away all rights. Motivated by anti-patent activism, strategic altruism, or academic convention. The effect: all DAC screening data is now legally unencumbered.
- **Freeze-and-Burst (openair-cyan):** Community developed the device, then froze for 20 months, then returned for a single-day certification burst. The OSHWA UID (US001095) is now official, but nobody's maintaining the hardware designs.

**New finding in v4:** The open-sustainable-technology directory's AI content review policy (Jul 19, 2026) signals that AI agents are now auto-generating climate tech PRs. Governance for the "everything directory" is evolving reactively.

### 3. 🌊 Ocean: The Structural Gap

**Key signal:** Zero dedicated repositories. The gap isn't a bug. It's a feature of the governance landscape.

- **No community** → no code maintainers → no repositories
- **No regulation** → no requirement to share → no incentive to open-source
- **No institutional home** → no funding for code development → no sustained development

**New finding in v4:** The June 19, 2026 precipitation-buoyancy POD (5 commits, same file) is the closest ocean-relevant code in existence. It evaluates model accuracy, not intervention scenarios. The ocean's "closest friend" in open source is a mirror, not a telescope.

---

## Commit Tempo Comparison

| Theme | Avg Commits/Week (recent) | Peak Activity | Dominant Pattern | Institutional vs. Individual |
|-------|--------------------------|---------------|-----------------|------------------------------|
| ☀️ Solar | ~5/week (WRF alone: ~1/week) | 10 commits in 3 days (PCMDI, Sep 3-4) | Institutional, sustained | **Institutional** (NCAR, NOAA, PCMDI) |
| 🌍 Carbon | ~2/week (OST alone: ~1/week) | 6 commits in 1 day (OpenAir-Cyan, Feb 2024) | Catalogue/additive | **Mixed** (institutional directory + individual projects) |
| 🌊 Ocean | ~0.5/week (MDTF burst mode) | 5 commits in 1 day (MDTF, Jun 19, 2026) | Burst + long gaps | **Federal project** (NOAA-GFDL, intermittent) |

---

## The Gas Station Analogy

Imagine three towns building fuel infrastructure for a road trip:

- **Solar town** built a **gas station network** (WRF, PCMDI). It's extensive, well-maintained, and used by everyone. But nobody designed it for SRM-specific fuel. You have to adapt regular gasoline to work in an SRM engine.

- **Carbon town** built a **repair garage** (open-sustainable-technology directory) and a **prototype workshop** (openair-cyan, DAC repos). The garage is well-stocked with parts, but the prototype was certified and then locked. The CC0 researchers decided to give away all their blueprints.

- **Ocean town** hasn't built **anything yet**. There's a map of what the town could look like (academic papers), a few pieces of lumber (Oceananigans.jl), and a mirror (MDTF diagnostics) to check if the road is straight. But no station, no garage, no workshop.

---

## Top 10 Layer Sites (Cross-Theme)

| # | Repository | Stars | Theme | Last Commit | Episode Role |
|---|-----------|-------|-------|-------------|-------------|
| 1 | open-sustainable-technology | 2,552 | 🌍 Carbon | Sep 9, 2026 | The Great Catalogue — start here for any climate tech |
| 2 | WRF | 1,762 | ☀️ Solar | Jun 8, 2026 | The atmospheric model that accidentally owns SRM |
| 3 | Oceananigans.jl | 1,413 | 🌊 Ocean | (not pulled) | The ocean model that doesn't simulate interventions |
| 4 | PCMDI/pcmdi_metrics | 133 | ☀️ Solar | Sep 17, 2026 | The evaluation toolkit that prevents 1.00 roundoff lies |
| 5 | MDTF-diagnostics | 80 | 🌊 Ocean | Aug 14, 2026 | The ocean's closest friend (precip-buoyancy POD) |
| 6 | openair-cyan | 76 | 🌍 Carbon | Feb 12, 2024 | The DIY DAC device that got certified then frozen |
| 7 | ClimateMARGO.jl | 73 | ☀️ Solar | Aug 17, 2026 | The climate-economic model that woke from hibernation |
| 8 | Carbon_Capture_ML | 56 | 🌍 Carbon | May 8, 2024 | The frozen survey of ML-for-CC methods |
| 9 | DAC_peroxovanadates | 2 | 🌍 Carbon | Sep 23, 2025 | The CC0 signal — research as public infrastructure |
| 0 | srm-forever | 0 | ☀️ Solar | Aug 26, 2026 | The zero-star theorist with Weitzman's framework |

---

## Governance Implications (Cross-Theme)

### The Evaluation Gap

Both solar and ocean geoengineering depend on evaluation tools designed for other purposes. WRF evaluates weather. PCMDI evaluates models. NDTF evaluates precipitation-buoyancy relationships. **Nobody evaluates SRM or ocean interventions.**

If solar geoengineering were ever deployed at scale, we'd use PCMDI metrics to assess whether it worked. But PCMDI was never designed to answer "did SRM reduce temperatures by the right amount?" The evaluation infrastructure *precedes* the intervention it's supposed to evaluate.

### The License Problem

Carbon capture repos use three different license strategies:
- **Open-sustainable-technology:** Per-project licenses (various)
- **OpenAir-Cyan:** MIT
- **DAC_peroxovanadates:** CC0 (public domain)

Three licenses. Three philosophies. The CC0 choice is the most disruptive: it means a company can use the DAC screening data in a commercial product without even attributing the researcher. This either maximizes adoption or enables exploitation. Which is it?

### The Ocean Governance Vacuum

Ocean geoengineering has no license standard, no community of practice, and no governance model. This isn't a gap that will fill itself. It's a **structural absence** that reflects the political, legal, and financial reality of ocean intervention research.

---

## 🎙️ Episode Planning — Updated (v4)

| Episode | Theme | Key Questions | Fresh Commit Evidence |
|---------|-------|---------------|----------------------|
| **#1** | ☀️ Solar Geoengineering | Why is SRM code so scarce? Can interactive models democratize the discourse? Arctic risks? CMIP6 evaluation as governance infrastructure? | WRF: 10 commits (v4.8.0, solar radiation fix May 2026); PCMDI: 10 commits in 3 days (v4.2.1, roundoff fix Sep 2026); srm-forever: 4 commits (Weitzman discounting, Aug 2026); ClimateMARGO: 2 README updates after 2yr dormancy |
| **#2** | 🌍 Carbon Capture | Can open source break the $1,000/ton DAC cost barrier? What makes OpenAir-Cyan special? Are peroxides the sorbent of the future? The CC0 revolution? The governance lag at OST? | OST: 10 commits in 10 weeks (2,552★, AI policy update); OpenAir-Cyan: 6-commit burst then freeze (OSHWA certified); DAC_peroxovanadates: CC0 adoption Sep 2025; Carbon_Capture_ML: frozen survey |
| **#3** | 🌊 Ocean Intervention | Why is ocean geoengineering the empty quadrant? What would open-source OAE look like? Is the silence itself a governance signal? MDTF as the ocean-adjacent lifeline? | **Zero repos found**; MDTF: 5 commits on precip-buoyancy POD (Jun 19, 2026); WRF: indirect ocean coupling only; Ocean gap confirmed via 10+ search queries |

---

## 📋 Research Log — Updated

| Date | Activity | Version |
|------|----------|---------|
| 2026-09-03 | Repository created; initial research notes pushed | v0 |
| 2026-09-17 | v1: Initial commit trend analysis from 8 repositories; branches created | v1 |
| 2026-09-17 | v2: Ecosystem-level analysis including ocean models | v2 |
| 2026-09-17 | v3: Fresh commit histories pulled from 12 repositories; detailed profiles pushed | v3 |
| **2026-09-18** | **v4: Fresh commit histories re-pulled and updated; srm-forever Weitzman analysis added; OST AI governance policy documented; MDTF sediment data integration** | **v4** |
| 2026-09-18 | v4: WRF C4ISR mission profile cross-referenced; MDTF MCS precip-buoyancy POD confirmed as ocean-adjacent closest tool | v4 |
| 2026-09-18 | v4: Ocean governance analysis completed; constitutional gap framework documented | v4 |

---

## Quick Links

- 🔗 **Repo:** https://github.com/bro26man-hash/climate-pod-research
- ☀️ Solar branch: https://github.com/bro26man-hash/climate-pod-research/tree/solar-geoengineering
- 🌍 Carbon branch: https://github.com/bro26man-hash/climate-pod-research/tree/carbon-capture
- 🌊 Ocean branch: https://github.com/bro26man-hash/climate-pod-research/tree/ocean-intervention
- 📊 Cross-theme analysis (main): https://github.com/bro26man-hash/climate-pod-research/blob/main/CROSS-THEME-ANALYSIS-SEP2026.md

---

*Last updated: September 2026 (v4) | Data source: GitHub API commit histories from 12 repositories*
*Next update: Q4 2026 (v5) — plan to pull October commit data for seasonal trend analysis*