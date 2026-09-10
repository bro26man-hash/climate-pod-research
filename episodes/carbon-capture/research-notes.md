# 🌱 Carbon Capture (CDR) — Research Notes

**Source:** GitHub API-based project discovery + commit-history analysis
**Branch:** `carbon-capture`
**Scope:** Carbon Dioxide Removal — Direct Air Capture (DAC), sorbent materials, CDR databases & verification

---

## ✦ Project Discoveries

| # | Project | Repo | Stars | Last Activity | Theme |
|---|---------|------|------|---------------|-------|
| 1 | **open-sustainable-technology** (umbrella directory) | [protontypes/open-sustainable-technology](https://github.com/protontypes/open-sustainable-technology) | 2,546 ⭐ | Sep 2026 | Best discovery-layer index of OSS climate tools |
| 2 | **forest-risks** (forest carbon risk models) | [carbonplan/forest-risks](https://github.com/carbonplan/forest-risks) | 35 ⭐ | Jan 2024 | CDR verification — published, now dormant |
| 3 | **cdr-database** (CDR project evaluation DB) | [carbonplan/cdr-database](https://github.com/carbonplan/cdr-database) | 29 ⭐ | Feb 2025 | CDR methodology / evaluation — light maintenance |
| 4 | **ClimaLand.jl** (soil carbon module) | [CliMA/ClimaLand.jl](https://github.com/CliMA/ClimaLand.jl) | 71 ⭐ | Sep 2026 | Process-based land/soil carbon |
| 5 | **DAC_peroxovanadates** (computational sorbents) | [tjz21/DAC_peroxovanadates](https://github.com/tjz21/DAC_peroxovanadates) | 2 ⭐ | Aug 2026 | DFT screening of DAC materials |
| 6 | **DAC_peroxotitanates** (computational sorbents) | [tjz21/DAC_peroxotitanates](https://github.com/tjz21/DAC_peroxotitanates) | 2 ⭐ | Aug 2026 | DFT screening of DAC materials |

**Other finds:**
- `o7-machinehum/electro-swing-dacc` — DIY electro-swing DAC plans (open hardware, Aug 2026)
- `terranexum/OpenCarbon` — open carbon-management planning tool (Jul 2023)
- `api-evangelist/clairity` / `spiritus` — climate-tech company profiles (company dirs, not code)

---

## 📈 Commit Trend Summary

Carbon capture on GitHub shows **two sharply different modes**:

1. **The CDR-verification/databases layer is in maintenance-to-dormant mode.**
   - `carbonplan/forest-risks` — essentially complete: last commit Jan 2024 (pre-commit/grammar badges), i.e. >2 years quiescent. The science was published; the repo is now a citation artifact reshaping carbon-market regulation rather than receiving code.
   - `carbonplan/cdr-database` — a small, self-contained burst in Feb 2025 (PRs #265/#266: switching analytics to Plausible, removing Google Analytics) then quiet. Effectively `~1-2` commits/month with a brief人居 migration spike. Active enough to stay alive, not enough to call "developing."

2. **The DAC materials-science layer had a nascent August 2026 burst.**
   - A pair of computational-chemistry repos (`tjz21/DAC_peroxovanadates`, `tjz21/DAC_peroxotitanates`, each 2★) received DFT-level updates in Aug 2026 — quantum-mechanical screening of peroxo-complex sorbents. This is "open computational chemistry for next-gen sorbents" in embryo: tiny, pre-print-adjacent, but directionally interesting.

3. **Soil/land carbon** remains the most actively maintained process side (`ClimaLand.jl`, `v1.12.0`/`v1.12.1` Sep 2026).

**Net read:** Open-source DAC is pinned to *materials discovery* (sorbent screening) and *CDR verification databases*; genuine system-engineering / scale-up commits are vanishingly rare. The August 2026 materials burst suggests a possible wave of open DFT sorbent work — worth tracking.

---

## 💡 Talking Points

1. **The $1000/ton question — can open source help?** The open DAC world is tiny and fragmented: a handful of DFT sonderium repos and two maintenance-mode CDR databases. Big engineering progress is almost entirely closed (Point Source Carbon, Climeworks, Heirloom) and IP-locked.
2. **Two modes, one story.** Distinguish (a) the mature-but-dormant *verification* layer (CarbonPlan — science done, now policy) from (b) the infant *materials-discovery* layer (open DFT sorbents). These need different podcast framings.
3. **The DIY / open-hardware signal.** `o7-machinehum/electro-swing-dacc` represents a grassroots "open DAC plans" impulse — low-cost, reproducible, but far from commercial scale. A vivid podcast contrast to industrial front-end loader.
4. **Forest & soil carbon are the "easy" open wins.** `forest-risks` already influenced policy despite 35 stars; land/soil carbon (`ClimaLand.jl`) is the quietly productive process side.
5. **Watch the Aug 2026 DAC materials cluster.** If peroxo-vanadate/titanate DFT screening grows beyond 2 repos, it could mark the start of open, computed sorbent discovery for DAC — a genuine open-source contribution to cost reduction.

---

## 🔑 Key Terminology

- **CDR (Carbon Dioxide Removal)** — umbrella for techniques removing CO₂ from the atmosphere.
- **DAC (Direct Air Capture)** — engineered capture directly from ambient air; energy- and sorbent-intensive.
- **Electro-swing DAC** — electrochemical regeneration of a sorbent, potentially simpler thermal cycle.
- **DFT screening** — density-functional theory computation of sorbent binding energies, used to pre-select candidates.
- **Peroxo-complex sorbents** — vanadium/titanium peroxide frameworks studied for CO₂ binding.
- **BECCS / Enhanced Weathering** — other CDR families (biomass+storage; mineral dissolution); barely represented in open code.
- **CDR verification** — measuring/monitoring stored carbon; CarbonPlan's principal contribution.

---

*Commit data pulled from GitHub API: carbonplan/forest-risks (Jan 2024), carbonplan/cdr-database (Feb 2025), tjz21 DAC repos (Aug 2026), ClimaLand.jl (Sep 2026), protontypes/open-sustainable-technology (Sep 2026).*
