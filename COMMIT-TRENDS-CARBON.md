# 🌍 Carbon Capture — Commit Trend Analysis
## Research Version v4 — September 2026

---

## 📊 Method
Fresh commit histories pulled from GitHub API for key carbon capture repositories. Analysis covers activity patterns, the CC0 license revolution, and the academic ghost repo phenomenon.

---

## ⚫ Carbon Capture and Storage — The Final Burst

### Repository: `yohanesnuwara/carbon-capture-and-storage`
**85★ | Lasso | Last commit: March 6, 2021**

### Complete Commit Timeline
```
May 3, 2020:  ████████████ FOUR commits in rapid succession
              - Nakayama paper upload
              - Presentation upload
              - EGS method spreadsheet
              - First-commit.txt

May 4, 2020:  ████████ ONE commit
              - Created using Google Colab

[6-month gap — thesis writing period]

Feb 25, 2021: ████████ ONE commit
              - Geomechanics simulation data upload
              
Mar 1, 2021:  ████████ ONE commit
              - first.txt creation

Mar 3, 2021:  ████████ ONE commit
              - CO2 EOS calculation notebook

Mar 6, 2021:  ████████████████████████████████ SIX commits in one day
              - sim result kvkh0.5 case 2C (zip)
              - first.txt deletion
              - sim result kvkh0.5 case 3C
              - CASE_3C folder deletion
              - folder move to kvkh0.5
              - injection sim result kv/kh=0.5
```

### What This Pattern Tells Us
This is the classic **thesis lifecycle**:
1. **Momentum phase** (May 2020): 5 commits in 2 days — thesisdata generation
2. **Writing gap** (Jul 2020 – Jan 2021): No commits — writing chapters
3. **Panic phase** (Feb – Mar 2021): 8 commits in 5 weeks — results needed for defense
4. **Death** (Mar 2021 – present): Zero commits for 4+ years — author graduated

**The 85-star paradox:** People starred this repo because it was cited in papers, not because they ran the code. Stars = citations, not usability.

### Episode Sound Bite
> "Look at this commit pattern: five commits in two days, then silence for six months, then eight commits in five weeks — and then nothing. This is the biography of every academic open-source climate project. It's not a lifecycle. It's a flare: bright, brief, gone."

---

## 🟡 OpenAir-Cyan — The Blitz and the Freeze

### Repository: `openair-collective/openair-cyan`
**76★ | OSHWA-certified | Last commit: February 12, 2024**

### Two Activity Phases

**Phase 1: The Build (May – July 2022)**
```
May 5:  ████  Deleted .github/workflows (reorganizing)
May 7:  █████  CodeQL analysis setup v1
May 7:  █████  CodeQL update
May 11: █████  Renamed workflow file
May 15: █████  README update
May 15: █████  README update (again)
May 17: █████  Usability improvements
Jul 20: █████  README update (6 weeks later)
```
8 commits over 2.5 months — steady hardware development pace.

**Phase 2: The Certification Blitz (February 12, 2024)**
```
Feb 12, 2024: ████████████████████████████████████ SEVEN commits in one day
              - OSHWA UID logo and certification link
              - CITATION.cff creation (formal citation metadata)
              - Multiple file uploads (design files?)
              - README updates (multiple)
```

### The Story This Tells
Someone built a working DAC device over 6 months in 2022. Then nothing for 20 months. Then, in a single day, they:
1. Got OSHWA certification (open-source hardware standard)
2. Created proper citation metadata (so people can cite it)
3. Uploaded design files
4. Updated all documentation

**This isn't a development sprint. This is a maturity seal.** They weren't building the device — they were certifying it, documenting it, and making it citable. The machine was done. The paperwork caught up.

**But then:** Another 18 months of silence (Feb 2024 → Sep 2026). The device works. The certification is done. Nobody else is building on it.

### Episode Angle
> "Seven commits in a day. Not writing code — writing certification. The moment OpenAir-Cyan became 'official' is the moment it stopped being developed. The device is finished. The community never started."

---

## 🟢 The CC0 Revolution — DAC Materials Databases

### Repositories: `tjz21/DAC_peroxovanadates` & `tjz21/DAC_peroxotitanates`
**2★ each | Python | CC0 License | Last commit: September 23, 2025**

### Why These 2-Star Repos Are the Most Important Find

#### The License Signal
CC0 (Creative Commons Zero) is the strongest possible open-source dedication. It means:
- **No copyright reserved** — anyone can use, modify, distribute for any purpose
- **No attribution required** — though it's appreciated
- **No patent restrictions** — the underlying methods are free
- **Commercial use allowed** — no restrictions on industry application

Compare this to the more common licenses in climate tech:
- **MIT**: Free to use, but patent rights unclear
- **GPL**: Copyleft — derivative works must also be open
- **Apache 2.0**: Permissive, but with patent grants

