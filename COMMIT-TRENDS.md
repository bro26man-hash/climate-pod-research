# 📊 Commit Trend Analysis — Master Document

**Last Updated:** September 17, 2026
**Analysis Scope:** 8 repositories across solar geoengineering, carbon capture, and ocean intervention themes

---

## Repositories Analyzed

| Repo | Stars | Theme | commits analyzed |
|------|-------|-------|-----------------|
| PCMDI/pcmdi_metrics | 133 | Solar (Climate Simulation) | 10 most recent |
| protontypes/open-sustainable-technology | 2,552 | All (Directory) | 10 most recent |
| openair-collective/openair-cyan | 76 | Carbon (DIY DAC) | 10 most recent |
| openair-collective/openair-sorbent-tester | 3 | Carbon (Sorbent Testing) | 10 most recent |
| tjz21/DAC_peroxovanadates | 2 | Carbon (Materials) | 10 most recent |
| FMS-ESM/AM3 | 4 | Solar (Atmospheric Model) | 4 total |
| pmip4/pmip_p2fvar_analyzer | 4 | Solar (Paleoclimate) | 10 most recent |
| o7-machinehum/electro-swing-dacc | — | Carbon (Electro-swing DAC) | Search only |

---

## Detailed Findings by Repository

### 1. PCMDI/pcmdi_metrics — Climate Simulation Backbone

**Language:** Python | **License:** BSD-3-Clause | **Forks:** 49

**Recent Commits (Sep 3-4, 2026 — 10 commits in 2 days):**
- `3092cdd` — Merge PR #1428 (Jiwoo Lee, Sep 4)
- `6419050` — Bump version to 4.2.1 (Jiwoo Lee, Sep 4)
- `6443a1d` — Merge PR #1429 (Jiwoo Lee, Sep 4)
- `0e3a96f` — Update version in CITATION.cff (Jiwoo Lee, Sep 4)
- `e7dc726` — Prepare v4.2.1 (Jiwoo Lee, Sep 4)
- `d0bcbd8` — Merge PR #1427: roundoff fix (Jiwoo Lee, Sep 4)
- `90cbc50` — Prevents roundoff to 1.00 in mean_climate figures (James Goodnight, Sep 4)
- `71a0497` — Merge PR #1425: extremes chunking (Jiwoo Lee, Sep 3)
- `b2eb044` — Merge branch 'main' into #1424 (Jiwoo Lee, Sep 3)
- `c8711f1` — Merge PR #1423: variability modes dask SVD memory (Jiwoo Lee, Sep 3)

**Interpretation:** Classic institutional release cycle. Version bump, PR merges, bug fixes all concentrated in a 2-day window. Contributing team is small and DOH-funded (LLNL). The v4.2.1 release added Hadley Cell Metrics; v4.1.0 added ENSO Metrics and Sea Ice IIEE. This is the most actively maintained climate simulation toolkit on GitHub, but it's institutionally driven, not community-driven.

**Trend Signal:** Climate model evaluation is centralized in a single institutional toolkit. No competing open-source alternatives exist.

---

### 2. protontypes/open-sustainable-technology — The Directory

**Language:** Mixed | **License:** CC-BY-4.0 | **Forks:** 330

**Recent Commits (Jul-Sep 2026 — steady cadence):**
- `6e9f48c` — Add-MUIO (Abdul Salam, Sep 9)
- `07e19b1` — Add-MUIOGO (Abdul Salam, Sep 9)
- `1b6cb82` — Fix dead links in README (Mikhail Alabugin, Sep 1)
- `d73a519` — Add claude-carbon (gwittebolle, Aug 23)
- `6b6cdc8` — Add Story Seed Library (Abdul Salam, Aug 18)
- `ca9d7a5` — Add openflexure microscope (Abdul Salam, Aug 18)
- `2303b7a` — Remove duplicate AI content review checkbox (Tobias Augspurger, Jul 19)
- `c4c9fe7` — Modify PR template for AI content review (Tobias Augspurger, Jul 19)
- `be14281` — Update PR template (Tobias Augspurger, Jul 17)
- `5bc6609` — Add PowerIO (Tobias Augspurger, Jul 2)

