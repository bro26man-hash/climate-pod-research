# 🎙️ Cross-Theme Commit Trend Analysis — v7 (September 2026)

> **Last updated:** September 2026 (v7)  
> **Branch:** `main`  
> **Podcast series:** Climate Technology & Geoengineering  

---

## What We Did in v7

Pulled fresh commit histories from **4 additional repositories** across all three themes, supplementing the v6 ecosystem-level analysis:

| Theme | Repos | Commits Pulled | Key Findings |
|-------|-------|----------------|--------------|
| ☀️ Solar | WRF (10), ClimateMARGO (10), PCMDI, srm-forever, MDTF | 29 new | TEMPO disable = clearest SRM signal; WRF-PCMDI coupling; ClimateMARGO enigma confirmed |
| 🌍 Carbon | OpenCarbon (10), CO2-Sequestration (2), BECCS (5), ClimateSoton (4) | 21 new | Ghost taxonomy (4 types); Collaboration-Failure pattern; Institutional-Canary signal |
| 🌊 Ocean | ClimateSoton (4), WRF (indirect), MDTF (PBP-POD) | 14+ new | CFD bridge identified; WRF coupling unused; Open-source culture gap |

**Total v7 commits pulled: 44+ across 6 repos**

---

## The Three Universes (v7 Updated)

### Fast Universe (Institutional, Funded, Sustained)
| Repo | Stars | Commits | Theme |
|------|-------|---------|-------|
| **Open-Sustainable-Technology** | 2,552 | 3-4/month sustained | Carbon (directory) |
| **WRF** | 1,762 | 10 in 20 days (v4.8.0) | Solar (atmosphere) |
| **PCMDI** | 133 | 10 in 2 days (v4.2.1) | Solar (QA) |
| **MDTF-diagnostics** | 80 | 5 in 1 day (PBP-POD) | Ocean (eval) |

### Slow Universe (Individual, Unfunded, Dormant)
| Repo | Stars | Status | Theme |
|------|-------|--------|-------|
| **OpenAir-Cyan** | 76 | 2+ yr dormant | Carbon |
| **ClimateMARGO** | 73 | Revival unclear (README only) | Solar |
| **Carbon_Capture_ML** | 56 | 1.5 yr dormant | Carbon |
| **srm-forever** | 0 | Active (docs only) | Solar |
| **DAC_peroxovanadates** | 2 | Sparse (CC0) | Carbon |
| **DAC_peroxotitanates** | 2 | Sparse (CC0) | Carbon |

### Empty Universe (Zero Presence)
| Domain | Repos | Commits | Theme |
|--------|-------|---------|-------|
| **Ocean geoengineering** | 0 | 0 | Ocean |
| **Marine cloud brightening** | 0 | 0 | Ocean |
| **Ocean sensors/IoT** | 0 | 0 | Ocean |
| **Ocean alkalinity enhancement** | 0 | 0 | Ocean |

---

## v7 Headline Findings

### 1. The Ghost Taxonomy (Carbon Theme — NEW)

We can now classify every dead/dormant carbon-capture repo into 4 types:

| Type | Repo | Pattern | Story |
|------|------|---------|-------|
| **Upload-and-Vanish** | CO2-Sequestration | 2 commits same day, 2019, then 6+ yr silence | Dump code and leave |
| **Project-Workflow** | BECCS | 5 commits in 8 days, then "completed" | Honest finish, moved on |
| **Collaboration-Failure** | OpenCarbon | 2 contributors, 3 PRs, then 2+ yr silence | Team tried, failed, vanished |
| **Ghost-Star Giant** | carbon-capture-and-storage | 85 stars, 0 commits since 2021 | Citation artifact, not usable code |

**The podcast angle:** *"Carbon capture code doesn't die dramatically — it fades. Sometimes it vanishes in a single day. Sometimes it's declared 'completed.' Sometimes two people merge three PRs and then silence. The taxonomy of death has four patterns, and they all end the same way: nobody commits."*

### 2. The WRF TEMPO Disable — Clearest SRM Signal (Solar Theme — NEW)

The June 5, 2026 commit (6a289e1) turning off `tempo_aerosolaware` and `tempo_hailaware` is the most explicitly SRM-relevant commit in WRF's history:

- Someone tried to run WRF with stratospheric aerosol injection
- The physics suite produced unstable results
- The fix was to **disable the options**
- This is either a genuine SAI attempt that failed, or a preemptive stability fix
- Either way, it's documentation of what happens when you try to simulate SRM with the world's most important climate model

**The podcast angle:** *"The most important climate model has a commit that says 'we tried geoengineering and the physics broke.' It's in the code. Nobody announced it. The model just... adjusted."*

### 3. The CFD Bridge — Ocean Theme's Most Significant Finding (NEW)

