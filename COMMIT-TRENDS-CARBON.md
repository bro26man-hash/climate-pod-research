# 🌍 Carbon Capture — Commit Trend Analysis

**Last updated:** September 2026
**Data source:** GitHub List Commits API, 5 repos, 35+ commits analyzed

---

## Velocity Pages

### 🔴 Fast Universe (Institutional)
**No fast-universe carbon capture repos found.** This is the headline finding.

Unlike solar geoengineering (where PCMDI provides institutional-grade evaluation infrastructure), carbon capture on GitHub has **no equivalent of PCMDI** — no continuous-integration, multi-contributor, versioned software for evaluating or optimizing DAC processes at scale.

The gap is structural: carbon capture is dominated by **proprietary industrial R&D** (Climeworks, Carbon Engineering, Global Thermostat) that doesn't show up on GitHub. The open-source carbon capture ecosystem is **repair shops and notebooks, not production lines.**

### 🟡 Slow Universe (Academic/Hobby Burst)
**openair-collective/openair-cyan** — 76★

- **6 commits in 1 day** (Feb 12, 2024 — OSHWA certification blitz)
- Pattern: Single-day burst for certification, then 2.5 years dormancy
- Contributors: 2-3 active (KCollins, DaOfficialWizard, ZanzyTHEbar)
- Signal: **Open hardware standardization is a one-shot event, not a pipeline**
- Episode note: The OSHWA UID (US001095) is the repo's most important output — more important than any code commit

**ClimateMARGO/ClimateMARGO.jl** — 73★

- **10 commits in 30 months** (Jan 2022 – Aug 2026)
- Pattern: Setup burst (2022, 5 commits), then extreme dormancy (2023–2026), then README revival (Aug 2026)
- Contributors: 2 (Fons van der Plas, Henri Drake)
- Signal: **Academic software lifecycle — build once, cite forever, update rarely**
- Episode note: The Jul 2023 commit adding Pluto notebook link is the only "community-facing" update

**IsaH93/dac-moving-bed-digital-twin** — 0★

- Updated Jul 2026, commit history shorter than 10
- Pattern: Single maintainer, physics-informed modeling
- Signal: **The most technically rigorous DAC code is the least visible**
- Episode note: If this repo could get 50 stars, it would represent a new category: "open-source DAC process simulation"

### ⚫ Empty Universe (New Entrants)
**Rudra57/Direct-Air-Capture** — 0★
- 4 commits in 1 day (Jun 11, 2026)
- Notebook-only, no established community

**terranexum/OpenCarbon** — 2★
- Minimal activity, early-stage concept

---

## The Carbon Captains vs. The Ocean Gap

| Dimension | Solar Geoengineering | Carbon Capture | Ocean Intervention |
|-----------|---------------------|----------------|--------------------|
| **Most active repo** | PCMDI/pcmdi_metrics (133★) | OpenAir-Cyan (76★) | None |
| **Institutional backbone** | PCMDI (CMIP) | None | None |
| **Hardware code** | None (all software) | OpenAir-Cyan (open hardware) | None |
| **Fastest velocity** | 10 commits/2 weeks | 6 commits/1 day | N/A |
| **Dormancy pattern** | Paper-driven (years) | Certification-driven (years) | N/A |
| **Governance code** | 1 repo (Zereo0317) | 0 repos | 0 repos |

**Key insight:** Carbon capture has **hardware** (OpenAir-Cyan) but no **evaluation infrastructure** (no DAC equivalent of PCMDI). Solar geoengineering has **evaluation infrastructure** (PCMDI) but no **hardware**. Ocean intervention has neither.

---

## Episode 2 Architecture

### Opening question
*Can open source + CC0 break the $1000/ton DAC cost barrier?*

### Three act structure
1. **Act 1 — The Hardware Promise:** OpenAir-Cyan's OSHWA-certified DIY DAC device shows that open hardware can make the blueprints public. But 2.5 years of dormancy after the OSHWA blitz raises a question: does open hardware have a lifecycle after certification?
2. **Act 2 — The Physics Gap:** isaH93's digital twin is the only repo modeling real DAC physics (sorbent beds, Toth isotherm, LDF kinetics). Without process simulation, the open-source DAC community is building hardware without understanding why some designs work and others don't.
3. **Act 3 — The Economic Frame:** ClimateMARGO's policy optimization model says: at what carbon price does DAC become economical? The answer depends on learning rates that the open-source community could accelerate — if it were active.

### Closing question
*If the best DAC code models sorbent physics, the best DAC hardware is CC0-certified, and the best DAC economics are modeled in Julia — why can't any of these three communities talk to each other?*

---

## The Missing Middle

The carbon capture GitHub ecosystem has:
- ✅ Hardware designs (OpenAir-Cyan)
- ✅ Process simulation (IsaH93, niche)
- ✅ Policy optimization (ClimateMARGO)
- ❌ **Integration platform** — no tool that connects hardware specs → process simulation → economic analysis

This is the "missing middle" — the equivalent of PCMDI for carbon capture doesn't exist. Whoever builds a **DAC evaluation framework** (open-source, CC0, continuous-integration) would fill the most impactful gap in the carbon capture software ecosystem.
