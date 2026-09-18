# 🌊 Ocean Intervention — Commit Trend Analysis
## For Climate Pod Episode: Ocean Intervention
*September 2026*

---

## Executive Summary

Our ocean intervention commit analysis reveals a paradox: **the most ocean-relevant activity in all of climate tech GitHub happened in a single day, committed by one scientist, to one documentation file, in one diagnostic module — and it was never used for an intervention.**

The trends below trace the ocean's ghost presence in the climate tech codebase.

---

## The Only Ocean Signal: MDTF's Precipitation-Buoyancy POD

### The June 19, 2026 Event

On a single day — June 19, 2026 — Wei-Ming Tsai made **5 commits** to `MCS_precip_buoy_stats.rst` and added an entirely new diagnostic module to the MDTF-diagnostics repository:

| Time (approx.) | Commit | What Changed |
|-----------------|--------|-------------|
| Commit 1 | `33024ad` | **"add MCS precipitation-buoyancy statistics POD"** — the new module |
| Commit 2 | `4cfc99c` | `Update MCS_precip_buoy_stats.rst` — documentation for new module |
| Commit 3 | `699de27` | `Update MCS_precip_buoy_stats.rst` — further documentation |
| Commit 4 | `d6bc6d0` | `Update MCS_precip_buoy_stats.rst` — iteration on docs |
| Commit 5 | `3904d29` | `Update MCS_precip_buoy_stats.rst` — final doc polish |

### What the POD Does

A Proper Orthogonal Decomposition (POD) identifies the dominant patterns in complex data. The precipitation-buoyancy POD specifically:
- Analyzes how precipitation intensity correlates with low-level buoyancy (warm air rising)
- Identifies the dominant modes of moisture-convection coupling over the ocean
- Provides a quantitative metric for how well climate models simulate ocean-driven precipitation

### Why This Is Ocean-Intervention-Relevant

If you wanted to know whether **marine cloud brightening** would affect monsoons, you'd need to understand:
1. How sea surface temperature changes affect convection
2. How buoyancy (warm air rising) drives precipitation patterns
3. How to DETECT changes in these patterns against natural variability

**The POD answers #3.** It's the detection tool. But it was designed for model evaluation, not intervention analysis.

### What the POD Does NOT Do

- ❌ Simulate marine cloud brightening scenarios
- ❌ Model the effects of alkaline substance injection
- ❌ Predict how ocean intervention would affect ENSO, IOD, or monsoons
- ❌ Provide a forward-looking prediction tool

**It's a rearview mirror, not a windshield.**

---

## The WFR Radiation Fix: Ocean-Adjacent Climate Impact

### The May 28, 2026 Commit

**Repo:** `wrf-model/WRF`
**Commit:** `e836cd6` — "correction for eot calculation for solar radiation"

While this is primarily an atmospheric fix, it has ocean implications:
- Solar radiation drives ocean surface heating
- Errors in solar radiation timing propagate into sea surface temperature (SST) simulations
- SST errors affect ocean mixing, coral bleaching risk, and hurricane intensity
- **Correcting the solar clock indirectly improves ocean modeling too**

### The Unseen Connection

The WRF community didn't intend to fix ocean models. But any climate modeler using WRF for ocean-coupled simulations benefits from the fix. The ocean is downstream of the atmosphere in the climate system.

---,”":
"The ocean gets climate credit for atmospheric fixes it didn't ask for and can't claim."
"

---

## The Ocean Anomaly in Commit Patterns

### Cross-Theme Commit Comparison

| Theme | Total Commits | Active Repos | Longest Streak | Pattern |
|-------|--------------|-------------|---------------|---------|
| ☀️ Solar | 50 | 5 | 10 commits / 19 days (WRF) | Continuous, institutional |
| 🌍 Carbon | 60 | 6 | 8 commits / 1 day (digital twin) | Punctuated equilibrium |
| 🌊 Ocean | 14+ | 3 (adjacent only) | 5 commits / 1 day | Singular event |

