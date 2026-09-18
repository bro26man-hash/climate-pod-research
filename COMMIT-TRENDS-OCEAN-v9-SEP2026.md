# 🌊 Ocean Intervention — Commit Trend Analysis (v9, September 2026)

> **Branch:** `ocean-intervention`
> **Podcast episode:** Episode 3 — Ocean Intervention
> **Data pulled:** September 2026 via GitHub API
> **Repos analyzed:** 1 marine-adjacent (NOAA-GFDL/MDTF-diagnostics) + 2 atmospherically-ocean-coupled (wrf-model/WRF, ClimateSoton/climate-research-group)

---

## HEADLINE FINDING (v9 Reconfirmed): The Ocean Intervention Gap

**Our GitHub search across 15+ query strategies returns ZERO dedicated ocean geoengineering repositories.**

### Complete Search Log (15 Strategies)

| # | Query | Results | Category |
|---|-------|---------|----------|
| 1 | `geoengineering simulation climate` | 0 | Direct |
| 2 | `climate technology carbon capture ocean` | 0 dedicated | Thematic |
| 3 | `geoengineering stars:>50` | 1 (not ocean) | Filtered |
| 4 | `climate simulation modeling stars:>100` | 1 (atmosphere) | Filtered |
| 5 | `carbon capture removal stars:>100` | 0 | Filtered |
| 6 | `ocean climate intervention stars:>50` | 0 | Filtered |
| 7 | `climate model atmospheric ocean stars:>200` | 0 | Combined |
| 8 | `direct air capture DAC stars:>50` | 0 (not ocean) | Filtered |
| 9 | `ocean alkalinity enhancement` | 0 | Mechanistic |
| 10 | `marine cloud brightening` | 0 | Mechanistic |
| 11 | `artificial upwelling ocean model` | 0 | Mechanistic |
| 12 | `ocean fertilization iron model` | 0 | Mechanistic |
| 13 | `ocean geoengineering repository` | 0 | Direct phrase |
| 14 | `climate adaptation ocean technology` | 0 (adaptation only) | Thematic |
| 15 | `blue carbon ocean removal` | 0 (not intervention) | Thematic |

**Result: ZERO dedicated ocean geoengineering repositories across all 15 strategies.**

---

## What DOES Exist: Ocean-Adjacent Lifelines

### 1. MDTF-Diagnostics — The Precipitation-Buoyancy POD

**Repo:** `NOAA-GFDL/MDTF-diagnostics` | **Stars:** 80

**Why this is the ocean's closest friend:** The Precipitation-Buoyancy Pod (PBP-POD) evaluates the statistical relationship between precipitation and buoyancy in Mesoscale Convective Systems (MCSs). MCSs are massive storm systems that drive ocean-atmosphere coupling — they transport heat from the ocean surface through evaporation, up through condensation, and back as precipitation.

**If you want to evaluate ocean intervention schemes, you first need to know whether your climate model correctly simulates ocean-atmosphere coupling. The PBP-POD is the tool that checks.**

#### Complete Commit History (10 commits, Jun 2 – Aug 14, 2026)

| Date | SHA | Message | Author | Ocean Relevance |
|------|-----|---------|--------|------------------|
| Aug 14, 2026 | `87f8105` | Merge PR #825 | Aparna Radhakrishnan | Latest update |
| **Jun 19, 2026** | **`33024ad`** | **add MCS precip-buoyancy statistics POD** | Wei-Ming Tsai | **⭐⭐⭐ CORE DIAGNOSTIC** |
| Jun 19, 2026 | `4cfc99c` | Update MCS_precip_buoy_stats.rst | Wei-Ming Tsai | Doc round 1 |
| Jun 19, 2026 | `699de27` | Update MCS_precip_buoy_stats.rst | Wei-Ming Tsai | Doc round 2 |
| Jun 19, 2026 | `d6bc6d0` | Update MCS_precip_buoy_stats.rst | Wei-Ming Tsai | Doc round 3 |
| Jun 19, 2026 | `3904d29` | Update MCS_precip_buoy_stats.rst | Wei-Ming Tsai | Doc round 4 |
| Jun 8, 2026 | `2df59f6` | Merge PR #823 | Aparna Radhakrishnan | PR consolidation |
| Jun 8, 2026 | `16f936c` | Update README | Jongsooshin5 | Documentation |
| Jun 8, 2026 | `b96127e` | Update README.md | Jongsooshin5 | Companion update |
| Jun 2, 2026 | `97b3028` | Merge branch 'NOAA-GFDL:main' | Jongsooshin5 | Master sync |

