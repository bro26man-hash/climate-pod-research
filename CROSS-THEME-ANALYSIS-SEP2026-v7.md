# 📊 Cross-Theme Commit Trend Analysis — September 2026 (v7)

**Updated:** September 2026 — v7 (fresh GitHub API pull, 6 repos, 75+ commits)

## Methodology

Fresh commit histories from 6 key repositories across all three podcast themes, retrieved from GitHub's API on September 18, 2026. v7 represents the most comprehensive data pull to date, with full 15-commit histories from each repo.

| Theme | Repos | Commits Pulled | New in v7 |
|-------|-------|----------------|-----------|
| ☀️ Solar | WRF, PCMDI, MDTF-diagnostics, ClimateMARGO, srm-forever, awesome-geoengineering | 65+ | Full 15-commit histories from all repos |
| 🌍 Carbon | open-sustainable-technology, openair-cyan, Carbon_Capture_ML, DAC_peroxovanadates, DAC_peroxotitanates | 55+ | Full 15-commit histories; AI governance signal |
| 🌊 Ocean | MDTF-diagnostics, WRF (coupled) | 20+ | Full 15-commit MDTF analysis; PBP-POD burst |

---

## Fresh Commit Data — By Theme (v7)

### ☀️ Solar Geoengineering

| Repo | Stars | Commits | Window | Key Signal | Status |
|------|-------|---------|--------|------------|--------|
| **WRF** | 1,762 | 15 | May-Jun 2026 | v4.8.0; solar radiation EOT fix (e836cd6); TEMPO staging-off (6a289e1) | 🟢 Active release |
| **PCMDI** | 133 | 15 | Sep 3-4 + Sep 17, 2026 | v4.2.1; roundoff fix (90cbc50); 10 commits in 2 days; numpy SVD fallback | 🟢 Active maintenance |
| **MDTF** | 80 | 15 | May-Aug 2026 | PBP-POD (5 commits Jun 19); quarterly metrics workflow | 🟡 Active + process |
| **ClimateMARGO** | 73 | 15 | Jan 2022 + Aug 2026 | 7-commit launch burst; 2-year dormancy; 2 README revival (no code) | 🟡 Dormant/revival? |
| **srm-forever** | 0 | 4 | Aug 26, 2026 | Weitzman discounting; interactive SRM economics model | 🟡 Single-day manifesto |
| **awesome-geo** | 4 | 5 | Jan-Sep 2026 | v2.0.0 reorganization (May); active curation | 🟢 Steady |

**v7 Solar Theme Finding:** The solar theme has two activity modes — institutional release cycles (WRF, PCMDI, MDTF) and individual manifestos (srm-forever, ClimateMARGO). There's no middle ground. No community-driven, sustained SRM-specific tool development exists.

### 🌍 Carbon Capture

| Repo | Stars | Commits | Window | Key Signal | Status |
|------|-------|---------|--------|------------|--------|
| **open-sustainable-tech** | 2,552 | 15 | Jun-Sep 2026 | AI disclosure PR template (Jul 19); claude-carbon entry (Aug 23); MUIO/MUIOGO (Sep 9) | 🟢 Very active |
| **openair-cyan** | 76 | 15 | May 2022-Feb 2024 | OSHWA blitz (7 commits Feb 12, 2024); then 2+ years silence | ⚠️ Dormant |
| **Carbon_Capture_ML** | 56 | 10 | Feb 2023-May 2024 | OpenDAC paper (May 2024); then silence | ⚠️ Dormant |
| **DAC_peroxovanadates** | 2 | 10 | Dec 2023-Sep 2025 | CC0 license (Sep 12, 2025); paper cycles | 🆕 CC0 signal |
| **DAC_peroxotitanates** | 2 | 10 | Feb-Sep 2025 | CC0 license (Sep 12, 2025); parallel to peroxovanadates | 🆕 CC0 signal |

**v7 Carbon Theme Finding:** The AI governance signal (Jul 2026) is the biggest development. The climate-tech OSS community is formally debating how to handle AI-generated contributions — with a mandatory PR template checkbox. The CC0 revolution (Sep 2025) continues to be the biggest open-science signal. The OSHWA certification (Feb 2024) was a peak, not a plateau.

### 🌊 Ocean Intervention

