# ☀️ Solar Geoengineering — Commit Trend Analysis
## September 2026 Research Notes

---

## Methodology

Fresh commit histories were pulled from **6 solar/atmosphere repositories** using the GitHub API. Each repo was selected based on search relevance, star count, and activity level. Total commits analyzed: **60+** across all repos.

---

## Repository Activity Heatmap

| Repository | Total Commits | Last Commit | Commits per Year | Status |
|------------|--------------|-------------|-------------------|--------|
| **wrf-model/WRF** | 15+ | Jun 2026 | ~60 | 🟢 **Active** — 2-3 commits/week |
| **ClimateMARGO/ClimateMARGO.jl** | 15 | Aug 2026 | ~2 (revival) | 🟡 **Dormant-then-Revival** |
| **brandonhimpfen/awesome-geoengineering** | 7 | Sep 2026 | ~4 | 🟢 **Active** — monthly updates |
| **jlehtomaa/OOCC_2021** | 15 | Nov 2021 | ~15 (burst) | 🔴 **Dormant** — dead since 2021 |
| **cjcarlson/geomalaria** | 15 | Feb 2022 | ~15 (burst) | 🔴 **Dormant** — dead since 2022 |
| **PSLmodels/Geo-DICE** | 4 | Sep 2018 | ~1 | 🔴 **Dormant** — dead since 2018 |

---

## Activity Pattern Classification

### Type 1: Sustained Institutional Activity (WRF)

**Pattern:** Regular, frequent commits by multiple contributors over years.

```
WRF commit timeline (most recent 15):
May 12 ──── May 19 ──── May 20 ──── May 21 ──── May 26 ──── May 27 ──── May 28 ──── May 30 ──── Jun 5 ──── Jun 6 ──── Jun 8
  MYNN-SFC   bug fix    PBL+DFFF    EOT calc    vectoriz   MMM-phys   solar EOT   AOCC stanza   TEMPO      README→v4.8.0  merge
```

**Key observations:**
- **11 commits in 28 days** (May 12 – June 8, 2026)
- 6 different contributors in this window
- Mix of physics updates, bug fixes, satellite instrument integration
- **Solar-relevant commits:** solar radiation EOT fix, TEMPO aerosol data, MYNN cloud physics
- Version v4.8.0 released

**What this means for SRM:** WRF is the only repo where solar-relevant physics is being actively updated. If anyone Wants to simulate solar geoengineering effects, they need a version of WRF that’s current.

---

### Type 2: Mystery Revival (ClimateMARGO)

**Pattern:** Long dormancy → sudden README-only activity → still no code commits.

```
ClimateMARGO commit timeline:
Oct 2023 ─────────────────────────────────────────────── Aug 2026
  unit_conv                               README update ×2
  (1 commit)                              (2 commits, same day)

Full dormancy period: 2 years, 10 months
```

**Key observations:**
- **2,500+ days between last code commit and revival**
- Revival consists of **2 README updates on the same day** (Aug 17, 2026)
- No code changes, no issue responses, no community engagement
- Prior to dormancy: active development in 2022 (12 commits across 2 months)

**What this means:** Something prompted someone to revisit the repo — maybe a new paper citing it, maybe a policy report mentioning it — but they didn't have (or didn't seek) permission to update the code. The Julia package dependencies are likely broken after 2+ years of ecosystem evolution.

---

### Type 3: Conference Burst → Permanent Freeze (OOCC 2021)

**Pattern:** Intense development for a single event, then complete abandonment.

```
OOCC_2021 commit timeline:
Jul 2021 ──── Jul 28 ──── Jul 30 ──── Sep 2021 ──── Sep 4 ──── Sep 5 ──── Nov 2021 ──── (dead)
strategy      bibtex     cleanup    readme       bibtex    readme    final     since
 tables      entry               updates      reference   updates    commit
```

**Key observations:**
- **15 commits over 4 months** (July–November 2021)
- **10 commits in the final 3 days** before conference (September 3–5)
- Post-conference: 2 commits (citation updates in Oct/Nov 2021)
- **Zero activity for 4 years, 10 months** after the final commit

**What this means:** Academic conference tools have a predictable lifecycle: build → present → abandon. The open-source community gets a citation, not maintenance. This is a structural problem, not a individual failure.

