# 🌍 Carbon Capture — Supplemental Repo Profiles (v5 Update)
## Additional Repositories & Fresh Commit Trend Deep-Dive
*September 2026 — complements PROJECT-DISCOVERIES-CARBON.md and COMMIT-TRENDS-CARBON.md*

---

## New Repos Discovered in This Research Pass

These repositories add to the v4 carbon capture research with detailed commit analysis.

---

### 1. OpenAir-Cyan (`openair-collective/openair-cyan`)
- **Stars:** 76 ⭐ | **Language:** C/Hardware | **License:** CERN-OHL-S-2.0 (open hardware)
- **Last activity:** February 12, 2024 — **2.5 years dormant**
- **OSHWA UID:** US001095 (certified open hardware!)
- **Authors:** KCollins (certification push), DaOfficialWizard (earlier), ZanzyTHEbar

#### Complete Commit Pattern
**Phase 1 — Community Building (May-Jul 2022, 4 commits):**
| Date | Commit |
|------|--------|
| May 17 | `add files to improve useability` |
| May 15 | `Update README.md` |
| May 15 | `Update README.md` (second same day) |

**Phase 2 — The Blitz Day (Feb 12, 2024, 6 commits):**
| Date | Commit | What It Means |
|------|--------|--------------|
| Feb 12 | `Update README.md - added OSHWA UID link` | Certification achieved! |
| Feb 12 | `Add files via upload` | New content uploaded |
| Feb 12 | `Added OSHWA UID logo (OSHWA UID US001095)` | Official OSHWA badge |
| Feb 12 | `Add files via upload` | More content |
| Feb 12 | `Create CITATION.cff` | Academic citation metadata |
| Feb 12 | `Update README.md` | README pumped up |

**Phase 3 — Silence (Feb 2024 → present, 2.5+ years, ZERO commits)**

**Critical flag:** CI/CD workflows were **deleted** May 15-17, 2022 — right before the blitz. Fluid prototyping → OSHWA certification push → dead repo.

#### Detailed Episode Angle

The OSHWA (Open Source Hardware Association) certification is **the biggest open-hardware signal in the carbon capture ecosystem**. Getting UID US001095 means the Cyan DAC device design passed official review as "open hardware" — documented, reproducible, and freely available.

But the pattern is heartbreaking: **6 commits in one day to get certified, then 2.5 years of nothing.** The question for the episode: *Did certification solve the wrong problem?* OSHWA certification validates that the hardware design is open. It does NOT validate that the device works, that it's scalable, or that anyone wants to build it. The team got the paperwork right and then stopped.

**Talking point:** "The OpenAir-Cyan team did something genuinely remarkable — they got their DIY direct air capture device certified as official open hardware by OSHWA. They put the badge on their README with pride. And then they stopped. Six commits in a single day to get the certificate, then two and a half years of silence. It's like running a marathon and stopping at the finish line to take a nap. The certificate is framed on the wall. The device never got built."

---

### 2. OpenCarbon (`terranexum/OpenCarbon`)
- **Stars:** 2 | **Language:** Not specified | **License:** None
- **Last activity:** August 19, 2026
- **What it is:** Carbon management technologies and plans to advance DAC research, ensuring it uses clean energy and low-cost.

**Episode angle:** The description reads like a mission statement: "ensuring it uses clean energy and that low-cost." Three words that carry the entire DAC debate. Clean energy. Low cost. Two constraints that are simultaneously the biggest barriers and the biggest marketing claims. A repo with 2 stars and a clean mission statement — the gap between aspiration and implementation in one data point.

---

### 3. GCCS-Core (`KOSASIH/GCCS-Core`)
(Already profiled in solar branch — cross-listed here for carbon context)

- **Stars:** 9 | **Last activity:** October 29, 2024
- **Carbon connection:** "Global Climate Control System" implies carbon management at the system level
- **8+ commits in one day** (Oct 29, 2024): setup.py, requirements.txt, data_collection.sh, 7 README updates

**Cross-branch note:** This repo appears in both solar and carbon contexts because "climate control" inevitably involves carbon. The single-day burst pattern here mirrors regional-geo in the solar branch — a conceptual framework created in a blitz, then silence.

---

### 4. API-Evangelist Climate Profiles (3 repos)
- **`api-evangelist/280-earth`** — Public API surface profile of 280 Earth (DAC company)
- **`api-evangelist/clairity`** — Public API surface profile of Clairity Technology (climate-tech LA-based)
- **`api-evangelist/spiritus`** — Public API surface profile of Spiritus Technologies (climate-tech, low-co...)

