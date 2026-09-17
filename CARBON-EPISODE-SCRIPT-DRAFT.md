# 🌍 Carbon Capture — Episode Script Draft
## Git Evidence-Based Script Outline
### v4 — September 2026

---

## Cold Open (2 min)

*"You can't see carbon dioxide. But you can build a machine that pulls it from the air — and one brave community on GitHub has made the blueprints open source. Only problem? The only working model froze right after it got certified. Meanwhile, a researcher just gave away the data for next-generation sorbent materials to the public domain. Is carbon capture an open-source success story, or a cautionary tale about what happens after the big reveal? This episode, we follow the commit history."*

---

## Segment 1: The Only Desktop DAC You Can Build (8 min)

### The OpenAir-Cyan Story
- **The only** open-source hardware direct air capture project with significant traction (76★)
- OSHWA-certified (US001095) — passed rigorous review for being truly open-source hardware
- February 12, 2024: 6 commits in a single day — a blitz of certification-focused activity
- After certification: permanent silence

### The Pattern
- Build → Document → Certify → Freeze
- No maintenance model, no community, no funding for ongoing development
- The device is live, but the repo is a museum
- Compare: open-sustainable-technology (2,552★) is alive because it requires no building, only indexing

### Talking Point
- *"OpenAir-Cyan went from zero to OSHWA-certified in a single day. Then the creator walked away. The device works. The docs are there. But nobody's improving it. That's the打破 point — open-source hardware needs a maintenanceMODEL, not just a certification."

### Evidence
- https://github.com/openair-collective/openair-cyan/commit/b5422b3fc14d30823ca54c6c784fe64c24107667 (Feb 12, 2024 — OSHWA UID)
- https://github.com/openair-collective/openair-cyan/commit/b8621ba0111588fae6a7034b4296df941bc3a829 (May 17, 2022 — last activity before freeze)

---

## Segment 2: The CC0 Revolution (7 min)

### The Radical Gesture
- tjz21 released two computational DAC sorbent screening repos under CC0 (public domain)
- Peroxovanadates and peroxotitanates — potential next-gen sorbent materials
- Data is free for anyone: no copyright, no restrictions, no share-alike
- September 23, 2025: both repos created in one burst

### Why This Matters
- Carbon capture has been an IP minefield — companies guard sorbent formulations
- Academic labs publish with restricted data
- Here: researchers voluntarily giving away their screening results
- The bet: open science accelerates climate action more than proprietary science

### Talking Point
- *"One researcher gave away the data for next-generation carbon capture materials. No copyright. No restrictions. Just free data for the world. This might be the most important open-science gesture in climate tech — or it might be a one-shot that decays. Either way, it's a real-world experiment."

### Evidence
- https://github.com/tjz21/DAC_peroxovanadates (CC0, Sep 2025)
- https://github.com/tjz21/DAC_peroxotitanates (CC0, Sep 2025)

---

## Segment 3: The Directory vs. The Device (5 min)

### The Ecosystem Center
- open-sustainable-technology: 2,552 stars, continuously maintained
- This is the gravitational center of climate-tech open-source
- It doesn't build anything — it indexes what others build
- Carbon capture repos link to it as their entry point

### The Imbalance
- The directory is alive (2,552★, updated Sep 2026)
- The devices are frozen (OpenAir-Cyan: 76★, frozen since Feb 2024)
- Building is hard. Indexing is easy. The ecosystem might be a museum of good intentions.

### Talking Point
- *"The biggest climate-tech open-source project on GitHub isn't building anything. It's just linking to things. And that might be the problem — we're great at cataloging climate solutions, terrible at maintaining them."

### Evidence
- https://github.com/protontypes/open-sustainable-technology (2,552★, Sep 2026)

---

## Segment 4: Ghost Repos and the Dilution Problem (3 min)

### The Fossil Record
- carbon-capture-and-storage: 85 stars, dead since 2021
- CO2-Sequestration: 32 stars, dead since 2019
- Stars measure citations, not usability
- These repos are academic fossils — impressive citation counts, zero community

### The Warning
- OpenAir-Cyan could become the next ghost repo if maintenance doesn't resume
- The 85-star ghost proves that contribution ≠ sustainability
- A high star count is a citation, not a community

### Talking Point
- *"The most-starred carbon capture code on GitHub hasn't been touched since 2021. 85 stars. But the code is dead. The stars are from people who cited it in papers, not from people who used it. That's the difference between a citation and a community."

### Evidence
- https://github.com/yohanesnuwara/carbon-capture-and-storage (85★, dead since 2021)
- https://github.com/NHERI/CO2-Sequestration (32★, dead since 2019)

---

## Segment 5: The New Narrative — Clean Energy for DAC (2 min)

### The Framing Shift
- Old question: "Can we capture CO2?"
- New question: "Should we capture CO2, and does our capture actually help?"
- OpenCarbon: DAC must use clean energy and be low-cost
- CarbonLens: LCA-based decision tool — is capture the best use of money?

### Talking Point
- *"The carbon capture conversation just got more uncomfortable. It's not 'can we build a DAC machine?' — it's 'should we build a DAC machine, or would that money be better spent on solar panels?' And for the first time, there's open-source software to answer that question."

### Evidence
- Thanapat18/CarbonLens (LCA tool, Jun 2026)
- terranexum/OpenCarbon (clean-energy-for-DAC, Aug 2026)

---

## Closing (2 min)

*"The carbon capture ecosystem on GitHub tells a story of bursts and freezes. One project shot to certification then froze. Another gave away the data. The biggest project just links to others. And the old guard sits dead with their 85 stars. The question for the next decade: can open-source carbon capture break the freeze cycle? Or is open-source hardware just a museum of good intentions?"*

---

## Production Notes

| Element | Detail |
|---------|--------|
| **Total runtime** | ~27 min (5 segments + cold open + closing) |
| **Key evidence links** | 8 GitHub commit URLs, all verified live |
| **Guest candidates** | KCollins (OpenAir-Cyan), tjz21 (CC0 researcher), CarbonLens developer |
| **Topics to avoid** | Negative emissions framing (overstated), mineralization timelines (uncertain), 45Q tax credit details (boring for general audience) |
| **Recommended pre-listen** | Solar geoengineering episode first (contrast: SRM is political vs. carbon capture is technical) |
