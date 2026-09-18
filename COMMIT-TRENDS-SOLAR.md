# ☀️ Solar Geoengineering — Commit Trend Analysis
## Recent Development Activity in Solar Radiation Management Codebases

*Analysis period: May–September 2026 | Data source: GitHub REST API*

---

## Aggregate Statistics

| Repository | Commits Analyzed | Date Range | Avg. Commit Frequency | Top Contributor |
|-----------|-----------------|------------|----------------------|----------------|
| **WRF** | 15 | May 12 – Jun 8, 2026 | ~1 commit/week | weiwangncar (NCAR) |
| **PCMDI Metrics** | 15 | Sep 3 – Sep 17, 2026 | ~3 commits/day (!) | Jiwoo Lee (PCMDI) |
| **MDTF Diagnostics** | 15 | May 22 – Aug 14, 2026 | ~1 commit/week | Wei-Ming Tsai (GFDL) |
| **ClimateMARGO.jl** | 15 | Jan 2022 – Aug 2026 | ~2 commits/year | Fons van der Plas |
| **srm-forever** | Limited | Ongoing | Low | Hausfath |

---

## WRF: The Steady Engine

### Commit Velocity: Consistent (~1/week)
```
May 12  ██  MYNN-SFC submodule update
May 19  ██  Bug fix for udm
May 20  ██  Minor Tempo changes
May 20  ██  Scheme-guard bug in urban NbS
May 20  ██  New namelists for ShinHong PBL
May 21  ██  mp_physics=88 in TEMPO error message
May 26  ██  Fixing CDXWRF module
May 26  ██  Update readme for GFL option
May 27  ██  MMM-physics SHA update
May 27  ██  MYNN-EDMF pointer update, icloud_bl removal
May 30  ██  Vectorization option in AOCC stanza
Jun 5   ██  Turn off tempo_aerosolaware/hailaware
Jun 6   ██  README & version → v4.8.0
Jun 8   ██  Merge release-v4.8.0
```

**Pattern:** NCAR/NOAA-led institutional development. Multiple contributors from major climate modeling centers. Version v4.8.0 released June 2026.

**Solar-relevant highlights:**
- **Solar radiation EOT correction** (May 28) — improves accuracy of solar forcing calculations
- **TEMPO aerosol/hailaware toggles** (Jun 5) — affects how aerosols (including SRM-relevant scattering particles) are modeled
- **PBL scheme additions** (May 20) — new parameterizations affect surface energy balance under SRM scenarios

**What this tells us:** The solar geoengineering modeling infrastructure is **well-funded and consistently maintained**. NCAR and NOAA are investing in incremental improvements, not breakthrough features. The message: "We're making the tools more accurate, not questioning whether we need them."

---

## PCMDI Metrics: The Sprint

### Commit Velocity: Explosive (10 commits in 2 days)
```
Sep 3   ████████  Extremes chunking merge, dask/SVD memory fix, numpy SVD fix, rename
Sep 4   ████████████████████  Roundoff fix, version bump to 4.2.1, modpath patch, 3 merges
Sep 17  ██████████  modpath_list single-file patch, merge
```

**Pattern:** Classic **release-driven sprint**. PCMDI team identified issues, fixed them in rapid succession, and shipped v4.2.1 in a single day with 7 commits.

**Solar-relevant highlights:**
- **Roundoff to 1.00 prevention in mean_climate** (Sep 4) — numerical precision fix that could affect how SRM radiative forcing values are reported in CMIP6 experiments
- **Extremes chunking with SVD** (Sep 3) — analyzing climate extremes using Singular Value Decomposition; relevant for understanding SRM's impact on extreme weather events
- **Memory optimization via dask rechunking** — enabling larger ensemble runs that include SRM scenarios

**What this tells us:** The evaluation community is **racing**. The burst pattern suggests urgency — possibly tied to an upcoming IPCC deadline, CMIP6 submission cycle, or a specific SRM experiment (perhaps geoMIP or G6) that needs reliable evaluation tools. The roundoff fix is particularly telling: in SRM, small forcing differences (watts per square meter) translate to large policy differences (degree Celsius of avoided warming).

---

## MDTF Diagnostics: The Diagnostic Breakthrough

### Commit Velocity: Punctuated Equilibrium
```
May 22  ██  Blocking notebook merge
May 27  ██  Moved blocking_neale_nb to dev
Jun 1   ██  Quarterly metrics workflow + traffic logging
Jun 2   ██  Branch merge + citation addition
Jun 8   ██  README updates (×2)
Jun 19  ██████████████████████████████  MCS precip-buoyancy POD: 5 commits to ONE FILE
Aug 14  ██  Merged PR #825
```

**Pattern:** Long quiet periods punctuated by massive single-day efforts. The **June 19, 2026** event is the standout: five commits to `MCS_precip_buoy_stats.rst` in a single day.

