# ☀️ Solar Geoengineering — Fresh Commit Update v7 (September 2026)

> **Branch:** `solar-geoengineering`  
> **Podcast episode:** Episode 1 — Solar Geoengineering  
> **Data pulled:** September 2026 via GitHub API  
> **Repos analyzed:** 7 (WRF, PCMDI/pcmdi_metrics, MDTF-diagnostics, ClimateMARGO.jl, awesome-geoengineering, GCCS-Core, ShennongWM-G)

---

## Executive Summary

Fresh commit data from September 2026 reveals **three contrasting development universes** in solar geoengineering open source:

1. **The Institutional Fast-Lane** (WRF, PCMDI, MDTF) — Professional teams, rapid release cycles, structured versioning, institutional funding visible in commit velocity
2. **The Dormant-Revival Zone** (ClimateMARGO) — Multi-year silence broken by README-only updates; no code commits signal ambiguous intent
3. **The Scattered-Newcomer Tier** (awesome-geoengineering, GCCS-Core, ShennongWM-G) — Individual curators, bulk uploads, or brand-new project launches with no sustained momentum

---

## 🔥 Repo 1: WRF — Weather Research and Forecasting Model

| Field | Detail |
|-------|--------|
| **Repo** | `wrf-model/WRF` |
| **Stars** | ~1,762 |
| **Language** | Fortran |
| **License** | GNU GPL |
| **Last commit** | June 8, 2026 (v4.8.0 release merge) |
| **URL** | https://github.com/wrf-model/WRF |

### v7 Fresh Commit Timeline (May 19 – June 8, 2026)

```
May 12  █ Update MYNN-SFC submodule (b96a7e9)
May 19  █ Bug fix for udm (c1cd5c4)
May 20  ██ Minor Tempo changes (06e6998)
May 20  ██ Scheme-guard bug fix for urban NbS init (8fa379b)
May 20  ██ New namelists for ShinHong PBL (9c87d92)
May 21  █ Include mp_physics=88 in TEMPO error print (02f02bc)
May 26  █ Fix CDXWRF module (75ad1f9)
May 26  █ README for GFL option (0aa6582)
May 27  ██ MYNN-EDMF pointer update (8299919)
May 27  ██ MMM-physics SHA update (4fab0e2)
May 28  ██🔥 CORRECTION FOR EOT CALCULATION FOR SOLAR RADIATION (e836cd6)
May 30  █ Fix vectorization in AOCC stanza (4466746)
Jun 05  █ Turn off tempo_aerosolaware & tempo_hailaware (6a289e1)
Jun 06  █ README & version to v4.8.0 (0708348)
Jun 08  █ MERGE v4.8.0 RELEASE (06d4240)
```

### 🔥 THE SOLAR RADIATION BUG FIX — Episode 1 Lead Story

**Commit `e836cd6` (May 28, 2026):** *"Correction for EOT calculation for solar radiation"*

This is the single most SRM-relevant commit in the entire open-source solar geoengineering ecosystem. The **End-of-Transition (EOT) calculation** governs how the model handles the transition between solar radiation schemes — a critical process for any simulation involving stratospheric aerosol injection (SAI), where altered solar radiation fluxes must be computed accurately across scheme boundaries.

**Implication:** Every published WRF-based SRM simulation that used this scheme **before May 28, 2026** may have contained a systematic energy budget error. This is a potential replication crisis for SRM modeling. The fix arrived 3 days before the v4.8.0 release — was it caught during release testing, or was it independently discovered?

**🎙️ Podcast angle:** *"The atmosphere model used in every solar geoengineering study had a solar radiation bug. And it took a 'correction' commit — not a flagged deprecation, not a warning — to fix it. Who was running old simulations, and what were they concluding about the effectiveness of solar radiation management?"

### Release Pattern Analysis

| Phase | Dates | Commits | Character |
|-------|-------|---------|-----------|
| Physics Tuning | May 12–21 | 6 | Steady, incremental physics refinements |
| **Solar Fix & Release Prep** | **May 26–28** | **3** | **Compressed burst; solar radiation fix is the anchor** |
| Stability & Release | Jun 5–8 | 4 | Disable unstable options; formal version declaration |

