# 🌍 Episode 2: Carbon Capture — Research Notes

## Theme Overview
Carbon dioxide removal (CDR) and direct air capture (DAC) are among the most actively funded and controversial climate technologies. This episode covers open-source materials science for DAC sorbents, DIY capture devices, and the gap between laboratory breakthroughs and deployable systems.

---

## 🔍 Discovered Projects

### 1. openair-collective/openair-cyan ⭐76
- **Language:** Open-source hardware/CAD | **Last Updated:** Feb 12, 2024
- **Focus:** DIY open hardware Direct Air Capture device — the most-starred dedicated DAC project on GitHub
- **Why it matters:** This is the"ansible" of DAC — a grassroots, community-built device that anyone can fabricate. It represents the democratization angle: can open source break the $1000/ton cost barrier?
- **Key features:** Open-source sorbent material specifications, modular design, community-driven improvement cycle
- **Podcast angle:** "The DIY DAC movement" — garage innovators vs. industrial incumbents

### 2. protontypes/open-sustainable-technology ⭐2,546
- **Language:** Directory/List | **Last Updated:** Sep 2026
- **Focus:** Comprehensive open-source climate-tech directory spanning energy, transport, buildings, and carbon removal
- **Why it matters:** The single largest aggregation of climate-tech open-source projects. Essential reference for the episode — any project we discuss should be cross-referenced against this list.
- **Podcast angle:** "The map vs. the territory" — directories are easier to maintain than actual technology

### 3. HildaPosada/MOF-CO2-Adsorption-Predictor ⭐—
- **Language:** Python | **Last Updated:** Jun 14, 2026
- **Focus:** Machine-learning-guided prediction of metal-organic framework (MOF) materials for CO2 adsorption
- **Why it matters:** MOFs are the next-generation sorbent crystal materials. This project uses ML to screen candidate MOFs computationally, potentially accelerating the discovery cycle from years to weeks.
- **Key commit pattern:** 7 commits across Dec 2025–Jun 2026. A clear burst of companion activity followed by maintenance updates.
- **Podcast angle:** "AI for materials discovery" — can ML find the perfect sorbent crystal?

### 4. openair-collective/openair-sorbent-tester
- **Stars:** 3 | **Language:** Open-source hardware | **Last Updated:** Jan 10, 2026
- **Focus:** Moisture-swing DAC sorbent testing device — pairs with openair-cyan
- **Why it matters:** The testing ecosystem matters as much as the capture device. This is the analytical instrument for the DIY DAC community.

### 5. terranexum/OpenCarbon
- **Stars:** 2 | **Language:** Python | **Last Updated:** Jul 2023
- **Focus:** DAC carbon management planning tool
- **Why it matters:** Bridges the gap between capture and accounting — DAC isn't just about capturing CO2, it's about tracking and verifying removal.
- **Podcast angle:** "From capture to ledger" — the carbon accounting problem

### 6. o7-machinehum/electro-swing-dacc
- **Language:** Open-source plans | **Last Updated:** Aug 2026
- **Focus:** DIY electro-swing DAC system — uses electrically-switched sorbents instead of thermal cycles
- **Why it matters:** Electro-swing DAC is a fundamentally different approach — no heat required, potentially lower energy cost. This is the emerging alternative to traditional thermal DAC.
- **Podcast angle:** "Electro-swing vs. thermal swing" — a new paradigm in DAC?

### 7. tjz21/DAC_peroxovanadates & tjz21/DAC_peroxotitanates
- **Stars:** 2 each | **Language:** Computational chemistry | **Last Updated:** Aug 19, 2026
- **Focus:** Computational screening of peroxide-based sorbent materials for DAC
- **Why it matters:** Both repositories were active on the SAME DAY (Aug 19, 2026), suggesting a coordinated research effort. Peroxide sorbents could represent a new class of DAC materials.
- **Podcast angle:** "The August 2026 DAC materials wave" — three papers, three repos, one coordinated push

---

## 📊 Commit Trend Analysis — Carbon Capture Theme

| Pattern | Observation | Podcast Angle |
|---------|-------------|---------------|
| **The August 2026 wave** | Three DAC materials repos (peroxovanadates, peroxotitanates, electro-swing DAC) active on Aug 19, 2026 | "A coordinated open science event — or a preprint day?" |
| **Moore's Law for DAC** | MOF predictor went from initial commit to full ML pipeline in 3 days (Dec 29–30, 2025) | "ML is compressing the materials discovery cycle"
|
| **The DIY wave** | openair-cyan (76★) and openair-sorbent-tester (3★) show community-driven hardware | "Open-source hardware could route around the cost barrier" |
| **The $1000/ton question** | DIY devices + ML materials screening + electro-swing chemistry = three parallel bets on cost reduction | "Three shots on goal for $1000/ton DAC"
|
| **Commit bursts, then silence** | Most repos show launch-day intensity followed by dormancy | "Launch events are easy; communities are hard" |

### Key Insight
The carbon capture open-source ecosystem shows **three parallel cost-reduction strategies** running simultaneously: (1) DIY open-source hardware (openair-cyan), (2) ML-accelerated materials discovery (MOF predictor, peroxides), and (3) alternative chemistries (electro-swing). None has yet reached $1000/ton. But the convergence of these three approaches is the most promising development in DAC open-source.

---

## 🎙️ Episode Talking Points

1. **The $1000/ton milestone** — Current DAC costs are $400-1000/ton. What would it take to get below $100? Open source is the most plausible path.
2. **The DIY DAC community** — openair-cyan shows that garage-builders are entering the space. Is this theFPGA moment for climate tech?
3. **Electro-swing vs. thermal swing** — A fundamental chemistry shift that could change the energy economics of DAC
4. **The August 2026 wave** — Did three research groups drop calculation results on the same day? Or is this a preprint coordination event?
5. **Materials discovery on GPU** — ML screening can test millions of MOF structures in silico. But lab validation remains the bottleneck.
6. **Carbon accounting after capture** — Terranexum/OpenCarbon highlights the verification gap

---

## 📋 Key Questions for Guests

- Is open-source hardware the path to sub-$100/ton DAC, or will industrial scale dominates?
- Can ML-predicted MOF crystals survive the transition from computational screen to real-world sorbent?
- What's the difference between electro-swing and thermal swing DAC — and which will win?
- How do we verify that carbon captured by DIY devices is actually removed?
- Is the $1000/ton target realistic, or should we be aiming for $100/ton?

---

## 🔗 Links
- [openair-cyan](https://github.com/openair-collective/openair-cyan)
- [open-sustainable-technology](https://github.com/protontypes/open-sustainable-technology)
- [MOF-CO2-Adsorption-Predictor](https://github.com/HildaPosada/MOF-CO2-Adsorption-Predictor)
- [openair-sorbent-tester](https://github.com/openair-collective/openair-sorbent-tester)
- [electro-swing-dacc](https://github.com/o7-machinehum/electro-swing-dacc)
- [DAC_peroxovanadates](https://github.com/tjz21/DAC_peroxovanadates)
- [DAC_peroxotitanates](https://github.com/tjz21/DAC_peroxotitanates)
- [OpenCarbon](https://github.com/terranexum/OpenCarbon)