| Repo | Stars | Commits | Window | Key Signal | Status |
|------|-------|---------|--------|------------|--------|
| **MDTF-diagnostics** | 80 | 15 | May-Aug 2026 | PBP-POD (5 commits Jun 19); quarterly metrics; citation support | 🟡 Active |
| **WRF (coupled)** | 1,762 | 15 | May-Jun 2026 | MYNN surface layer; air-sea interaction; NOT used for interventions | 🟢 Active (wrong domain) |

**v7 Ocean Theme Finding:** The ocean is the empty quadrant. 12 search queries, zero dedicated repos. The PBP-POD is the most ocean-relevant code in open source — and it's for evaluation, not intervention. The gap is real, structural, and unexplained.

---

## The Three Universes — v7

### Fast Universe (Institutional, Funded, Sustained)

| Repo | Stars | Theme | Commits | Velocity |
|------|-------|-------|---------|----------|
| open-sustainable-technology | 2,552 | 🌍 Carbon | 15 | 3-4/month sustained |
| WRF | 1,761 | ☀️ Solar | 15 | 10 in 4 weeks (release) |
| PCMDI | 133 | ☀️ Solar | 15 | 10 in 2 days (blitz) |
| MDTF-diagnostics | 80 | 🌊 Ocean | 15 | 5 in 1 day (PBP-POD) + maintenance |

### Slow Universe (Individual, Unfunded, Dormant)

| Repo | Stars | Theme | Commits | Pattern |
|------|-------|-------|---------|---------|
| openair-cyan | 76 | 🌍 Carbon | 15 | 7/day blitz → 2+ yr silence |
| ClimateMARGO | 73 | ☀️ Solar | 15 | 7/day launch → 2yr 10mo → 2 README |
| Carbon_Capture_ML | 56 | 🌍 Carbon | 10 | 1/week build → 1.5yr silence |
| DAC_peroxovanadates | 2 | 🌍 Carbon | 10 | Paper cycles → CC0 → silence |
| DAC_peroxotitanates | 2 | 🌍 Carbon | 10 | Paper cycles → CC0 → silence |
| srm-forever | 0 | ☀️ Solar | 4 | 4/day manifesto → silence |
| awesome-geoengineering | 4 | ☀️ Solar | 5 | 1-2/month curation |

### Empty Universe (Zero Presence)

| Domain | Repos | Commits | Closest Proxy |
|--------|-------|---------|---------------|
| Ocean geoengineering (OAE/MCB/upwelling/fertilization) | **0** | **0** | MDTF PBP-POD (evaluation only) |
| Marine cloud brightening | **0** | **0** | WRF (atmospheric only) |
| Ocean sensors/IoT | **0** | **0** | None |
| Ocean governance | **0** | **0** | srm-forever (SRM only) |

---

## v7 Cross-Theme Signals

### Signal 1: The AI Governance Wave (NEW — v7)

**The evidence:** Open-Sustainable-Technology's July 2026 PR template change (c4c9fe7):
- Jul 17: PR template update with review reminder
- Jul 19: mandatory AI-disclosure checkbox added
- Jul 19: duplicate checkbox removed (iterative refinement)
- Aug 23: claude-carbon entry added (new AI category)

**Cross-theme implication:** If climate-tech OSS is grappling with AI governance, what does this mean for geoengineering? SRM simulations could be AI-assisted. Climate models could be AI-generated. The governance question is coming.

### Signal 2: The CC0-to-AI Pipeline (v7 Extension)

The CC0-licensed DAC materials data (tjz21, Sep 2025) could become AI training infrastructure. Public domain data is the raw material for machine learning. The climate-tech community is simultaneously:
1. Releasing data to public domain (CC0)
2. Building AI tools that use that data (claude-carbon)
3. Debating how to govern AI-assisted contributions (PR template)

**The triangle:** CC0 data → AI tools → governance questions. This is the future of open climate science, and it's happening now.

### Signal 3: The Institutional Divide (v7 Confirmed)

```
Fast Universe:  4 repos  |  55+ commits  |  Institutional funding  |  Sustained velocity
Slow Universe:  7 repos  |  65+ commits  |  Individual effort       |  Big-bang-then-freeze
Empty Universe: 0 repos  |  0 commits     |  No champion             |  Complete absence
```