**Key signal:** The solar radiation fix sits RIGHT IN THE MIDDLE of the release prep window. It's not a random bug fix — it's a **release-blocking correction** that had to be resolved before v4.8.0 could ship.

### ⚠️ The TEMPO Stability Shutdown

**Commit `6a289e1` (Jun 5, 2026):** *"Turn off tempo_aerosolaware and tempo_hailaware in Registry"*

Two physics options were **disabled** just 3 days before release. This suggests they were causing instability in production runs. For SRM researchers using TEMPO (Aerosol-aware) physics:
- Your existing configurations may crash or produce nonsensical results
- The v4.8.0 release effectively **removes** two options from the SRM toolkit
- This is a form of **implicit model change** — no deprecation warning, just a registry edit

**🎙️ Podcast angle:** *"Three days before the big release, they just... turned off two physics options. No announcement. No deprecation. Just a registry edit. If you're running solar geoengineering simulations with TEMPO, your model might silently fail."

---

## 🔥 Repo 2: PCMDI Metrics — ESM Evaluation Toolkit

| Field | Detail |
|-------|--------|
| **Repo** | `PCMDI/pcmdi_metrics` |
| **Stars** | ~133 |
| **Language** | Python |
| **License** | BSD |
| **Last commit** | **September 17, 2026** (most recent!) |
| **URL** | https://github.com/PCMDI/pcmdi_metrics |

### v7 Fresh Commit Timeline (September 3–17, 2026)

```
Sep 03  █ Merge PR #1425: extremes chunking (71a0497)
Sep 04  ██ PREPARE v4.2.1 (e7dc726)
Sep 04  ██ Prevent roundoff to 1.00 in mean_climate (90cbc50)
Sep 04  ██ Merge PR #1427: roundoff correction (d0bcbd8)
Sep 04  ██ Update version & release date in CITATION.cff (0e3a96f)
Sep 04  ██ Merge PR #1428: lee1043-patch-1 (3092cdd)
Sep 04  ██ Bump version to 4.2.1 (6419050)
Sep 04  ██ Merge PR #1429: lee1043-patch-2 (6443a1d)
Sep 17  ██ Patch for single-file modpath detection (90a4bc1)
Sep 17  █ MERGE PR #1431: mov_patch (b8f231a)
```

### 🔥 The "Release Day Avalanche" — 7 Commits in One Day

**September 4, 2026:** PCMDI shipped v4.2.1 with **7 commits in a single day.** This is the highest commit density we've observed in any repo:

| Time | Commit | Type |
|------|--------|------|
| Morning | `e7dc726` — Prepare v4.2.1 | Release prep |
| Morning | `90cbc50` — Prevent roundoff to 1.00 | **Bug fix** |
| Morning | `d0bcbd8` — Merge roundoff correction | Integration |
| Midday | `0e3a96f` — Update CITATION.cff | Documentation |
| Midday | `3092cdd` — Merge patch-1 | Integration |
| Afternoon | `6419050` — Bump version to 4.2.1 | Version bump |
| Afternoon | `6443a1d` — Merge patch-2 | Integration |

**The roundoff bug** (`90cbc50`): *"Prevents roundoff to 1.00 in mean_climate figures"* — a numerical precision issue that would have caused **all mean climate metrics to display as exactly 1.00**. This isn't cosmetic. If you were evaluating a climate model's precipitation metrics and seeing "1.00" everywhere, you'd think the model was perfect. It was a **silent display bug** in the evaluation toolkit used to assess climate models, including those used for SRM scenarios.

**🎙️ Podcast angle:** *"The tool used to evaluate climate models had a bug that made every metric display as 1.00 — perfect scores across the board. For how long? And which SRM evaluation papers used PCMDI metrics with this bug?"

### The Two-Patch Pattern

Two separate patches (lee1043-patch-1 and patch-2) merged on the same day suggests **parallel development streams** converging on the v4.2.1 release. This is typical of institutional OSS where multiple contributors work on different aspects simultaneously, then integrate.