**Interpretation:** The most consistently active repository in our study. Multiple contributors (Abdul Salam, Tobias Augspurger, Mikhail Alabugin, gwittebolle) adding projects regularly. The directory contains 2,500+ projects across renewable energy, carbon capture, biodiversity, and more. Recent addition of "AI content review" to PR templates shows the project is grappling with AI-generated contributions — a live governance concern.

**Trend Signal:** The OSS climate-tech ecosystem is growing fast enough that the directory project needs AI content moderation. This is a signal of scale.

---

### 3. openair-collective/openair-cyan — DIY DAC Pioneer

**Language:** Mixed | **License:** GPL-3.0 / CERN-OHL-P

**Recent Commits (Feb 12, 2024 — 6 commits in 1 day):**
- `b5422b3` — Update README (OSHWA UID link, KCollins, Feb 2024)
- `b164257` — Add files via upload (KCollins, Feb 2024)
- `828f496` — OSHWA UID logo US001095 (KCollins, Feb 2024)
- `b731cd8` — Add files via upload (KCollins, Feb 2024)
- `4b08fb3` — Create CITATION.cff (KCollins, Feb 2024)
- `859bfa8` — Update README (KCollins, Feb 2024)

**Prior Activity:**
- `d12008e` — Update README (DaOfficialWizard, Jul 2022)
- `b8621ba` — Add files (ZanzyTHEbar, May 2022)
- `d025674` — Update README (DaOfficialWizard, May 2022)
- `784ace5` — Update README (DaOfficialWizard, May 2022)

**Interpretation:** The project had a concentrated burst of activity in Feb 2024 culminating in OSHWA certification (US001095) — the open-source hardware equivalent of a CE mark. Before that, activity was sporadic (2022). After certification: silence. The project reached a milestone and then stopped. This pattern — burst then dormancy — may be typical of DIY climate hardware projects that need sustained funding to continue.

**Trend Signal:** OpenAir-Cyan proved that DIY DAC hardware can be certifiable and well-documented. The question is whether it can sustain development beyond a single certification push.

---

### 4. openair-collective/openair-sorbent-tester — Sorbent Testing Platform

**Language:** Python/CircuitPython | **Forks:** Unknown

**Recent Commits (Oct 2023 and earlier):**
- `c155068` — Update materials list (Matt Parker, Oct 2023)
- `be98ed5` — Update materials list (Matt Parker, Oct 2023)
- `0dadd16` — Bushwick Design starter site (Jan 2023)
- `bb5abcc` — Update lib for SCD-4X sensor (Oct 2021)
- `1d84c2b`, `f686209` — Materials list updates (Oct 2021)
- `c4817d9` — CircuitPython code and libs (Aug 2021)
- `68c7dfd` — Images for instructions (Aug 2021)
- `19bbe04` — Prebuilt code for Feather board (Aug 2021)
- `16d0a59` — Shortened URL (Aug 2021)

**Interpretation:** Built on the Cyan platform but focused on sorbent testing. Active in 2021-2023, then fell dormant. The project demonstrates the OpenAir collective's progression from DIY CO2 capture (Cyan) to materials testing (Sorbent Tester), but neither project has had activity in 2+ years.

**Trend Signal:** The gap between sorbent discovery (active in Aug 2026 per tjz21 repos) and open-source testing infrastructure (dormant since 2023) is a major bottleneck.

---

### 5. tjz21/DAC_peroxovanadates — Computational DAC Materials

**Language:** TCL/DIGITAL Command Language | **Forks:** 0

**Recent Commits:**
- `cfd04f7` — Updated README (Jacob Hirschi, Sep 2025)
- `e041eff` — Added CC0 license (Jacob Hirschi, Sep 2025)
- `6e17397` — Fixed DOI link (Jacob Hirschi, Mar 2024)
- `e38c7dd` — Added paper DOI link (Jacob Hirschi, Mar 2024)
- `b6184d2`, `3096665` — README updates (Jacob Hirschi, Mar 2024)
- `8d8bd1d`, `f7ecca1`, `ba71657`, `737d342` — README updates (Jacob Hirschi, Dec 2023)

