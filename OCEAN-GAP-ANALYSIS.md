# 🌊 The Ocean Gap — A GitHub Research Analysis

**Date:** Sep 2026
**Method:** GitHub repository search across 7 query strategies
**Conclusion:** Ocean geoengineering has zero presence in open-source code

---

## Search Strategy

| # | Query | Expected Results | Actual Results |
|---|-------|------------------|----------------|
| 1 | `geoengineering ocean` | Ocean fertilization, OAE repos | 0 ocean-specific |
| 2 | `ocean alkalinization` | OAE simulation tools | 0 |
| 3 | `iron fertilization` | Fe fertilization models | 0 |
| 4 | `ocean intervention climate` | General ocean geoengineering | 0 |
| 5 | `marine geoengineering` | Ocean-based CDR | 0 |
| 6 | `ocean CDR` | Carbon dioxide removal from ocean | 0 |
| 7 | `ocean climate simulation` | Ocean climate models | General climate only, no geoengineering |

---

## What DOES Exist (Adjacent Tools)

These are the closest open-source tools to ocean geoengineering simulation:

| Repo | Stars | What It Does | Geoengineering Gap |
|------|-------|-------------|-------------------|
| Oceananigans.jl | 1,413 | Ocean fluid dynamics (Julia) | No alkalinity, no tracers for engineered interventions |
| veros | 400 | Ocean simulator (Python/JAX) | No nutrient cycling, no geoengineering modules |
| OceanBioME.jl | 80 | Ocean biogeochemistry (Julia) | Models *natural* carbon cycle, not engineered additions |
| MDTF-diagnostics | 80 | Climate diagnostics (Jupyter) | Precipitation-buoyancy POD, closest to ocean process diagnostics |
| MAOOAM | 22 | Ocean-atmosphere coupling | Dormant 3 years, no geoengineering extensions |
| Climatology.jl | 20 | Ocean state/climatology | Reference data, not simulation |

---

## Four Hypotheses for the Gap

### H1: Governance Hypothesis
The London Protocol prohibits ocean fertilization in international waters. Researchers may avoid public repositories to prevent regulatory attention or political controversy. GitHub is public. Ocean geoengineering research may be happening in private labs, closed datasets, or paper-only workflows.

**Evidence against:** Some related work (e.g., iron fertilization research) is published openly in scientific journals. The confidentiality barrier seems to be specific to *code repositories*, not publications.

### H2: Complexity Hypothesis
Ocean geoengineering requires Earth-system-scale models. A single researcher or small team cannot build an OAE (Ocean Alkalinity Enhancement) simulation from scratch. It needs:
- Ocean circulation models (decades of development)
- Chemical equilibria (counter-ion effects, dissolution kinetics)
- Ecological impact models (phytoplankton responses)
- Economic models (mining, distribution, cost)

**Evidence for:** The existing ocean models (Oceananigans, veros) are developed by large teams over many years. No one has built a geoengineering plugin.

### H3: Interest Hypothesis
The carbon capture community has DIY enthusiasts (OpenAir-Cyan). The ocean geoengineering community has no equivalent. This may be because:
- Ocean intervention requires ship time ($$$) — not laptop experiments
- The ecological risks are higher — fewer people want to be associated
- The policy barrier is higher — London Protocol compliance concerns

**Evidence for:** 0 repos across all 7 search strategies is a strong signal. The carbon capture community has 6+ active repos.

### H4: Risk-Aversion Hypothesis
GitHub repos are permanent and public. An ocean geoengineering repo could be:
- Cited by contrarians
- Used for activist purposes
- Associated with ecological damage if deployed
- Politically toxic for grant applications

**Evidence for:** Research in this field is heavily published in high-impact journals (Nature, Science). Researchers have institutional incentives to be visible in publishing but may avoid visible code repositories.

---

## The "Discovery Gap" as Governance Signal

The absence of ocean geoengineering code on GitHub is not just a technical gap. It is a **governance signal** — the research community may be self-regulating through infrastructure absence.

**Implications for the podcast:**
1. **Transparency:** If ocean geoengineering ever becomes a policy option, the lack of open-source simulation tools means there's no publicly accessible model to evaluate. The science would be trust-based, not code-based.
2. **Reproducibility:** Without open code, ocean geoengineering research cannot be independently verified. This is a reproducibility crisis for geoengineering.
3. **Governance gap:** The missing code layer mirrors the missing governance layer. We have no policy models (OOCC_2021 is solar-only, and it's dormant), and no ocean models. Both gaps are structural.

---

## What Would an Open-Source Ocean OAE Model Look Like?

Based on the adjacent tools analyzed:

```
oae-sim/ (hypothetical)
├── ocean_circulation/    ← Built on Oceananigans.jl or veros
├── alkalinity_tracer/    ← New: DIC + alkalinity advection-diffusion
├── dissolution_kinetics/ ← New: olivine/limestone dissolution rates
├── ecological_impact/    ← New: phytoplankton community response
├── counter_ion/          ← New: Na+, Mg2+ balance for OAE
├── economic_model/       ← New: mining, grinding, shipping cost
└── governance/           ← New: London Protocol compliance checker
```

None of these modules exist in any public repo. Oceananigans has `tracers` but no alkalinity-specific implementation. OceanBioME has `carbonate chemistry` but no *engineered* additions.

---

## Recommendations for the Episode

1. **Frame the silence as a story:** "Why is there no GitHub code for ocean geoengineering when there IS code for solar geoengineering governance (OOCC_2021) and carbon capture (Carbon_Capture_ML)?"
2. **Interview angle:** Ask ocean modelers why they don't build geoengineering modules. Is it technical difficulty, governance concern, or something else?
3. **The "build it before you need it" angle:** Both SRM and ocean intervention lack simulation tools. If either becomes a policy option in the next 5 years, we'd be starting from scratch.
4. **The governance parallel:** The code gap mirrors the governance gap. No simulation tools ↔ no governance frameworks. Both are missing.

---

*This analysis documents the ocean geoengineering gap discovered during GitHub repository research for the Climate Technology & Geoengineering podcast series.*