# 📊 Ocean Intervention — Commit Trend Deep-Dive

> **Branch:** `ocean-intervention`  
> **Analysis Date:** 2026-09-16

---

## Summary Statement

> **Ocean geoengineering is the empty quadrant of climate-tech GitHub.** Unlike solar (sparse but present), carbon (surging materials + quiet systems), the ocean intervention category has virtually no dedicated open-source repositories — only adjacent climate models and data tools that touch the ocean as a passive component.

---

## The Five Structural Barriers to Open-Source Ocean Geoengineering

### 1. Institutional Siloing 🏛️
- Ocean research dominated by ≈10 institutions worldwide (Woods Hole, Scripps, GEOMAR, CSIRO, JAMSTEC)
- Their codebases are internal; data pipelines are proprietary
- **GitHub signal:** Zero dedicated OAE or iron fertilization repos found

### 2. Data Sensitivity 🔒
- Ocean observations require research vessels, proprietary sensors, and regulated deployments
- Open data pipelines don't exist the way they do for atmospheric monitoring
- **GitHub signal:** No open ocean observation/monitoring repositories

### 3. Experimental Complexity 🚢
- Ocean interventions require physical ship deployments, not just code execution
- Software is a small fraction of total research effort
- **GitHub signal:** No simulation-only repos can capture the ocean intervention pipeline

### 4. Governance Vacuum ⚖️
- No international framework governs ocean geoengineering
- Without social license, no incentive to open-source intervention simulation
- **GitHub signal:** Zero governance/ethics repositories for ocean intervention

### 5. Funding Misalignment 💰
- Climate-tech VC flows to energy, DAC, SRM — not ocean
- No startup ecosystem to generate open-source ocean code
- **GitHub signal:** No startup-backed ocean geoengineering reps

---

## The Adjacent Ecosystem (What Exists)

| Category | Repo | Stars | Status | Role |
|----------|------|-------|--------|------|
| Climate model w/ ocean coupling | WRF | 1,761 | Active (institutional) | Ocean module exists but closed |
| Climate-economic w/ ocean | ClimateMARGO.jl | 73 | Burst active (Julia) | Models ocean in trade-off framework |
| Hydrology (ocean precip) | Xanthos | 38 | Silent (2023) | Ocean-adjacent, no intervention |
| Climate diagnostics | MDTF-diagnostics | 80 | Active (bot updates) | CMIP6 ocean analysis |
| Data operations | clisops | 25 | Bot-maintained | Ocean data post-processing |
| Paleoclimate/CMIP6 | pmip4 | 4 | Bot-active | Ocean paleo data analysis |

---

## The Missing Layer Map

| Layer | Solar ☀️ | Carbon 🌍 | Ocean 🌊 |
|-------|----------|-----------|----------|
| **Physics simulation** | Sparse (WRF closed) | Surging (materials) | ❌ Virtually none |
| **Economic/policy models** | Active (ClimateMARGO) | Active (ClimateMARGO) | ❌ None found |
| **Hardware/open designs** | N/A | Emerging (DIY) | ❌ None found |
| **Regional risk assessment** | Active (Arctic, malaria) | Limited | ❌ None found |
| **Governance modeling** | Conceptual (OOCC_2021) | None | ❌ None found |
| **Observation/monitoring** | Sparse | Sparse | ❌ None found |

---

## 🎙️ Talking Points

- "If you search GitHub for 'ocean geoengineering,' you get zero dedicated repositories. That's the biggest open-source gap in climate tech."
- "Ocean research isn't missing from OSS because scientists aren't interested — the institutional gatekeepers won't let the data out."
- "SRM has sparse but real open code. DAC has a Sept 2026 materials surge. The ocean has nothing — and that itself is the story."
- "Governance precedes code: every domain lacking governance modeling (SRM, ocean) also lacks simulation code."