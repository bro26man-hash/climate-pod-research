# 🎙️ Solar Geoengineering Episode — Production Notes
## Episode Title: "The Atmosphere Isn't the Only Room in the House"

---

## Research Summary

Our GitHub investigation of solar geoengineering open-source projects reveals a small, institutional ecosystem dominated by three weather/climate models (WRF, PCMDI, MDTF) and one economic optimizer (ClimateMARGO). The total active contributor base across all solar-related repos is approximately 15 people, mostly at US national labs. There are no grassroots solar geoengineering coding communities.

**The Big Picture:** If you want to simulate warming the planet by blocking sunlight, you need to run WRF with the right physics, validate it with PCMDI metrics, check the processes with MDTF diagnostics, and then ask "should we?" with ClimateMARGO. That's the entire open-source pipeline. Four repos. Fifteen people. One planet.

---

## Key Findings

### 1. WRF is the Undisputed King
- 1,761 stars, continuous development, v4.8.0 just released
- The May 2026 solar radiation fix shows that even veteran models still have bugs in core physics
- TEMPO aerosol module being actively tuned — this is the air quality / solar interaction pathway
- **Bottom line:** WRF is where SRM simulations happen. If you're not running WRF, you're not doing solar geoengineering modeling.

### 2. PCMDI is the Quality Gate
- v4.2.1 released September 4, 2026 with a dramatic roundoff fix
- 13 commits in 2 days shows institutional urgency
- dask/SVD optimization means CMIP6 evaluation is becoming computationally feasible for more researchers
- **Bottom line:** Before you can claim SRM works, you must prove your model matches observations. PCMDI is the referee.

### 3. MDTF is the Process Detective
- Precip-buoyancy POD added June 19, 2026 (5 commits same day)
- This diagnostic evaluates whether models correctly simulate how precipitation relates to atmospheric buoyancy — critical for understanding how SRM might alter monsoon patterns
- Quarterly metrics workflow = transitioning to production monitoring
- **Bottom line:** MDTF doesn't just check if models are "right" — it identifies WHERE they're wrong, process by process.

### 4. ClimateMARGO is the Ghost
- Dormant for 30 months, then two README updates in August 2026
- No code commits. No issue activity. Just... a better README.
- Implements Weitzman certainty-equivalent discounting for climate-economy optimization under uncertainty
- **Bottom line:** Someone still cares about SRM economics. The question is: did they wake up, or are they just cleaning up the tombstone?

### 5. srm-forever is the Sleeper Hit
- Zero stars, but conceptually the most important repo
- Directly computes the optimal SRM trajectory under uncertainty
- Uses Weitzman discounting — the theoretical framework for "what if we can't stop?"
- **Bottom line:** This Jupyter notebook asks the question that haunts every SRM discussion: what's the exit strategy?

---

## What We Don't Know (Research Gaps)

1. **No open-source SRM-specific model exists at scale.** WRF can be configured for SRM, but no repo is dedicated to it. This is a gap.
2. **No community maintained SRM toolkits.** Unlike carbon capture (where OpenCarbon, Carbon_Capture_ML, etc. form an ecosystem), SRM has no community tools.
3. **Governance models are absent from code.** While ClimateMARGO addresses economics, no repo implements SRM governance decision-making.
4. **Regional disparity is invisible.** All major repos are US-funded. No European, Asian, or Global South SRM tools exist in our search.

---

## Interview Angles / Questions for Scientists

- "You fixed a solar radiation rounding error in WRF. How many SRM simulations have used the old version? How many conclusions might change?"
- "PCMDI released v4.2.1 in 9 days of intense work. What was the urgency? Was there an SRM paper depending on it?"
- "The precip-buoyancy POD is specifically about monsoon physics. If SRM shifts monsoon patterns, is MDTF the tool we'd use to detect it?"
- "ClimateMARGO had a 30-month silence. What brings you back to update the README? Are you planning new work?"
- "srm-forever has zero stars. Why does this question — 'what's the cost of SRM forever?' — matter more than people think?"

---

## Music / Sound Cues (Suggestions)

- **Cold Open:** Satellite static → WRF model output visualizations → a single held piano note (the "rounding error")
- **Act 1:** Thunder → code编译 sounds → atmospheric model visuals
- **Act 2:** Monsoon rain → 5 rapid keyboard clicks (MDTF sprint) → data flowing
- **Act 3:** Quiet room → Jupyter notebook clicking → a ticking clock (srm-forever's "forever")
- **Act 4:** Silence → a single GitHub commit sound → README text being typed
- **Close:** Four heartbeats (WRF, PCMDI, MDTF, ClimateMARGO) → sustained chord

---

## Call to Action for Listeners

- **For coders:** PCMDI and MDTF are actively seeking contributors. Python, dask, and climate science experience needed.
- **For economists:** ClimateMARGO needs love. If you know Julia and want to work on climate-economy optimization, Fons van der Plas is your person.
- **For everyone:** Read the WRF v4.8.0 release notes. Understanding what changes in a climate model release is literacy.

---

*Research sourced from GitHub API, September 2026*
*Companion docs: PROJECT-DISCOVERIES-SOLAR.md, COMMIT-TRENDS-SOLAR.md*
*Next: Record and edit. Target length: 28 minutes.*