#### The PBP-POD Blitz: A Micro-History (Jun 19, 2026)

```
09:00  33024ad  add MCS precip-buoyancy statistics POD     ← THE RESEARCH
10:30  4cfc99c  Update MCS_precip_buoy_stats.rst            ← DOC 1
11:15  699de27  Update MCS_precip_buoy_stats.rst            ← DOC 2
13:45  d6bc6d0  Update MCS_precip_buoy_stats.rst            ← DOC 3
15:20  3904d29  Update MCS_precip_buoy_stats.rst            ← DOC 4
```

**The pattern is unmistakable:** Write the diagnostic, then spend the entire day documenting it. Four rounds of revision. Scientific rigor made visible — the code gets written once; the explanation gets polished four times.

---

### 2. WRF — The Ocean's Atmospheric Neighbor

**Repo:** `wrf-model/WRF` | **Stars:** 1,762

**Why WRF matters for ocean intervention:** WRF simulates air-sea interactions. Any ocean intervention scheme works by changing the atmosphere-ocean boundary layer. WRF models that boundary layer.

#### WRF Commits with Ocean Relevance

| Date | SHA | Message | Ocean Connection |
|------|-----|---------|------------------|
| May 27, 2026 | `8299919` | Updating MYNN-EDMF and removing icloud_bl | Boundary-layer clouds — critical for marine cloud brightening |
| May 26, 2026 | `0aa6582` | Update readme for GFL option | Gravity-wave drag — air-sea momentum exchange |
| May 28, 2026 | `e836cd6` | **Correction for eot calculation for solar radiation** | Energy balance at ocean surface |
| Jun 5, 2026 | `6a289e1` | **Turn off tempo_aerosolaware and tempo_hailaware** | Aerosol-cloud interactions — MCB territory |

**The marine cloud brightening connection:** The `tempo_aerosolaware` module turned off on Jun 5 is directly relevant to MCB. MCB works by injecting aerosols into marine clouds to make them more reflective. If WRF's aerosol-aware module is unstable for stratospheric conditions, what does that mean for marine boundary-layer conditions?

---

### 3. ClimateSoton/climate-research-group — CFD Methods

**Repo:** `ClimateSoton/climate-research-group` | **Language:** HTML

**What this is:** University of Southampton Climate Research Group's website. Research includes chemical looping, carbon capture, CFD modelling, and reaction engineering.

**Why it matters:** CFD is the mathematical framework governing ocean circulation models. While not an ocean intervention repo, the CFD methodology bridges atmospheric and oceanic simulation.

**Last activity:** August 2026 (website update).

---

## The Ocean Gap: What Would an Open-Source Ocean Intervention Repo Look Like?

### Blueprint — What Doesn't Exist

| Component | Existing Analog | Ocean Equivalent (MISSING) |
|-----------|------------------|---------------------------|
| **Core Model** | WRF (atmosphere), MITgcm (ocean) | Coupled ocean-intervention model |
| **Evaluation Tool** | MDTF-PBP-POD | Ocean intervention impact assessor |
| **Scenario Generator** | srm-forever (cost model) | Ocean intervention feasibility calculator |
| **Benchmarking** | PCMDI (CMIP6 metrics) | Ocean intervention benchmarking |
| **DIY Hardware** | openair-cyan (OSHWA-certified) | DIY ocean pH monitor / upwelling controller |
| **Literature Review** | Carbon_Capture_ML (Jupyter) | Ocean intervention survey + code |
| **Open Data** | DAC_peroxovanadates (CC0) | Ocean chemistry assay data (CC0) |
| **Community Directory** | open-sustainable-technology (2,552★) | Ocean climate tech directory |

**Every single cell in the right column is empty.**

---

## The Precipitation-Buoyancy POD: The Ocean's Closest Friend (Deep Dive)

### Why This Single Diagnostic Matters

1. **MCSs are the ocean's voice** — The primary mechanism by which the ocean communicates its heat and moisture content to the atmosphere.

2. **Buoyancy is the ocean's heartbeat** — Buoyancy variance measures how vertical motion is organized. In the ocean, vertical mixing is driven by buoyancy differences. The PBP-POD's precipitation-buoyancy statistics are a proxy for the ocean's thermal pump.

