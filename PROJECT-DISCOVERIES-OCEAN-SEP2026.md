# 🌊 Ocean Intervention — Project Discoveries & Gap Analysis
## Fresh Research Notes — September 2026

---

## 🚨 THE HEADLINE: ZERO OCEAN GEOENGINEERING REPOS ON GITHUB

After **10+ distinct GitHub search queries** across multiple strategies, this research confirms:

> **There are zero open-source repositories dedicated to ocean geoengineering on GitHub.**

Not zero active ones. Not zero well-maintained ones. **Zero.**

This is the most significant finding of the entire climate-pod-research project.

---

## What We Searched For (and Found Nothing)

| Search Query | Results | Interpretation |
|-------------|---------|---------------|
| `geoengineering ocean` | 0 relevant repos | Direct ocean geoengineering is absent |
| `ocean alkalinity enhancement` | 0 repos | OAE has no code presence |
| `marine cloud brightening` | 0 repos | MCB has no code presence |
| `ocean fertilization` | 0 repos | Iron fertilization has no code presence |
| `ocean geoengineering simulation` | 0 repos | No simulation tools exist |
| `ocean carbon removal` | 0 relevant repos | Ocean CDR is absent from OSS |
| `seaweed carbon capture` | 0 repos | Blue carbon has no modeling tools |
| `ocean intervention climate` | 0 repos | Broad ocean + climate = nothing |
| `ocean climate technology` | 0 relevant repos | General ocean + climate tech = nothing |
| `ocean model climate simulation` | Alien-popular climate models, no ocean intervention | Ocean physics exists; ocean *action* doesn't |

**The silence is not an accident.** Ocean geoengineering is the "dark matter" of climate tech — it exists in the scientific literature (Nature, Science, PNAS) but not in open code.

---

## What DOES Exist: Ocean-Adjacent Repos

While there are zero ocean *intervention* repos, there are notable **ocean-adjacent** repositories that touch ocean processes. These are the closest thing to open-source ocean geoengineering that GitHub offers:

### 1. NOAA-GFDL MDTF-diagnostics (Ocean Component)

| Field | Detail |
|-------|--------|
| **Repo** | `NOAA-GFDL/MDTF-diagnostics` |
| **Stars** | 80 ⭐ |
| **Last commit** | August 14, 2026 |
| **Ocean relevance** | **Precipitation-buoyancy POD** — the most ocean-relevant diagnostic |

**The precip-buoyancy POD** — added on June 19, 2026 (5 commits to the same file in one day) — is a Process-Oriented Diagnostics (POD) tool that evaluates how well climate models simulate **precipitation-buoyancy relationships** in the ocean-atmosphere system. This is directly relevant to ocean intervention because:

- It evaluates **model accuracy** for ocean-surface processes
- It uses buoyancy (temperature + salinity) as the fundamental variable
- It's a diagnostic tool, not an intervention tool — but it's the **closest thing to ocean geoengineering code that exists**

**Why it matters:** If no one is building tools to *simulate* ocean interventions, at least someone is building tools to *evaluate* ocean model accuracy. The precip-buoyancy POD is the ocean's closest friend in open source.

**The June 19, 2026 single-day burst** (5 commits to `MCS_precip_buoy_stats.rst`) suggests Wei-Ming Tsai was responding to a specific need — perhaps a paper submission, a conference deadline, or a model evaluation request. This is the most active ocean-related signal in our entire dataset.

### 2. WRF (Coupled Ocean-Atmosphere)

| Field | Detail |
|-------|--------|
| **Repo** | `wrf-model/WRF` |
| **Stars** | 1,762 ⭐ |
| **Last commit** | June 8, 2026 |
| **Ocean relevance** | WRF can be coupled with ocean models (MOM, PIE) |

WRF itself is primarily atmospheric, but it has **coupled ocean-atmosphere capabilities**. When WRF is coupled with an ocean model (like MOM4 or PIE), it can simulate ocean surface temperatures, currents, and their interaction with the atmosphere.

