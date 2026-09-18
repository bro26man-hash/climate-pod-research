# 🎙️ Episode Brief: Carbon Capture (v9)

> **Branch:** `carbon-capture`  
> **Theme:** Carbon Capture, Removal, and Sequestration (CDR)  
> **Duration target:** 45-60 minutes  
> **Research basis:** 9 repos analyzed, 100+ commits pulled, 3 commit patterns identified

---

## The Big Question

**If carbon capture is essential to most climate scenarios, why is there almost no actively maintained open-source code for it — and what does the surge of CC0 and OSHWA certifications tell us about whether open-source can actually scale the technology?**

---

## Act 1: The Directory vs. The Tools

**The setup:** The only actively maintained carbon capture repo on GitHub is a *directory* — Open-Sustainable-Technology (2,552 stars, ~3-4 commits/month, every month). It's a curated list of 2,500+ climate tech projects. It's not a simulation tool, not a hardware design, not a materials screening code. It's the Wikipedia of climate tech.

**The implication:** If you want to find open-source DAC code, CCS simulators, or carbon accounting tools, you start here. But the directory is the ecosystem — the actual tools are elsewhere (or don't exist).

**The AI governance signal (Jul 2026):** Three commits over 3 days that changed the PR template to require an AI-disclosure checkbox. Then a "remove duplicate checkbox" commit the same day. The community is actively debating how to handle AI-assisted contributions. The `claude-carbon` entry (Aug 2023) is now a category: AI tools for carbon-aware compute scheduling.

**Sound bite:** *"The most actively maintained carbon capture repo on GitHub is a list. And the biggest debate happening on its commit history isn't about chemistry or physics — it's about whether AI should disclose its involvement in every pull request."*

---

## Act 2: The One-Day Releases

### OpenAir-Cyan — The OSHWA Blitz

**The setup:** A DIY direct air capture machine. Open-source hardware. OSHWA-certified (UID US001095). 76 stars.

**The commits:**
- **May 2022:** 3 commits over 3 days (README, usability improvements)
- **Feb 12, 2024:** **6 commits in 24 hours** — OSHWA UID logo, CITATION.cff, README updates, file uploads
- **Then:** 2+ years of silence

**The story:** On February 12, 2024, one person (K Collins) made the OpenAir-Cyan project "official." Added the OSHWA certification logo. Created a formal citation file. Uploaded the final hardware documentation. This was the v1.0 release. But then nobody touched it for over two years.

**The question:** Is OpenAir-Cyan the beginning of open-source hardware for carbon capture — or is it a proof of concept that demonstrated the process but couldn't sustain momentum?

**Sound bite:** *"Six commits. One day. An OSHWA certification number. And then silence. The first open-source carbon capture machine got its papers in order and then... nobody built version two."*

### Carbon-Capture-and-Storage — The Academic Ghost

**The setup:** 85 stars. The most popular carbon capture repo on GitHub. Reservoir simulation, rock physics, seismic modeling, geomechanics for CCS monitoring.

**The commits:**
- **May 2020:** 1 commit (created with Google Colab)
- **Feb 2021:** 1 commit (geomechanics data)
- **Mar 1-6, 2021:** 7 commits (thesis package: simulation results, notebooks, cleanup)
- **Then:** 4+ years of silence

**The story:** On March 6, 2021, the author made 6 commits in one day. Simulation results were packaged. Folders were reorganized. Intermediate files were deleted. The thesis was submitted. Then the repo went completely dark.

**The paradox:** 85 stars but zero maintenance. People are still finding and starring this repo. But it's a snapshot of a BSc thesis from 2021, not a living tool. The stars measure citations, not usability.

**Sound bite:** *"85 people starred this repo. But the last real work happened on March 6, 2021 — thesis packaging day. The most-starred carbon capture project on GitHub is a time capsule."*

---

## Act 3: The One-Person Field

### Carbon_Capture_ML — The Lone Surveyor

**The setup:** The definitive survey of carbon capture machine learning papers. "For the benefit of all humanity." 56 stars. Single author.

**The commits:**
- **Feb 2-5, 2023:** 4 commits in 4 days (paper storm: MOFsimplify, process papers)
- **Mar 2023:** 1 commit (new paper)
- **...10 months...**
- **Jan 2024:** 2 README updates (preparing for new paper)
- **Mar-Apr 2024:** 2 README updates
- **May 8, 2024:** **OpenDAC paper added** (the most significant addition)
- **...16+ months...**

**The pattern:** This is a paper-driven lifecycle. Bursts of additions tied to publication deadlines, then long gaps while the field consolidates, then another burst. The OpenDAC addition (May 2024) represents the most current, high-impact research in DAC materials.

**The question:** Can a field be built on one person's shoulders? Zikri Bayraktar is the only person maintaining the definitive ML survey for carbon capture. What happens when he graduates? What happens when he moves on?

**Sound bite:** *"The definitive survey of machine learning for carbon capture is maintained by one person. He works in bursts: four papers in four days, then ten months of silence. This is both the strength and the fragility of open-source science."*

---

## Act 4: The CC0 Revolution

**The setup:** In September 2025, two repositories — `DAC_peroxovanadates` and `DAC_peroxotitanates` — both adopted the CC0 public domain license. Both are computational screening datasets for potential DAC sorbent materials. Both were updated on the same day (September 23, 2025).

**The pattern:** CC0 is not the standard open-source license (MIT, Apache, GPL). It's a "no rights reserved" dedication. By adopting CC0, the researchers are saying: "This data is not ours. It belongs to everyone. Use it however you want."

**The parallel movement:** OpenAir-Cyan uses OSHWA (open-source hardware certification). The DAC_peroxovanadates/titanates repos use CC0 (public domain data). These are two different answers to the same question: **How do you make carbon capture research legally open?**

- **Hardware side:** OSHWA gives you a certification number, a badge, community recognition
- **Data side:** CC0 gives you public domain status, no legal ambiguity, maximum reuse

**Neither movement has merged.** They're operating in parallel, with different communities, different norms, different legal frameworks.

**Sound bite:** *"Two groups of researchers are trying to solve the same problem — how to make carbon capture open — and they don't even know about each other. One is certifying hardware. The other is abandoning copyright. Both are right. Both are incomplete."*

---

## The Three Commit Patterns (Synthesis)

| Pattern | Repo | Signature | What It Tells Us |
|---------|------|-----------|------------------|
| **Ceremonial** | OpenAir-Cyan | 6 commits/1 day, then freeze | Hardware projects have a "launch day" then maintenance gap |
| **Academic Ghost** | Carbon-Capture-Storage | 6 commits/1 day, then 4yr silence | Thesis repos are snapshots, not living tools |
| **Paper Pipeline** | Carbon_Capture_ML | Bursts, then 10mo gaps, then bursts | Literature surveys track publication cycles |
| **Institutional** | Open-Sustainable-Technology | 3-4 commits/month, every month | Only directories get sustained maintenance |

**The uncomfortable truth:** The only carbon capture repo with consistent, ongoing development is a *directory* — not a tool, not a device, not a model. The ecosystem is maintained; the technology is not.

---

## Key Themes for Discussion

1. **The $1000/ton gap** — The DOE target for DAC is $1000/ton (recently slashed to $100/ton). No open-source repo is actively working on cost reduction. The active repos are directories, surveys, and certified hardware. The cost-reduction work is happening in secret, in national labs and well-funded startups.

2. **The citation ghost problem** — 85 stars on a dead repo. Is that a success or a failure? The repo is cited, referenced, starred — but nobody maintains it. This is the academic incentive problem: publish or perish, but maintain or ... ?

3. **The one-person dependency** — Carbon_Capture_ML is a one-person operation. What's the continuity risk? What's the succession plan? This is true for most niche open-source science projects.

4. **The CC0 vs. OSHWA fork** — Two legal frameworks for two different media. Neither has won. Neither has merged. The carbon capture open-source community is fragmented before it even forms.

---

## Recommended Listening Queue (Related Repos)

| Repo | Why Listen | Stars | Status |
|------|-------------|-------|--------|
| `protontypes/open-sustainable-technology` | The directory — only active repo, 2,552 stars | 2,552 | 🟢 Active |
| `openair-collective/openair-cyan` | The hardware — OSHWA-certified, then frozen | 76 | ⚠️ Frozen |
| `zikribayraktar/Carbon_Capture_ML` | The survey — one person, paper-driven | 56 | ⚠️ Dormant |
| `yohanesnuwara/carbon-capture-and-storage` | The ghost — 85 stars, dead since 2021 | 85 | 💀 Ghost |
| `tonyzyl/CO2-Soft-sensor` | The hybrid model — DAE-LSTM for CO2 sensing | 16 | ⚠️ Sparse |
| `Beckybams/AI-for-Carbon-Capture` | The AI optimization — synthetic industrial data | 25 | ⚠️ Dormant |
| `tjz21/DAC_peroxovanadates` | The CC0 revolution — public domain data | 2 | 🆕 New |

---

## Research Deep Dives (v9 Additions)

- [ ] OSHWA certification process and what US001095 means
- [ ] OpenDAC dataset and benchmark for DAC materials
- [ ] CC0 license implications for research data
- [ ] MOFsimplify (Metal-Organic Framework screening) methodology
- [ ] CO2 equation-of-state (EOS) modeling in reservoir simulation
- [ ] claude-carbon category in Open-Sustainable-Technology (AI governance signal)

---

## Research Log (v9)

| Date | Activity |
|------|----------|
| 2026-09-18 | v9: Episode brief synthesized from 9 repos, 100+ commits, fresh GitHub API data |
| 2026-09-18 | v9: Three commit patterns identified (Ceremonial / Academic Ghost / Paper Pipeline) |
| 2026-09-18 | v9: CC0 vs. OSHWA parallel movements documented |
| 2026-09-18 | v9: One-person dependency risk flagged for Carbon_Capture_ML |
| 2026-09-18 | v9: OpenAir-Cyan OSHWA certification story finalized |
| 2026-09-18 | v9: Carbon-Capture-and-Storage ghost paradox highlighted (85★ / dead since 2021) |