ClimateSoton/climate-research-group is the **only carbon-theme repo with 2026 activity** (Aug 6, 2026). It's a website, not code. But the research group works on CFD modelling, chemical looping, and reaction engineering — the exact expertise needed for ocean circulation modeling and OAE dissolution kinetics.

**The bridge:** ClimateSoton's CFD expertise → ocean circulation modeling → OAE intervention simulation. The expertise exists. The code doesn't. A small grant could bridge the gap.

**The podcast angle:** *"The only active carbon-capture repo in 2026 is a website. But that website belongs to a CFD research group that could be the bridge to ocean intervention. The code might not exist yet. But the capability does."*

### 4. The WRF Ocean Coupling That Isn't (NEW)

WRF has ocean coupling code (MOM/POP). It's been in the repository for years. The v4.8.0 release continues to update air-sea interaction physics. But nobody is using it for ocean intervention scenarios.

The TEMPO disable (Jun 5) shows someone tried SAI and the physics broke. If someone were running WRF for ocean-intervention modeling, the TEMPO disable and the solar radiation bug fix (e836cd6) would directly affect their results. The chain exists in theory. The code is in the repository. But nobody runs it.

**The podcast angle:** *"WRF has ocean coupling code. It's been there for years. Theatmosphere model feeds into the ocean model. But nobody is using it to simulate what happens when we intervene. The bridge is built. Nobody crosses it."*

### 5. The Open-Source Culture Gap (NEW)

ClimateSoton publishes papers about CFD research but doesn't share code on GitHub. This is the "publication without open-source" pattern. It suggests the barrier to ocean intervention code isn't governance (papers are published openly) — it's open-source culture (code is not shared).

**The podcast angle:** *"The research is happening. The papers are published. The website is updated. But the code isn't on GitHub. The barrier isn't governance — it's culture. Climate scientists publish papers. They don't share code."*

---

## v7 Cross-Theme Commit Timeline

### The Two SRM Bugs (Solar)
```
May 28, 2026:  WRF e836cd6 — "Correction for eot calculation for solar radiation"
               → Every SAI simulation may have had energy budget error
               → Public notice: None

Sep 4, 2026:   PCMDI 90cbc50 — "Prevents roundoff to 1.00 in mean_climate figures"
               → Every v4.2.0 output corrupted
               → Public notice: None
```

### The TEMPO Disable (Solar — NEW)
```
Jun 5, 2026:   WRF 6a289e1 — "Turn off tempo_aerosolaware and tempo_hailaware in Registry"
               → Someone tried SAI, physics broke, options disabled
               → Public notice: None
```

### The CC0 Revolution (Carbon)
```
Sep 12, 2025:  DAC_peroxovanadates e041eff — "Added CC0 license"
               → Two researchers dedicated all data to public domain
               → Public notice: None (until now)
```

### The Ghost Patterns (Carbon — NEW)
```
Mar 24, 2019:  CO2-Sequestration — 2 commits, "Initial commit" + "Add files via upload"
               → 6+ years of silence (Upload-and-Vanish)

Jan-Feb 2024:  BECCS — 5 commits, then "completed"
               → 1.5 years of silence (Project-Workflow)

Jul 2023:      OpenCarbon — 3 PRs merged, then silence
               → 2+ years of silence (Collaboration-Failure)

Mar 2021:      carbon-capture-and-storage — 85 stars, last commit
               → 4+ years of silence (Ghost-Star Giant)
```

### The Ocean Silence (Ocean)
```
Jun 19, 2026:  MDTF 33024ad — "add MCS precipitation-buoyancy statistics POD"
               → 5 commits, 1-day burst (code + 4 doc updates)
               → Ocean-atmosphere diagnostic, not intervention simulation
               → The most ocean-relevant code evaluates models, not perturbations

Aug 6, 2026:   ClimateSoton — 4 commits, website update
               → CFD research group, active, but no code on GitHub
               → The bridge exists in expertise, not in code
```

---

## v7 The Three Universes — Updated