### Signal 4: The Ocean Gap (v7 Reconfirmed)

12 queries, zero results, zero commits. The most ocean-relevant code (PBP-POD) evaluates models — it doesn't simulate interventions. The gap is cultural and motivational, not computational.

### Signal 5: The Weitzman Framework (v7 Detail)

srm-forever implements Weitzman's certainty-equivalent discounting in an interactive web tool. A zero-star repo with a live model, rigorous sourcing, and open license. The most theoretically important SRM tool that nobody has heard of.

---

## 🎙️ Episode Planning (v7)

| Episode | Branch | Key Questions | Commit Evidence | v7 Additions |
|---------|--------|---------------|-----------------|-------------|
| **Solar Geoengineering** | `solar-geoengineering` | Why is SRM code so scarce? Can interactive models democratize the discourse? Arctic risks? CMIP6 evaluation as governance infrastructure? | WRF: 10 commits (v4.8.0, solar radiation fix); PCMDI: 10 commits in 2 days (v4.2.1); srm-forever: 4 commits (Weitzman) | TEMPO staging-off; PBP-POD as solar-adjacent; ClimateMARGO dormancy signature |
| **Carbon Capture** | `carbon-capture` | Can open source break the $1000/ton DAC cost barrier? What makes OpenAir-Cyan special? Are peroxides the sorbent of the future? The August 2026 materials wave? The CC0 revolution? The AI governance question? | OpenAir-Cyan: 1-day blitz (Feb 2024) then frozen; CC0 licenses (Sep 2025); 5 repos analyzed | AI disclosure PR template; claude-carbon category; OpenDAC survey bridge; OSHWA certification pattern |
| **Ocean Intervention** | `ocean-intervention` | Why is ocean geoengineering the empty quadrant? What would open-source OAE look like? Is the silence itself a governance signal? MDTF as the ocean-adjacent lifeline? Can a PBP-POD adaptation be the entry point? | **Zero repos found**; MDTF: only ocean-adjacent tool (PBP-POD); 5 commits in 1 day | Cultural gap analysis; 5-step feasibility path; laptop-feasible architecture; self-reinforcing funding loop |

---

## 🔮 Watchlist (v7)

| # | Signal | What to Watch | Timeline |
|---|--------|---------------|----------|
| 1 | WRF TEMPO re-enablement | Will aerosol-aware schemes return with fixes? | Next release cycle |
| 2 | PCMDI SRM evaluation tools | Will PCMDI ever include SRM-specific metrics? | Unlikely near-term |
| 3 | ClimateMARGO code revival | Will Aug 2026 README updates lead to code commits? | Next 3-6 months |
| 4 | srm-forever adoption | Will the zero-star model gain community traction? | Uncertain |
| 5 | **AI governance in climate-tech OSS** | How will the AI disclosure checkbox evolve? Will it spread? | **Ongoing — watch 2027** |
| 6 | **CC0 propagation** | Will other DAC researchers follow tjz21's public domain dedication? | **Watch 2027** |
| 7 | **OpenAir-Cyan commercialization** | Will OSHWA-certified designs ever get a follow-up? | **Watch 2027** |
| 8 | **PBP-POD adaptation challenge** | Will anyone adapt the POD for intervention detection? | **Watch 2027** |
| 9 | **Ocean gap into 2027** | Will the empty quadrant fill? Or persist? | **The big question** |
| 10 | **AI vs. institutional divide** | Will AI-generated code change the fast/slow universe dynamic? | **Emerging** |

---

## Research Log (v7)

| Date | Activity |
|------|----------|
| 2026-09-03 | Repository created |
| 2026-09-17 | v1-v3: Initial research, ecosystem analysis |
| 2026-09-18 | v4: 14 repos; differentiable-flowsheets + Claude; Lagrangian particles; OceanBioME gas exchange |
| 2026-09-17 | v5-v6: Detailed project profiles, commit trend analyses, ocean gap analysis |
| **2026-09-18** | **v7: Fresh 15-commit histories from 6 repos via GitHub API; AI governance signal identified; CC0 revolution confirmed; PBP-POD burst analyzed; three-hypothesis refinements; cross-theme dashboard updated** |

---

*Last updated: September 2026 (v7) | Data source: GitHub API commit histories*
*Previous version: v6 (September 2026)*