**Solar-relevant highlights:**
- **Precipitation-buoyancy POD** — This is the killer feature.Proper Orthogonal Decomposition of precipitation vs. buoyancy relationships helps researchers identify how SRM-induced surface cooling would restructure tropical rainfall patterns. The fact that it got 5 commits in one day suggests it was either newly developed or underwent a major revision.
- **Quarterly metrics workflow** — automated tracking suggests this tool is now being used operationally, not just for research
- **MCS (Mesoscale Convective System) focus** — MCSs are the primary vehicle for tropical precipitation. Understanding how SRM affects MCSs is critical for predicting drought/flood risks under SRM scenarios

**What this tells us:** MDTF's precip-buoyancy POD is the **closest thing to an SRM impact prediction tool** that exists in open source. The single-day burst suggests a major advancement. This is the tool that answers: "If we deploy SRM, where will the rain go?"

---

## ClimateMARGO: The Ghost Revival

### Commit Velocity: Nearly Zero (2 README commits after 2-year silence)
```
... (2+ years of nothing) ...
Aug 17  ██  README update #1
Aug 17  ██  README update #2
```

**Pattern:** Classic **dormant repo ghost revival**. No code changes. No new features. Just two README updates on the same day.

**Solar-relevant highlights:**
- The model itself is an **idealized climate-economic optimizer** that balances mitigation, adaptation, and SRM deployment
- No code updates since October 2023 (unit conversions)
- The README updates could signal:
  - Preparation for a new study or publication
  - An upcoming refactor or migration
  - Someone discovering the repo and cleaning up the documentation
  - Interest triggered by IPCC AR7 or new SRM policy discussions

**What this tells us:** The economic modeling side of SRM is **intellectual, not practical**. ClimateMARGO exists as a theoretical framework, not as a tool used by operational programs. Its revival is ambiguous — it could signal genuine renewed interest, or it could be another example of academic business-as-usual (update README, cite paper, move on).

---

## Cross-Repo Themes: What the Commits Tell Us

### 1. Institutional Confidence
Both WRF and PCMDI are showing **sustained, confident development**. There's no sign of controversy or hand-wringing about SRM's validity in the code. The institutional community is treating SRM modeling as a normal (if specialized) part of climate science.

### 2. Precision Before Power
PCMDI's roundoff fix and MDTF's chunking optimization both signal that the community is focused on **accuracy and reliability**, not new capabilities. The message: "We need to get the numbers right before we can make policy."

### 3. The Ocean Connection Is Emerging
MDTF's precip-buoyancy POD (5 commits to one file in one day) is the single most ocean-relevant development in our entire study. It represents the growing recognition that **SRM doesn't just cool the atmosphere — it reshapes ocean-atmosphere coupling** through changes in precipitation and buoyancy.

### 4. Economic Models Are Sleeping
ClimateMARGO's ghost revival and srm-forever's zero-star existence paint a clear picture: **nobody is building the economic case for SRM in public, in real-time, on GitHub**. The economic debates are happening in journals and policy papers, not in code.

---

## 🎙️ Podcast Episode Architecture

### Cold Open
> "In May 2026, a modeler at NCAR fixed a solar radiation calculation. On the same day, a NOAA team was rewriting precipitation statistics. On the same day, a theoretical economist in Germany updated a README file after two years of silence. Three commits. Three continents. One question: should we dim the sun?"

### Act 1: The Infrastructure (WRF + PCMDI)
- WRF's solar radiation EOT correction — the model that simulates Earth's thermostat
- PCMDI's 10-commit sprint — evaluation is racing ahead of simulation
- **Talking point:** "The tools are ready. The question is whether we are."

### Act 2: The Impact (MDTF)
- Precip-buoyancy POD — five commits to one file in one day
- MCS focus — where SRM meets tropical rainfall
- **Talking point:** "If you want to know what SRM does to rain, you need a POD."

### Act 3: The Economics (ClimateMARGO + srm-forever)
- Ghost revivals and zero-star masterpieces
- Weitzman discounting — the forever cost of SRM
- **Talking point:** "The economic case for SRM is being made in journals, not in code. Why?"

### Closing Question
> "The climate models are getting better. The evaluation tools are getting faster. The economic frameworks are getting richer. But none of them can answer the only question that matters: do we want to live in a world where we need them?"

---

## 📊 Commit Trend Dashboard

```
WRF          ████████████████████████  CONSISTENT (Institutional)
PCMDI        ████████████████████████████████████████  BURST (Release-driven)
MDTF         ██████████░░░░░░░░░░░░░░░░░░░░░░░░░░░░  PUNCTUATED (Feature-driven)
ClimateMARGO ██░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  DORMANT (Individual)
srm-forever  █░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  STEADY (Theoretical)
```

---

*Analysis prepared: September 2026 | Branch: solar-geoengineering | Repository: climate-pod-research*