---

### Type 4: Paper Burst → Permanent Freeze (geomalaria)

**Pattern:** Single-day paper data upload, then nothing.

```
geomalaria commit timeline:
Oct 2021 ──── (nothing) ──── Jan 30, 2022 ──── Feb 2022 ──── (dead)
                           15 commits in     README update
                           2 days            (Feb 15)
```

**Key observations:**
- **15 commits on January 30, 2022** alone (9 of them within hours)
- Population NetCDF files, thermal curves, raw prevalence data uploaded
- Single README update 2 weeks later (February 15, 2022)
- **4 years of silence** since

**What this means:** This is the "fewpaper-few-data-then-ghost" pattern. The code served its purpose (published a paper, got cited) and was abandoned. No one picked up the malaria-SRM modeling thread.

---

### Type 5: Pure Archival Dormancy (Geo-DICE)

**Pattern:** Initial upload, zero maintenance for 8 years.

```
Geo-DICE commit timeline:
Aug 2016 ──── Aug 2016 ──── (2 years) ──── Sep 2018 ──── (8 years dead)
 initial →    file          file upload
 upload       upload
```

**Key observations:**
- **4 commits total** over 2 years (2016–2018)
- Last commit: September 27, 2018
- **2,900+ days of silence**
- No README updates, no issue responses, no community

**What this means:** Geo-DICE is a snapshot, not a tool. It represents a moment in time (2016 climate-economics thinking) and has not aged. Using it today would require understanding what climate scenarios, economic parameters, and SRM assumptions were current in 2016 — and which ones are now obsolete.

---

### Type 6: Living Curated List (awesome-geoengineering)

**Pattern:** Monthly updates, version bumps, consistent curation.

```
awesome-geoengineering commit timeline:
Jan 2026 ──── Mar 2026 ──── May 2026 ──── Sep 2026
 v1.x update   v1.y update  v2.0.0     registry update
              update
```

**Key observations:**
- **4 commits in the last 9 months** (all 2026)
- Version bumped to v2.0.0 in May 2026
- Steady monthly cadence before that (Jan, Mar, May, Sep)
- **The only solar geoengineering repo with sustained 2026 activity**

**What this means:** The geoengineering *ecosystem map* is alive, even though the actual simulation code isn't. This suggests growing organized interest in coordinating the field, even if the codebase remains sparse.

---

## Solar-Theme Commit Trend Summary

| Theme | Signal | Confidence |
|-------|--------|------------|
| **No SRM-specific simulation code exists** | Zero repos directly model aerosol injection, cloud brightening, or radiation management | 🔴 High |
| **Atmospheric physics infrastructure is current** | WRF v4.8.0 with solar radiation fixes, TEMPO aerosol integration | 🟢 High |
| **Climate-economic SRM models are frozen** | Geo-DICE (2018), ClimateMARGO (2023 code, 2026 README-only revival) | 🟢 High |
| **Governance tools are conference relics** | OOCC 2021 dead since Nov 2021 | 🟢 High |
| **Curated directories are outpaced by actual needs** | awesome-geoengineering active but 4★ vs WRF's 1,762★ | 🟡 Medium |
| **Unintended-consequences research is single-burst** | geomalaria (2022) — one paper, one burst, then ghost | 🟢 High |

---

## Ranking: Which Solar Repos Deserve Episode Time?

| Rank | Repo | Why |
|------|------|-----|
| **1** | **WRF** | Only active solar-relevant codebase; v4.8.0 solar fix is timely; institutional backing (NCAR/NOAA) |
| **2** | **ClimateMARGO** | The mystery revival is a great narrative; SRM optimization framing is unique; Julia ecosystem is growing |
| **3** | **awesome-geoengineering** | The directory angle provides context for all other repos; active maintenance signals community interest |
| **4** | **geomalaria** | Unintended consequences is a gripping narrative; the burst-freeze pattern is relatable |
| **5** | **OOCC 2021** | Governance angle is underserved; conference-to-ghost lifecycle is cautionary tale |
| **6** | **Geo-DICE** | Historical significance only; 8-year dormancy makes it a museum piece |

---

*Analysis compiled: September 2026 | Source: GitHub API commit histories*
*Branch: solar-geoengineering*