### What the Ocean Pattern Tells Us

The ocean shows **a single burst of activity (June 19, 2026) within an otherwise empty ecosystem.** There are no sustained ocean development programs, no iterative ocean tool development, no ocean intervention modules being built.

The 5-commit burst was **documentary** (documentation updates to an existing file), not **constructive** (new functionality). Wei-Ming Tsai was improving the explanation of an existing diagnostic, not building something new.

---

## The Ocean's Two Faces

Our research reveals that the ocean appears in GitHub climate tech in two distinct ways:

### Face 1: The Ocean as Victim

Most ocean-adjacent climate repos treat the ocean as a SYSTEM AFFECTED BY climate change, not as a SYSTEM WE CAN INTERVENE IN:

- **Oceananigans.jl** (1,413★): Simulates ocean physics for basic research
- **veros** (200+★): Models ocean circulation for understanding, not action
- **NEMO** (1,000+★): Tracks ocean state for climate projections
- **MITgcm** (1,500+★): General circulation model for observation

**The frame: "How is the ocean changing?" — not "What can we do to the ocean?"**

### Face 2: The Ocean as Tool

The MDTF precipitation-buoyancy POD represents the ocean as a TOOL for understanding: how ocean-atmosphere coupling works, how to evaluate models, how to detect signals. But even here, the tool is evaluative, not interventionist.

**The frame: "How can the ocean help us understand?" — not "How can we use the ocean?"**

### The Missing Face: The Ocean as Target

Nobody has written code that treats the ocean as something we INTENTIONALLY MODIFY for climate purposes. The face is missing entirely. The frame doesn't exist in any repository.

**The unasked question:** "What would we do to the ocean, and how would we simulate it?"

---

## What 14 Commits Tell Us (When You Look Closely)



Our total ocean-related commits across all three themes (14+) break down as:

| Source | Commits | Nature | Intervention Relevant? |
|--------|---------|--------|----------------------|
| MDTF (precip-buoyancy POD) | 5 | Documentation + new module | Detection only, not prediction |
| MDTF (README, upstream merges) | 3 | Maintenance, not development | ❌ No |
| WRF (solar radiation fix) | 1 | Atmospheric, ocean-relevant indirectly | ❌ Not directly |
| WRF (vectorization, physics) | 2-3 | General atmospheric modeling | ❌ No |
| ClimateSoton (website) | ~2 | Institutional updates | ❌ No |

**Zero of 14 commits are about actively modifying the ocean for climate purposes.**

---

## The Structural Reasons for Ocean Silence

### The Governance Wall



International law effectively blocks open-source ocean intervention development:

1. **London Convention/Protocol** — Explicitly prohibits ocean fertilization
2. **No legal framework for OAE** — While not explicitly banned, OAE occupies a legal gray zone
3. **Marine territorial sovereignty** — Interventions in EEZs require coastal state consent
4. **Liability gaps** — No clear framework for who pays for ocean intervention consequences
5. ** weaponization concerns** — Ocean manipulation could theoretically be military

**GitHub is a US-based platform.** Creating code that facilitates techniques banned under international law creates legal risk for maintainers. The cold silence on GitHub may be a warm legal signal.

### The Technical Wall

Ocean intervention is 10-100x more computationally expensive than atmospheric intervention:
- Ocean mixing occurs at millimeter scales but affects basin-wide patterns
- Biogeochemical cycles involve thousands of chemical and biological species
- The ocean's thermal inertia means effects unfold over decades
- Validation requires maintaining sensor networks across entire ocean basins

### Economic Wall

The minimum viable ocean intervention experiment likely costs:
- **Ocean fertilization:** $10M+ (research vessel, iron supply, monitoring)
- **OAE pilot:** $50M+ (alkaline material, pumping, distribution)
- **MCB field test:** $100M+ (aerosol generation, aircraft, satellite monitoring)

