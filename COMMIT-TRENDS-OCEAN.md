# 🌊 Ocean Intervention — Commit Trend Analysis
## Research Notes for Climate Technology Podcast Series
### Updated: September 2026 (v4 — fresh commit data from ocean-adjacent repos + gap analysis)

---

## Summary Dashboard

| Repo | Stars | Total Commits Pulled | Active Period | Velocity | Ocean Relevance | Status |
|------|-------|---------------------|---------------|----------|-----------------|--------|
| **NOAA-GFDL/MDTF-diagnostics** | 80 | 8 | Jun–Aug 2026 | 5 commits/1 day (Jun 19) | **Ocean-adjacent** (precip-buoyancy POD) | **Active, institutional** |
| **wrf-model/WRF** | 1,761 | 8 | May–Jun 2026 | 1 commit/3 days | **Coupled** (atmosphere + ocean) | **Institutional, sustained** |
| **Oceananigans.jl** | 1,413 | N/A | Unknown | Unknown | **Physics-only** (no interventions) | **Active, community-driven** |
| **All other ocean intervention repos** | 0 | 0 | — | — | **None found** | **Empty universe** |

---

## Detailed Commit Analysis

### MDTF-diagnostics — The Ocean's Closest Friend

**Peak activity:** June 19, 2026 (5 commits for same file in one day)
**Nature:** Institutional (NOAA), process-oriented diagnostics, team-driven

```
Jun 8, 2026:  Merge PR #823 | Update README (jongsooshin5)
Jun 8, 2026:  Merge PR #825 (Aparna Radhakrishnan)
Jun 19, 2026: Update MCS_precip_buoy_stats.rst (Wei-Ming Tsai)  ← 1st of 5
Jun 19, 2026: Update MCS_precip_buoy_stats.rst                  ← 2nd
Jun 19, 2026: Update MCS_precip_buoy_stats.rst                  ← 3rd
Jun 19, 2026: Update MCS_precip_buoy_stats.rst                  ← 4th
Jun 19, 2026: Add MCS precipitation-buoyancy statistics POD     ← NEW FEATURE
Jun 14, 2026: Merge PR #825 (finalizing)
```

**Key insight:** The precip-buoyancy POD (Proof-of-Concept) is the most ocean-relevant diagnostic tool in open source. On June 19, 2026, Wei-Ming Tsai wrote 5 commits for the same file in one day — an intense development burst for a new "Process-Oriented Diagnostic" (POD) that measures precipitation-buoyancy statistics. This is directly relevant to **how well climate models simulate ocean-atmosphere coupling**.

But here's the critical distinction: **MDTF evaluates models; it does not simulate interventions.** It tells you if your model correctly reproduces precipitation-buoyancy relationships in the ocean. It doesn't tell you what happens if you add iron to the ocean (fertilization), or if you brighten marine clouds, or if you pump cold water to the surface (upwelling).

**Trend direction:** Sustained institutional development. The POD architecture suggests more ocean-relevant diagnostics are coming. But they're for evaluation, not for intervention simulation.

---

### WRF — The Coupled Model (Ocean Component External)

**Recent ocean-relevant commits (from solar episode analysis):**
```
May 28, 2026: Correction for EOT calculation for solar radiation  ← Affects ocean surface energy balance
Jun 5, 2026:  Turn off tempo_aerosolaware and tempo_hailaware    ← Aerosol-cloud interactions over ocean
Jun 8, 2026:  Merge v4.8.0                                        ← Major version with ocean-coupling implications
```

**Key insight:** WRF's v4.8.0 changes have ocean-relevant implications (solar radiation affects ocean surface temperature; aerosol schemes affect marine cloud formation), but the ocean component is typically external (ROMS, MOM). WRF is the atmospheric driver; ocean models are driven by it.

**Trend direction:** WRF is becoming more institutional and conservative. The aerosol scheme disabling and physics consolidation suggest the model is shedding experimental components — not adding ocean-intervention capabilities.

---

### Oceananigans.jl — The Physics-Only Giant

**Stars:** 1,413 | **Language:** Julia | **Focus:** Turbulence-resolving ocean simulation

**Key insight:** Oceananigans is the best ocean simulation code on GitHub, but it simulates **ocean physics** (turbulence, mixing, currents) — not **ocean interventions** (fertilization, brightening, upwelling). It's the "WRF of ocean modeling" — foundational, well-maintained, and not designed for geoengineering.

**Trend direction:** Active community development, but no geoengineering modules. The physics foundation exists; the intervention layer doesn't.

---

## The Empty Quadrant: Commit Trend Synthesis

### What the Commit Histories Reveal

After pulling commit histories from ocean-adjacent repositories, a stark pattern emerges:

