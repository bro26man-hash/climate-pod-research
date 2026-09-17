# 🌍 Carbon Capture — Episode Research Notes

**Podcast Theme:** Direct Air Capture (DAC) & Carbon Dioxide Removal (CDR) — Pulling CO₂ from the atmosphere
**Branch:** `carbon-capture`
**Last Updated:** September 2026

---

## 🎙️ Episode Angle

Carbon capture on GitHub reveals **two distinct modes of development** that mirror the field itself: (1) atomic-level materials science — Open calculations of novel sorbent molecules (vanadates, titanates), and (2) bursty system-engineering commits — DIY hardware projects that surge in activity around funding or milestones. The August 2026 surge in DAC materials repositories suggests a new wave of open computational chemistry for next-gen sorbents. The $1000/ton cost barrier is the central question: can open source accelerate the breakthrough?

---

## 🔍 Project Discoveries

### Tier 1 — Most Active & Impactful

| Repo | Stars | Forks | Language | Last Commit | Description |
|------|-------|-------|----------|-------------|-------------|
| **[openair-collective/openair-cyan](https://github.com/openair-collective/openair-cyan)** | 76 | 5 | — | Feb 12, 2024 | DIY small-scale open hardware direct air carbon capture (DACC) device. OSHWA-certified (US001095). GPL-3.0/CERN-OHL-P licensed. Includes assembly instructions, Q&A, CO2 capture measurements. |
| **[openair-collective/openair-sorbent-tester](https://github.com/openair-collective/openair-sorbent-tester)** | 3 | — | Python | Jan 10, 2026 | Open hardware sorbent tester for moisture swing DACC sorbents. Builds on the Cyan platform's materials work. |

### Tier 2 — Materials Science & Computational Chemistry

| Repo | Stars | Forks | Language | Last Commit | Description |
|------|-------|-------|----------|-------------|-------------|
| **[tjz21/DAC_peroxovanadates](https://github.com/tjz21/DAC_peroxovanadates)** | 2 | — | TCL | Aug 19, 2026 | Computational Science Implementation for "Implementing Tetraperoxovanadates as Direct Air Carbon Capture Materials." Published in *Chem. Soc. Rev.* (2023). |
| **[tjz21/DAC_peroxotitanates](https://github.com/tjz21/DAC_peroxotitanates)** | 2 | — | — | Aug 19, 2026 | Computational SI for "Tetraperoxotitanates for High-Capacity Direct Air Capture of Carbon Dioxide." Published in *Chem. Mater.* (2024). |
| **[ChemicalEngineeringAI/Carbon-Capture](https://github.com/ChemicalEngineeringAI/Carbon-Capture)** | — | — | — | Aug 23, 2026 | Curated links and resources for carbon capture and storage / direct air capture research. |

### Tier 3 — System-Level & Finance

| Repo | Stars | Forks | Language | Last Commit | Description |
|------|-------|-------|----------|-------------|-------------|
| **[o7-machinehum/electro-swing-dacc](https://github.com/o7-machinehum/electro-swing-dacc)** | — | — | — | Aug 19, 2026 | Research collection for building an electro-swing direct air carbon capture device. Electro-swing DAC uses voltage to switch sorbents between capture and release. |
| **[somlettes/CarbonNeg](https://github.com/somlettes/CarbonNeg)** | — | — | — | Oct 22, 2025 | Carbon removal synthetic covering DAC, mineralization tech, and negative emissions solutions. |
| **[terranexum/OpenCarbon](https://github.com/terranexum/OpenCarbon)** | 2 | — | — | Jul 19, 2023 | Carbon management technologies and planning for open-source-friendly DAC deployment. |

---

## 📊 Commit Trend Analysis

### What the commit histories reveal:

**1. The DIY hardware project has the most institutional-grade momentum.** OpenAir-Cyan (76★, 5 forks) had its last burst on Feb 12, 2024 — 6 commits in a single day by KCollins, adding OSHWA certification, citation files, and README updates. This is a project that matured from prototype to certification. Chemically, it uses calcium hydroxide/hydrated lime in a passive direct air capture system powered by a 1.5W air pump.

**2. Materials science is where the new action is.** The August 2026 surge — three separate DAC materials repositories updated on the same day (Aug 19, 2026) — signals coordinated computational chemistry work. The peroxovanadates and peroxotitanates papers represent a specific research direction: transition metal peroxides as high-capacity CO₂ sorbents. These are being codified as Open Computational Implementations (SCI protocols), making lab results reproducible and searchable.

**3. Electro-swing DAC is the emerging hardware frontier.** Electro-swing DAC uses voltage to switch sorbents between a CO₂-binding state and a release state — potentially enabling modular, scalable capture. The electro-swing-dacc repo (Aug 2026) is a research collection, not yet a build guide — the field is still in the literature-review phase.

**4. System-level planning is quiet.** OpenCarbon (last commit Jul 2023), CarbonNeg (Oct 2025), and CarbonCapture smart contracts show that the "integrated system design + deployment planning" layer of carbon capture is under-developed on GitHub compared to both materials science and DIY hardware.

### Trending Themes:
- ✅ **Open hardware DACC** (OpenAir-Cyan) — the most mature GitHub presence in DAC
- ✅ **Computational sorbent discovery** — peroxovanadates, peroxotitanates, emerging August 2026 wave
- ⚡ **Electro-swing DAC** — voltage-switchable sorbents, early-stage but promising
- ⚠️ **System integration & deployment planning** — large gap between lab material and deployed system
- 🔮 **Open scientific computation** (SCI/TCL protocols) making materials research reproducible

---

## 🎙️ Key Episode Questions

1. **Can open source break the $1000/ton barrier?** Current DAC costs are ~$250-600/ton for pilot plants. Open-source materials discovery could accelerate sorbent development — but materials science needs much more than code.
2. **What makes OpenAir-Cyan special?** It's the only DAC project with proper hardware licensing (CERN-OHL-P), certification (OSHWA), and community documentation — a model for how open hardware succeeds in climate tech.
3. **Are peroxides the sorbent of the future?** The coordinated August 2026 commits on vanadates and titanates suggest a research community forming around transition-metal peroxides for DAC — worth investigating the science.
4. **Will electro-swing DAC change the economics?** If voltage can replace heat for sorbent regeneration (the current bottleneck), the energy equation changes dramatically. The GitHub presence is still nascent.

---

## 🔗 Related Resources
- **OpenAir-Cyan docs:** https://openair-collective.github.io/openair-cyan/
- **Cyan DataShare:** https://sites.google.com/view/cyan-datashare/
- **Peroxovanadates paper (2023):** DOI 10.1039/D3SC05381D
- **Peroxotitanates paper (2024):** DOI 10.1021/acs.chemmater.4c01795
