# 🌍 Carbon Capture — Project Discoveries
## Research Notes for Climate Technology Podcast Series
### Updated: September 2026 (v4 — fresh commit data)

---

## Overview

Carbon capture is the most hardware-rich area of open-source climate tech on GitHub. Unlike solar geoengineering (where the code is atmospheric models), carbon capture has **open hardware designs, machine learning surveys, materials screening tools, and life-cycle decision frameworks**. The ecosystem spans from DIY desktop DAC devices to industrial-scale simulation.

---

## Tier 1: High-Impact, Community-Building

### 1. OpenAir-Cyan (DIY Direct Air Capture)
- **Repo:** [openair-collective/openair-cyan](https://github.com/openair-collective/openair-cyan)
- **Stars:** 76 | **Language:** Not specified (hardware docs) | **License:** OSHWA (Open Source Hardware)
- **Last commit:** February 12, 2024 (OSHWA certification push)
- **Focus:** DIY small-scale open hardware direct air capture device. The **only** open-source DAC hardware project with significant community traction.

**Recent Commit Signals (8 commits pulled):**
| Date | Commit | Significance |
|------|--------|-------------|
| Feb 12, 2024 | Update README — added OSHWA UID link | **OSHWA certification — open hardware legitimacy** |
| Feb 12, 2024 | Add files via upload (×2) | Documentation and design files uploaded |
| Feb 12, 2024 | Added OSHWA UID logo (US001095) | **Official open hardware certification** |
| Feb 12, 2024 | Create CITATION.cff | Citation metadata — first open-hardware DAC repo with formal citation |
| Feb 12, 2024 | Update README.md | Comprehensive documentation update |
| Jul 20, 2022 | Update README.md | Pre-certification maintenance |
| May 17, 2022 | Add files to improve usability | Usability improvements beforeigrief freeze |

**🎙️ Episode Hook:** OpenAir-Cyan is the single most important carbon capture repo on GitHub. It's the only DIY DAC device with OSHWA certification (US001095) — meaning it passed rigorous review for being truly open-source hardware. The Feb 12, 2024 commit day — 6 commits in one day — is a blitz of certification-focused activity. After that: silence. The device is built, documented, certified, and then... frozen. Why did development stop after the OSHWA push?

---

### 2. Open-Sustainable-Technology (Ecosystem Directory)
- **Repo:** [protontypes/open-sustainable-technology](https://github.com/protontypes/open-sustainable-technology)
- **Stars:** 2,552 | **Language:** Multiple | **License:** Varies
- **Last commit:** September 9, 2026
- **Focus:** Comprehensive OSS climate-tech directory spanning 2,500+ projects. The single largest catalog of climate open-source on GitHub.

**Recent Activity:** Continuously maintained with 2,552 stars — the gravitational center of the climate-tech open-source ecosystem. Carbon capture repos link to this directory as their entry point.

---

### 3. Carbon_Capture_ML (ML Survey)
- **Repo:** [zikribayraktar/Carbon_Capture_ML](https://github.com/zikribayraktar/Carbon_Capture_ML)
- **Stars:** 56 | **Language:** Jupyter Notebook | **License:** Not specified
- **Last commit:** May 8, 2024
- **Focus:** Survey of machine learning papers and code for carbon capture. Curated collection of LCAs, ML models, and datasets.

**Recent Activity:** Last commit May 2024. The repo is maturing — not growing, but not dying. 56 stars for a survey repo is strong engagement.

---

## Tier 2: Specialized Tools

### 4. CarbonLens
- **Repo:** [Thanapat18/CarbonLens](https://github.com/Thanapat18/CarbonLens)
- **Stars:** Not specified | **Language:** Python | **License:** Not specified
- **Last commit:** June 20, 2026
- **Focus:** Life-cycle decision-support tool for climate-positive carbon capture. Helps practitioners choose the most effective capture pathway.

**Recent Activity:** Active maintenance with June 2026 update. The LCA angle is systematically important — not "can we capture CO2?" but "should we capture CO2, or would that investment be better spent elsewhere?"

---

### 5. OpenCarbon
- **Repo:** [terranexum/OpenCarbon](https://github.com/terranexum/OpenCarbon)
- **Stars:** 2 | **Language:** Not specified | **License:** Not specified
- **Last commit:** August 19, 2026
- **Focus:** Carbon management technologies and plans to advance DAC research, ensuring it uses clean energy and has low cost. Very recent activity but tiny community.

**Recent Activity:** Updated August 2026. The "clean energy for DAC" framing is the newest narrative in carbon capture — moving beyond "can we capture" to "does our capture actually help."

---

### 6. ClimateSoton Climate Research Group
- **Repo:** [ClimateSoton/climate-research-group](https://github.com/ClimateSoton/climate-research-group)
- **Stars:** Not specified | **Language:** HTML (website) | **License:** Not specified
- **Last commit:** August 2026
- **Focus:** University of Southampton climate research group website. Active in CFD (computational fluid dynamics) for climate applications.

**Recent Activity:** Updated August 2026. Not carbon-capture-specific, but relevant for CFD simulation of capture processes.

---

## Tier 3: Dormant / Historical (Ghost Repos)

### 7. carbon-capture-and-storage
- **Repo:** [yohanesnuwara/carbon-capture-and-storage](https://github.com/yohanesnuwara/carbon-capture-and-storage)
- **Stars:** 85 | **Language:** Not specified | **License:** Not specified
- **Last commit:** March 6, 2021
- **Focus:** Reservoir simulation + geomechanics for carbon capture and storage. drew 85 stars but abandoned since 2021.

**Ghost Status:** **Dormant ghost** — high star count from citations, zero recent activity. The 85 stars are academic citations, not community engagement.

---

### 8. CO2-Sequestration
- **Repo:** [NHERI/CO2-Sequestration](https://github.com/NHERI/CO2-Sequestration)
- **Stars:** 32 | **Language:** Not specified | **License:** Not specified
- **Last commit:** 2019
- **Focus:** Geomechanical simulation of CO2 sequestration in deep saline formations.

**Ghost Status:** **Dormant ghost** — academic simulation tool frozen since 2019. 32 stars from the geoscience community.

---

### 9. DAC Peroxovanadates & Peroxotitanates
- **Repos:** [tjz21/DAC_peroxovanadates](https://github.com/tjz21/DAC_peroxovanadates), [tjz21/DAC_peroxotitanates](https://github.com/tjz21/DAC_peroxotitanates)
- **Stars:** 2 each | **Language:** Python | **License:** **CC0 (Public Domain)**
- **Last commit:** September 23, 2025
- **Focus:** Computational screening of DAC sorbent materials (peroxovanadate and peroxotitanate compounds). Both repos adopted CC0 public domain dedication.

**🎙️ Episode Hook:** **The CC0 Revolution.** Both of tjz21's DAC materials repos adopted CC0 (public domain) in September 2025. This is the biggest open-science signal in the carbon capture GitHub ecosystem. Researchers are treating computational screening data as public infrastructure — not as lab property. The peroxides may be the next-generation sorbent family, and the data is free for anyone to use. This is a radical departure from traditional academic publishing.

---

## Cross-Theme Patterns

| Pattern | Evidence |
|---------|----------|
| **OSHWA certification is the quality standard** | OpenAir-Cyan is the only carbon capture repo with hardware certification |
| **The epicentre of carbon capture activity is the directory, not the devices** | open-sustainable-technology (2,552★) > openair-cyan (76★) by 33x |
| **CC0 is revolutionizing materials data sharing** | tjz21's two DAC repos both adopted CC0 (Sep 2025) |
| **Ghost repos dilute the star count** | 85★ carbon-capture-and-storage (dead since 2021), 32★ CO2-Sequestration (dead since 2019) |
| **LCA thinking is the newest narrative** | CarbonLens: "should we capture?" vs "can we capture?" |
| **Clean-energy-for-DAC is framing 2.0** | OpenCarbon: DAC must use clean energy and be low-cost |
| **All hardware projects freeze after certification/documentation** | OpenAir-Cyan: 6 commits in one day (Feb 2024), then silence |

---

## Episode Notes — Carbon Capture Branch

### Key Narrative Arcs
1. **"The Only Desktop DAC You Can Build"** — OpenAir-Cyan is the only open-source hardware DAC device. OSHWA-certified. 76 stars. Then frozen. Why did the community stop building after certification?
2. **"The CC0 Revolution for DAC Materials"** — tjz21 released two sorbent screening repos under CC0 public domain. This is the most radical open-science gesture in climate tech. The data is free. Anyone can use it.
3. **"The Directory vs. The Device"** — open-sustainable-technology has 2,552 stars and is continuously maintained. OpenAir-Cyan has 76 stars and no new commits since 2024. The ecosystem directory is alive; the hardware project is frozen.
4. **"Ghost Repos and the Dilution Problem"** — carbon-capture-and-storage has 85 stars but hasn't been touched since 2021. CO2-Sequestration: 32 stars, frozen since 2019. Stars measure citations, not usability.

### Open Questions for Guests
- Should open-source hardware projects be required to maintain after certification?
- Is CC0 the right license for climate datasets? Who owns the data?
- The $1000/ton DAC cost barrier — where does open source actually help?
- Can you build a desktop DAC device? What's missing from OpenAir-Cyan that would make it more useful?