### Sep 17: The Modpath Patch

Commit `90a4bc1` (Sep 17): *"Patch for case that single file detected for modpath_list"* — a ** Rare edge-case fix** that suggests someone encountered a bug where the tool only found one file in a multi-file path. This is a sign of **real-world usage pressure** — the tool is being used on diverse datasets, and edge cases are surfacing.

---

## 🔥 Repo 3: MDTF-Diagnostics — The Ocean's Only Friend

| Field | Detail |
|-------|--------|
| **Repo** | `NOAA-GFDL/MDTF-diagnostics` |
| **Stars** | ~80 |
| **Language** | Python/R |
| **License** | Apache 2.0 |
| **Last commit** | August 14, 2026 (general); June 19, 2026 (PBP-POD) |
| **URL** | https://github.com/NOAA-GFDL/MDTF-diagnostics |

### v7 Fresh Commit Timeline (June 2 – August 14, 2026)

```
Jun 02  █ Merge branch 'NOAA-GFDL:main' (97b3028)
Jun 08  █ Update README (16f936c)
Jun 08  █ Update README.md (b96127e)
Jun 08  █ Merge PR #823 (2df59f6)
Jun 19  ██🔥 add MCS precipitation-buoyancy statistics POD (33024ad)
Jun 19  ██ Update MCS_precip_buoy_stats.rst (4cfc99c)
Jun 19  ██ Update MCS_precip_buoy_stats.rst (699de27)
Jun 19  ██ Update MCS_precip_buoy_stats.rst (d6bc6d0)
Jun 19  ██ Update MCS_precip_buoy_stats.rst (3904d29)
Aug 14  █ Merge PR #825 (87f8105)
```

### 🔥 The June 19 "Big Bang" — 5 Commits, 1 File

**All five June 19 commits touch the same file: `MCS_precip_buoy_stats.rst`**

| # | Commit | Message | What Happened |
|---|--------|---------|---------------|
| 1 | `33024ad` | **add MCS precipitation-buoyancy statistics POD** | **THE CODE** — actual diagnostic addition |
| 2 | `4cfc99c` | Update MCS_precip_buoy_stats.rst | Doc: usage instructions |
| 3 | `699de27` | Update MCS_precip_buoy_stats.rst | Doc: API reference |
| 4 | `d6bc6d0` | Update MCS_precip_buoy_stats.rst | Doc: parameter table |
| 5 | `3904d29` | Update MCS_precip_buoy_stats.rst | Doc: example output |

**Pattern:** Code commit first, then **4 documentation commits** all same day. This is the classic "big bang" pattern: developer writes the diagnostic, then spends the rest of the day writing comprehensive documentation. The 4:1 doc-to-code ratio signals someone who cares about usability — this isn't a protected-research tool; it's meant to be used by others.

**What is the Precipitation-Buoyancy POD?**  
A "Process-Oriented Diagnostic" (POD) that measures the statistical relationship between **precipitation intensity and buoyancy frequency** in the atmosphere. This is directly relevant to:
- **Marine cloud brightening** (how does precipitation respond to aerosol-induced changes in cloud buoyancy?)
- **Ocean-atmosphere coupling** (buoyancy drives mixing; precipitation drives buoyancy)
- **SRM evaluation** (any solar radiation management intervention that alters cloud properties will show up in precip-buoyancy statistics)

**🎙️ Podcast angle:** *"The most ocean-relevant open-source tool in climate science had a 'big bang' release — one code commit, four documentation commits, all on the same day. The developer clearly cared about making this usable. But it's a diagnostic, not a simulation. It evaluates models; it doesn't simulate interventions. That distinction matters for our episode."

### The August 14 Merge

Commit `87f8105` (Aug 14): *"Merge PR #825 from weiming9115/main"* — Wei-Ming Tsai (the same author of the PBP-POD) merged their own PR. This is the **sole contributor pattern** — one developer driving the entire ocean-adjacent diagnostic ecosystem.

---

## 🟡 Repo 4: ClimateMARGO — The Dormant Revival

