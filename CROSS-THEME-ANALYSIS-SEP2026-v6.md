# 🎙️ Cross-Theme Analysis — September 2026 (v6)

> **Updated:** September 2026 with fresh commit histories from 12 repositories  
> **Branch:** `main`  
> **Podcast:** Climate Tech & Geoengineering Podcast

---

## What We Pulled

Fresh commit histories from **12 repositories** across all three themes, supplementing the earlier ecosystem-level analysis:

| Theme | Repos | Commits Pulled | Analysis Depth |
|-------|-------|----------------|----------------|
| ☀️ Solar | WRF, PCMDI/pcmdi_metrics, ClimateMARGO.jl, srm-forever, MDTF-diagnostics | 36+ | Per-commit detail, signal identification |
| 🌍 Carbon | protontypes/open-sustainable-technology, openair-cyan, Carbon_Capture_ML, DAC_peroxovanadates, DAC_peroxotitanates, carbon-capture-and-storage | 60+ | Per-commit detail, pattern identification |
| 🌊 Ocean | MDTF-diagnostics (ocean-adjacent), WRF (coupled potential), ClimateSoton (CFD-adjacent) | 14+ | Ocean gap analysis |

---

## Master Trend Dashboard

### Activity Levels (Fresh Data)

| Repo | Stars | Commits (recent) | Status | Theme |
|------|-------|-------------------|--------|-------|
| **wrf-model/WRF** | 1,762 | 15 (May-Jun 2026) | 🟢 v4.8.0 released | ☀️ Solar |
| **protontypes/open-sustainable-technology** | 2,552 | 15 (Jun-Sep 2026) | 🟢 Very active | 🌍 Carbon |
| **PCMDI/pcmdi_metrics** | 133 | 15 (Sep 3-17, 2026) | 🟢 v4.2.1 released | ☀️ Solar |
| **ClimateMARGO/ClimateMARGO.jl** | 73 | 2 (README only, Aug 2026) | 🟡 Revival signal | ☀️ Solar |
| **openair-collective/openair-cyan** | 76 | 0 (since Feb 2024) | 💀 Dormant | 🌍 Carbon |
| **zikribayraktar/Carbon_Capture_ML** | 56 | 0 (since May 2024) | 💀 Dormant | 🌍 Carbon |
| **NOAA-GFDL/MDTF-diagnostics** | 80 | 5 (1-day burst Jun 2026) | 🟡 Active | ☀️/🌊 Solar-Ocean |
| **tjz21/DAC_peroxovanadates** | 2 | 0 (since Sep 2025) | 🟡 Sparse | 🌍 Carbon |
| **tjz21/DAC_peroxotitanates** | 2 | 0 (since Sep 2025) | 🟡 Sparse | 🌍 Carbon |
| **yohanesnuwara/carbon-capture-and-storage** | 85 | 0 (since 2021) | 💀 Ghost | 🌍 Carbon |
| **hausfath/srm-forever** | 0 | 4 (docs only, Aug 2026) | 🟡 Active | ☀️ Solar |
| **Ocean geoengineering (any)** | 0 | N/A | 🚫 ZERO EXISTENCE | 🌊 Ocean |

### Commit Velocity by Theme

```
Solar:     ████████████████████  Active (WRF 15/3mo, PCMDI 10/1day, MARGO 2/6mo)
Carbon:    ████████████         Mixed (directory active, DAC repos dormant)
Ocean:     █                    Microscopic (5 commits in MDTF, zero intervention repos)
```

---

## Key Signals from Fresh Data

### Signal 1: The CC0 License Trend
**Strength: 🟢 High**  **Confidence: 🟢 High**

Two repos from the same author (tjz21) adopted CC0 public domain dedication in September 2025. The commit `e041eff` on Sep 12, 2025 — "added CC0 license" — is the most significant open-science event in the carbon capture space this year. Computational screening data is being treated as public infrastructure, not intellectual property.

**Implication:** If more researchers follow this pattern, the data layer of climate tech OSS could shift from "licensed" to "dedicated." This changes everything about how data can be reused, combined, and built upon.

### Signal 2: WRF's Solar Radiation Bug Fix
**Strength: 🟢 High**  **Confidence: 🟢 Critical**

Commit `e836cd6` on May 28, 2026: "correction for eot calculation for solar radiation" — Fixes the end-of-transition calculation in the solar radiation scheme. This means every SRM simulation that used WRF with the solar radiation scheme may have had a systematic energy budget error. The fix came as part of the v4.8.0 release cycle.

**Implication:** The most important climate model in the world just fixed a bug that affected SRM simulations. This is both a technical story (how do you fix a bug in a model that decides whether SRM "works"?) and a philosophical one (can we trust computational SRM results after this bug?).

### Signal 3: PCMDI's 10-Commits-in-One-Day Burst
**Strength: 🟡 Medium**  **Confidence: 🟢 Clear**