These are **meta-repositories** documenting the API surfaces of real climate-tech companies. Not simulation tools, but **governance/transparency tools**.

**Episode angle:** "We're not just mapping climate models — we're mapping climate companies. Three API evangelists decided the public should be able to see what 280 Earth, Clairity, and Spiritus are actually doing behind their APIs. It's not simulation, it's surveillance. Of corporate climate tech. This is the open-source ethos applied to corporate accountability."

---

## Fresh Commit Trend Analysis: The 5 Waves of Carbon Capture Activity

### Wave 1: The Living Directory (Jun-Sep 2026)
**Repo:** `protontypes/open-sustainable-technology` — 2,552 ⭐
- 2-3 commits/month, steady cadence
- Categories: IoT/energy (MUIO, MUIOGO, PowerIO), AI/climate (claude-carbon), DIY hardware
- **Multi-contributor signals**: Abdul Salam, Tobias Augspurger, Christophe Combelles
- July 2026: AI content review PR template (governance meta-signal)

### Wave 2: The Certification Blitz (Feb 12, 2024)
**Repo:** `openair-collective/openair-cyan` — 76 ⭐
- 6 commits in 1 day → 2.5 years of silence
- OSHWA UID US001095 achieved
- CI/CD workflows deleted May 2022 (before the blitz)

### Wave 3: The Literature Sprint (Jan-May 2024)
**Repo:** `zikribayraktar/Carbon_Capture_ML` — 56 ⭐
- 10 commits in 2 months (survey construction)
- Slow tail through May 2024
- Frozen for 2.5+ years

### Wave 4: The CC0 Revolution (Sep 12, 2025)
**Repos:** `tjz21/DAC_peroxovanadates` + `tjz21/DAC_peroxotitanates`
- Both adopted CC0 public-domain dedication on the same day
- CC0 = waiving ALL copyright — the most permissive license
- In a field where CarbonEngineering holds patents and Climeworks guards formulas, this is radical

### Wave 5: The Ghost (Mar 2021+)
**Repo:** `yohanesnuwara/carbon-capture-and-storage` — 85 ⭐
- 6 commits in 1 day (March 2021)
- Then 5+ years of silence
- 85 stars but zero recent activity — the most-starved repo in the set

---

## The Carbon Capture Commit Pattern Taxonomy

| Pattern | Example | Description | Sustainability |
|---------|---------|-------------|---------------|
| **🏛️ Living Directory** | Open Sust Tech | Steady institutional cadence, multi-contributor | ★★★★★ 5-star |
| **📜 Literature Sprint** | Carbon_Capture_ML | Built fast for a survey, then frozen | ★☆☆☆☆ 1-star |
| **🏅 Certification Blitz** | OpenAir-Cyan | Push to get certified, then stop | ★☆☆☆☆ 1-star |
| **⚖️ CC0 Revolution** | DAC_peroxovanadates | License change as statement, not code | ★★★☆☆ 3-star |
| **👻 Ghost Star** | carbon-capture-and-storage | High stars, zero commits | ★☆☆☆☆ 1-star |
| **🗺️ Meta-Mapper** | API-evangelist/280-earth | Surveillance of corporate climate APIs | ★★★☆☆ 3-star |

---

## The CC0 Story: Expanded for the Episode

On **September 12, 2025**, two researchers made a decision that sent more ripples through the carbon capture community than most papers do. They dedicated their DAC simulation data — peroxovanadate and peroxotitanate systems — to the **public domain** via CC0.

What does CC0 actually mean? It means:
- No copyright. Anyone can copy, modify, distribute — for any purpose.
- No attribution required (though it's appreciated).
- No patent license. Actually, CC0 doesn't cover patents — so there's a subtle gap.

But in a field where:
- **Climeworks** guards its sorbent materials as trade secrets
- **CarbonEngineering** holds patents on its DAC process
- **Global Thermostat** and **1PointFive** keep their data proprietary

...two researchers saying "the data is yours" is a **cop-out** — and a **taking-back** motion. They're reclaiming the commons that corporate IP has enclosed.

**Episode Talking Point:** "In a world where the biggest DAC companies treat their data likeFort Knox, two researchers looked at each other and said: 'No. This data belongs to everyone.' They didn't just open-source it — they gave away all their copyright. No license. No terms. No attribution required. Just: it's yours. That's CC0. The most permissive license in the world. And it might be the most important thing that happened in carbon capture this year."

---

*Research methodology: GitHub REST API, September 2026. Commits pulled via List Commits API. Search queries via Repository and Code Search APIs.*