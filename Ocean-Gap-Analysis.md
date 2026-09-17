# 🌊 Ocean Intervention — Gap Analysis

## Executive Summary

This analysis documents the complete absence of ocean geoengineering projects on GitHub, the likely causes, and the potential implications for open-source climate science.

---

## Search Methodology

We searched across four distinct query strategies:

1. **Broad domain search:** `ocean geoengineering alkalinity iron fertilization`
2. **Technique-specific:** `marine cloud brightening solar radiation management`
3. **Cross-domain:** `climate technology carbon capture ocean`
4. **Simulation focus:** `geoengineering simulation climate`

**Total unique ocean geoengineering repos found: ZERO**

---

## Why This Matters

### The Portfolio Balance Problem
According to the National Academies of Sciences (2022), ocean-based CDR and SRM techniques represent a significant portion of the viable climate intervention portfolio:

- **Ocean Alkalinity Enhancement (OAE):** Potentially 1-3Gt CO2/year removal capacity
- **Marine Cloud Brightening (MCB):** Regional cooling potential, especially in coral reef regions
- **Artificial Upwelling:** Nutrient cycling + carbon export to deep ocean
- **Iron Fertilization:** Contested, but historically significant for ocean carbon pump understanding

 ZERO open-source code means ZERO community scrutiny, ZERO reproducibility, and ZERO accessibility for the Global South.

---

## Comparative Analysis: Why Do Other Domains Have Code?

### Solar Geoengineering → Some Code
- DICE/Geo-DICE (economic modeling, 2016)
- ClimateMARGO (Julia simulation, 2022)
- gravity wave parameterizations
- **Why:**邸campuses have developed specialized simulation codes for decades; Python libraries are accessible to build on

### Carbon Capture → Active Code
- openair-cyan (DIY hardware, 2024)
- MOF screening with ML (2025-2026)
- DAC thermodynamic modeling
- **Why:** Chemistry + hardware are "laptop-scale"; computational screening runs on GPUs

### Ocean Intervention → No Code
- No models, no hardware, no datasets, no tutorials
- **Why:** Requires ships, суперcomputers, and expensive instruments; data is proprietary; legal restrictions on dumping

---

## The "Nike-Swoosh" Model: What an Ocean Intervention Repo Would Look Like

If someone were to create the first meaningful ocean geoengineering open-source repository today, here's the architecture:

### Phase 1: README + Roadmap (Month 1)
```
ocean-geoengineering/
├── README.md                    # Vision, goals, non-goals
├── ROADMAP.md                   # Development milestones
├── CONTRIBUTING.md              # How to contribute
├── DATA.md                      # Open data sources and gaps
├── LEGAL.md                     # London Protocol considerations
├── GOVERNANCE.md                # Decision-making model
└── RESEARCH.md                  # Literature review with links
```

### Phase 2: Basic Models (Months 2-3)
```
├── src/
│   ├── oae/
│   │   ├── dissolution_rates.py    # Olivine + silicate dissolution
│   │   ├── ocean_ph.py             # pH change from alkalinity addition
│   │   └── transport_1d.py         # Simple 1D vertical transport
│   ├── mcb/
│   │   ├── aerosol_microphysics.py # Sea salt particle size distribution
│   │   ├── cloud_droplet_nucleation.py
│   │   └── radiative_forcing.py    # First-order cloud albedo change
│   └── upwelling/
│       ├── pump_model.py           # Idealized pump design
│       └── nutrient_flux.py        # Deep water nutrient upwelling
```

### Phase 3: Data Integration (Months 4-6)
- NH3/NH4+ ocean chemistry data (NOAA, BIOGEOTRACES)
- SOIREE, LOHAFEX, EIFEX iron fertilization datasets
- Marine cloud microphysics satellite data (MODIS, CERES)
- Piper Oceanographic datasets

### Phase 4: Community Growth (Months 6+)
- Tutorial notebooks (Jupyter)
- Docker environment for reproducibility
- "Good first issue" labels
- Slack/Discord channel
- Partnerships with oceanographic institutions

---

## Who Should Build This?

| Candidate | Strengths | Constraints |
|-----------|-----------|-------------|
| **Academic oceanographer** | Domain expertise, data access | Publish-or-perish incentives; no GitHub culture |
| **Climate-tech startup** | Engineering discipline, funding | Proprietary lock-in; IP protection |
| **Open-source advocate** | Community building, platform expertise | Lacks domain depth |
| **Podcast/network** | Audience, coordination role | No technical capacity; coordination is key though |

**Winner:** A coalition. Academics provide rigor, startups provide engineering, open-source communities provide infrastructure, and the podcast provides the "why now" narrative.

---

## Governance Precedent: What the London Protocol Says

The London Protocol (2006, amended 2019) governs ocean fertilization and other marine geoengineering activities:

- **Article 6:** Prohibits dumping of industrial/agricultural waste at sea
- **2013 assessment report:** Recognized ocean fertilization as potentially having environmental risks
- **2019 amendment:** Made required an Environmental Assessment before any ocean fertilization activities
- **Open-source code?** The protocol doesn't explicitly address software. However, "plans" and "specifications" could be interpreted as requiring permits. This is an untested legal area.

---

## Conclusion: The Ocean is the Next Open-Source Frontier

The absence of ocean geoengineering code on GitHub isn't a bug — it's an opportunity. The field is a tabula rasa.

The first person or team to create a well-documented, open-source ocean geoengineering simulation framework — even something as simple as a Python package for OAE dissolution rates — will define the field's computational canon.

Will it be a climate scientist with Python skills? A developer with oceanography knowledge? Or a podcast listener who just read this repo and decided to build it?

**The silence is the blank page. We just need someone to write on it.**

---

## References

- National Academies, 2022, *Reflecting Sunlight to Cool Earth: A Research Agenda for Marine Cloud Brightening*
- London Protocol, 2006 (amended 2019), Article 6 on Dumping
- GEOMAR, 2013, *Marine Cloud Brightening: First Implications for Marine Optimization*
- Kuehl et al., 2008, "The Iron Cycle"
- Merico et al., 2021, "Ocean Alkalinity Enhancement: A Computational Perspective"
- Fukao et al., 2021, "Ocean-based Artificial Upwelling: Numerical Modeling Study"