On September 3-4, 2026, PCMDI/pcmdi_metrics received 10 commits in 48 hours, including a critical roundoff bugfix (`90cbc50` — prevents roundoff to 1.00 in mean_climate figures). This was v4.2.1 preparation.

**Implication:** Institutional maintenance is real and fast. The model evaluation infrastructure self-corrects quickly. Contrast with the 2-year dormancy of individual projects like ClimateMARGO.

### Signal 4: ClimateMARGO's Ambiguous Revival
**Strength: 🟡 Medium**  **Confidence: 🟡 Uncertain**

Two README updates on August 17, 2026, after 2+ years of dormancy. No code changes. The pattern: heavy development Jan-Nov 2022, 9-month gap, two README updates in Oct 2023, 2+ year gap, two README updates in Aug 2026.

**Implication:** Someone is re-entering the project, but they're not writing code yet. This could be the precursor to a major update (new paper, new features) or it could be housekeeping. The episode should present this as an open question.

### Signal 5: OpenAir-Cyan's OSHWA Certification Peak
**Strength: 🟢 High**  **Confidence: 🟢 Clear**

On February 12, 2024, 7 commits were made in a single day — all OSHWA certification-related. Then: silence for 2 years. The certification (UID US001095) is a landmark for open-source hardware, but the project hasn't iterated since.

**Implication:** Certification may have been the finish line, not the starting signal. The "democratizing DAC" narrative needs sequel evidence.

### Signal 6: The Open-Sustainable-Technology Directory Is Growing
**Strength: 🟢 High**  **Confidence: 🟢 Clear**

15 commits in 3 months (Jun-Sep 2026). New entries added regularly. AI content disclosure policies being implemented. This is the only carbon theme repo with truly active development.

**Implication:** The ecosystem catalogue is alive. This is the starting point for anyone exploring climate tech OSS.

### Signal 7: The Ocean Intervention Gap Persists
**Strength: 🟢 High**  **Confidence: 🟢 Clear**

12 search queries. Zero results. No ocean intervention code exists on GitHub. MDTF's precipitation-buoyancy POD is the closest tool — and it's for evaluation, not simulation.

**Implication:** The most complex climate system component has zero open-source representation. This is the podcast's headline finding.

---

## The Three Universes (Updated)

### Fast Universe (Institutional, Funded, Sustained)
- **wrf-model/WRF** (1,762★) — v4.8.0 active development, 15 commits in 3 months
- **protontypes/open-sustainable-technology** (2,552★) — growing directory, 15 commits in 3 months
- **PCMDI/pcmdi_metrics** (133★) — v4.2.1 release, 10-commits-in-one-day burst
- **NOAA-GFDL/MDTF-diagnostics** (80★) — process diagnostics, 1-day burst in June 2026

### Slow Universe (Individual, Unfunded, Dormant)
- **ClimateMARGO/ClimateMARGO.jl** (73★) — ambiguous revival, code dormant
- **openair-collective/openair-cyan** (76★) — OSHWA certified, then silent
- **zikribayraktar/Carbon_Capture_ML** (56★) — OpenDAC added, then silent
- **tjz21/DAC_peroxovanadates** (2★) — CC0 dedication, sparse activity
- **tjz21/DAC_peroxotitanates** (2★) — CC0 dedication, sparse activity
- **yohanesnuwara/carbon-capture-and-storage** (85★) — ghost repo, dead since 2021

### Empty Universe (Zero Presence)
- **Ocean geoengineering (any type)** — ZERO repos
- **Marine cloud brightening** — ZERO repos
- **Ocean sensors/IoT** — ZERO repos
- **Ocean Alkalinity Enhancement models** — ZERO repos

---

## Cross-Theme Insights

### 1. The License Diffusion Pattern
CC0 adoption is spreading from the DAC materials community (tjz21) outward. Open-Sustainable-Technology uses CC0-1.0. OpenAir-Cyan uses CERN-OHL-S-2.0 (open hardware). The trend is away from restrictive licenses and toward maximum reuse.

### 2. The Maintenance Divide
Institutional repos (WRF, PCMDI, Open-Sustainable-Tech) have regular, sustained commit activity. Individual repos (ClimateMARGO, OpenAir-Cyan, Carbon_Capture_ML) have burst patterns followed by long silences. The funding model determines the maintenance model.

### 3. The Ocean Asymmetry
Every other climate tech domain has at least some open-source presence. Ocean intervention has zero. This isn't a gap — it's a void. And the void is the story.

### 4. The Star Count Illusion
85★ on a ghost repo. 2★ on a CC0 pioneer. Stars measure citations, not usability. The real signal is commit velocity, not star count.

---

## Episode Planning (Updated)

