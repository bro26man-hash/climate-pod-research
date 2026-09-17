# Ocean Intervention — Commit Trend Analysis

## Overview

This is the most unusual finding in the entire research project. Unlike solar geoengineering (PCMDI, 133 stars; AM3, legacy; srm-forever, emerging) and carbon capture (OpenAir-Cyan, 76 stars; DAC materials wave; cost models), ocean geoengineering has zero meaningful open-source presence on GitHub. This is not a data collection failure — it has been confirmed across multiple search strategies and query variations.

## Search Strategy and Results

Queries attempted: "ocean geoengineering", "ocean alkalinity enhancement", "iron fertilization", "marine cloud brightening", "ocean intervention marine technology", "ocean monitoring pH sensor", "ocean geoengineering simulation", "artificial upwelling", "seaweed carbon farming".

Total ocean-specific repositories found: 0.

The only ocean-adjacent project found in any search was Team50-Labs/NebuGrid-OpenSource (0 stars) — fog-harvesting for arid coastal environments. Not ocean geoengineering, but tangentially related.

What this means: The absence is not because ocean geoengineering does not exist in science — it is one of the most actively researched areas in climate science, with major programs at WHOI, Scripps, GEOMAR, and IOC-UNESCO. The absence is specifically from open-source code repositories. This is a platform-specific gap, not a research gap.

## Three Hypotheses for the Ocean Gap

### H1: Institutional Gatekeeping

Ocean geoengineering research is concentrated in a handful of institutions (WHOI, Scripps, IOC-UNESCO, GEOMAR) that publish in closed journals and share data through institutional channels, not GitHub. The culture of ocean science predates the open-source movement by decades. Oceanographers share data through NCEI, GTSPP, and Argo — not through Git repositories.

Evidence: The closest thing to ocean modeling infrastructure on GitHub is PCMDI metrics package (133 stars), which evaluates climate models but does not specifically support ocean intervention scenarios.

Implication: The ocean geoengineering community is institutionally older and more closed than the atmospheric or carbon capture communities. Replacing institutional data-sharing with open-source collaboration would require a cultural shift, not just tooling.

### H2: Governance and Liability

Ocean interventions carry unique legal and governance complexity. The London Convention/London Protocol directly regulates ocean fertilization research. The risk of being associated with unregulated ocean experiments may deter public code sharing. Scientists may self-censor to avoid regulatory scrutiny.

Evidence: The London Protocol's 2013 decision statement on ocean fertilization explicitly notes that none of the activities support reporting on ocean fertilization and other marine geoengineering activities. This regulatory environment creates a chilling effect on public-facing research tools.

Implication: The GitHub silence may reflect a regulatory environment where ocean geoengineering research is legally sensitive. Sharing code that could be used to plan or simulate ocean interventions might carry legal risk that atmospheric or carbon capture tools do not.

### H3: Experimental Complexity Barrier

Solar radiation management can be modeled with radiative transfer codes. Direct Air Capture can be prototyped in a garage (OpenAir-Cyan, 76 stars). Ocean interventions require ship time in remote waters, multi-year sensor deployments, and complex biogeochemical monitoring — the barrier to GitHub-ready prototypes is enormously higher.

Evidence: The DAC community produced OpenAir-Cyan — a working, buildable, OSHWA-certified hardware device. No equivalent exists for ocean interventions. The experimental infrastructure required (ships, sensors, sampling) is orders of magnitude more expensive than an air pump and lithium hydroxide.

Implication: The maker revolution that produced OpenAir-Cyan has not reached ocean geoengineering because the maker revolution requires tools that are cheap, safe, and portable. Ocean geoengineering is none of these.

## Comparison Across Three Themes

| Dimension | Solar Geoengineering | Carbon Capture | Ocean Intervention |
|-----------|---------------------|----------------|-------------------|
| Active repos | 2-3 | 5-7 | 0 |
| Highest-star repo | 133 (PCMDI) | 2552 (Open Sustainable Tech) | 0 |
| Dedicated simulation frameworks | 0 | 0 | 0 |
| DIY/Open Hardware | 0 | 1 (OpenAir-Cyan, 76 stars) | 0 |
| Recent activity (2026) | 1 repo | 4-5 repos | 0 |
| Coordinated release events | No | Yes (Aug 19, 2026) | No |
| Institutional vs Community | Institutional burst | Mixed | Absent |

## What Would Open-Source Ocean Intervention Look Like?

Despite the absence, here are concrete open-source projects that could serve the ocean geoengineering community:

1. Open Ocean Alkalinity Data Platform — Shared database of alkalinity addition experiments, with sensor calibration protocols and data pipelines
2. Carbonate Chemistry Simulation Toolkit — Open-source modeling of ocean carbonate chemistry changes following alkalinity addition (Python, using existing ocean model frameworks)
3. Marine Cloud Brightening Design Repository — Open-source designs for spray nozzles, droplet size optimization, and atmospheric transport modeling for cloud brightening experiments
4. Ocean Iron Fertilization Flux Model — Python/C++ model tracking iron release, phytoplankton bloom dynamics, and carbon export efficiency
5. Seaweed LCA Tool — Life-cycle assessment tool for seaweed farming as a carbon removal strategy, including growth modeling, burial rates, and lifecycle emissions

## The Governance Signal

The absence on GitHub may itself be the most important finding. If ocean geoengineering is the most potentially impactful climate intervention category (the ocean absorbs 90% of excess heat and 30% of anthropogenic CO2), and it has zero open-source presence, then the governance and institutional barriers are higher than for any other climate-tech domain.

This is not just a podcast episode — it is a fundamental observation about how climate innovation gets organized on the internet. The ocean geoengineering community exists in scientific journals but not in open code. The question for policymakers is: should there be an open-source ocean geoengineering research program, and if so, what would it look like?

## Key Episode Questions

1. Why is ocean geoengineering invisible on GitHub? The answer is not technical — it is institutional, legal, and cultural. What would it take to change that?
2. What would an open-source ocean alkalinity project look like? Open data from alkalinity addition experiments, open sensor designs for pH monitoring, open modeling of carbonate chemistry — but who would run it?
3. Is the absence itself a governance signal? The silence on GitHub may reflect the London Protocol restrictions on ocean fertilization research — scientists self-censor to avoid regulatory scrutiny.
4. Can digital twins prepare the ground? If we can model ocean systems in silico (PCMDI metrics, Earth digital twins) before physical deployment, that might lower the governance risk enough to attract open-source development.
5. What is the difference between ocean research that can be open-sourced vs. that which cannot? Sensor designs and data pipelines are shareable; actual ocean experiments are not. Where is the line?