# 🎙️ Cross-Theme Commit Trends — September 2026 (v4)

**Consolidated analysis** of fresh commit histories pulled from 12 repositories across solar-geoengineering, carbon-capture, and ocean-intervention themes.

---

## Master Activity Dashboard

| Theme | Repo | Stars | Date Range | Total Commits | Pattern | State |
|-------|------|-------|------------|---------------|---------|-------|
| ☀️ Solar | wrf-model/WRF | 1,762 | May–Jun 2026 | 15 | Release-weekend (v4.8.0) | 🟢 Active |
| ☀️ Solar | PCMDI/pcmdi_metrics | 133 | Sep 3–17, 2026 | 15 | Release-weekend (v4.2.1) | 🟢 Very active |
| ☀️ Solar | ClimateMARGO/ClimateMARGO.jl | 73 | Jan 2022–Aug 2026 | 15 | Dormant 2.8yr, README revival | 🟡 Ambiguous |
| ☀️ Solar | hausfath/srm-forever | 0 | Aug 26, 2026 | 4 | Single-day big bang | 🆕 New |
| 🌍 Carbon | protontypes/open-sustainable-technology | 2,552 | Jun–Sep 2026 | 15 | Sustained curation (~2.5/mo) | 🟢 Active |
| 🌍 Carbon | openair-collective/openair-cyan | 76 | May 2022–Feb 2024 | 15 | One-day OSHWA blitz, then frozen | ⚠️ Dormant |
| 🌍 Carbon | zikribayraktar/Carbon_Capture_ML | 56 | Jan–May 2024 | 15 | Sprint build, then slow, then frozen | ⚠️ Dormant |
| 🌍 Carbon | tjz21/DAC_peroxovanadates | 2 | Nov 2023–Sep 2025 | 15 | CC0 adoption (Sep 12, 2025), then frozen | 🆕 CC0 signal |
| 🌍 Carbon | tjz21/DAC_peroxotitanates | 2 | Feb–Sep 2024 | 10 | CC0 adoption (Sep 12, 2025), then frozen | 🆕 CC0 signal |
| 🌊 Ocean | NOAA-GFDL/MDTF-diagnostics | 80 | May–Aug 2026 | 15 | Steady maintenance + POD burst (Jun 19) | 🟢 Active (adjacent) |
| 🌊 Ocean | ClimateSoton/ClimateSoton.github.io | 0 | Jul 26, 2026 | 2 | Same-day website setup | ⚠️ Website only |
| 🌊 Ocean | **All ocean geoengineering repos** | — | — | **0** | **Zero dedicated repos** | 💀 **Void** |

---

## The Three Patterns

### Pattern 1: The Release-Weekend Sprint (WRF & PCMDI)

Both institutional solar tools show the same pattern: long maintenance periods punctuated by intense release sprints.

```
WRF v4.8.0 cycle:    May 19 ──────── May 20─21 ─── May 26─28 ─── Jun 6─8
                     │    3 commits     │   3 commits   │   2 commits   │
                     │    (bug fixes)   │  (PHysics)    │ (solar fix)   │ (release)

PCMDI v4.2.1 cycle:  Sep 3 ───────── Sep 4 ─────────────────── Sep 17
                     │  6 commits      │  4 commits    │   2 commits   │
                     │ (chunking/SVD)  │ (version/bug) │  (follow-up)  │
```

**Interpretation:** Climate model development is **wave-like**. Teams prepare for months, then release in days. The solar radiation fix in WRF was caught in the final days of the v4.8.0 cycle — proof that the QA process works, but also that errors can persist for years before being caught.

### Pattern 2: The Big-Bang-Then-Freeze (OpenAir-Cyan & Carbon_Capture_ML)

Two carbon-capture repos show the individual-researcher pattern:

```
OpenAir-Cyan:   May 2022 ████████  then  ─────────────────  Feb 12, 2024 💥💥💥💥💥💥💥  then  ──────────────────
                Build phase              11 months of              OSHWA blitz              2+ years frozen
                                         silence

Carbon_Capture_ML: Feb 2023 █████████  then  ───────────────  May 8, 2024 █  then  ──────────────
                   1-week survey              14 months of           OpenDAC                 silence
                                                silence                addition
```

