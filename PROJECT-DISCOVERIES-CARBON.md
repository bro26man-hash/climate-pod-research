# 🌍 Carbon Capture — Project Discoveries

**Last updated:** September 2026
**Research cycle:** v5 — GitHub API dive, 8 repos surveyed, 35+ commits analyzed

---

## Summary

Carbon capture on GitHub reveals a sharp divide: **open hardware DAC projects** (OpenAir-Cyan, 76★) have passionate communities putting out real hardware designs, while **software/modeling projects** (ClimateMARGO, DAC digital twins) are either dormant or nascent. The CC0/open-source licensing movement is reshaping the landscape — and the $1000/ton cost barrier is the episode's center of gravity.

---

## 1. openair-collective/openair-cyan ⭐76

**URL:** https://github.com/openair-collective/openair-cyan
**Language:** (Open hardware documentation)
**Maintainer:** KCollins, DaOfficialWizard, ZanzyTHEbar

### What it is
DIY small-scale open hardware **direct air carbon capture** device called "Cyan." This is the most prominent open-source DAC project on GitHub — published hardware designs, documentation, and a community around building affordable CO₂ capture at small scale.

### Why it matters for the podcast
OpenAir-Cyan is the **physical counterargument to "DAC is too expensive"** — if you can build one with open designs, the cost model breaks. The OSHWA (Open Source Hardware Association) UID (US001095) certification adds legitimacy.

### Recent commit snapshot (Feb 2024 — OSHWA blitz)
| Date | Commit | Author |
|------|--------|--------|
| Feb 12 | Update README — added OSHWA UID link | KCollins |
| Feb 12 | Add files via upload | KCollins |
| Feb 12 | Added OSHWA UID logo (OSHWA UID US001095) | KCollins |
| Feb 12 | Add files via upload | KCollins |
| Feb 12 | Create CITATION.cff | KCollins |
| Feb 12 | Update README | KCollins |
| Jul 20, 2022 | Update README | DaOfficialWizard |
| May 17, 2022 | Add files to improve usability | ZanzyTHEbar |
| May 15, 2022 | Update README | DaOfficialWizard |
| May 15, 2022 | Update README | DaOfficialWizard |

**Verdict:** 🟡 **Slow Universe** — 6 commits in one day (Feb 2024 OSHWA certification push), then 2.5 years silence. The OSHWA blitz was a landmark: 6 commits in 24 hours, all about open hardware certification. The burst pattern is similar to academic repos, but this time driven by hardware standardization, not papers.

---

## 2. ClimateMARGO/ClimateMARGO.jl ⭐73

**URL:** https://github.com/ClimateMARGO/ClimateMARGO.jl
**Language:** Julia
**Maintainer:** Fons van der Plas, Henri Drake

### What it is
Julia implementation of MARGO, an **idealized climate-economic modeling framework** for optimizing trade-offs between emissions mitigation, adaptation, and carbon removal. Not a DAC simulation — it's a policy optimization tool that evaluates different climate interventions including carbon capture.

### Why it matters
ClimateMARGO provides the **economic framing** for carbon capture episodes: at what point does DAC become cost-effective relative to mitigation? The Julia language choice signals a academic/research community, not an engineering one.

### Recent commit snapshot (2022–2026 — very slow)
| Date | Commit | Author |
|------|--------|--------|
| Aug 17, 2026 | Update README.md | Fons van der Plas |
| Aug 17, 2026 | Update README.md | Fons van der Plas |
| Oct 18, 2023 | Update unit_conversions.jl | Fons van der Plas |
| Jul 6, 2023 | Add Pluto notebook link | Fons van der Plas |
| Nov 14, 2022 | Update Project.toml | Fons van der Plas |
| Nov 12, 2022 | JuMP and Ipopt compat upgrade | Fons van der Plas |
| Feb 10, 2022 | Removed deprecated web apps | Henri Drake |
| Feb 4, 2022 | Added CITATION.bib | Henri Drake |
| Jan 13, 2022 | Fixed typo | Henri Drake |
| Jan 12, 2022 | Updated doc deployment | Henri Drake |

