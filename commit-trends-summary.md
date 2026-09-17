# 📊 Cross-Theme Commit Trend Summary

*Compiled from live GitHub API data: September 2026*

---

## Methodology

Commits were fetched via GitHub's REST API (`/repos/{owner}/{repo}/commits`) for the default branch of each repository listed in the corresponding theme notes. "Activity" is measured by recency of the most recent commit and frequency of commit cadence. "Trend" captures whether a repository is growing (new commits, active collaboration) or stagnating (last commit >2 years ago, no new activity).

---

## Solar Geoengineering — Commit Trends

| Repository | Stars | Last Commit | Activity Level | Trend |
|---|---|---|---|---|
| **ClimateMARGO/ClimateMARGO.jl** | 73 | Aug 2026 | 🟢 High | Growing — active README & code updates by single primary author (Fons van der Plas / Henri Drake) |
| **FMS-ESM/AM3** | 4 | Mar 2015 | 🔴 Dead | Stagnant — 11+ years without a commit; archived legacy model |
| **srm-ecology/climate_analogs** | 0 | Jul 2026 | 🟡 Emerging | Growing — 10 commits in Jun–Jul 2026 by 2 contributors (Ruoyu Chen, SophiaChen-codes) |
| **ChinmayaSaran/sai-climate-tradeoffs** | 0 | May 2026 | 🟡 Emerging | Launched — single burst of 2 commits May 2026 (initial + complete) |
| **protontypes/open-sustainable-technology** | 2,552 | Sep 2026 | 🟢 High | Very active — continuous curation, ~5+ commits/month in 2026 by multiple contributors |
| **brandonhimpfen/awesome-geoengineering** | 4 | Sep 2026 | 🟡 Active | Curated — frequent README updates, ~3–4 per quarter, single maintainer |
| **pmip4/pmip_p2fvar_analyzer** | 4 | Sep 2025 | 🟡 Stale | Low traffic — last commit >10 months ago |

### Key Trend
The SRM simulation code on GitHub is **stratified**: a small core of legacy Fortran (AM3) is functionally dead; one modern Julia optimization framework (ClimateMARGO) is actively growing; and the "simulation-adjacent" activity (climate_analogs, sai-climate-tradeoffs) represents lightweight, transparency-first alternatives to heavyweight GCMs. The real momentum is in **curation and visualization** (open-sustainable-technology, awesome-geoengineering) rather than in running the actual climate models.

---

## Carbon Capture — Commit Trends

| Repository | Stars | Last Commit | Activity Level | Trend |
|---|---|---|---|---|
| **tjz21/DAC_peroxovanadates** | 2 | Aug 2026 | 🟡 Emerging | Coordinated — updated same day as peer titanates repo, suggests active materials-screening program |
| **tjz21/DAC_peroxotitanates** | 2 | Aug 2026 | 🟡 Emerging | Same — twin repo to vanadates, same author, same date |
| **terranexum/OpenCarbon** | 2 | Jul 2023 | 🟠 Dormant | Bursty — commits concentrated in May–July 2023 by 2 contributors (Dahl Winters, Shrila Esturi) |
| **o7-machinehum/electro-swing-dacc** | 0 | Aug 2026 | 🟡 Emerging | New — single recent update, no stars, community knowledge-base style |
| **api-evangelist/climeworks, spiritus, clairity, 280-earth** | — | Sep 2026 | 🟡 Active | Updated — all four company profiles refreshed in Sept 2026, tracking commercial DAC ecosystem metadata |
| **protontypes/open-sustainable-technology** | 2,552 | Sep 2026 | 🟢 High | Extensive CDR section with many linked projects |

### Key Trend
Carbon capture GitHub activity reveals **two distinct surface rhythms**:
1. **Materials science commits are synchronizing** — the simultaneous August 2026 updates to both peroxovanadates and peroxotitanates (same author) suggest a coordinated open computational chemistry push for next-gen sorbents. This is a genuinely new signal.
2. **System-level engineering (OpenCarbon) went dormant in 2023** but remains a reference point for DIY/policy-oriented DAC. The gap between atomic materials (active, sync'd) and system engineering (dormant) may widen if OpenCarbon doesn't get new contributors.

---

## Ocean Intervention — Commit Trends

| Repository | Stars | Last Commit | Activity Level | Trend |
|---|---|---|---|---|
| **Team50-Labs/NebuGrid-OpenSource** | 0 | Aug 2026 | 🟡 Minimal | Small coastal fog-harvesting/drip irrigation project, NOT ocean geoengineering |
| **prashaant1926/open-earth-digital-twin-simulation** | 0 | Oct 2025 | 🟠 Dormant | Single initialization commit, research outline as much as runnable code |
| **protontypes/open-sustainable-technology** | 2,552 | Sep 2026 | 🟢 High | Has Hydrosphere/Ocean sections but NO ocean geoengineering entries |

### Key Trend
**There is no ocean geoengineering repository on GitHub with meaningful commit activity.** This is the podcast's headline finding. The gap exists because: (1) ocean experiments can't be forked like code, (2) iron fertilization carries governance stigma from the 2012 Haida incident, and (3) marine science institutions don't culture open-source software the way climate-modeling institutions do. The "empty quadrant" in the 2×2 matrix (Solar/Capture vs. Ocean/Energy) is populated by code in three of four cells, but ocean intervention has virtually nothing.

---

## Cross-Theme Observations

1. **The "Curation Economy"**: The most-stars Proj on every theme is a **directory/curation repo** (open-sustainable-technology, awesome-geoengineering), not a simulation tool. Listeners will discover climate tech through curated lists more than through running models.

2. **The Legacy Trap**: Foundational models (AM3, 2015) coexist with modern wrappers (ClimateMARGO, 2023+) but aren't being updated. The podcast should note that **the tools we'd most want to see open (GCMs for SRM, ocean models for OAE) are precisely the ones most likely to be closed**.

3. **The Synchronization Signal**: Carbon capture materials science shows unusual coordination (twin repos, synced commit dates). This is a good "trope" for the episode — open-source climate research is becoming **more coordinated**, not less.

4. **The Ocean Gap is a Governance Gap**: The absence of ocean geoengineering code isn't a software problem — it's a **governance, trust, and institutional culture** problem that manifests as a software/open-source problem. Any episode that only references GitHub data will miss the deeper story.

5. **DIY Movement is Real**: electro-swing-dacc (0 stars, but exists) and OpenCarbon's BioDAC concept show that **individual contributors** are attempting to democratize carbon capture. No equivalent exists for ocean intervention or SRM at the individual-contributor level yet.
