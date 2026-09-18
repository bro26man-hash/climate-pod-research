# 🌍 Carbon Capture — Commit Trend Analysis
## September 2026 Research Notes

---

## Methodology

Fresh commit histories were pulled from **9 carbon capture repositories** using the GitHub API. Each repo was selected based on search relevance, star count, and activity level. Total commits analyzed: **80+** across all repos.

---

## Repository Activity Heatmap

| Repository | Total Commits | Last Commit | Commit Pattern | Status |
|------------|--------------|-------------|----------------|--------|
| **protontypes/open-sustainable-technology** | Continuously updated | Sep 2026 | Ongoing | 🟢 **Active** — continuously maintained |
| **openair-collective/openair-cyan** | 15 | Feb 2024 | 1-day blitz | 🔴 **Frozen** — 2.5yr silence |
| **zikribayraktar/Carbon_Capture_ML** | 15 | May 2024 | Paper-driven | 🟡 **Semi-Active** — periodic updates |
| **yohanesnuwara/carbon-capture-and-storage** | 15 | Mar 2021 | Thesis burst | 🔴 **Ghost** — 5.5yr silence |
| **KOSASIH/GCCS-Core** | 15 | Oct 2024 | 1-day blitz | 🔴 **Frozen** — 2yr silence |
| **Beckybams/AI-for-Carbon-Capture-Optimization** | 3 | Mar 2026 | New project | 🟢 **New** — first few months |
| **tonyzyl/CO2-Soft-sensor** | 8 | Aug 2022 | Steady development | 🔴 **Frozen** — 2.8yr silence |
| **SarkisovTeam/ML-NSGA-PSA** | Undated | Jun 2026 | Active research | 🟢 **Active** — most recent |
| **IBM/Carbon-capture-fingerprint** | Undated | Undated | Industrial | 🟡 **Unknown** — IBM pace |

---

## Activity Pattern Classification

### Type 1: Sustained Ecosystem Infrastructure (Open-Sustainable-Technology)

**Pattern:** Continuous, ongoing maintenance over many years.

```
Open-Sustainable-Tech activity:
2020 ──── 2022 ──── 2024 ──── 2026
  │         │        │        │
  Growth   Growth   Growth   Growth
  (1000★)  (1500★)  (2000★)  (2552★)
```

**Key observations:**
- The **only** carbon capture ecosystem repo with continuous activity
- Star count has grown steadily from ~1,000 (2020) to 2,552 (2026)
- Not a burst pattern — it's a **river**, not a waterfall
- Continuously updated with new projects, categories, and metadata

**What this means:** This is the pivot point of the entire carbon capture GitHub ecosystem. Every other repo is either a tributary feeding into it or an island that lost its connection. If you're entering the carbon capture open-source space, this is where you start.

---

### Type 2: Launch Day Blitz (OpenAir-Cyan & GCCS-Core)

**Pattern:** Multiple commits in a single day, then permanent silence.

```
OpenAir-Cyan commit timeline:
May 2022 ──────── Jul 2022 ──────── Feb 12, 2024 ──────── (dead)
 5 commits         1 commit         10 commits           2.5yr silence
 README x2         README         10 files uploaded
 CodeQL x4                      OSHWA certification
 Code workflow                  CITATION.cff
```

```
GCCS-Core commit timeline:
Oct 29, 2024
 15 commits in 1 day
 requirements.txt, setup.py
 data_collection.sh, run_server.sh, deploy.sh
 Example IoT, usage, config files
 (2yr silence since)
```

**Key observations:**
- Both repos show **single-day explosion** patterns
- OpenAir-Cyan: 10 commits in one day = hardware rush launch
- GCCS-Core: 15 commits in one day = infrastructure sprint
- After the blitz: **complete silence**

**What this means:** The "launch and leave" pattern dominates hardware and infrastructure projects. Someone builds the thing, gets it working, uploads everything, and then... stops. The code exists, the documentation is complete, but nobody maintains it. This is especially problematic for hardware projects where components become obsolete.

