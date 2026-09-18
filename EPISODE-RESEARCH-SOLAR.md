# 🎙️ Episode Research Brief — Solar Geoengineering
## Episode Title (Working): "The Bright Idea: Solar Geoengineering's Code Problem"

---

## Logline

Solar geoengineering is the only climate intervention that can be deployed fast enough to matter this decade — but there's almost no open-source code written specifically to simulate it. We went looking for SRM-specific repositories on GitHub and found... almost nothing. Instead, we found atmospheric models, evaluation toolkits, and a single-day burst of theoretical work that asks the question nobody wants to answer: what does it cost to keep shining the sky forever?

---

## Key Findings (from 12 repositories, 10+ GitHub search queries)

### Finding 1: The SRM Code Gap
- **0 repositories** dedicated exclusively to solar geoengineering simulation
- SRM is *modeled within* atmospheric models (WRF), economic models (DICE, MARGO), and evaluation toolkits (PCMDI) — but no standalone SRM codebase exists
- The awesome-geoengineering list (4★, actively maintained) contains papers and organizations but very few code repositories

### Finding 2: The WRF Solar Radiation Correction (May 2026)
- wrf-model/WRF committed `e836cd6` on May 28, 2026: "correction for EOT calculation for solar radiation"
- This fix affects how WRF calculates the energy budget at the end of a simulation timestep
- Any SRM scenario modeled with WRF before mid-2026 may have had a systematic error in solar radiation absorption
- **Governance implication:** published SRM modeling studies using pre-v4.8.0 WRF may need re-evaluation

### Finding 3: The PCMDI Roundoff Fix (September 2026)
- PCMDI/pcmdi_metrics committed `90cbc50` on Sep 4, 2026: "prevents roundoff to 1.00 in mean_climate figures"
- Without this fix, model evaluation metrics could show a perfect 1.00 ratio (model = observations) as an artifact of floating-point rounding
- 5 commits in a single day to push v4.2.1 — institutional intensity behind climate evaluation
- **Governance implication:** clean-looking evaluation metrics may actually be artifacts

### Finding 4: srm-forever — The Zero-Star Theorist
- hausfath/srm-forever: 0 stars, 4 commits, all on August 26, 2026
- Implements Weitzman certainty-equivalent discounting for SRM cost dynamics
- Interactive model comparing SRM-only vs combined mitigation+CDR strategies
- **The question it answers:** "What does it cost to keep SRM running forever?"
- **Why it matters:** this is the theoretical backbone for any SRM governance framework, and it exists as code — but nobody has starred it

### Finding 5: ClimateMARGO's Ambiguous Revival
- 2 README updates on August 17, 2026 after 2 years, 10 months of complete dormancy
- No code commits. No issue activity. Just two README pushes.
- ClimateMARGO is a climate-economic model that includes SRM as a decision variable
- **Interpretation A:** Genuine revival — someone noticed the model is relevant again
- **Interpretation B:** Academic citation cleanup — updating links because the paper is being cited
- **The ambiguity is the story:** geoengineering research oscillates between "politically radioactive" and "increasingly discussed but still unfunded"

---

## Interview Candidates (from GitHub)

| Priority | Repository | Contact Path | Angle |
|----------|-----------|-------------|-------|
| 🥇 | hausfath/srm-forever | GitHub profile → email | The theorist who built the framework nobody's using |
| 🥈 | wrf-model/WRF team | WRF mailing list / Anthony Islas (lead) | The atmospheric modelers who accidentally own SRM simulation |
| 🥉 | PCMDI metrics team | Jiwoo Lee (active maintainer) | The evaluators who fix roundoff errors that could change policy |

---

## Talking Points

1. **The paradox of SRM simulation:** The most important tool for simulating solar geoengineering (WRF) was never designed for that purpose. It's a weather model. SRM researchers borrow it, adapt it, and hope the physics is close enough.

2. **The governance gap:** PCMDI metrics produce the evaluation figures that IPCC reports use. A roundoff error that makes models look perfect isn't just a technical bug — it's a governance vulnerability.

3. **The cost of forever:** srm-forever asks a question that climate economists have been avoiding: if we deploy SRM, what does it cost to *keep it running* for centuries? Stop mid-century, and you get rapid warming. The Weitzman framework provides the mathematical answer, but the political answer is much harder.

4. **The ghost repo pattern:** ClimateMARGO (73★) and Geo-DICE (2★) aren't failures — they're evidence. Climate-economic models for SRM go dormant when funding dries up. The code persists, but the community disperses. Stars measure citations, not momentum.

---

## Script Structure Suggestion (30 min)

| Segment | Time | Content |
|---------|------|--------|
| Cold open | 2 min | "On May 28, 2026, someone fixed a solar radiation calculation in a weather model. It sounds boring. It might be the most important geoengineering story you haven't heard."
| The code gap | 6 min | Why there's no SRM-specific code; what exists instead |
| WRF deep dive | 8 min | v4.8.0, the solar radiation fix, what it means for past studies |
| The evaluation problem | 6 min | PCMDI, roundoff errors, and the governance of clean numbers |
| srm-forever | 5 min | Zero stars, infinite importance; the Weitzman framework |
| ClimateMARGO revival | 3 min | Two README pushes after 34 months — what does it mean? |
| Outro | 2 min | Where to learn more (awesome-geoengineering, WRF docs, srm-forever) |

---

*Research compiled from GitHub commit histories: WRF, PCMDI/pcmdi_metrics, ClimateMARGO.jl, srm-forever, OOCC_2021, Geo-DICE, awesome-geoengineering*
*Search queries: "geoengineering", "climate simulation modeling", "solar radiation management", "SRM simulation"*
*Updated: September 2026 (v4)*