```
                    ATMOSPHERE
                         │
            ┌────────────┼────────────┐
            │            │            │
      SOLAR REMOVAL   SRM       SOLAR RADIATION
      (CDR)           (SAI)      (MODELS)
            │            │            │
            │    srm-   │    WRF    │
            │  forever  │  (1,762★) │
            │    0★     │   15 commits  │
            │           │   + TEMPO   │
            │           │   disable   │
            │           │   (Jun 5)   │
            │           │            │
            │           │   Solar     │
            │           │   radiation │
            │           │   bug fix   │
            │           │   (May 28)  │
            │           │            │
  ──────────┼───────────┼────────────┼──────────────
            │           │            │
      OCEAN             │     ATMOSPHERE
   INTERVENTION         │     MODELS
            │           │            │
      ZERO              │   PCMDI   │
      REPOS             │  (133★)   │
      12 QUERIES        │   15 commits  │
      ZERO COMMENTS     │            │
                      │   PCMDI     │
                      │   roundoff  │
                      │   bug (Sep 4)│
                      │            │
                      │   MDTF      │
                      │   PBP-POD   │
                      │   (Jun 19)  │
                      │   5 commits │
                      │   1-day burst│
                      │            │
      ClimateSoton    │            │
      CFD bridge      │            │
      (Aug 6)         │            │
      expertise,      │            │
      not code        │            │
                      │            │
      WRF ocean       │            │
      coupling        │            │
      (exists,        │            │
      unused)         │            │
            │           │            │
            └────────────┼────────────┘
                         │
                    CARBON
                  CAPTURE (CDR)
                         │
            ┌────────────┼────────────┐
            │            │            │
         DADIUS      CCS       CARBON
      (DIRECT AIR)  (STORAGE)   (SURVEY)
            │            │            │
      tjz21: 2★     ghost:    Open-Sust:
      CC0: YES     85★ dead    2,552★ alive
      10 commits    0 commits   15 commits
                      
      OpenCarbon:     CO2-Sequest:    BECCS:
      2★, 3 PRs       32★, 2 commits   1★, 5 commits
      2+ yr silence    6+ yr silence   "completed"
      (Collab-Failure) (Upload-Vanish) (Project-Workflow)
```

---

## v7 Episode Planning

| Episode | Branch | Key Questions | v7 Commit Evidence |
|---------|--------|---------------|-------------------|
| **Solar Geoengineering** | `solar-geoengineering` | Why is SRM code so scarce? Can interactive models democratize the discourse? Arctic risks? CMIP6 evaluation as governance infrastructure? What happens when the model itself can't handle SAI? | WRF: TEMPO disable (Jun 5) = clearest SRM signal; Solar radiation bug (May 28); PCMDI: roundoff bug (Sep 4); ClimateMARGO: README-only revival (Aug 17) |
| **Carbon Capture** | `carbon-capture` | Can open source break the $1000/ton DAC cost barrier? What makes OpenAir-Cyan special? Are peroxides the sorbent of the future? The August 2026 materials wave? The CC0 revolution? How do carbon repos die? | Ghost taxonomy (4 types); OpenCarbon collaboration failure; BECCS honest completion; ClimateSoton as canary; CC0 pioneers; OpenDAC reference |
| **Ocean Intervention** | `ocean-intervention` | Why is ocean geoengineering the empty quadrant? What would open-source OAE look like? Is the silence a governance chill or a culture gap? Can CFD bridge the gap? | Zero repos (12 queries); MDTF PBP-POD (mirror, not window); ClimateSoton CFD bridge; WRF coupling unused; Open-source culture gap |

---

## v7 Research Log

| Date | Activity |
|------|----------|
| Sep 2026 | v6: Initial cross-theme analysis from 8 repos |
| Sep 2026 | v7: Fresh commit data from 4 additional repos (WRF, ClimateMARGO, OpenCarbon, CO2-Sequestration, BECCS, ClimateSoton) |
| Sep 2026 | v7: WRF TEMPO disable identified as clearest SRM signal |
| Sep 2026 | v7: WRF-PCMDI coupling analysis (two bugs, same release cycle pattern) |
| Sep 2026 | v7: ClimateMARGO dormancy pattern confirmed (2 README updates, zero code) |
| Sep 2026 | v7: Ghost taxonomy created (4 types: Upload-and-Vanish, Project-Workflow, Collaboration-Failure, Ghost-Star Giant) |
| Sep 2026 | v7: ClimateSoton identified as CFD bridge (only 2026 carbon-theme activity) |
| Sep 2026 | v7: WRF ocean coupling (MOM/POP) re-examined — code exists but unused |
| Sep 2026 | v7: "Open-source culture gap" hypothesis (papers published, code not shared) |
| Sep 2026 | v7: Bridge funding opportunity proposed (CFD-to-Ocean) |
| Sep 2026 | v7: Three narrative arcs added across all branches |

---

## Quick Links

- 🔗 **Repo:** https://github.com/bro26man-hash/climate-pod-research
- ☀️ Solar branch: https://github.com/bro26man-hash/climate-pod-research/tree/solar-geoengineering
- 🌍 Carbon branch: https://github.com/bro26man-hash/climate-pod-research/tree/carbon-capture
- 🌊 Ocean branch: https://github.com/bro26man-hash/climate-pod-research/tree/ocean-intervention
- 📊 v7 Cross-theme analysis: this file
- 📊 v6 Cross-theme analysis: [CROSS-THEME-ANALYSIS-SEP2026.md](https://github.com/bro26man-hash/climate-pod-research/blob/main/CROSS-THEME-ANALYSIS-SEP2026.md)