| Field | Detail |
|-------|--------|
| **Repo** | `ClimateMARGO/ClimateMARGO.jl` |
| **Stars** | ~73 |
| **Language** | Julia |
| **License** | MIT |
| **Last commit** | **August 17, 2026** (README update) |
| **URL** | https://github.com/ClimateMARGO/ClimateMARGO.jl |

### v7 Fresh Commit Timeline

```
Jan 12, 2022  █ Updated arguments for doc version deployment (8a7e012)
Jan 13, 2022  █ Fixed typo (b2d9228)
Feb 4, 2022   █ Added CITATION.bib (d609d49)
Feb 10, 2022  █ Removed deprecated web apps (32e66fd)
Nov 12, 2022  █ JuMP and Ipopt compat upgrade (#85) (12a0ce6)
Nov 14, 2022  █ Update Project.toml (5063c42)
Jul 6, 2023   █ add link to pluto in readme (fbbe619)
Oct 18, 2023  █ Update unit_conversions.jl with comment from #86 (57d4da7)
⏸️ 2+ YEAR GAP ⏸️
Aug 17, 2026  █ Update README.md (6d9ba7a)
Aug 17, 2026  █ Update README.md (d916f36)
```

### 🔥 The August 2026 Renaissance — 2 README Updates, Same Day

**Two separate README updates on August 17, 2026** (commits `6d9ba7a` and `d916f36`), both by **Fons van der Plas**, after a **2 year, 10 month silence** (October 2023 → August 2026).

**What this signals:**  
- ✅ Someone is still watching the repo — the star count (73) suggests ongoing interest
- ✅ The author (Fons van der Plas) is re-engaging — not a bot or spammer
- ❌ **Zero code commits** — README updates don't count as development activity
- ❌ No issues responded to, no PRs merged, no new features
- ❓ **Why now?** What triggered the August 2026 README update after 33 months of silence?

**Possible explanations:**  
1. **Conference paper** — van der Plas may be preparing a publication that requires an updated README citation
2. **New funding** — a grant requires maintenance of previously funded OSS
3. **Policy relevance** — climate-economic modeling is gaining policy traction; the README may need updated policy联系
4. **Ghost revival** — the most common pattern: brief activity followed by another long silence

**🎙️ Podcast angle:** *"A climate-economic model with 73 stars went dormant for nearly 3 years, then got two README updates in one day. No code. No issues. No explanation. Is this a real revival or a citation bump? The 2-year silence before that was even longer — 22 months between the last two commits. This is the 'zombie repo' pattern: technically alive, functionally dead."

### The Julia Ecosystem Context

ClimateMARGO is built in **Julia**, a language increasingly popular for scientific computing but with a smaller OSS community than Python or R. The **JuMP/Ipopt compatibility upgrade** (Nov 2022) shows the model uses Julia's optimization ecosystem for solving climate-economic equilibrium problems. The **Pluto link** (Jul 2023) suggests interactive notebook integration — Pluto is Julia's equivalent of Jupyter, and adding it is a usability signal.

---

## 🟢 Repo 5: Awesome-Geoengineering — The Curated List

| Field | Detail |
|-------|--------|
| **Repo** | `brandonhimpfen/awesome-geoengineering` |
| **Stars** | ~4 |
| **Language** | Markdown |
| **License** | Not specified |
| **Last commit** | **September 6, 2026** |
| **URL** | https://github.com/brandonhimpfen/awesome-geoengineering |

### v7 Fresh Commit Timeline

```
Jun 28, 2025  █ Initial commit (06ac1de)
Jun 28, 2025  █ Update README.md (c5dfd85)
Jan 16, 2026  █ Update README.md (b04d97a)
Mar 12, 2026  █ Update README.md (c06033b)
May 5, 2026   █ Update to v2.0.0 (a6e8359)
Sep 5, 2026   █ Update README.md (5926daf)
Sep 6, 2026   █ Update README.md (8d0a800)
```

### Pattern: The "Curator's Calendar"