**Verdict:** 🟡 **Slow Universe** — 20 months between commits (Aug 2026 README updates), long dormancy periods. Two maintainers, one burst (2022 setup), then near-zero activity. The 2026 README updates suggest someone's trying to revive it.

---

## 3. Rudra57/Direct-Air-Capture

**URL:** https://github.com/Rudra57/Direct-Air-Capture
**Language:** Jupyter Notebook
**Stars:** 0
**Created:** June 2026

### What it is
An exploratory notebook project using **data-driven modeling** to evaluate DAC technology as a climate solution for removing CO₂ from the atmosphere.

### Recent commit snapshot (Jun 2026 — all in one day)
| Date | Commit | Author |
|------|--------|--------|
| Jun 11 | Update README | Rudra Pratap Singh |
| Jun 11 | Update README | Rudra Pratap Singh |
| Jun 11 | Add files via upload | Rudra Pratap Singh |
| Jun 11 | Initial commit | Rudra Pratap Singh |

**Verdict:** ⚫ **Empty Universe (carbon side)** — 4 commits in one day, notebook-only, no stars. The "hello world" of DAC repos. But it signals that new creators are entering the space.

---

## 4. terranexum/OpenCarbon

**URL:** https://github.com/terranexum/OpenCarbon
**Stars:** 2
**Updated:** Aug 2026

### What it is
Carbon management technologies and plans to advance research and innovation in direct air capture, ensuring clean energy usage and low-cost operation.

**Verdict:** ⚫ **Empty Universe** — 2★, minimal activity. Early-stage concept project.

---

## 5. IsaH93/dac-moving-bed-digital-twin

**URL:** https://github.com/IsaH93/dac-moving-bed-digital-twin
**Language:** Python
**Updated:** Jul 2026

### What it is
A **digital twin** for Direct Air Capture's moving-bed TVSA (Temperature Vacuum Swing Adsorption) process — couples continuous sorbent physics (Toth isotherm, LDF kinetics) with a SimPy discrete-event simulation platform.

### Why it matters
This is the most technically rigorous DAC software found: not just "DAC is important" but actually modeling the **physics of the sorbent bed** in operation. A digital twin approach could be the path to understanding real-world DAC performance vs. lab claims.

**Verdict:** 🟡 **Slow Universe** — single maintainer, recently updated, no commit history visible. The physics-informed modeling approach is the most credible engineering effort in the DAC software space.

---

## The CC0 / Open-Source Revolution Angle

A critical thread running through these repos: **the licensing and openness question.** OpenAir-Cyan's OSHWA certification is the clearest signal — it's not just "open source" but "open hardware," with a UID that makes it citable and verifiable. ClimateMARGO's CITATION.bib (2022) formalizes academic citation for software. DAC digital twins are pushing the physics fidelity envelope.

### The $1000/ton question
The podcast's central economic claim: **DAC costs ~$600–$1000/ton CO₂.** The open-source counterargument:
- OpenAir-Cyan says: build it yourself for a fraction of commercial costs
- Digital twins say: optimize the process to reduce energy/loss
- Policy models (ClimateMARGO) say: when does open-source undercut commercial?

**Episode 2 angle:** *Can open source + CC0 break the $1000/ton DAC cost barrier?* The answer isn't simple — hardware costs vs. energy costs vs. learning curves are all separate equations.

---

## Trend Lines to watch

1. **OpenAir-Cyan OSHWA ripple effect** — will other open DAC projects seek OSHWA certification?
2. **Digital twin sophistication** — moving from "DAC is a concept" to "here's the sorbent physics" (IsaH93's repo leads this)
3. **ClimateMARGO revival** — if the 2026 README updates signal renewed activity, the economic framing tool could become central
4. **CC0 licensing momentum** — if more DAC projects adopt open hardware licenses, the cost curve argument strengthens dramatically