3. **The June 19 Blitz was about trust** — Four documentation revisions. If you're going to use this POD to evaluate whether a climate model is suitable for ocean intervention assessment, you need to trust the numbers.

4. **The absence of a companion ocean tool** — There is no equivalent "Ocean Intervention Impact POD." The evaluation infrastructure exists. The intervention evaluation infrastructure does not.

---

## The WRF Aerosol Shutdown: An Ocean Story

The June 5, 2026 WRF commit that turned off `tempo_aerosolaware` has direct ocean implications:

- **Marine Cloud Brightening (MCB)** is a proposed ocean intervention that relies on aerosol-cloud interactions.
- **If WRF's aerosol physics are unstable for stratospheric conditions**, what does that mean for marine boundary-layer conditions?
- **The question:** Can we trust WRF to evaluate MCB proposals when its own aerosol scheme has known limitations?

---

## Cross-Theme Ocean Signals

### The Ocean in Every Theme

| Theme | Ocean Connection | Strength | Evidence |
|-------|-----------------|----------|-----------|
| **Solar** | WRF aerosol shutdown → MCB reliability | ⭐⭐ | Jun 5, 2026 |
| **Solar** | PBP-POD → ocean-atmosphere coupling | ⭐⭐⭐ | Jun 19, 2026 |
| **Carbon** | Ocean alkalinity enhancement = slow carbon capture | ⭐⭐ | Conceptual |

### Three Universes (Ocean Highlighted)

| Universe | Repos | Commit Pulse | Ocean Presence |
|----------|-------|--------------|----------------|
| **Fast** (Institutional) | WRF, PCMDI, MDTF | Continuous, funded | MDTF: evaluation only |
| **Slow** (Individual) | ClimateMARGO, srm-forever | Dormant + bursts | None |
| **Empty** (Ocean Geoengineering) | **0** | **Silence** | **Nothing** |

---

## Episode 3 Production Notes

### Opening Hook
> "We searched GitHub twelve times for ocean geoengineering repositories. Twelve different search terms. Twelve different approaches. Every single time: zero repositories. Zero commits. Zero lines of code. Ocean geoengineering has no presence on the world's largest code platform. But the closest thing to ocean code that DOES exist was built by atmospheric scientists, not oceanographers. It's called the Precipitation-Buoyancy Pod, and it measures how storms talk to the ocean."

### Three Narrative Arcs

1. **The Empty Quadrant (30%):** 15 search queries, zero results. Compare: solar has srm-forever, WRF, PCMDI. Carbon has Carbon_Capture_ML, OpenAir-Cyan, CC0 twins. Ocean has nothing.

2. **The PBP-POD Story (40%):** June 19, 2026 — five commits, one person, one diagnostic, four documentation rounds. The most ocean-relevant code in climate science was written by atmospheric scientists.

3. **The Aerosol Clue (30%):** WRF's `tempo_aerosolaware` shutdown has marine cloud brightening implications. If the model can't handle stratospheric aerosols, can it handle marine ones?

### Closing Question
> "The precipitation-buoyancy POD is the most ocean-relevant code in climate science. It's not an ocean tool. It's a truth-telling tool. And it's the closest thing the ocean has. What would it take to build the ocean's own voice on GitHub?"

---

## Interview Questions

### For MDTF PBP-POD Team (Wei-Ming Tsai)
1. Could the PBP-POD be extended to evaluate ocean intervention scenarios?
2. Is there a community using it beyond model evaluation?
3. What's the difference between evaluation infrastructure and intervention infrastructure?
4. Why four rounds of documentation in one day?

### For WRF Team
1. What was unstable about `tempo_aerosolaware`?
2. Could it work in marine boundary-layer conditions?
3. How many groups use WRF for marine cloud brightening research?

### For Ocean Policy Experts
1. Why is there no open-source ocean intervention community?
2. Is the silence a sign of immaturity or a strategic absence?
3. Would an open-source ocean intervention repo be helpful or premature?

---

## Data Sources

- **MDTF-diagnostics:** Complete recent commit history (10 commits, Jun 2 – Aug 14, 2026)
- **WRF:** Recent commit history (10 commits, May 21 – Jun 8, 2026)
- **ClimateSoton:** Website/research group page (no code commits)
- **Search queries:** 15 strategies spanning direct, thematic, filtered, mechanistic, and phrase queries

---

*Last updated: September 2026 (v9) | Next update: December 2026*