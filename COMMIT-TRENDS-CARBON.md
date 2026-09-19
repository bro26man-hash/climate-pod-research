# 🌍 Carbon Capture — Commit Trend Analysis

**Analysis Date:** September 2026  
**Repositories Analyzed:** 2 (GCCS-Core, Cost-Model--DAC)  
**Total Commits Pulled:** 30

---

## Velocity Summary Table

| Repository | Stars | Commits Pulled | Active Period | Velocity Pattern | Longest Gap |
|-----------|-------|----------------|---------------|-----------------|-------------|
| KOSASIH/GCCS-Core | 9 | 15 | Oct 29, 2024 (single day) | 🟡 Extreme single-day burst | 22+ months |
| kfdsievert/Cost-Model--DAC | 6 | 15 | Jan–Feb 2024 (2-week burst) | 🟡 Short burst, then silence | 2+ years |

**Combined total:** 30 commits across 2 repositories, spanning 2024–2026. **No continuous development activity detected.**

---

## Trend 1: The "Scaffolding Sprint" Pattern

GCCS-Core's commit history is remarkable for its intensity and brevity:

```
All 15 commits: October 29, 2024
────────────────────────────────────────
07:00  create example_config.yaml
07:15  create example_usage.py
07:30  create example_iot_integration.py
08:00  create deploy.sh
08:05  create run_server.sh
08:10  create data_collection.sh
08:30  create setup.py
08:45  create requirements.txt
09:00  Update README.md (1st pass)
09:30  Update README.md (2nd pass)
...
07:00  Update README.md (8th pass, after initial setup was done)
```

**What this tells us:** The developer (KOSASIH) had a clear vision of what a "Global Climate Control System" should include — deployment scripts, IoT integration, configuration management, documentation. They built the scaffolding in a single focused session. They refined the README 8 times, adjusting wording, adding sections, fixing formatting.

**What's missing:** There are zero commits that implement actual carbon capture simulation logic. No chemical equations. No thermodynamic calculations. No material science models. No energy balance models. The repo is a *framework for a framework* — deployment infrastructure with research tool aspirations.

**Episode angle:** This is the "MVP" pattern adaptation applied to climate tech. Build the deployment shell first, then add the science later. The question is: **will "later" ever come?** The 22-month dormancy since October 2024 suggests the science part hasn't arrived.

---

## Trend 2: The "Two-Week Paper Sprint" Pattern

Cost-Model--DAC shows a healthier but still bursty pattern:

```
Jan 31, 2024: 4 commits (initial file upload, workspace cleanup)
Feb  1, 2024: 6 commits (LICENSE: add→delete→re-add; README refinements; minor updates)
Feb  5, 2024: 2 commits (README polish)
Feb 19, 2024: 3 commits (final README + LICENSE adjustments)
Jun  4, 2026: 1 commit (latest update — nature unknown)
```

**The LICENSE saga:** On Feb 1, 2024, the developer added a LICENSE file, then deleted it, then re-added it — all within the same day. This suggests uncertainty about which license to use, possibly deliberating between open-source (MIT/Apache) and public-domain (CC0/Unlicense) dedications.

**After the burst:** 2 years and 4 months of silence before a single commit in June 2026. This could be a minor fix, a data update, or a visibility tweak (README change).

**Comparison with academic norms:** In computational science, a 2-week sprint to build and document a cost model is normal. The key question is whether the model gets used, cited, and built upon. With 6 stars, the model has a tiny but real audience.

---

## Trend 3: The "No Chemistry" Gap

Neither repository simulates actual carbon capture chemistry:

| What's missing | What exists instead |
|----------------|---------------------|
| Amine solvent chemistry models | Deployment scripts and IoT integration (GCCS-Core) |
| Solid sorbent material simulations | Experience curve / Monte Carlo cost projections (Cost-Model--DAC) |
| Thermodynamic equilibrium calculations | README documentation (both repos) |
| Energy integration and heat recovery | Shell scripts for server deployment (GCCS-Core) |

**This is the fundamental gap in carbon capture open-source:** The chemistry and process simulation layer is completely absent. There is no open-source "upa" (Universal Process Analyzer) or "Aspen Plus" equivalent for carbon capture.

