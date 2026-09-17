# 🔀 Cross-Theme Commit Trend Summary

**Date:** September 2026
**Repositories Analyzed:** 14 across solar geoengineering, carbon capture, and ocean intervention themes
**Method:** GitHub commit API — detailed history pulled for all active repos

---

## Master Statistics

| Metric | Solar | Carbon | Ocean |
|--------|-------|--------|-------|
| Active repos (2026) | 3-4 | 0 | 0 |
| Total commits (recent window) | ~50 | ~30 | 0 |
| Institutional repos | 3 (WRF, PCMDI, MDTF) | 0 | 0 |
| Community/DIY repos | 2 (orbital-sim, srm-forever) | 1 (OpenAir-Cyan, frozen) | 0 |
| Governance tools | 3 | 0 | 0 |
| Single-day blitzes | 3 (orbital-sim, srm-forever, OpenAir-Cyan) | 3 (OpenAir-Cyan, peroxostar, Carbon_Capture_ML) | 0 |
| Dormant/ghost repos | 1 (ClimateMARGO) | 3 (climate-capture-and-storage, Carbon_Capture_ML, peroxovanadates) | N/A (no repos) |
| Most recent burst | Sep 2026 (PCMDI v4.2.1, orbital-sim) | Aug 2026 (peroxotitanates) | N/A |

---

## Trend 1: Institutional Bursts Dominate All Active Climate Software

**Pattern:** The only active, sustained development comes from well-funded institutions. Community-driven climate software is effectively absent.

**Solar evidence:**
- PCMDI/pcmdi_metrics: 15 commits in 3 days for v4.2.1 release (Sep 2–4, 2026)
- WRF: 15 commits over 4 weeks for v4.8.0 release (May–Jun 2026)
- MDTF-diagnostics: 15 commits in project-based bursts (May–Aug 2026)

**Carbon evidence:**
- No active institutional repos
- All institutional-scaled work (reservoir simulation) is dead

**Ocean evidence:**
- Zero repos to analyze

**Implication:** "If you want climate software that's actually maintained, you need an institution behind it. Community projects are either tiny or dead."

---

## Trend 2: The Single-Day Blitz and Freeze Pattern

**Pattern:** Multiple projects across both solar and carbon themes show intense single-day development followed by permanent freezing. The "artifact then abandon" pattern.

**Solar evidence:**
- orbital-climate-simulator: 12 commits in 24 hours (Sep 15–16, 2026)
- srm-forever: 4 commits in 1 day (Aug 26, 2026)

**Carbon evidence:**
- OpenAir-Cyan: 15 commits in 1 day (Feb 12, 2024), then frozen
- DAC_peroxovanadates: 8 commits in 1 day (Dec 5, 2023), then sparse
- Carbon_Capture_ML: 12 commits in 10 days (Jan 2023), then frozen

**Ocean evidence:**
- Zero projects to exhibit this pattern

**Implication:** "The carbon capture and solar geoengineering communities share a pattern: build something impressive in a day, then walk away. No maintenance culture."

---

## Trend 3: The August 2026 Cross-Theme Convergence

**Pattern:** Both solar and carbon repos show activity spikes in August 2026, suggesting a shared external stimulus (IPCC timeline, policy event, funding cycle).

**Solar:**
- hausfath/srm-forever: Complete rebuild (Aug 26, 2026)
- ClimateMARGO.jl: README revival (Aug 17, 2026) after 2.5-year dormancy
- MAOOAM/MDTF-diagnostics: continued activity

**Carbon:**
- DAC_peroxotitanates: Updated Aug 19, 2026
- ERIE-ATMO: Updated Apr 2026 (earlier)

**Ocean:**
- Zero activity to compare

**Implication:** "August 2026 was the month when SRM economics and DAC materials both woke up. What's happening in the world that makes solar intervention and ocean chemistry feel urgent at the same time?"

---

## Trend 4: Dormancy Is Features, Not Bugs

**Pattern:** The baseline state of climate software is stillness. Activity is the exception; dormancy is the rule.

**Solar dormancy:**
- ClimateMARGO.jl: 2 years 10 months between code commits
- MDTF-diagnostics: project-based cadence, 2-month gaps

**Carbon dormancy:**
- climate-capture-and-storage: 5 years 6 months frozen
- OpenAir-Cyan: 2 years 5 months frozen
- Carbon_Capture_ML: 2 years 4 months frozen

**Ocean dormancy:**
- Not applicable — there are zero repos

**Implication:** "If you're depending on open-source climate tools, you're joining a community of the dead and the sleeping. The code equivalents of ghost towns."

---

## Trend 5: The Governance Gap Scale

