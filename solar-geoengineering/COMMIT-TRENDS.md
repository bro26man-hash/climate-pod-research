# ☀️ Solar Geoengineering — Commit Trend Analysis

## Methodology
Commit histories pulled from the 5 most relevant solar geoengineering repositories found on GitHub. Analysis covers activity patterns, release cycles, and development health.

---

## Repository Commit Histories

### PCMDI/pcmdi_metrics ⭐ 133
**Most recent commits (Sep 3–4, 2026):**
- `3092cdd` — Merge PR #1428 (Jiwoo Lee, Sep 4)
- `6419050` — Bump version to 4.2.1 (Jiwoo Lee, Sep 4)
- `6443a1d` — Merge PR #1429 (Jiwoo Lee, Sep 4)
- `0e3a96f` — Update version and release date in CITATION.cff (Jiwoo Lee, Sep 4)
- `e7dc726` — Prepare v4.2.1 (Jiwoo Lee, Sep 4)
- `d0bcbd8` — Merge PR #1427 (Jiwoo Lee, Sep 4)
- `90cbc50` — Prevents roundoff to 1.00 in mean_climate figures (James Goodnight, Sep 4)
- `71a0497` — Merge PR #1425 (Jiwoo Lee, Sep 3)
- `b2eb044` — Merge branch 'main' into 1424_jsgoodni_extremes_chunking (Jiwoo Lee, Sep 3)
- `c8711f1` — Merge PR #1423 (Jiwoo Lee, Sep 3)

**Pattern:** Institutional burst — 10 commits in 2 days. Version release, PR merges, and bug fixes clustered. This is typical of funded institutional development, not community-driven open source.

### FMS-ESM/AM3
**Last commits (2015):**
- Legacy Fortran atmospheric model
- No meaningful activity since 2015
- Represents the "classic" climate modeling approach — closed, monolithic, institutional

### pmip4/pmip_p2fvar_analyzer ⭐ 4
**Last commits (Sep 2025):**
- Maintenance-level updates
- Low activity, specialized user base

### RhondaMueller/Codes-RFG-Arctic-Impacts ⭐ 1
**Last commits (Apr 2024):**
- Single-author research project
- Academic code, not maintained after publication

### QuantaEnergy/.Symbol
**Activity:** Minimal — reference data and links, not a simulation project

---

## Cross-Cutting Trend Observations

### 1. Institutional Bursts Dominate
The most active solar geoengineering-adjacent repo (PCMDI) shows 10 commits in 2 days — a version release cycle. This is the pattern of institutionally-funded climate software, not grassroots open-source development.

### 2. LegacyCode Persists
The classic SRM simulation tools (AM3) are frozen in 2015 Fortran. No Python successor has emerged in the open-source ecosystem.

### 3. Dormancy Is the Default
4 of 5 solar geoengineering repos show no activity in the past year. The one exception (PCMDI) is institutionally funded and follows release-driven sprints.

### 4. The Evaluation-vs-Simulation Gap
The most active code (PCMDI metrics) is for *evaluating* models, not *running* them. Open-source SRM simulation tools are conspicuously absent. This is a critical gap for democratizing the SRM debate.

### 5. Academic Code Comes and Goes
Single-use research repos (RhondaMueller, pmip4) appear, serve a paper's peer review, then go dormant. No sustainability model for research software in this domain.

---

## Statistical Summary

| Metric | Value |
|--------|-------|
| Repos analyzed | 5 |
| Total stars across all | 142 |
| Most recent commit | Sep 4, 2026 |
| Oldest commit | 2015 (AM3) |
| Repos active in last 6 months | 1 (PCMDI) |
| Repos active in last year | 3 |
| Repos with >5 contributors | 1 (PCMDI) |
| Average time since last commit | ~2.5 years |

---

## Episode Questions
- If the best SRM simulation tools are closed-source, who gets to shape the narrative?
- Would an open-source, browser-based SRM simulator change public understanding?
- What does the evaluation-over-simulation gap tell us about power in climate science?
- How do we feel about the "cargo cult" problem — using tools we don't understand to manage a planet we don't fully understand?