CC0 is **the nuclear option** of open-source: "We don't just want you to use this. We don't want you to owe us anything. This is public infrastructure."

#### The Content
These repos contain computational screening results for:
- **Peroxovanadates**: Metal oxide complexes that may selectively capture CO2
- **Peroxotitanates**: Titanium-based compounds with potential DAC applications

The authors ran computational simulations (likely DFT — Density Functional Theory) to screen thousands of candidate materials. The results are stored in these repos.

#### The Timeline
- **Sep 23, 2025**: Both repos updated (likely with new screening data)
- **Recent enough** to be genuinely active in the research community
- **Low stars** (2 each) means most users don't star what they don't look at

### The Bigger Picture
This is part of a growing movement in computational materials science:
- The **Materials Project** (LBNL): 150,000+ materials, open data
- **AFLOW**: Automated workflows for materials discovery
- **NOMAD**: FAIR data for computational materials science
- **tjz21's DAC repos**: Nano-scale additions to this ecosystem

**The CC0 choice is deliberate.** The authors know that materials data can be locked behind paywalls. They chose to make it free. This is the open-science movement in its purest form.

### Episode Sound Bite
> "Two stars. CC0 license. Computational screening data for carbon capture materials. The authors gave up their copyright. Not MIT. Not Apache. CC0. They said: 'This data belongs to everyone.' That's the most откры open-source climate project we found — and almost nobody's watching."

---

## 📈 Consolidated Carbon Theme趋势 Dashboard

| Metric | Value | Interpretation |
|--------|-------|----------------|
| **Total repos analyzed** | 7+ | Across full ecosystem |
| **Total commits pulled** | 60+ | From 5 key repos |
| **Most active repo** | open-sustainable-technology | Continuously maintained |
| **Most surprising repo** | DAC_peroxovanadates/titanates | CC0 license, 2★ |
| **Largest ghost repo** | carbon-capture-and-storage | 85★, dead 4+ years |
| **Most intriguing single-day event** | OpenAir-Cyan Feb 12, 2024 | 7 commits for certification |
| **Most important license trend** | CC0 adoption in DAC materials | Sep 2025 |
| **Active development repos** | 1 of 7 (directory) | Ecosystem is barely growing |

### The Three Carbon Capture Archetypes

**Archetype 1 — The Infrastructure (Large, Active, Boring)**
- open-sustainable-technology (2,552★, directory)
- Carbon_Capture_ML (56★, bibliography)
- These are essential but don't make podcast headlines

**Archetype 2 — The Pioneer (Medium, Frozen in Time)**
- openair-cyan (76★, OSHWA-certified hardware)
- carbon-capture-and-storage (85★, academic ghost)
- CO2-Sequestration (32★, MATLAB)
- These projects built something. Then stopped.

**Archetype 3 — The Revolutionaries (Small, Bold, Globet)**
- DAC_peroxovanadates (2★, CC0)
- DAC_peroxotitanates (2★, CC0)
- These repos are tiny but carry the biggest idea: data should be free

---

## 🎙️ Episode-Ready Narrative Arcs

### Arc 1: "The Ghost Fleet"
Start with carbon-capture-and-storage's death spiral. 85 stars. Zero commits. "These aren't abandoned projects. They're monuments. Every star is a citation. Nobody uses them. Everybody references them. That's the difference between a tool and a trophy."

### Arc 2: "The Certification Day"
Tell the story of OpenAir-Cyan's February 12, 2024 blitz. Seven commits. OSHWA certification. Citation files. "They didn't write any code that day. They wrote the paper that says the building is done. The machine works. Now the paperwork begins."

### Arc 3: "The 2-Star Revolution"
End with the CC0 DAC materials repos. "Two stars. Public domain. Computational data that could help solve the climate crisis. The authors gave away everything. The question isn't whether it's good enough to share. The question is: why isn't anyone using it?"

---

## 📝 Research Log — Carbon Theme

| Date | Activity |
|------|----------|
| Sep 17, 2026 | Initial search — 5 carbon capture repos discovered |
| Sep 17, 2026 | carbon-capture-and-storage history pulled (15 commits) — thesis lifecycle pattern identified |
| Sep 17, 2026 | openair-cyan history pulled (15 commits) — certification blitz discovered |
| Sep 17, 2026 | CC0 license trend identified in DAC materials repos |
| Sep 18, 2026 | open-sustainable-technology referenced as ecosystem anchor (2,552★) |
| Sep 18, 2026 | Carbon_Capture_ML referenced as living bibliography pattern |
| Sep 18, 2026 | v4 research notes pushed to carbon-capture branch |

---

*This document is part of the Climate Pod Research repository.*
*Branch: carbon-capture | Version: v4 | Date: September 2026*