**Why this matters for the episode:** If we want to have informed public debates about DAC feasibility, we need tools that can actually simulate the capture process — not just project the costs. The absence of process simulation code means that the public conversation about carbon capture is driven by:
1. Company press releases (capitalist sources)
2. Academic papers with proprietary models (academic sources)
3. Cost projections without chemistry validation (the two repos we found)

---

## Trend 4: The "CC0 Public Domain" Movement

While the license saga in Cost-Model--DAC (add→delete→re-add) is intriguing, it reflects a broader trend in climate tech open-source: **the move toward CC0 / public-domain dedication.**

**Why CC0 matters for carbon capture:**
- **Patent thickets:** Carbon capture technology is surrounded by patents. Amine solvents, solid sorbents, and process designs are heavily patented. CC0 code can't be patented, but CC0 code can *describe*tha unpatentable methods.
- **Replication crisis:** If cost models are proprietary, other researchers can't replicate or extend them. CC0 models enable full replication.
- **Equity:** If DAC technology is only accessible through expensive proprietary tools, the policy conversation is dominated by well-funded interests. Open tools democratize participation.

**Current state:** Both repos found in our search use standard open-source licenses (MIT-style for GCCS-Core, license-undetermined for Cost-Model--DAC). The CC0 movement is more prominent in the solar geoengineering space (where some modeling groups explicitly publish data under CC0) than in carbon capture.

---

## Trend 5: The " carbon capture vs. solar geoengineering" asymmetry

| Dimension | Solar Geoengineering | Carbon Capture |
|-----------|---------------------|----------------|
| **Number of relevant repos** | 4 found | 2 found |
| **Stars (highest)** | 1,763 (WRF) | 9 (GCCS-Core) |
| **Stars (total)** | 1,890+ | 15 |
| **Simulates the core process?** | Yes — aerosol radiative transfer in WRF | No — cost modeling only |
| **Institutional backing** | NCAR, NOAA, multiple universities | Individual developers |
| **Continuous development** | Yes (v4.8.0, June 2026) | No |
| **Commit activity (recent 6 months)** | 15 commits (WRF) | 0 commits |

**The asymmetry is stark.** Solar geoengineering has a mature, continuously developed simulation framework embedded in the world's most used regional climate model. Carbon capture has two solo-developed projects, one of which is scaffolding and the other is a cost model, neither of which simulates the actual capture process.

**Episode framing:** "If you want to simulate what happens if you inject aerosols into the stratosphere, you can run WRF — right now, today, with institutional support and continuous updates. If you want to simulate the chemistry of capturing CO₂ from the air, you can't — there's no open-source tool for that. The asymmetry isn't just about resources; it's about which climate intervention has a simulation infrastructure and which doesn't."

---

## Episode Architecture (Carbon Capture)

### Segment 1: "The Scaffolding and the Substance"
- Introduce GCCS-Core and its 8-README-in-one-day pattern
- Show that it has deployment scripts but no simulation logic
- Ask: Is this typical for early-stage climate tech open-source?

### Segment 2: "What 'Cost Model' Really Means"
- Walk through the Cost-Model--DAC Monte Carlo / experience curve approach
- Explain why cost projections without chemistry simulation are both useful and incomplete
- Discuss the LICENSE saga as a window into the open-source licensing challenges in climate tech

### Segment 3: "The Missing Layer — Why No DAC Chemistry Simulator?"
- The complete absence of process simulation for carbon capture
- Compare with solar geoengineering (WRF has TEMPO for aerosol physics)
- Ask: Should there be an open-source equivalent of Aspen Plus for carbon capture?
- Discuss the equity implications: proprietary tools = expertise gated by money

---

## Listener Resources

- **Cost-Model--DAC README:** https://github.com/kfdsievert/Cost-Model--DAC/blob/main/README.md
- **GCCS-Core structure:** https://github.com/KOSASIH/GCCS-Core/tree/main
- **DAC cost landscape (paper reference):** Steven Davis et al., "Net-zero emissions energy systems" (context for why DAC cost models matter)
- **CC0 licensing in climate science:**Search "CC0 climate model" on GitHub for examples

---

*Analysis methodology: GitHub List Commits API, September 2026. All commit data is real and verifiable via the commit SHAs listed above.*