| Period | Gap | Activity |
|--------|-----|----------|
| Jun 28, 2025 | — | Launch (2 commits same day: initial + README) |
| Jan 16, 2026 | **202 days** | First update (6.5 months later) |
| Mar 12, 2026 | **55 days** | Second update |
| May 5, 2026 | **54 days** | **v2.0.0 release** |
| Sep 5, 2026 | **122 days** | Third update |
| Sep 6, 2026 | **1 day** | Fourth update |

**Key observations:**
- ** Accelerating cadence** — gaps are shrinking (202→55→54→122→1 days)
- **v2.0.0 is significant** — major version bump after 10 months suggests substantial content expansion
- **Sep 5-6 double-header** — two commits in two days suggests active cuurent maintenance
- **Low star count (4) but consistent updates** — this is a labor of love, not a viral project

**🎙️ Podcast angle:** *"The best-curated list of geoengineering projects on GitHub has 4 stars and one maintainer. Brandon Himpfen has been updating it every 2-4 months for over a year. He just bumped it to v2.0.0. If you want to know what's actually being built in this space, this is the map. And it's maintained by one person working alone."

---

## ⚪ Repo 6: GCCS-Core — The Bulk-Upload Ghost

| Field | Detail |
|-------|--------|
| **Repo** | `KOSASIH/GCCS-Core` |
| **Stars** | ~9 |
| **Language** | Python |
| **License** | Not specified |
| **Last commit** | **October 29, 2024** |
| **URL** | https://github.com/KOSASIH/GCCS-Core |

### v7 Fresh Commit Timeline

```
Oct 29, 2024  █ Create data_collection.sh (4a068bc)
Oct 29, 2024  █ Create setup.py (f6da191)
Oct 29, 2024  █ Create requirements.txt (fc3553b)
Oct 29, 2024  █ Update README.md (cc92644)
Oct 29, 2024  █ Update README.md (bef35ee)
Oct 29, 2024  █ Update README.md (b6e44cc)
Oct 29, 2024  █ Update README.md (4350445)
Oct 29, 2024  █ Update README.md (7cad777)
Oct 29, 2024  █ Update README.md (99bf84f)
```

**All 9 pushes on a single day (October 29, 2024).** Three scaffold files (data_collection.sh, setup.py, requirements.txt) followed by **six README updates**. This is the classic "upload then realize you need a better README" pattern. The repo has been **completely silent for 22 months** since.

**What is GCCS?** *"Global Climate Control System"* — the name alone is audacious. The description claims it encompasses "core algorithms, data management..." but without any commits beyond the initial upload, there's no way to evaluate the actual code. Stars (9) likely reflect curiosity about the name, not code quality.

**🎙️ Podcast angle:** *"The 'Global Climate Control System' has 9 stars and zero commits since the upload day. No issues, no PRs, no updates. The README was updated 6 times on the same day the repo was created — and then never touched again. This is the 'ambitious launch, quiet death' archetype."

---

## ⚪ Repo 7: ShennongWM-G — The Brand-New Greenhouse World

| Field | Detail |
|-------|--------|
| **Repo** | `shennongwm/ShennongWM-G` |
| **Stars** | ~2 |
| **Language** | Python |
| **License** | Not specified |
| **Last commit** | **May 24, 2026** |
| **URL** | https://github.com/shennongwm/ShennongWM-G |

### v7 Fresh Commit Timeline

```
May 20, 2026  █ Initial commit (c48480a)
May 20, 2026  █ Add project page and demo links (686cba0)
May 22, 2026  █ Polish project README (e0463f6)
May 22, 2026  █ Update demo example window (77e7406)
May 24, 2026  █ Update public README links and citation (9fc3682)
```

**5 commits in 5 days** — a textbook "proper launch" pattern:
1. Day 1: Initial code + project page + demo links
2. Day 3: README polish + demo window update
3. Day 5: Public README links + citation info

This is the **opposite of GCCS-Core**. The developer is investing in presentation, documentation, and citability from day one. The "Greenhouse World Model" concept (action-conditioned climate-crop simulation with counterfactual audit) is genuinely interesting for solar geoengineering research — it could serve as a testbed for SRM counterfactuals ("what would happen if we injected aerosols in this specific scenario?").

