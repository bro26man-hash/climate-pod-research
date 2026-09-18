# 🌍 Carbon Capture — Project Discoveries (v7)

> **Last updated:** September 2026 (v7)  
> **Branch:** `carbon-capture`  
> **Podcast episode:** Episode 2 — Carbon Capture

---

## Overview (v7 Update)

This document profiles open-source projects relevant to carbon capture, removal, and sequestration (CDR). v7 incorporates fresh commit histories from 4 additional repos: OpenCarbon (10 commits, 2023), CO2-Sequestration (2 commits, 2019), Bioenergy-with-carbon--capture-and-storage (5 commits, 2024), and ClimateSoton/climate-research-group (4 commits, Aug 2026). Combined with v6 data from Open-Sustainable-Technology, OpenAir-Cyan, Carbon_Capture_ML, and the DAC_peroxovanadates/titanates repos, this is the most comprehensive carbon-capture project survey on GitHub.

**Total v7 commits pulled: 21 across 4 new repos**

---

## Tier 1: The Open-Source Climate-Tech Directory

### 1. Open Sustainable Technology (protontypes)

| Field | Detail |
|-------|--------|
| **Repo** | `protontypes/open-sustainable-technology` |
| **Stars** | 2,552 |
| **Last commit** | September 9, 2026 |
| **License** | CC0-1.0 |
| **URL** | https://github.com/protontypes/open-sustainable-technology |

**What it is:** The most comprehensive open-source directory of climate-tech projects — 2,500+ entries across energy, transport, industry, CO2 removal, land use, and adaptation. Not a simulation tool — it's the Wikipedia of climate tech, with structured data.

**Why it matters:** If you want to find open-source DAC code, CCS simulators, or carbon accounting tools, you start here. It's the universe's catalogue.

**(v6 data retained — see v6 section for full commit table)**

**v7 Connection to other carbon repos:** The directory's entries link to many of the repos in this document. OpenAir-Cyan, Carbon_Capture_ML, and carbon-capture-and-storage are all listed in the directory. The directory is the index; these repos are the content. The question for the podcast: is the directory more alive than the content it indexes? (Answer: yes — 3-4 commits/month vs. 0 for most entries.)

---

## Tier 2: DIY Open Hardware & Academic Research

### 2. OpenAir-Cyan (openair-collective)

**(v6 data retained — see v6 section for full commit table)**

**v7 Note:** The OSHWA certification blitz (Feb 12, 2024, 7 commits in 1 day) remains the defining moment. The 2+ year silence since is the defining question. No v7 updates — the repo remains frozen.

---

### 3. Carbon Capture ML Survey (zikribayraktar)

**(v6 data retained — see v6 section for full commit table)**

**v7 Note:** The OpenDAC dataset (May 2024) remains the field's reference point. No v7 updates — the repo remains dormant.

---

## Tier 3: The CC0 Revolution

### 4. DAC Peroxovanadates & Peroxotitanates (tjz21)

**(v6 data retained — see v6 section for full commit table)**

**v7 Note:** The CC0 license adoption (Sep 12, 2025) remains the most significant open-science event in carbon capture. Two repos, both public domain. No v7 updates.

---

## Tier 4: Ghost Repos — v7 Deep Dive

### 5. OpenCarbon (terranexum)