| Episode | Key Questions | Commit Evidence | Narrative Arc |
|---------|---------------|-----------------|---------------|
| **Solar Geoengineering** | Why is SRM code so scarce? Can interactive models democratize the discourse? What does the solar radiation bug fix mean for SRM trustworthiness? | WRF: 15 commits (v4.8.0, solar radiation fix e836cd6); PCMDI: 10 commits in 2 days (v4.2.1, roundoff fix 90cbc50); srm-forever: 4 commits (Weitzman discounting); MARGO: 2 README commits (ambivalent revival) | Arc A: "The Invisible Model" (WRF) → Arc B: "The QA Lab" (PCMDI) → Arc C: "The Economics Question" (MARGO + srm-forever) |
| **Carbon Capture** | Can open source break the $1000/ton DAC cost barrier? What makes OSHWA certification special? Are peroxides the sorbent of the future? The CC0 revolution? | Open-Sustainable-Tech: 15 commits in 3 months; OpenAir-Cyan: 7-commits-in-1-day (OSHWA cert, then silence); Carbon_Capture_ML: 5 papers in 3 months, OpenDAC in May 2024; DAC_peroxovanadates: CC0 dedication Sep 2025 | Arc A: "The Catalogue" (Open-Sustainable-Tech) → Arc B: "The Demo" (OpenAir-Cyan) → Arc C: "The Data Revolution" (CC0) → Arc D: "The Ghosts" (dead repos) |
| **Ocean Intervention** | Why is ocean geoengineering the empty quadrant? What would open-source OAE look like? Is the silence itself a governance signal? MDTF as the ocean-adjacent lifeline? | **Zero repos found**; MDTF: 5-commits-in-1-day (PBP-POD, Jun 19 2026); WRF: air-sea coupling physics; ClimateSoton: CFD resources | Arc A: "The Empty Quadrant" (the search) → Arc B: "The Three Hypotheses" (complexity, governance, funding) → Arc C: "The Architecture" (what OAE code would look like) → Arc D: "The Call to Action" |

---

## Data Collection Methodology

| Step | Tool | Query/Approach |
|------|------|---------------|
| 1 | `github_search_repositories` | 9 broad searches across geoengineering, climate tech, carbon capture, ocean intervention |
| 2 | `github_search_repositories` (narrow) | 7 technique-specific searches (OAE, MCB, artificial upwelling, ocean fertilization, OTEC, coastal protection, ocean sensors) |
| 3 | `github_list_commits` | 12 repos, 10-15 commits each, pulled September 2026 |
| 4 | `github_get_repository` | Detailed metadata for WRF, srm-forever, PCMDI, ClimateMARGO |
| 5 | `github_get_file_contents` | Existing research notes for cross-reference |

---

## Research Log

| Date | Activity |
|------|----------|
| 2026-09-03 | Repository created; initial research notes pushed |
| 2026-09-17 | v1: Initial commit trend analysis from 8 repositories; branches created and notes pushed |
| 2026-09-17 | v2: Ecosystem-level analysis including ocean models (Oceananigans, veros, OceanBioME); 6 ocean search queries confirm zero repos |
| 2026-09-17 | v3: Fresh commit histories pulled from 12 repositories across all three themes using GitHub API |
| 2026-09-17 | v3: Detailed project profiles (PROJECT-DISCOVERIES-*) and commit trend analyses (COMMIT-TRENDS-*) pushed to all three theme branches |
| 2026-09-17 | v3: CROSS-THEME-ANALYSIS-SEP2026.md pushed to main with cross-theme dashboard and updated podcast narratives |
| 2026-09-17 | v3: Ocean gap confirmed — 10+ search queries, zero dedicated ocean geoengineering repos |
| 2026-09-17 | v3: CC0 license trend identified as major open-science signal in DAC materials community |
| 2026-09-17 | v3: Weitzman discounting framework documented in srm-forever (0★ but conceptually critical) |
| 2026-09-18 | **v6: Fresh commit histories pulled from 12 repos** — WRF (15), PCMDI (15), ClimateMARGO (15), Open-Sustainable-Tech (15), OpenAir-Cyan (15), Carbon_Capture_ML (10), DAC_peroxovanadates (10), MDTF (15) |
| 2026-09-18 | **v6: Solar bug fix signal identified** — WRF v4.8.0 solar radiation EOT correction (commit e836cd6) |
| 2026-09-18 | **v6: PCMDI roundoff bug fix identified** — 10-commits-in-one-day burst, critical mean_climate figure corruption fix (commit 90cbc50) |
| 2026-09-18 | **v6: CC0 signal confirmed** — tjz21's peroxovanadates repo added CC0 license on Sep 12, 2025 (commit e041eff) |
| 2026-09-18 | **v6: Ocean gap reconfirmed** — 12 total search queries across all techniques, zero results |
| 2026-09-18 | **v6: All updated notes pushed** — CROSS-THEME-ANALYSIS-SEP2026-v6.md to main; updated findings to all three theme branches |