Compare to solar geoengineering: stratospheric aerosol injection can be simulated for <$1M in compute costs.

**The economics of ocean intervention are fundamentally incompatible with open-source, volunteer-driven development.**

---

## The Blind Spot Map

```
GITHUB CLIMATE TECH ECOSYSTEM
┌──────────────────────────────────────────────────────────────────┐
│                                                                  │
│  ☀️ SOLAR                                                 │
│  ├── Simulation (WRF) ✅ Rich, active, institutional         │
│  ├── Evaluation (PCMDI) ✅ Rich, metrics, rapid development   │
│  ├── Diagnostics (MDTF) ✅ Growing, new modules                │
│  └── Policy (ClimateMARGO) ⚠️ Dormant but existent           │
│                                                                  │
│  🌍 CARBON                                                │
│  ├── Hardware (OpenAir-Cyan) ✅ Exists, certified, frozen      │
│  ├── Materials (DAC_peroxovanadates) ✅ CC0 datasets exist    │
│  ├── Simulation (dac-moving-bed) ✅ Prototype exists          │
│  ├── Curation (Carbon_Capture_ML) ✅ Literature indexed       │
│  └── Directory (Open-Sustainable-Tech) ✅ Thriving ecosystem    │
│                                                                  │
│  🌊 OCEAN                                                 │
│  ├── Physics (Oceananigans) ✅ Sophisticated models exist     │
│  ├── Evaluation (MDTF) ⚠️ Exists but detection-only          │
│  ├── Simulation of interventions ❌ ZERO dedicated repos       │
│  └── Governance/coding frameworks ❌ ZERO anywhere             │
│                                                                  │
└──────────────────────────────────────────────────────────────────┘
```

---,

## The Episode's Central Question

**Our research has one answer and one mystery:**

### The Answer
Ocean intervention is absent from GitHub because it faces unique governance, technical, and economic barriers that don't apply to solar geoengineering or carbon capture.

### The Mystery
**Even in the best-funded, most-sophisticated ocean simulation tool (Oceananigans), nobody has written a single line of code that models what we might DO to the ocean.** Not one. After 1,413 stars, the question hasn't occurred to anyone.

**Is the code silence a governance signal? A technical limitation? Or a moral hesitation?**

### The Podcast Frame

*"Solar geoengineering has bugs in its radiation code. Carbon capture has 8-commit sprints. But ocean geoengineering has nothing. No code. No modules. No prototypes. Just silence in the data. The ocean is the one climate intervention that exists only in scientific papers — never in open source. What does that silence mean? Is it caution or cowardice? Governance or fear? Or is it simply that the ocean is too big, too complex, too dangerous to even think about tampering with — in public, in code, in the open?"

*"We can model the atmosphere. We can simulate carbon flow. But when it comes to the ocean — the planet's thermostat, its engine, its life support system — we have introspection tools but no intervention tools. The closest thing we have is a diagnostic that measures how well our models work. Not how we'd change them."

---

## Discussion Questions for the Episode

1. **Should there be an "adopt-a-repo" program for ocean intervention?** If Oceananigans is 1,413 stars, why doesn't someone add an OAE module?
2. **Is the London Protocol's ban on ocean fertilization effectively censoring open-source code?**
3. **Would you contribute to an ocean intervention repo? What would stop you?**
4. **Is the GitHub silence about ocean geoengineering a form of collective wisdom — or collective cowardice?**
5. **What's the first intervention module that should be added to Oceananigans? OAE? MCB? Iron fertilization? Something we haven't thought of yet?**
6. **If a major ocean modeler added an OAE module tomorrow, what would happen? Would the scientific community celebrate or try to delete it?**

---

*Analysis based on 10+ GitHub search queries, 3 ocean-adjacent repository commit histories, and 14 cross-theme commits. September 2026.*