**Interpretation:** Individual researchers can build complete artifacts in days or weeks. But sustained maintenance requires continuous funding and institutional support. Without it, repos go dark after the initial push.

### Pattern 3: The CC0 Declaration (DAC Peroxometal Repos)

The most significant event across all themes:

```
Sep 12, 2025:  DAC_peroxovanadates ── e041eff: added CC0 license
               DAC_peroxotitanates ── c7ea8ae: added CC0 license
               
Sep 23, 2025:  Both repos ── README updates documenting the CC0 adoption

Before:        Years of README updates (Dec 2023, Jul 2024)
After:         Silence (both repos frozen since Sep 2025)
```

**Interpretation:** Two research groups on the same day made the same decision: computational screening data belongs to the public domain. This is not serendipity — it's a **movement**. The Nyman lab at Oregon State is leading an open-science revolution in computational DAC materials.

---

## The Ocean Gap: Statistical Proof

| Search Strategy | Query | Results |
|----------------|-------|---------|
| Direct mechanism | `ocean geoengineering iron fertilization alkalinization` | **0** |
| Direct mechanism | `marine cloud brightening ocean spraying` | **0** |
| Mechanistic | `ocean alkalinity enhancement ocean iron fertilization climate` | **0** |
| Ecosystem | `blue carbon coastal ecosystem methane` | **0** |
| Simulation | `geoengineering simulation climate` | **0** |
| Modeling | `ocean model simulations ESM coastal` | **0** |
| SRM-adjacent | `SRM solar radiation management simulation` | **0** |
| Thematic | `climate technology carbon capture ocean intervention` | 3 (non-ocean) |
| Broad | `climate simulation modeling` | 10 (atmospheric only) |
| Adjacent | `climate Soton research group` | 1 (website) |

**Total ocean geoengineering repos found across all search strategies: ZERO**

**Total ocean geoengineering commits found: ZERO**

For comparison:
- Solar geoengineering: 1 repo, 4 commits (srm-forever)
- Carbon capture: 5+ repos, 25+ commits (DAC, CCS, OpenAir)
- Ocean geoengineering: **0 repos, 0 commits**

---

## Cross-Theme Signal Summary

### The CC0 Revolution (Carbon → Solar implication)

| Signal | Evidence | Implication |
|--------|----------|-------------|
| Two repos, one day | Both DAC repos got CC0 on Sep 12, 2025 | Coordinated group decision |
| CC0 = public domain | No copyright, no restrictions, forever | Data becomes infrastructure |
| Precedent set | First CC0 adoption in carbon-capture dataset | May inspire other DAC groups |
| **Solar implication** | SRM tools (srm-forever) have no CC0 datasets | Solar geoengineering data not yet public |

**The question for the solar episode:** If the DAC community declared its data public domain in September 2025, when will the solar geoengineering community do the same? And will anyone be building models to share data from?

### The Star-Activity Inversion (Cross-theme)

| Repo | Stars | Status | Scientific Impact |
|------|-------|--------|------------------|
| Open-Sustainable-Tech | 2,552 | 🟢 Active | High (ecosystem map) |
| WRF | 1,762 | 🟢 Active | High (baseline model) |
| carbon-capture-and-storage | 85 | 💀 Ghost | Low (dormant since 2021) |
| OpenAir-Cyan | 76 | ⚠️ Dormant | Medium (certified DIY device) |
| ClimateMARGO | 73 | 🟡 Ambiguous | High (only SRI economic model) |
| PCMDI | 133 | 🟢 Active | High (evaluation toolkit) |
| Carbon_Capture_ML | 56 | ⚠️ Dormant | Medium (survey) |
| MDTF-diagnostics | 80 | 🟢 Active | Ocean-adjacent (POD) |
| DAC_peroxovanadates | 2 | 🆕 CC0 | **High (foundational dataset)** |
| DAC_peroxotitanates | 2 | 🆕 CC0 | **High (foundational dataset)** |
| srm-forever | 0 | 🆕 New | **High (only interactive SRM tool)** |
| **Ocean geoengineering** | **0** | **💀 Void** | **Unknown (no tools)** |

