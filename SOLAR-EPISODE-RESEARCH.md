# 🎙️ Solar Geoengineering Episode — Research Dossier (v4)

## Episode Title (Working)
"The Solar Fix: Modeling Geoengineering's Climate Math"

## Core Thesis
The most sophisticated climate models on Earth (WRF) are actively refining their solar radiation physics — but the open-source code that would let anyone *simulate* geoengineering scenarios is thin, dormant, and controlled by a tiny number of academic groups. We have the weather model; we don't have the geoengineering module.

## Commit Evidence (September 2026 Fresh Pull)

| Signal | Repo | evidence |
|--------|------|----------|
| Solar radiation EOT correction | WRF (May 28) | Code change to how sunlight energy balance is computed |
| TEMPO aerosol awareness disabled | WRF (Jun 5) | Simplification of aerosol-cloud interaction for stability |
| v4.8.0 release | WRF (Jun 8) | Major version with SRM-relevant physics updates |
| README-only revival | ClimateMARGO (Aug 17) | 2.5yr code drought — project on life support |
| v2.0.0 directory release | awesome-geoengineering (May) | The field's catalog gets its first major update |
| Final commit | Geo-DICE (Sep 2018) | 7 years of silence — academic code half-life |
| Governance model frozen | OOCC_2021 (Nov 2021) | 15 commits then stop — the "who decides" question has no living code |
| Ecological impact code | geomalaria (Feb 2022) | Malaria-SRM coupling — complete but frozen |

## Key Narratives

### Narrative 1: "The Fix That Changes Everything"
WRF v4.8.0's solar radiation correction (May 28, 2026) is the kind of commit that sounds boring but changes everything. When you fix how sunlight is computed in the most used climate model, you change every SRM simulation that's ever been run. The TEMPO aerosol toggle (Jun 5) suggests the model is simplifying aerosol physics — which could mean SRM studies using WRF need to account for this change.

**Sound bite:** *"The sun's math just got fixed, and it changes how we simulate blocking it."*

### Narrative 2: "The Governance Black Hole"
There is exactly one open-source model of SRM governance — OOCC_2021 by Jann Leppänen. 15 commits in 4 months of intense work, then 5 years of silence. The question "who decides whether to deploy SRM?" has no living code answer. The governance layer of geoengineering is a ghost town.

**Sound bite:** *"We have models for how to cool the planet. We have no models for who gets to decide."*

### Narrative 3: "The Zombie Economy"
ClimateMARGO went dormant for 2.5 years, then got two README updates in August 2026. No code. No tests. Just a README. This is the academic pattern: publish a model, lose funding, and maintain only the documentation that proves you once existed.

**Sound bite:** *"The climate model woke up to update its LinkedIn profile, then went back to sleep."*

### Narrative 4: "One Person's Life's Work"
Brandon Himpfen's awesome-geoengineering is the only consistently maintained catalog of open-source geoengineering tools. 14 months, 7 commits, one person. If he stops maintaining it, the field's map goes stale. The entire SRM software ecosystem is one curator away from obsolescence.

**Sound bite:** *"The wiki of geoengineering is one person's weekend project."*

## Interview Questions (If We Got Access)
1. WRF developers: "How does the solar radiation EOT correction change SRM simulation results? Have you seen downstream impacts?"
2. ClimateMARGO maintainer: "What would it take to restart code development? Is the Julia ecosystem ready?"
3. OOCC_2021 author: "Why did you stop? Is there a maintained successor? What happened to the governance model?"
4. awesome-geoengineering curator: "What's the most surprising omission from the list? What's the most dangerous inclusion?"
5. geomalaria author: "What did the malaria-SRM coupling reveal? Would you do anything differently knowing what you know now?"

## Further Reading (From Commit Histories)
- WRF v4.8.0 release notes (github.com/wrf-model/WRF/releases)
- ClimateMARGO.jl documentation (github.com/ClimateMARGO/ClimateMARGO.jl)
- OOCC_2021 paper: "One Climate Committee" governance framework
- awesome-geoengineering v2.0.0 index
- geomalaria tutorial: malaria risk in SRM worlds

## Episode Length Estimate
25-35 minutes (deep-dive technical episode)

## Production Notes
- **Cietal footage:** WRF output visualizations, climate-economics optimization plots
- **Graphics needed:** Solar radiation parameterization diagram, SRM governance flowchart, timeline of commit activity
- **Music cue:** Something that sounds like sunlight through clouds — ethereal, then industrial

---

*Research compiled: September 2026 | Branch: solar-geoengineering*