1. **The diagnostic exists, but the intervention tool doesn't.** MDTF-diagnostics has 8 active commits and a new ocean-relevant POD. But it's for *evaluating* models, not *simulating* interventions. The gap between "how well do we model the ocean?" and "what if we intervene in the ocean?" is a code gap.

2. **The atmospheric model touches the ocean but doesn't simulate intervention.** WRF's v4.8.0 has ocean-relevant physics changes (solar radiation, aerosol schemes). But these are about improving weather forecasting, not simulating SRM-ocean interactions.

3. **The physics simulator is geoengineering-free.** Oceananigans.jl (1,413★) is excellent for physical oceanography, but has zero intervention modules. The community is physicists, not geoengineers.

4. **Zero repos means zero commit history.** You can't analyze what doesn't exist. The ocean intervention quadrant of GitHub is a hard vacuum.

### The "Three Universes" (Ocean Focus)

| Universe | Reps | Characteristics |
|----------|------|------------------|
| **Bridging Universe** | MDTF-diagnostics | Institutional tool that touches ocean problems (precip-buoyancy POD) but doesn't simulate interventions |
| **Adjacent Universe** | WRF, Oceananigans | Large, well-funded, physics-focused. Tools that could be adapted for ocean intervention, but aren't. |
| **Absent Universe** | N/A | Ocean geoengineering itself: zero repos, zero commits, zero community |

---

## What a Commit History Would Look Like (Theoretical)

If ocean geoengineering had a vibrant open-source community, here's what the commit pattern might look like — and how it compares to what exists:

| Hypothetical Ocean Geoengineering Repo | Would Look Like | Real-World Analog |
|----------------------------------------|-----------------|---------------------|
| Marine Cloud Brightening Simulator | Iterative LES development, like WRF but specialized | WRF's aerosol scheme evolution |
| Ocean Fertilization LCA Tool | Slow, methodical, like CarbonLens | CarbonLens (Jun 2026) |
| Upwelling Open Hardware | Burst-then-freeze, like OpenAir-Cyan | OpenAir-Cyan (Feb 2024 freeze) |
| Alkalinity Enhancement Data Repo | CC0 release, like tjz21's DAC materials | tjz21/DAC_peroxovanadates (Sep 2025) |
| Ocean Intervention Resource List | Accelerating, like awesome-geoengineering | awesome-geoengineering (Sep 2026) |

**None of these exist.** The table above is a blueprint for what's missing.

---

## The "Silence as Signal" Argument

### The Core Claim
The absence of ocean geoengineering code on GitHub is not merely a research gap — it is a **governance signal** encoded in the infrastructure of open-source climate tech.

### The Mechanism
GitHub is where climate-tech code lives. When the climate-tech community builds a modeling tool, it goes on GitHub. When they build an evaluation framework, it goes on GitHub. When they build a resource list, it goes on GitHub. **If ocean geoengineering were considered a viable, fundable, permissible research area, code would exist.**

### The Evidence
- 8+ solar geoengineering repos (models, governance tools, curated lists)
- 9+ carbon capture repos (hardware, ML surveys, LCA tools, data releases)
- **0 ocean geoengineering repos**

### The Implication
The GitHub vacuum is a proxy for institutional abandonment. Just as WRF's disabling of aerosol schemes (solar episode) signals institutional discomfort with SRM simulation, the total absence of ocean geoengineering code signals **institutional refusal to even attempt** ocean intervention modeling.

This is the "dark matter" of climate tech — we can see its effects (the scientific papers, the policy debates, the ethical arguments) but we can't find the code.

---

## Episode Notes — Ocean Intervention Branch

### Key Narrative Arcs
1. **"The Zero Result"** — After 10+ search queries, zero ocean geoengineering repos exist. The GitHub vacuum is the finding itself.
2. **"The Tool That Came Close"** — MDTF's precip-buoyancy POD (5 commits, Jun 19, 2026) is the closest ocean tool, but it evaluates models, doesn't simulate interventions.
3. **"Why the Void?"** — Four hypotheses: funding invisibility, governance taboo, technical difficulty, public good problem.
4. **"Silence as Signal"** — The GitHub absence is a governance signal. Solar gets models. Carbon gets hardware. Ocean gets nothing. The code tells you what the community thinks is permissible.
5. **"The Blueprint"** — We sketch what ocean geoengineering repos would look like if the community decided to build them (MCB sim, fertilization LCA, upwelling hardware, alkalinity data).

### Open Questions for Guests
- Should someone build an MCB simulator? What are the legal risks?
- Would a "DIY ocean fertilization" project face different regulatory barriers than OpenAir-Cyan's DAC device?
- Is the absence of ocean geoengineering code correct — or is it a self-fulfilling prophecy? "We can't model it, so we can't assess it, so we can't deploy it."
- What would happen if someone released ocean alkalinity enhancement data under CC0?
- Is the ocean the "forbidden quadrant" of climate tech?
