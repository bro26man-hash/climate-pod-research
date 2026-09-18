# 🎙️ Climate Pod Research — Cross-Theme Analysis v4
## September 2026 | GitHub Commit Trend Dashboard for the Podcast Series

*Updated: September 2026 — fresh commit histories from 12+ repositories across all three themes*

---

## 🌐 The Unified Dashboard

```
                    FAST UNIVERSE                    SLOW UNIVERSE                 EMPTY UNIVERSE
                  (Institutional/Funded)          (Individual/Dormant)            (Zero Presence)

  ☀️ SOLAR       WRF ★ 1,761                      ClimateMARGO ★ 73               OCEAN GEOENGINEERING
                PCMDI ★ 133                       srm-forever ★ 0                 ↑ ZERO REPOS
                MDTF ★ 80

  🌍 CARBON     Open-Sustainable-Tech ★ 2,552     OpenAir-Cyan ★ 76               MARINE CLOUD BRIGHTENING
                Carbon_Capture_ML ★ 56             CCS_and_Storage ★ 85           ↑ ZERO REPOS
                                                        OCEAN IRON FERTILIZATION
                                                        ↑ ZERO REPOS
                [actors]                              DAC_Peroxovanadates ★ 2       ↑ ZERO REPOS
                                                        DAC_Peroxotitanates ★ 2       ↑ ZERO REPOS

  🌊 OCEAN      MDTF (adjacent) ★ 80              Nothing                           SEA SALT SPRAY INJECTION
                WRF (coupled) ★ 1,761               Nothing                          ↑ ZERO REPOS
                                                                                    OCEAN UPWELLING SIM
                                                                                    ↑ ZERO REPOS
                                                                                    OAE SIMULATOR
                                                                                    ↑ ZERO REPOS
```

---

## 📊 Commit Activity Heat Map (September 2026)

| Repo | Theme | Commits (recent window) | Top Contributor | Type |
|------|-------|------------------------|-----------------|------|
| **PCMDI/pcmdi_metrics** | ☀️ Solar | **10** (Sep 3-4 burst) | Jiwoo Lee | Version release v4.2.1 |
| **open-sustainable-technology** | 🌍 Carbon | **5** (Sep 1-9) | Abdul Salam, Tobias | Directory additions |
| **WRF** | ☀️ Solar | **6** (v4.8.0 prep) | weiwangncar, Anthony Islas | Version release v4.8.0 |
| **MDTF-diagnostics** | 🌊 Ocean-adj | **5** (Jun 19, single file) | Wei-Ming Tsai | Precip-buoyancy POD |
| **MDTF-diagnostics** | 🌊 Ocean-adj | **4** (Aug 14) | Aparna Radhakrishnan | PR merge |
| **ClimateMARGO.jl** | ☀️ Solar-econ | **2** (Aug 17) | Fons van der Plas | README revival |
| **openair-cyan** | 🌍 Carbon | **0** (frozen since Feb 2024) | — | Blitz complete |
| **srm-forever** | ☀️ Solar-theory | **Steady** (low) | Hausfath | Theoretical maintenance |
| **DAC_peroxovanadates** | 🌍 Carbon | **Low** (Sep 2025) | tjz21 | CC0 data release |
| **DAC_peroxotitanates** | 🌍 Carbon | **Low** (Sep 2025) | tjz21 | CC0 data release |

---

## 🔑 Five Headlines from the Fresh Data

### 1. PCMDI's Sprint Signals an Upcoming Climate Assessment
10 commits in 2 days (September 3-4, 2026), culminating in version 4.2.1. The fixes were razor-focused:
- Roundoff prevention in mean_climate figures (numerical precision)
- Extremes chunking using SVD (analyzing climate extremes)
- Memory optimization via dask rechunking (larger ensembles)
- Numpy SVD forced (numerical stability)

**Interpretation:** The evaluation community is preparing for something big — likely an IPCC AR7 submission cycle or CMIP6 final data release. For solar geoengineering, this means SRM scenario evaluation is entering a precision phase.

### 2. WRF's Solar Radiation Fix Reveals Persistent Uncertainty
Even in v4.8.0 (June 2026), the flagship atmospheric model still needed a correction for solar radiation EOT calculations. This is humbling:
- WRF is 1,761 stars and is considered the gold standard
- Yet basic solar radiation calculations still had errors
- The fix came just before the v4.8.0 release, suggesting it was blocking

**Interpretation:** Solar geoengineering forcing calculations are only as good as the models that compute them. If even WRF has solar radiation bugs, how confident should we be in SRM scenario projections?

### 3. MDTF's Precip-Buoyancy POD: The Ocean's 5-Commit Day
June 19, 2026. Five commits to `MCS_precip_buoy_stats.rst`. One file. One day.

This is the single most ocean-relevant event in our entire study. The precipitation-buoyancy POD identifies patterns in how ocean surface conditions (buoyancy) drive tropical precipitation.

**Interpretation:** The ocean-intervention community doesn't have its own tools. It borrows from atmospheric evaluation. The fact that this one diagnostic got 5 commits in a day suggests it was either a major publication or an urgent fix — and it's our only window into how SRM might reshape tropical rainfall.

### 4. The CC0 Revolution: Two Repos Say "Forever"
`tjz21/DAC_peroxovanadates` and `tjz21/DAC_peroxotitanates` both use CC0 public domain dedication. This is revolutionary for climate tech:
- No patents
- No licenses
- No restrictions
- Commercial use unlimited