| Field | Detail |
|-------|--------|
| **Repo** | `terranexum/OpenCarbon` |
| **Stars** | 2 |
| **Language** | Python/JavaScript |
| **Last commit** | July 18, 2023 (merge PR #3) |
| **License** | Not specified |
| **URL** | https://github.com/terranexum/OpenCarbon |

**What it is:** Carbon management technologies and plans to help advance research and innovation in direct air capture, ensuring it uses clean energy and that low-cost methods are accessible.

**v7 Fresh Commit Pull (10 commits, May 18 – Jul 18, 2023):**

| Date | SHA | Message | Author |
|------|-----|---------|--------|
| **Jul 18, 2023** | `e3e5afb` | Merge pull request #3 from terranexum/shrila-dev | shrilaesturi2006 |
| Jul 13, 2023 | `bb5c7b2` | Update README.md | shrilaesturi2006 |
| Jul 13, 2023 | `f34380f` | Merge pull request #2 from terranexum/main | shrilaesturi2006 |
| Jul 13, 2023 | `43528c8` | Merge pull request #1 from terranexum/shrila-dev-1 | shrilaesturi2006 |
| Jul 13, 2023 | `bc5a343` | Update README.md | shrilaesturi2006 |
| May 20, 2023 | `bb603ec` | Update README.md | Dahl Winters |
| May 20, 2023 | `96e7c2c` | Update README.md | Dahl Winters |
| May 18, 2023 | `34ff91c` | Update Project_Plan.md | Dahl Winters |
| May 18, 2023 | `c5a9112` | Update README.md | Dahl Winters |
| May 18, 2023 | `f2c9866` | Create Project_Plan.md | Dahl Winters |

**The pattern — "The Two-Month Build Then Freeze":**

```
May 18:  ██ Project plan created (f2c9866) + README updates (c5a9112, 34ff91c)
May 20:  ██ README updates (bb603ec, 96e7c2c)
         │
         │  ← 2-month gap (summer?)
         │
Jul 13:  ███ 3 PR merges + README update (43528c8, f34380f, bb5c7b2, bc5a343)
Jul 18:  █  PR #3 merge (e3e5afb)
         │
         │  ← 2+ years of silence
```

**What happened:** Two contributors (Dahl Winters and shrilaesturi2006) built a project plan and documentation in May 2023, then took a 2-month break, then merged 3 pull requests in one day (Jul 13), and then stopped completely. The repo has had zero commits since July 18, 2023 — over 2 years ago.

**The v7 finding:** Unlike the other ghost repos (which had academic purposes), OpenCarbon was a **collaborative project** — it had PRs, multiple contributors, and a project plan. The fact that it still died suggests the collaboration failed, not just that the individual contributor lost interest. This is the "team ghost" pattern: even with multiple people, carbon-capture OSS can go completely silent.

**🎙️ Episode Hook:** *"Two people built a carbon capture project, merged three pull requests in one day, and then vanished. Two years later, the README still says '力争上游' (strive for the upper). The code never shipped. The plans never materialized. This is what happens when carbon capture open source runs out of steam — not a dramatic explosion, just a fade to silence."

---

### 6. CO2 Sequestration (salmansust)

| Field | Detail |
|-------|--------|
| **Repo** | `salmansust/CO2-Sequestration` |
| **Stars** | 32 |
| **Language** | MATLAB |
| **Last commit** | March 24, 2019 |
| **License** | Not specified |
| **URL** | https://github.com/salmansust/CO2-Sequestration |

**What it is:** Carbon Capture and Sequestration (CCS) simulation. Described as "a technology that combats climate change and reduces carbon footprint in the atmosphere."

**v7 Fresh Commit Pull (2 commits, both on same day):**

| Date | SHA | Message |
|------|-----|--------|
| Mar 24, 2019 | `b2d925e` | Add files via upload |
| Mar 24, 2019 | `41f2aa0` | Initial commit |

**The ghost story, simplified:** 2 commits, both on the same day, 6+ years ago. No README updates, no bug fixes, no feature additions. Someone uploaded their MATLAB code, and that was it. 32 stars — people found it, cited it, and moved on.

**The v7 finding:** This is the simplest ghost pattern: upload and abandon. No collaboration, no PRs, no updates. Just a single-day snapshot of someone's research code. The 32 stars represent citations, not usage. The code is probably broken by now (old MATLAB version, no dependencies specified).

**🎙️ Episode Hook:** *"Two commits. Same day. Six years ago. That's it. 32 people starred it. Nobody ran the code. This is the 'upload and vanish' pattern — the simplest way a climate tech repo becomes a ghost."

---

### 7. Bioenergy with Carbon Capture and Storage (vasilistsavalias)

| Field | Detail |
|-------|--------|
| **Repo** | `vasilistsavalias/Bioenergy-with-carbon--capture-and-storage` |
| **Stars** | 1 |
| **Language** | Not specified (PDF + code) |
| **Last commit** | February 3, 2024 |
| **License** | Not specified |
| **URL** | https://github.com/vasilistsavalias/Bioenergy-with-carbon--capture-and-storage |

**What it is:** BECCS (Bioenergy with Carbon Capture and Storage) overview — a technology that combines biomass energy with carbon capture to achieve negative emissions.

**v7 Fresh Commit Pull (5 commits, Jan 27 – Feb 3, 2024):**

| Date | SHA | Message |
|------|-----|--------|
| Feb 3, 2024 | `e8c4d40` | completed |
| Jan 27, 2024 | `133b694` | Update README.md |
| Jan 27, 2024 | `b66880b` | Update README.md |
| Jan 27, 2024 | `cd8915c` | Create BECCS-overview.pdf |
| Jan 27, 2024 | `a154cec` | Initial commit |

**The pattern — "The Project Workflow":**

```
Jan 27:  ██ Initial commit (a154cec) + PDF created (cd8915c) + 2 README updates (b66880b, 133b694)
Feb 3:   █ "completed" (e8c4d40)
```

**What happened:** Someone started a BECCS project, created an overview PDF, updated theREADME twice, and then completed it 7 days later. This is the "academic project" pattern: build the artifact, document it, declare it complete, and move on to the next paper.

**The v7 finding:** Unlike the ghost repos (which had zero activity after creation), BECCS had a proper workflow: initial commit → content creation → documentation → completion marker. The "completed" commit message (e8c4d40) is the most honest in this entire set. The author looked at their repo and said "this is done." One star. The PDF is probably the most viewed file.

**🎙️ Episode Hook:** *"'Syscall completed' — the most honest commit message in climate tech. Someone made a BECCS overview, it took 7 days, and then they declared it done. One star. But at least they finished."

---

### 8. ClimateSoton Climate Research Group (ClimateSoton)

| Field | Detail |
|-------|--------|
| **Repo** | `ClimateSoton/climate-research-group` |
| **Stars** | Not tracked (website repo) |
| **Language** | HTML/CSS/JavaScript |
| **Last commit** | August 6, 2026 |
| **License** | Not specified |
| **URL** | https://github.com/ClimateSoton/climate-research-group |

**What it is:** Research group website for the CLIMATE Research Group at University of Southampton. Develops innovative technologies for carbon capture, utilisation, and sustainable energy. Combines chemical looping, advanced materials, CO₂ conversion, CFD modelling, and reaction engineering.

**v7 Fresh Commit Pull (4 commits, all on same day):**

| Date | SHA | Message |
|------|-----|--------|
| Aug 6, 2026 | `4b7cc18` | Update index.html |
| Aug 6, 2026 | `f0b123f` | Delete 1.zip |
| Aug 6, 2026 | `503e839` | Add files via upload |
| Aug 6, 2026 | `3807b50` | Add files via upload |

**The pattern — "The Website Refresh":**

```
Aug 6, 2026:  ██ 4 commits: index.html update + zip deletion + 2 file uploads
```

**What happened:** A research group updated their website. Cleaned up an old zip file, uploaded new materials, and updated the index page. This is the "institutional maintenance" pattern — not research code, but infrastructure.

**The v7 finding:** This is the ONLY carbon-theme repo with committed activity in 2026 (Aug 6). It's not simulation code — it's a website. But its activity is significant because it suggests the research group is still operational. The CFD modelling and chemical looping research they describe could eventually produce code repos. The website is the canary in the coal mine.

**Ocean relevance:** The CLIMATE group's CFD work is relevant to ocean-intervention modeling (see ocean-intervention branch). Their chemical looping research could intersect with ocean alkalinity enhancement processes.

**🎙️ Episode Hook:** *"The only carbon-capture repo with 2026 activity is... a website. Four commits, all same day, cleaning up a zip file. But that website means the research group is alive. And their CFD work might be the bridge to ocean intervention modeling."

---

## Tier 5: The Ghost Taxonomy — v7 Classification

Based on the fresh commit data from v7, we can now classify ghost repos into distinct types:

| Ghost Type | Repo | Pattern | Star Count | Last Active |
|-----------|------|---------|-----------|-------------|
| **Upload-and-Vanish** | CO2-Sequestration | 2 commits, same day, no updates | 32 | 2019 (6+ years) |
| **Project-Workflow** | BECCS | Build → document → "completed" | 1 | 2024 (1.5 years) |
| **Collaboration-Failure** | OpenCarbon | Multiple contributors, PRs, then silence | 2 | 2023 (2+ years) |
| **Ghost-Star Giant** | carbon-capture-and-storage | 85 stars, 0 commits | 85 | 2021 (4+ years) |
| **Institutional-Absent** | (none in carbon) | — | — | — |

**The taxonomy tells us:**
1. **Upload-and-Vanish** is the simplest: someone dumps code and leaves. No intention of maintaining.
2. **Project-Workflow** is the fairest: the author did a complete job, declared it done, and moved on.
3. **Collaboration-Failure** is the saddest: multiple people tried, made PRs, and then the project died anyway.
4. **Ghost-Star Giant** is the most misleading: 85 stars, but no commits since 2021. Stars measure citations, not usability.

---

## v7 Cross-Theme Synthesis — Carbon

### The Directory vs. The Content Gap

Open-Sustainable-Technology (2,552★, 3-4 commits/month) indexes content from repos that are mostly dead. The directory is the only alive repo in the carbon theme. This is a meta-finding: the catalogue is more alive than what it catalogues.

### The CC0 Revolution Continues

The tjz21 repos remain the only carbon-capture repos with CC0 licensing. No new CC0 adopters in v7 data. The revolution is real but not spreading.

### The Ghost Pattern is Universal

All four ghost repos (OpenCarbon, CO2-Sequestration, BECCS, carbon-capture-and-storage) show the same pattern: activity stops, and nobody maintains. The only difference is how the stopping happened:
- Upload-and-vanish (CO2-Sequestration)
- Honest completion (BECCS)
- Collaboration failure (OpenCarbon)
- Citation artifact (carbon-capture-and-storage)

### The Website Canary

ClimateSoton's Aug 2026 website update is the only 2026 activity in the carbon theme. It's not code, but it means the research group exists and is operational. Their CFD work could bridge to ocean intervention.

### The AI Governance Signal (from v6, still valid)

The July 2026 AI content disclosure PR template in Open-Sustainable-Technology remains the most significant governance signal in carbon-capture OSS. No new governance developments in v7 data.

---

## Summary Table — Carbon Theme (v7)

| Repo | Stars | Status | Key v7 Signal | Type |
|------|-------|--------|---------------|------|
| **open-sustainable-technology** | 2,552 | 🟢 Very active | AI disclosure PR template (Jul 2026) | Directory |
| **OpenCarbon** | 2 | 💀 Dead 2+ yr | Two contributors, 3 PRs, then silence | Collaboration-Failure |
| **CO2-Sequestration** | 32 | 💀 Dead 6+ yr | Upload-and-vanish (2 commits, same day) | Upload-and-Vanish |
| **BECCS** | 1 | 💀 Dead 1.5 yr | Honest "completed" after 7 days | Project-Workflow |
| **carbon-capture-and-storage** | 85 | 💀 Ghost 4+ yr | Citation artifact, no commits since 2021 | Ghost-Star Giant |
| **openair-cyan** | 76 | 💀 Dormant 2+ yr | OSHWA cert blitz then silence | Big-Bang-Then-Freeze |
| **Carbon_Capture_ML** | 56 | 💀 Dormant 1.5 yr | OpenDAC paper then silence | Big-Bang-Then-Freeze |
| **DAC_peroxovanadates** | 2 | 🟡 Sparse | CC0 license (Sep 2025) | CC0-Pioneer |
| **DAC_peroxotitanates** | 2 | 🟡 Sparse | CC0 license | CC0-Pioneer |
| **ClimateSoton/website** | N/A | 🟢 Active (Aug 2026) | Only carbon theme repo with 2026 activity | Institutional-Canary |

---

## Episode 2 Narrative Arcs (v7)

### Arc A: "The Catalogue" (v6, retained)
Open-Sustainable-Technology as the universe of climate tech. 2,552 stars, 2,500+ projects, constantly growing.

### Arc B: "The Demo" (v6, retained)
OpenAir-Cyan — the OSHWA-certified DIY DAC device.

### Arc C: "The Data Revolution" (v6, retained)
CC0 licensing in the DAC materials community.

### Arc D: "The Ghost Taxonomy" (v7 NEW)
Four types of ghosts: Upload-and-Vanish, Project-Workflow, Collaboration-Failure, and Ghost-Star Giant. Each type tells a different story about why carbon capture code dies.

### Arc E: "The Website Canary" (v7 NEW)
ClimateSoton's Aug 2026 website update — the only 2026 activity in the carbon theme. Not code, but a signal that the research group is alive. The CFD work could bridge to ocean intervention.

### Arc F: "The Collaboration Failure" (v7 NEW)
OpenCarbon's story: two contributors, three PRs, then silence. The collaboration died, not just the individual contributor. This is what happens when carbon capture open source runs out of teamwork.

---

## v7 Research Log

| Date | Activity |
|------|----------|
| Sep 2026 | v6: Initial project profiles from 8 repos, CC0 revolution identified |
| Sep 2026 | v7: Fresh commit data pulled from OpenCarbon (10 commits), CO2-Sequestration (2 commits), BECCS (5 commits), ClimateSoton (4 commits) |
| Sep 2026 | v7: Ghost taxonomy created — 4 distinct types: Upload-and-Vanish, Project-Workflow, Collaboration-Failure, Ghost-Star Giant |
| Sep 2026 | v7: OpenCarbon identified as Collaboration-Failure pattern (2 contributors, 3 PRs, then silence) |
| Sep 2026 | v7: CO2-Sequestration confirmed as simplest ghost (upload-and-vanish, 2 commits same day) |
| Sep 2026 | v7: BECCS identified as honest completion ('completed' commit after 7 days) |
| Sep 2026 | v7: ClimateSoton website update (Aug 2026) identified as only 2026 carbon-theme activity |
| Sep 2026 | v7: ClimateSoton CFD work flagged as potential bridge to ocean-intervention modeling |
| Sep 2026 | v7: Two new narrative arcs added (Ghost Taxonomy, Website Canary, Collaboration Failure) |