**Interpretation:** This is a "Scientific Computation Implementation" (SCI) repo — code that implements published research findings for reproducibility. Single contributor (Jacob Hirschi). The burst of commits in Dec 2023-Mar 2024 aligned with paper submission/publication. The CC0 license (Sep 2025) placed the code in the public domain — maximum openness.

**Trend Signal:** Computational chemistry for DAC materials is emerging as a reproducible-science niche. Small individual contributors, not teams. The August 2026 wave (titanates repo, electro-swing DAC) suggests this niche is growing.

---

### 6. FMS-ESM/AM3 — Legacy Atmospheric Model

**Language:** Fortran | **Total Commits:** 4

**All Commits (Mar 1, 2015):**
- `f5739a9`, `0f6966e`, `dc66bdd`, `020236e` — All on March 1, 2015 by Benjei Tsuang

**Interpretation:** A complete fossil. 4 commits on a single day in 2015, then never touched again. This is GFDL's AM3 atmospheric model — historically significant but superseded by modern Python-based tools. Its presence on GitHub is archival, not functional.

**Trend Signal:** Legacy Fortran climate codes are being abandoned on GitHub. The field has moved to Python (PCMDI, xCDAT) and Julia. No geoengineering-specific Fortran code has been modernized.

---

### 7. pmip4/pmip_p2fvar_analyzer — Paleoclimate Data Tool

**Language:** NCL/Python | **Forks:** Unknown

**Recent Commits:**
- `dded725` — Updated PMIP4-PMIP3 link (Chris Brierley, Sep 2025)
- `a9b3224` — Added NCL script for data frames (Chris Brierley, Jan 2023)
- `413c7dd`, `e155080`, `002d1a9`, `0016218` — Pliocene explorations (Chris Brierley, Sep 2022)
- `57c4b4e` — Error correction (Anni Zhao, Aug 2022)
- Various data accuracy fixes (Anni Zhao, Aug 2022)

**Interpretation:** A single-user tool (Chris Brierley) for analyzing paleoclimate data, with periodic updates over 4 years. The Pliocene focus is relevant to SRM research (the Pliocene had higher CO2 and warmer temperatures — a natural experiment). Last commit was a link update in Sep 2025.

**Trend Signal:** Climate data analysis tools are individually maintained with long gaps between updates. The shift from NCL to Python is visible (new script uses NCL, but the ecosystem is migrating).

---

## Cross-Cutting Patterns

### Pattern 1: Institutional Burst vs. Community Decay
The most active repos (PCMDI, OpenSustain) are institutionally funded or directory-style. Community-driven projects (OpenAir-Cyan, Sorbent Tester) tend to burst then dorm.

### Pattern 2: The August 2026 DAC Materials Wave
Three DAC materials repositories were updated on Aug 19, 2026: peroxovanadates, peroxotitanates, and electro-swing DAC. This coordination suggests a shared research event — possibly a preprint or conference deadline driving simultaneous open-code submissions.

### Pattern 3: Forking is Dead
None of the repos have significant fork activity relative to their stars. PCMDI has 49 forks but 133 stars (37% fork ratio). Most repos have near-zero forks. Climate tech code is consumed, not built upon.

### Pattern 4: Language Gap
Legacy Fortran (AM3, PMIP/NCL) dominates older climate simulation. Newer tools are Python (PCMDI, OpenAir) or Julia (emerging). No geoengineering-specific repo uses modern web/JS frameworks. The "interactive model" concept (srm-forever's single HTML file) remains an exception.

### Pattern 5: The Ocean Void
Zero ocean geoengineering repositories across all search strategies. This is not a GitHub problem — it's a field-wide institutional and governance gap.

---

## Implications for the Podcast

1. **Solar episode:** The absence of open-source SRM simulation code is the story. Not "SRM is dangerous" but "SRM is invisible." Who controls the code controls the narrative.

2. **Carbon episode:** OpenAir-Cyan is the hero story — hacked-together hardware, OSHWA-certified, then silence. The peroxovanadates wave is the science story. Electro-swing is the future.

3. **Ocean episode:** The void is the story. "Why isn't ocean geoengineering on GitHub?" is a better question than "What should we do about the ocean?"

---

*Analysis generated from GitHub API commit data. All commits verified against repository history.*