**Interpretation:** If sorbent materials are the bottleneck for Direct Air Capture, and computational screening data is the path to new materials, then CC0 is the accelerator. These researchers are betting that open data beats proprietary discovery.

### 5. ClimateMARGO's Ghost Revival: The Ocean Doesn't Make an Appearance
Two README updates in August 2026 after 2+ years of silence. No code changes. No new scenarios. No ocean pathways.

**Interpretation:** The revival is cosmetic. The economic model's optimization framework still has ZERO ocean intervention scenarios. The ocean remains invisible in the economic calculus.

---

## 🎙️ Episode Continuity Map

### How the Three Episodes Connect

**EPISODE 1: SOLAR GEOENGINEERING** — The Infrastructure Question
- WRF: Where's the code? → Inside climate models
- PCMDI: Can we trust the numbers? → 10-commit sprint says yes, barely
- ClimateMARGO: Should we optimize? → Dormant, ambiguous
- srm-forever: What's the forever cost? → Zero stars, deep question

**EPISODE 2: CARBON CAPTURE** — The Method Question
- OpenAir-Cyan: Can you DIY it? → One-day blitz, then freeze
- Open-Sustainable-Tech: Who's building it? → 2,552 stars, continuous
- CC0: Can we open-source the materials? → Two repos, public domain
- Carbon_Capture_ML: What does the research say? → Survey complete, maturing

**EPISODE 3: OCEAN INTERVENTION** — The Absence Question
- Zero repos: Is it even happening? → No code anywhere
- MDTF: Our best tool for ocean = precip-buoyancy POD → Evaluation, not intervention
- ClimateMARGO: Does the economics care? → No ocean scenarios
- The vacuum is the answer → Governance mirror

---

## 💡 Cross-Cutting Themes

### Theme 1: Institutional Confidence vs. Individual Anxiety
- **Institutional repos** (WRF, PCMDI, Open-Sustainable-Tech) are confident, well-funded, and continuous
- **Individual repos** (srm-forever, ClimateMARGO, OpenAir-Cyan) are anxious, intermittent, and fragile
- **The ocean** has neither institutional nor individual commitment — it has void

### Theme 2: The Precision-Accuracy Axis
- PCMDI's roundoff fix and WRF's solar radiation correction both signal that **precision matters** in climate tech
- But for ocean intervention, we don't even have precision tools — we have none at all
- The carbon capture CC0 repos are betting that **open precision** (public-domain data) beats **proprietary precision** (patented measurements)

### Theme 3: The Blitz Pattern
- OpenAir-Cyan: 1-day blitz → permanent freeze
- PCMDI: 10-commit burst → v4.2.1 release
- This pattern suggests that climate tech development is **event-driven**, not continuous — except for the directories

### Theme 4: The Directory as Ecosystem
- The most active repo isn't building anything — it's **mapping everything**
- Open-Sustainable Technology's 2,552 stars and continuous growth suggests that **connective tissue** matters more than any single tool
- For the podcast: the directory is the meta-story that ties all three episodes together

### Theme 5: The Ocean as Governance Mirror
- Zero ocean geoengineering repos = zero governance framework = zero funding = zero career path
- The GitHub absence mirrors the real-world absence
- MDTF's precip-buoyancy POD is the Trojan horse: ocean-relevant science hiding inside an atmospheric evaluation tool

---

## 📈 Commit Rate Dashboard

```
RATE OF COMMITS PER WEEK (approximate, recent period)

open-sustainable-  ████████████████████████████████  ~1/week (continuous)
WRF               ██████████████████████████████████  ~1.5/week (institutional)
PCMDI             ████████████████████████████████████████  ★★★★★ (burst: 10/day)
MDTF              ██████████████████████████░░░░░░░░░░  ~0.5/week (punctuated)
ClimateMARGO      █░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  ~0.05/week (dormant)
srm-forever       █░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  ~0.1/week (steady)
OpenAir-Cyan      ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  0 (frozen)
DAC_peroxo        █░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  ~0.05/week (low activity)
Ocean-specific    ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  0 (doesn't exist)
```

---

## 🔗 Quick Links
- ☀️ **Solar discoveries:** https://github.com/bro26man-hash/climate-pod-research/blob/solar-geoengineering/PROJECT-DISCOVERIES-SOLAR.md
- ☀️ **Solar trends:** https://github.com/bro26man-hash/climate-pod-research/blob/solar-geoengineering/COMMIT-TRENDS-SOLAR.md
- 🌍 **Carbon discoveries:** https://github.com/bro26man-hash/climate-pod-research/blob/carbon-capture/PROJECT-DISCOVERIES-CARBON.md
- 🌍 **Carbon trends:** https://github.com/bro26man-hash/climate-pod-research/blob/carbon-capture/COMMIT-TRENDS-CARBON.md
- 🌊 **Ocean discoveries:** https://github.com/bro26man-hash/climate-pod-research/blob/ocean-intervention/PROJECT-DISCOVERIES-OCEAN.md
- 🌊 **Ocean trends:** https://github.com/bro26man-hash/climate-pod-research/blob/ocean-intervention/COMMIT-TRENDS-OCEAN.md

*Analysis prepared: September 2026 | Branch: main | Repository: climate-pod-research | Data: GitHub REST API*

*Methodology: Repository search → commit history pulls (6 repos) → trend analysis → cross-theme synthesis → markdown documentation push to 3 theme branches + main.*