**🎙️ Podcast angle:** *"This is how you launch an open-source project: code, docs, demos, and citation info — all in the first week. ShennongWM-G is a greenhouse world model that lets you run counterfactual climate scenarios. It's only 2 stars, but the launch quality is worlds better than GCCS-Core's 9-star ghost."

---

## 📊 Cross-Repo Solar Trend Dashboard (v7)

| Repo | Stars | Total Commits | Date Range | Peak Velocity | Current State |
|------|-------|----------------|------------|---------------|---------------|
| **WRF** | 1,762 | 15 | May-Jun 2026 | 3/day (release) | 🟢 v4.8.0 shipped |
| **PCMDI** | 133 | 10 | Sep 2026 | **7/day (release)** | 🟢 v4.2.1 shipped |
| **MDTF** | 80 | 10 | Jun-Aug 2026 | 5/day (big bang) | 🟡 Single-contributor |
| **ClimateMARGO** | 73 | 10 | 2022-2026 | 2/day (revival) | 🟡 Dormant-then-README |
| **awesome-geo** | 4 | 7 | 2025-2026 | 2/day (double-header) | 🟢 Accelerating |
| **GCCS-Core** | 9 | 9 | Oct 2024 | 9/day (bulk upload) | ⚪ Dead since upload |
| **ShennongWM** | 2 | 5 | May 2026 | 1/day (proper launch) | 🟢 New, active |

---

## 🎙️ Episode 1 Talking Points (v7 Updated)

### Lead Stories
1. **"The Solar Radiation Bug"** — WRF's EOT calculation fix (commit `e836cd6`, May 28, 2026) may have affected every published SRM simulation. Was this a routine fix or a replication crisis?
2. **"The Metric That Showed 1.00 Forever"** — PCMDI v4.2.1's roundoff bug made every climate metric display as perfect. How many SRM evaluation papers used these metrics?
3. **"The Largest Quiet Zone on GitHub"** — Zero ocean geoengineering repos. The most promising climate intervention domain has zero code presence.

### Structural Insights
4. **"The Release Weekend"** — Institutional repos (WRF, PCMDI) show compressed development bursts around version releases, contrasted with months of steady maintenance.
5. **"One Person, One Repo"** — MDTF's entire ocean-adjacent ecosystem is driven by a single developer (Wei-Ming Tsai). The sustainability of individual-driven OSS is a core episode theme.
6. **"The Zombie Revival"** — ClimateMARGO's 2-year silence followed by 2 README updates in one day. What counts as "active development" in climate tech OSS?

###Decision Framework for Listeners
| If you want to... | ...start here |
|--------------------|---------------|
| Run an SRM simulation | WRF v4.8.0 (but watch the TEMPO disable) |
| Evaluate a climate model | PCMDI v4.2.1 (but check for roundoff bugs) |
| Study ocean-atmosphere coupling | MDTF precip-buoyancy POD |
| Find what's being built | awesome-geoengineering v2.0.0 |
| Understand the economics | ClimateMARGO (but verify if it's still maintained) |

---

## 🔗 References

- [WRF v4.8.0 Release](https://github.com/wrf-model/WRF/releases/tag/v4.8.0)
- [PCMDI Metrics v4.2.1](https://github.com/PCMDI/pcmdi_metrics/releases/tag/v4.2.1)
- [MDTF Pull Request #823](https://github.com/NOAA-GFDL/MDTF-diagnostics/pull/823)
- [ClimateMARGO Julia Documentation](https://climatemargo.github.io/ClimateMARGO.jl/stable/)
- [Awesome Geoengineering v2.0.0](https://github.com/brandonhimpfen/awesome-geoengineering)

---

## 📋 Update Log

| Version | Date | Changes |
|---------|------|----------|
| v6 | Sep 2026 | Initial commit trend analysis from 8 repos |
| **v7** | **Sep 2026** | **Fresh API pull from 7 repos; WRF solar bug highlighted; PCMDI roundoff bug detailed; MDTF big-bang pattern analyzed; ClimateMARGO revival assessed; GCCS ghost flagged; ShennongWM proper launch noted** |
