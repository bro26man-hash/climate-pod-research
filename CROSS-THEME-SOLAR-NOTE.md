# ☀️ Solar Geoengineering — Cross-Theme Research Note

**Branch:** solar-geoengineering
**Last Updated:** September 2026 (v3)
**Purpose:** Consolidated research note for the solar geoengineering episode, integrating findings from all three themes

---

## The Solar Geoening Episode: Core Narrative

The sun gets the tools. The atmosphere gets WRF (1,761★), PCMDI (133★), and MDTF (80★). The solar radiation physics gets constant attention — WRF just fixed a bug in its EOT calculation for solar radiation (May 28, 2026). The aerosol microphysics gets experimental options (TEMPO) that are being refined through staged release cycles.

But nobody has built an end-to-end solar geoengineering simulator. The components exist. The evaluation tools exist. The process diagnostics exist. They just aren't connected.

## Three Cross-Cutting Themes

### 1. The Integration Gap
WRF can model the atmosphere. PCMDI can evaluate the model. MDTF can diagnose the processes. But nobody has built a tool that answers "what happens if we inject sulfates into the stratosphere?" from start to finish. The components are world-class; the integration is zero.

### 2. The Paper-to-Tool Problem
actm-sai-csu is the exemplar: AI to detect SRM effects, 10 commits in 3 months, then 3.5 years silent. ClimateMARGO: 2.75 years without code commits, then README updates. The academic incentive structure rewards paper publication, not code maintenance. GitHub repos in climate tech are paper delivery vehicles, not software projects.

### 3. The Governance Vacuum
srm-forever (0★) is the only interactive SRM governance tool. It's a teaching tool, not a policy instrument. Geo-DICE and OOCC are tiny repos with simple governance models. The governance gap is as wide as the technical integration gap.

## What the Carbon Theme Has in Common
Both solar and carbon capture suffer from the paper-to-tool gap. Carbon_Capture_ML (56★) curates papers; it doesn't simulate anything. OpenAir-Cyan (76★) built hardware, then went dormant. The pattern is identical: excite the community, publish the paper, move on to the next grant.

## What the Ocean Theme Reveals by Contrast
The ocean quadrant has ZERO repos. Not zero maintained repos — zero repos. The ocean is the silence that makes the solar and carbon signals louder. When 6 carbon repos update in 5 days and WRF has 10 commits in 18 days, the ocean gets nothing.

## Episode Structure Suggestion

1. **The Tools We Have** (5 min): WRF v4.8.0, PCMDI v4.2.1, MDTF precipitation-buoyancy POD — world-class atmospheric modeling
2. **The Gap That Remains** (10 min): No end-to-end SRM simulator; srm-forever is a toy; actm-sai-csu died; ClimateMARGO might be waking up
3. **The Structural Problem** (10 min): Paper-to-tool pattern across all themes; academic incentives don't reward code maintenance; governance tools are nonexistent
4. **The What-If** (5 min): What would an integrated SRM simulation pipeline look like? Who would fund it? Who would maintain it?

## Key Quotes for the Episode

- "WRF just fixed a bug in how it calculates solar radiation. That's the foundation of every SRM simulation. But nobody's building on top of it."
- "ClimateMARGO was dormant for 2.75 years. Then someone updated the README. No code. Just the README. That's the story of open-source climate tech."
- "actm-sai-csu had a promising AI approach for detecting SRM effects. 10 commits, then silence for 3.5 years. The paper was published. The tool died."
- "srm-forever is the closest thing to a democratized SRM simulator. It has 0 stars. The author appears to be a student."
