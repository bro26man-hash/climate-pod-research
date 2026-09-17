# 📊 Carbon Capture — Commit Trend Deep-Dive

> **Branch:** `carbon-capture`  
> **Analysis Date:** 2026-09-16

---

## Summary Statement

> **The defining trend in open-source carbon capture is a bifurcation**: atomic-level materials-science repositories are surging (August 2026), while system-level engineering repositories have gone quiet. This creates a *materials surplus* paired with a *systems deficit* — the DAC equivalent of having great molecules but no reactors.

---

## Trend by Theme

### 1. DAC Materials Science — The August 2026 Surge
- **Pattern:** Two related repositories (peroxovanadates, peroxotitanates) published by the same author (tjz21) in August 2026
- **Key Insight:** Computational chemistry for carbon capture sorbents is going open — DFT, molecular dynamics, and materials screening are entering the open-source climate toolkit
- **Narrative Implication:** "Open computational chemistry for DAC" is becoming a real category, even if maintainer momentum is thin

### 2. Electro-Swing DIY Hardware — The Open-Hardware Frontier
- **Pattern:** Single-author initial push (Aug 2026)
- **Key Insight:** Electro-swing DAC — capture CO₂ using electrochemical potential swings — is being documented as open hardware. This is the capture equivalent of open-source robotics.
- **Narrative Implication:** The barrier to entry for DAC hardware design is falling; community hardware could parallel community software

### 3. System Engineering (OpenCarbon) — Silent Maintenance
- **Pattern:** Last commit July 2023; single author; bursty early activity
- **Key Insight:** Systems-level DAC planning (process design, cost modeling, deployment strategy) hasn't attracted the same open-source interest as materials science
- **Narrative Implication:** DAC's hardest problems — integration, scaling, cost — remain behind closed doors

### 4. Climate-Economic Modeling (ClimateMARGO.jl) — Policy Bridge
- **Pattern:** Bursty (2022 → 2023 → Aug 2026), single maintainer, 73 stars
- **Key Insight:** Julia-based optimization that explicitly models DAC deployment alongside emissions mitigation and adaptation — the economics layer is open even when the hardware layer isn't
- **Narrative Implication:** "Should we deploy DAC?" is being answered in open source; "how do we build it?" is not

---

## The Bifurcation Map

| Layer | Open Source Status | Example Repos | Trend |
|-------|-------------------|---------------|-------|
| **Atomic materials discovery** | 🟢 Surging (Aug 2026) | peroxovanadates, peroxotitanates | Rising SSH for new sorbents |
| **Electrochemical systems** | 🟡 Early open hardware | electro-swing-dacc | Self-published, no community yet |
| **System engineering** | 🔴 Silent since 2023 | OpenCarbon | No new contributors |
| **Cost & policy economics** | 🟢 Active (73★) | ClimateMARGO.jl | Mature, Julia ecosystem |
| **AI-assisted assessment** | 🟡 Emerging | ClimatiGPT, LLM tools | Evaluation layer, not design layer |

---

## 🎙️ Talking Points for the Episode

- "Two repositories appeared in August 2026 that simulate carbon capture sorbents at the atomic level — that's more open-source DAC chemistry than existed before this decade."
- "The materials-surge/system-silence split is the DAC version of a common open-source pattern: the cool lab tool gets open-sourced, but the boring integration work doesn't."
- "Electro-swing DAC plans as open hardware? That's the carbon capture equivalent of posting your 3D printer designs on Thingiverse."
- "ClimateMARGO.jl can tell us whether DAC makes economic sense — but it can't design the reactor that makes it happen."