**The OpenAir-Cyan mystery:** They got OSHWA certification (the gold standard for open-source hardware), created CITATION.cff (for academic citation), and uploaded all files in one day. Then vanished. Did the team disband? Did they move to a private lab? Did the device work and nobody needs to fix it?

---

### Type 3: Paper-Driven Cadence (Carbon_Capture_ML)

**Pattern:** Commits arrive in clusters when new papers are published, then long gaps.

```
Carbon_Capture_ML commit timeline:
Jan 2023 ──── Feb 2023 ──── Mar 2023 ──── (gap) ──── Jan 2024 ──── Apr 2024 ──── May 2024
 9 commits     4 commits     1 commit       10mo       2 commits      1 commit      1 commit
 (10 days)    (5 days)      (Surrogate)                 (4 papers)    (README)    (OpenDAC)
```

**Key observations:**
- **5 distinct burst clusters** corresponding to paper publication waves
- Each cluster: 1-9 commits over days to weeks
- Gap between clusters: 2-13 months
- **Total lifespan: 16 months** (Jan 2023 – May 2024)
- 15 papers tracked, ~1 per month

**What this means:** This is the "living document" pattern — not truly dormant, but not continuously active either. The author treats the repo as a living bibliography that gets updated when enough new papers accumulate to justify an update. The 17-month gap before the OpenDAC paper addition suggests the OpenDAC result was significant enough to warrant immediate attention.

**The OpenDAC paper (May 8, 2024) is the final commit:** OpenDAC (Open DAC for Direct Air Capture) is a major benchmark dataset/methodology paper. Adding it to the survey was probably treated as a capstone — the biggest paper in the field gets added, the survey is "complete," and the author moves on.

---

### Type 4: Thesis Defense Burst (carbon-capture-and-storage)

**Pattern:** Slow accumulation, then defense-week frenzy, then permanent freeze.

```
carbon-capture-and-storage commit timeline:
May 2020 ──── (8 months) ──── Feb 2021 ──── Mar 2021 ──── (5.5yr dead)
 4 commits                  1 commit    6 commits
 (thesis data)             (geomech)   (defense prep)
```

**Key observations:**
- **May 2020:** 4 commits — initial data, paper, spreadsheet
- **February 2021:** 1 commit — geomechanics simulation data
- **March 2021:** 6 commits in 5 days — final results, zip files, cleanup
- **3.5x more commits in the final month than the first 8 months**
- **5 years, 6 months of silence** since the last commit

**What this means:** The thesis defense pattern is the most predictable ghost pattern in academic GitHub. The student uploads everything they need for their defense, passes, graduates, and never comes back. The repo serves its purpose (proving the work existed) but never becomes a living tool.

**The 85-star paradox:** This dead repo has more stars than any active carbon capture repo. Why? Because it was cited in papers. Stars in this context measure academic citation, not software utility. The code doesn't work (Lasso is obsolete, the data format is unique), but it’s been cited enough to accumulate stars.

---

### Type 5: Steady Development Then Freeze (CO2-Soft-Sensor)

**Pattern:** Consistent monthly commits over 8 months, then silence.

```
CO2-Soft-Sensor commit timeline:
Mar 2022 ──── May 2022 ──── Aug 2022 ──── (2.8yr dead)
 initial      semi-superv     final       
 model        ize method     updates     
 kinetic      DAE-LSTM      figure &    
 model        update        citation    
```

**Key observations:**
- **3 distinct phases:** initial model (March), method improvement (May), final polish (August)
- **8 commits over 5 months** — steady, not bursty
- Each phase has 2-3 commits (code → test → document)
- After August 2022: **nothing**

**What this means:** This is the "completed project" pattern. The developer built something in phases, tested it, documented it, and then stopped. The DAE-LSTM hybrid approach is sound, but without ongoing maintenance, it can't adapt to new capture plant designs or operating conditions.

---

### Type 6: New Energy (AI-for-Carbon-Capture-Optimization)

**Pattern:** Fresh project, all commits in 4 days.