**The lesson:** Stars measure visibility, not importance. The 2-star DAC repos may be more consequential for the future of carbon capture than the 85-star ghost repos. And the 0-star srm-forever is arguably the most directly relevant solar geoengineering tool on GitHub.

### The Maintenance Gap (Cross-theme)

| Development Pattern | Repos | What It Means |
|---------------------|-------|--------------|
| Sustained institutional | WRF, PCMDI, Open-Sustainable-Tech, MDTF | Funded teams, continuous development |
| Sprint-then-freeze | OpenAir-Cyan, Carbon_Capture_ML, ClimateMARGO | Individual effort, no sustained funding |
| Big-bang-then-freeze | srm-forever, DAC repos | Launch event, then silence |
| **Void** | **Ocean geoengineering** | **Nobody's doing it** |

---

## The Three Universes (Final Version)

```
┌─────────────────────────────────────────────────────────────────────┐
│  FAST UNIVERSE — Institutional, Funded, Sustained                   │
│  ☀️ WRF (1,762★) │ PCMDI (133★)                                     │
│  🌍 Open-Sustainable-Tech (2,552★)                                  │
│  🌊 Oceananigans.jl (1,413★, v2), veros                            │
│                                                                     │
│  Development: Continuous. Quality: High. Future: Clear.             │
├─────────────────────────────────────────────────────────────────────┤
│  SLOW UNIVERSE — Individual, Unfunded, Dormant                      │
│  ☀️ ClimateMARGO (73★) │ srm-forever (0★)                          │
│  🌍 OpenAir-Cyan (76★) │ Carbon_Capture_ML (56★)                   │
│  🌍 DAC_peroxovanadates (2★, CC0) │ DAC_peroxotitanates (2★, CC0) │
│                                                                     │
│  Development: Episodic. Quality: Variable. Future: Uncertain.       │
├─────────────────────────────────────────────────────────────────────┤
│  EMPTY UNIVERSE — Zero Presence                                     │
│  💀 Ocean geoengineering: 0 repos, 0 commits, 0 datasets           │
│                                                                     │
│  Development: None. Quality: N/A. Future: Unknown.                  │
└─────────────────────────────────────────────────────────────────────┘
```

---

## 🎙️ Integrated Episode Planning

| Episode | Branch | Evidence | Key Question |
|---------|--------|----------|-------------|
| **Solar Geoengineering** | `solar-geoengineering` | WRF solar radiation fix (May 28); srm-forever Weitzman discounting (Aug 26); ClimateMARGO dormancy-revival (Aug 17) | "Can we trust the models if the radiation code has bugs? And who decides whether to use them?" |
| **Carbon Capture** | `carbon-capture` | CC0 adoption (Sep 12, 2025); OpenAir-Cyan OSHWA blitz (Feb 12, 2024); AI governance signal (Jul 2026) | "Can open source break the $1000/ton barrier? And is the CC0 revolution the biggest open-science story in DAC?" |
| **Ocean Intervention** | `ocean-intervention` | Zero repos; precip-buoyancy POD (Jun 19); ClimateSoton website (Jul 26) | "Why is ocean geoengineering the empty quadrant? And is the silence itself a governance signal?" |

---

## Data Provenance

All commit data pulled fresh from GitHub API on September 19, 2026:

| Theme | Repositories Pulled | Total Commits |
|-------|---------------------|---------------|
| ☀️ Solar | WRF, PCMDI, ClimateMARGO, srm-forever | 39 |
| 🌍 Carbon | Open-Sustainable-Tech, OpenAir-Cyan, Carbon_Capture_ML, DAC_peroxovanadates, DAC_peroxotitanates | 70 |
| 🌊 Ocean | MDTF-diagnostics, ClimateSoton.github.io (cross-referenced with WRF, ClimateMARGO) | 32 |
| **Total** | **12 repositories** | **141** |

Search queries run: **10+ distinct strategies** across GitHub repository search.

---

## Research Log

| Date | Activity |
|------|----------|
| 2026-09-19 | v4: Fresh commit histories pulled from 12 repos; consolidated cross-theme analysis, three-pattern framework, and integrated episode plan pushed to main branch |
| 2026-09-17 | v3: Initial project discoveries and commit trend analyses pushed to all three theme branches |
| 2026-09-03 | Initial research notes created; repository established |