**Pattern:** Governance infrastructure scales with the political visibility of the technology. Solar has the most, carbon has none, ocean has less than none (it doesn't exist).

| Technology | Governance Repos | Active | Quality |
|-----------|-----------------|--------|---------|
| Solar geoengineering | 3 (PCMDI metrics, SRM economics, awesome-geoengineering) | 2 of 3 | PCMDI metrics is institutional-grade |
| Carbon capture | 0 | 0 | None at all |
| Ocean intervention | 0 | 0 | None, and no dormant tools to wake up |

**Implication:** "Solar geoengineering has more governance infrastructure than carbon capture, purely because it's more politically controversial. The governance follows the controversy, not the need."

---

## Trend 6: Curation Outlives Code — Everywhere

**Pattern:** Curated lists and surveys are more durable than simulation code across all themes.

**Solar:** awesome-geoengineering (monthly updates, v2.0.0) — the most consistently maintained project
**Carbon:** Carbon_Capture_ML (survey-only, but frozen) — was the most useful carbon capture repo
**Ocean:** Nothing to curate — the ocean geoengineering space has no resources to list

**Implication:** "The most useful climate tech resource on GitHub might be a list, not a model. But there's nothing to list for ocean geoengineering."

---

## The Big Picture: A Three-Quadrant Map

```
                     HIGH ACTIVITY
                         |
        SOLAR ------    |      CARBON
        (institutional |      (artifact-then-
         bursts,       |       freeze; no
         active gov)   |       simulation)
                         |
    MORNING ---------+-+--------- EVE
                         |
        OCEAN ------    |     (EMPTY)
        (zero repos,     |
         zero tools,     |
         zero gov)       |
                         |
                     LOW ACTIVITY
```

**Solar geoengineering** is the only quadrant with active, institutional development and governance infrastructure. It's also the most politically controversial.

**Carbon capture** has a rich cultural artifact layer (DIY hardware, ML surveys, Web3 tokens) but zero active simulation code. It's the quadrant of "things that were built and abandoned."

**Ocean intervention** is the empty quadrant. No code, no tools, no governance, no community. Not even dormant projects to wake up.

---

## Episode Planning — Updated with Commit Evidence

| Episode | Branch | Key Questions | Commit Evidence |
|---------|--------|---------------|-----------------|
| **Solar Geoengineering** | `solar-geoengineering` | Why is SRM code so scarce? Can interactive models democratize the discourse? Arctic risks? CMIP6 evaluation as governance infrastructure? | WRF: 15 commits (v4.8.0); PCMDI: 15 commits (v4.2.1); orbital-sim: 12 commits/24 hrs; srm-forever: 4 commits/1 day; ClimateMARGO: 2.5-yr dormancy with revival|
| **Carbon Capture** | `carbon-capture` | Can open source break the $1000/ton DAC cost barrier? What makes OpenAir-Cyan special? Are peroxides the sorbent of the future? The August 2026 materials wave? | OpenAir-Cyan: 15 commits/1 day then frozen; 4 peroxostar repos updated Aug 2026; Carbon_Capture_ML: 12 commits/10 days then frozen; climate-capture-and-storage: 85 stars, 5 years dead; Web3 projects more active than scientific ones |
| **Ocean Intervention** | `ocean-intervention` | Why is ocean geoengineering the empty quadrant? What would open-source OAE look like? Is the silence itself a governance signal? MDTF as the ocean-adjacent lifeline? | Zero repos found across 7 search strategies; MDTF: only ocean-adjacent tool (precip-buoyancy POD); all 6 adjacent ocean models lack geoengineering modules; every OAE module would need to be built from scratch |

---

## Cross-Theme Narrative Arc

**Episode 1 (Solar):** "The only quadrant that works" — Institutional infrastructure, active governance, interactive tools. But also: political controversy drives funding, and the physics-python gap means the tools are fragmented.

**Episode 2 (Carbon):** "The cemetery of artifacts" — Frozen DIY devices, abandoned surveys, tokenized carbon. The build-then-freeze pattern repeats. No simulation code. Web3 developers are more active than climate scientists.

**Episode 3 (Ocean):** "The empty quadrant" — Zero repos, zero tools, zero governance. The silence is the story. If ocean geoengineering ever becomes a policy option, we'd be starting from zero. The code gap mirrors the governance gap.

**Through-line:** "The governance gap mirrors the code gap. Where there's no open-source simulation, there's no public accountability. And where there's no public accountability, there's no governance. We're building the physics without the policy.

---

*Cross-theme analysis conducted September 2026 using GitHub commit API data from 14 repositories across all three podcast themes.*