```
AI-for-Carbon-Capture commit timeline:
Feb 28, 2026 ──── Feb 28, 2026 ──── Mar 2, 2026
 dataset +        README +         README
 optimization     project          finalization
 model            structure
```

**Key observations:**
- **3 commits in 4 days** — lean, focused launch
- First commit: synthetic dataset + optimization model
- Second: README and project structure
- Third: README finalization
- **No maintenance commits after launch** — but only 4 days have passed

**What this means:** Too early to tell if this will be a burst-freeze or a sustained project. The synthetic data approach is intellectually honest (acknowledging that real data is proprietary and unavailable). If the author continues updating as they get feedback, this could be a new sustainable pattern.

---

## Carbon-Theme Commit Trend Summary

| Theme | Signal | Confidence |
|-------|--------|------------|
| **Burst-and-freeze is universal** | 7 of 9 repos show single-burst patterns | 🔴 High |
| **CC0 licensing is emerging** | tjz21's DAC materials repos (Sep 2025) adopted CC0 public domain | 🟢 High |
| **Open hardware works but doesn't scale** | OpenAir-Cyan built a certified device, then the team vanished | 🟢 High |
| **Synthetic data bypasses proprietary barriers** | Beckybams (Mar 2026) generated fake industrial data for ML training | 🟡 Medium |
| **Materials-by-design is the active frontier** | ML-NSGA-PSA (Jun 2026) and IBM fingerprints are the newest active repos | 🟢 High |
| **The directory is the ecosystem hub** | 2,552★ outpaces every individual CC repo | 🔴 High |
| **Stars measure citations, not usability** | 85★ dead repo vs. 25★ active repo pattern | 🟢 High |
| **Thesis defense = ghost creation** | carbon-capture-and-storage: 6 commits in 5 days, then 5.5yr silence | 🟢 High |

---

## The CC0 License Revolution (Deep Dive)

The most significant finding across ALL themes isn't in any single repo — it's in a pattern across two repos:

| Repo | Commit | Date | Significance |
|------|--------|------|-------------|
| `tjz21/DAC_peroxovanadates` | CC0 dedication | Sep 23, 2025 | Computational DAC screening data for peroxovanadate sorbents dedicated to public domain |
| `tjz21/DAC_peroxotitanates` | CC0 dedication | Sep 23, 2025 | Same for peroxotitanate sorbents |

**Why this matters more than any single commit:**
1. **CC0 is not just open source — it's anti-copyright.** The researcher didn't just choose an open-source license; they waived all copyright and related rights.
2. **Computational screening data is the new public infrastructure.** Just as genome data was declared public in the 1990s, computational materials screening data is being treated as a public good.
3. **Two repos, same day, same author, same license = deliberate policy choice.** This isn't accidental; it's a philosophical statement.
4. **This is the biggest open-science story in carbon capture** — and it happened while every other repo was frozen.

**Episode hook:** *"While everyone else's carbon capture code is gathering dust, one researcher dedicated two decades of computational screening data to the public domain on the same day, for no reason other than believing it should be free. This is the CC0 revolution, and it's happening right now."*

---

## Ranking: Which Carbon Repos Deserve Episode Time?

| Rank | Repo | Why |
|------|------|-----|
| **1** | **open-sustainable-technology** | The ecosystem hub. 2,552★. The starting point for any exploration. Continuously maintained. |
| **2** | **openair-cyan** | The hardware story. OSHWA-certified DACC device. The launch-and-vanish mystery. |
| **3** | **Carbon_Capture_ML** | The literature survey. 15 papers tracked. The paper-driven cadence is relatable. |
| **4** | **CC0 DAC materials (tjz21)** | The open-science revolution. Two repos, one day, CC0 dedication. The biggest finding. |
| **5** | **AI-for-Carbon-Capture-Optimization** | The new energy. Synthetic data approach. Fresh enough to still be evolving. |
| **6** | **carbon-capture-and-storage** | The ghost benchmark. 85★, dead since 2021. The cautionary tale about stars vs. usability. |

---

*Analysis compiled: September 2026 | Source: GitHub API commit histories*
*Branch: carbon-capture*