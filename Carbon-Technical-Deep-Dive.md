# 🌍 Carbon Capture — Technical Deep Dive

## DAC Chemistry Pathways

### Thermal Swing DAC
- **Mechanism:** Sorbent material absorbs CO2 at ambient temperature, then is heated to 80-120°C to release concentrated CO2
- **Leading projects:** Climeworks (Switzerland), Carbon Engineering (Canada, acquired by next decarbonization)
- **Energy cost:** 5-10 GJ per ton CO2 (primarily low-grade heat)
- **Open-source gap:** No open-source thermal swing DAC simulator exists

### Electro-Swing DAC ⚡ (Emerging)
- **Mechanism:** Electrically charged electrodes alternately absorb and release CO2 using voltage-switched sorbents
- **Key advantage:** No thermal cycle required — can run on low-grade electricity (including surplus renewable)
- **Open-source projects:** o7-machinehum/electro-swing-dacc
- **Potential:** Could achieve $100-200/ton if electrode materials improve
- **Limitations:** Lower CO2 concentration per cycle than thermal swing; electrode degradation over time

### MOF-Based Sorbents 🧪 (Computational Screening)
- **Mechanism:** Metal-organic framework crystals with tunable pore chemistry for selective CO2 adsorption
- **Key projects:** HildaPosada/MOF-CO2-Adsorption-Predictor, tjz21/DAC_peroxovanadates, tjz21/DAC_peroxotitanates
- **ML approach:** Graph neural networks trained on experimentally-measured CO2 uptake values
- **Breakthrough potential:** Could identify sorbents 100x faster than laboratory trial-and-error
- **Open problem:** Lab-to-real-world gap — predicted MOFs often underperform in humid, real-air conditions

---

## The $1000/ton Cost Roadmap

| Cost Component | Current | Open-Source Optimism Target |
|---------------|---------|----------------------------|
| Sorbent material | $200-400/ton | $50/ton (MOF + earth-abundant metals) |
| Heat/energy | $200-400/ton | $50/ton (electro-swing + surplus renewable) |
| Capture tower | $100-200/ton | $30/ton (DIY/modular design) |
| CO2 compression | $50-100/ton | $20/ton (standardization) |
| **Total** | **$550/ton** | **$150/ton** |

---

## The August 2026 DAC Materials Wave

On August 19, 2026, three repositories were simultaneously updated:
1. **DAC_peroxovanadates** — Computational screening of vanadium-peroxide sorbents
2. **DAC_peroxotitanates** — Computational screening of titanium-peroxide sorbents
3. **electro-swing-dacc** — DIY electro-swing DAC hardware plans

This cluster suggests either:
- A coordinated preprint/general submission day (most likely)
- A conference deadline (AGU Fall Meeting abstract deadline?)
- An informal research group releasing findings simultaneously

**This is podcast gold.** The question isn't whether peroxides work — it's whether the *open-source* community can replicate and extend the findings faster than proprietary labs.

---

## Open-Source Carbon Accounting

### The Verification Gap
Captured CO2 must be quantified, reported, and verified (MRV: Measurement, Reporting, Verification). OpenCarbon is the only open-source project addressing this. Key challenges:
- **Temporal resolution** — How often do you measure flux?
- **Spatial coverage** — Point sensors vs. atmospheric inversions
- **Permanence** — How do you prove the carbon stays captured for 100+ years?

----

## References & Further Reading
- DAC cost projections: National Academies, 2019, *Negative Emissions Technologies and Reliable Sequestration*
- MOF CO2 capture: Kaskoos et al., 2021, *Coordination Chemistry Reviews*
- Electro-swing adsorption: Fu et al., 2020, *Energy & Environmental Science*
- OpenAir-Cyan: https://github.com/openair-collective/openair-cyan
- MRV standards: Open Climate Registry, Gold Standard