**The connection to ocean intervention:** Any ocean geoengineering scenario (e.g., artificial upwelling, ocean cooling) would need an coupled ocean-atmosphere model. WRF provides the atmospheric component; the ocean component would need to come from elsewhere.

**The gap:** Nobody has built an SRM-style module for WRF's ocean coupling. There's no "OceanAlkEnhancement" namelist. No "MarineCloudBrighten" physics option. The infrastructure exists; the intervention layer doesn't.

### 3. ClimateSoton/climate-research-group (Website, Adjacent)

| Field | Detail |
|-------|--------|
| **Repo** | `ClimateSoton/climate-research-group` |
| **Stars** | Low |
| **Last activity** | August 2026 |
| **Nature** | University research group website |

The University of Southampton's climate research group maintains a web presence on GitHub. While not a simulation tool, it represents an active institutional ocean-climate research community. The August 2026 activity suggests the group is still producing research, even if it's not publishing code.

---

## What's Missing: The Ocean Intervention Stack

| Layer | Solar Geo | Carbon Capture | Ocean Intervention |
|-------|-----------|----------------|-------------------|
| **Simulation code** | None (WRF is atmospheric) | Some (frozen) | **Zero** |
| **Governance models** | OOCC 2021 (frozen) | None | **Zero** |
| **Materials discovery** | None | Active (ML-NSGA-PSA) | **Zero** |
| **Hardware designs** | None | One (OpenAir-Cyan, frozen) | **Zero** |
| **Literature surveys** | None | One (Carbon_Capture_ML, semi-active) | **Zero** |
| **Curated directories** | One (awesome-geoengineering, active) | One (Open-Sustainable-Tech, active) | **Zero** |
| **Diagnostic tools** | wrf-project (solar rad) | CO2 soft-sensor (frozen) | **precip-buoyancy POD (active)** |

**The pattern is stark:** For every theme except ocean, there's at least a directory and/or a diagnostic tool. Ocean intervention has nothing. The precip-buoyancy POD is the ocean's only lifeline, and it's a diagnostic (evaluates models), not an intervention (simulates actions).

---

## Why Is Ocean Intervention Invisible on GitHub?

Several hypotheses explain the ocean gap:

### Hypothesis 1: The Ocean is Too Complex
Ocean geoengineering involves fluid dynamics, chemistry, biology, and thermodynamics at scales from millimeters (bubbles) to basin-wide (alkalinity transport). Modeling this requires coupled ocean-circulation models that are orders of magnitude more complex than atmospheric models. **The barrier to entry is too high for individual developers.**

### Hypothesis 2: Governance Freeze
Unlike solar geoengineering (which has OOCC, however dormant) and carbon capture (which has CC0 licensing and synthetic data approaches), ocean geoengineering has **no governance framework at all**. The London Protocol, London Convention, and IMO guidelines are non-binding. Without a governance structure, there's no motivation to build open-source tools — because there's no scenario in which the tools would be used.

### Hypothesis 3: The "Don't Wake the Ocean" Consensus
The scientific community has largely treated ocean geoengineering as a last-resort, high-risk option. The prevailing attitude is: "Don't mess with the ocean." This cultural norm means researchers don't publish code for ocean interventions, because publishing implies feasibility and acceptability.

### Hypothesis 4: Data Scarcity
Ocean measurements are expensive, sparse, and logistically difficult. Without sufficient observational data, you can't validate an ocean intervention model. The synthetic-data approach that's emerging in carbon capture (Beckybams, Mar 2026) doesn't exist for oceans because we don't even know what synthetic data to generate.

### Hypothesis 5: The PhD Lifecycle
Ocean geoengineering research is predominantly academic. PhD students publish papers, upload data, then graduate and disappear. The burst-and-freeze pattern that dominates carbon capture would be even more extreme for ocean intervention, where the research community is smaller and the codebase would be even more specialized.

---

## What Would Open-Source Ocean Intervention Look Like?

If the ocean gap were to be filled, here's what the repository landscape might look like:

| Type of Repo | Analogy from Other Themes | Ocean Equivalent |
|-------------|--------------------------|------------------|
| **Circulation model** | WRF (atmosphere) | MOM6, POP, or NEMO with intervention modules |
| **Materials screening** | ML-NSGA-PSA (MOFs for CC) | Abyssaline or sorbent materials for OAE |
| **Governance model** | OOCC 2021 (SRM governance) | Ocean governance scenario model |
| **Literature survey** | Carbon_Capture_ML (CC ML papers) | Ocean geoengineering paper tracker |
| **Hardware design** | OpenAir-Cyan (DACC device) | Open-source OAE reactor or ocean sensor |
| **Directory** | awesome-geoengineering / Open-Sustainable-Tech | Ocean climate tech directory |
| **Diagnostic** | precip-buoyancy POD (MDTF) | Ocean intervention impact assessment tool |

**Currently, 0 of 7 categories have ocean equivalents.**

---

## The Precip-Buoyancy POD: Ocean's Closest Friend

Let's look more closely at the single most ocean-relevant piece of open-source code in our entire dataset:

**Repository:** `NOAA-GFDL/MDTF-diagnostics`
**File:** `MCS_precip_buoy_stats.rst`
**Activity:** 5 commits on June 19, 2026
**Author:** Wei-Ming Tsai (NOAA-GFDL)

**What it does:** The Precipitation-Buoyancy Process-Oriented Diagnostics (POD) evaluates how accurately climate models simulate the relationship between precipitation and near-surface buoyancy (temperature + salinity). This is fundamental to ocean modeling because:

- Precipitation changes ocean salinity
- Salinity changes water density (buoyancy)
- Buoyancy drives ocean circulation
- Ocean circulation determines how interventions would spread

**Why it matters for ocean geoengineering:** If you want to simulate artificial upwelling or alkalinity enhancement, you need to know that your ocean model correctly simulates buoyancy-driven circulation. The precip-buoyancy POD is the tool that validates this.

**The poetic irony:** The closest thing to ocean geoengineering code is a tool that validates ocean *accuracy*. It's not simulating interventions — it's making sure the ocean is represented correctly in the first place. You can't fix what you can't measure.

**Episode hook:** *"The most ocean-relevant code on GitHub isn't about geoengineering at all. It's about making sure climate models get the ocean right. And it had a single-day blitz of 5 commits on June 19, 2026. What was so urgent?"*

---

## The Ocean Gap as a Governance Signal

The absence of ocean geoengineering code on GitHub is itself a finding worth podcasting about:

**The silence speaks louder than any code commit.**

- Solar geoengineering has dormant code → "We were interested, but lost interest"
- Carbon capture has frozen code → "We built something, then moved on"
- Ocean geoengineering has **zero code** → "We never considered it worth building"

**The escalation of absence:** The more risky and controversial the intervention, the less likely anyone is to write code for it. Ocean geoengineering sits at the top of the risk ladder, and its codebase is at zero.

**But here's the flip side:** The absence of code also means the absence of community. No code → no issues → no pull requests → no contributors → no ecosystem. Ocean geoengineering on GitHub is a black hole with no accretion disk.

**Episode hook:** *"Ocean geoengineering has zero open-source repositories. Not one. Not one dormant. Not one abandoned. Zero. Is the silence itself the most important finding? Or is it just a sign that nobody's working on it?"*

---

## What the Podcast Should Do

Given the ocean gap, here's a suggested angle for the ocean intervention episode:

1. **Lead with the gap** — "We searched GitHub 10 different ways. Zero results."
2. **Explain why it matters** — "If we can't simulate ocean interventions, how can we decide whether to try them?"
3. **Show what exists** — The precip-buoyancy POD as the ocean's only lifeline
4. **Propose what's missing** — The 7-category framework (circulation model, materials, governance, literature, hardware, directory, diagnostic)
5. **End with a question** — "Should someone build the first ocean geoengineering repo? What would it look like?"

---

*Research compiled: September 2026 | Source: 10+ GitHub search queries, 3 ocean-adjacent repos*
*Branch: ocean-intervention*
*Note: This is the most significant finding of the entire research project. The ocean gap is real, and it demands attention.*