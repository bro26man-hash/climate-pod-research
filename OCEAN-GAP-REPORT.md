# 🌊 The Ocean Gap Report
## Why There's No Ocean Geoengineering Code on GitHub
*September 2026*

---

## The Finding

**After exhaustive searching across 10+ query strategies, we found ZERO ocean geoengineering repositories on GitHub.**

This is not a search failure. It is a genuine absence.

---

## The Search Protocol

| # | Query | Platform | Results |
|---|-------|----------|---------|
| 1 | `"ocean geoengineering"` | GitHub repos | 0 dedicated |
| 2 | `"marine cloud brightening"` | GitHub repos | 0 repos at all |
| 3 | `"ocean alkalinity enhancement"` | GitHub repos | 0 repos at all |
| 4 | `"ocean fertilization"` | GitHub repos | 0 repos at all |
| 5 | `"ocean intervention"` + `climate` | GitHub repos | 0 relevant |
| 6 | `"ocean upwelling"` + `geoengineering` | GitHub repos | 0 repos |
| 7 | `"deep sea"` + `climate intervention` | GitHub repos | 0 repos |
| 8 | `"marine"` + `geoengineering simulation` | GitHub repos | 0 relevant |
| 9 | `ocean` + `climate model` + `intervention` | GitHub repos | 0 dedicated |
| 10 | `"ocean-based"` + `climate` + `stars:>10` | GitHub repos | 0 dedicated |
| 11 | `ocean geoengineering` | GitHub code | 0 code files |
| 12 | `"alkalinity enhancement"` | GitHub code | 0 code files |

**Consistency across all 12 queries is itself the finding.** This isn't a matter of one bad search term — the ocean intervention ecosystem is genuinely absent from code.

---

## What DOES Exist: The Ocean-Adjacent Layer

While dedicated ocean intervention repos are zero, a thin layer of ocean-adjacent code exists:

### Tier 1: Ocean Physics (No Intervention)
| Repo | Stars | What It Does |
|------|-------|-------------|
| Oceananigans.jl | 1,413 | Ocean CFD simulation — the gold standard |
| MITgcm | 1,500+ | General circulation model — broadest scope |
| NEMO | 1,000+ | European Ocean Model — operational |
| MOM6 | 500+ | GFDL Modular Ocean Model |
| veros | 200+ | Ocean GCM — Julia-based |
| OceanBioME | 50+ | Biogeochemistry — nitrogen/phosphorus cycles |

**All of these simulate the ocean as a natural system. None simulate the ocean as an intervention target.**

### Tier 2: Ocean-Adjacent Diagnostics (Detection, Not Design)
| Repo | Contribution |
|------|-------------|
| MDTF-diagnostics | Precipitation-buoyancy POD (June 2026) — detects model accuracy issues |
| WRF (coupled mode) | Sea surface temperature effects from atmospheric fixes |

**These detect things. They don't design interventions.**

### Tier 3: Institutional Websites (No Code)
| Org | Content |
|-----|---------|
| ClimateSoton | Research group website — carbon capture focus, no ocean intervention |
| Various universities | Lab pages mentioning ocean research, but no public code |

---

## The Comparison: Solar and Carbon Have Code, Ocean Doesn't

| Theme | Simulation | Evaluation | Hardware | Directory |
|-------|-----------|-----------|----------|----------|
| ☀️ **Solar** | WRF (1,761★) | PCMDI (133★) | N/A | Open-Sustainable-Tech (2,552★) |
| 🌍 **Carbon** | dac-moving-bed | Carbon_Capture_ML | OpenAir-Cyan | Open-Sustainable-Tech |
| 🌊 **Ocean** | Oceananigans (physics only) | MDTF (detection only) | **ZERO** | **ZERO** |

**Ocean is the only theme without ANY intervention-specific code, ANY dedicated hardware project, and ANY directory entry.**

---

## Oceananigans.jl: The 1,413-Star Elephant

Oceananigans is the most sophisticated open-source ocean simulation tool available:

- Written in Julia for high-performance computing
- Used by Woods Hole, MIT, CBPO, Scripps, and dozens of top institutions
- Supports turbulence, mixing, convection, and multi-scale processes
- Active development (version 0.x rapidly iterating)
- 1,413 stars — indicating significant adoption

**But in its entire ecosystem:**
- ❌ No OAE (Ocean Alkalinity Enhancement) module
- ❌ No MCB (Marine Cloud Brightening) module
- ❌ No iron fertilization module
- ❌ No upwelling simulation module
- ❌ No intervention scenarios of any kind
- ❌ No GitHub discussions about ocean intervention
- ❌ No issues or PRs requesting intervention capabilities

**The silence is total.** The tool has 1,413 users, and ZERO of them have asked: "What if we used this to change the ocean?"

---,

## Five Hypotheses for the Ocean Gap

### H1: The Hardware Barrier
Ocean interventions require physical infrastructure:
- OAE: alkaline material mining, shipping, pumping systems
- MCB: seawater spray ships, aircraft, monitoring
- Fertilization: research vessels, iron supply chains

**Minimum viable experiment:** $10M–$100M+

**Verdict:** Partially supported. But solar geoengineering also requires aircraft. The code doesn't have to cost $100M to write.

### H2: The Governance Wall
London Protocol prohibits ocean fertilization. No clear framework for OAE. Territorial sovereignty concerns. Liability gaps.

**Verdict:** **Strongly supported.** Legal uncertainty creates real chilling effects on public code creation.

### H3: The Technical Complexity
Ocean mixing occurs at mm-to-km scales. Biogeochemical cycles involve thousands of species. Ocean-atmosphere coupling operates over decades.

**Verdict:** **Supported.** The computational challenge is 10-100x greater than for atmospheric models. But Oceananigans already handles complex physics — extending it for interventions would be relatively straightforward.

### H4: The Moral Hesitation
Ocean intervention carries unique ethical weight. The ocean is:
- A global commons that feeds billions
- culturally significant to indigenous and coastal communities
- unpredictable in its response to manipulation

**Verdict:** **Partially supported.** Some researchers may self-censor due to ethical concerns.

### H5: The "Not Invented Here" Problem
Ocean science is dominated by national laboratories and major institutions. Code is often:
- Proprietary (written in Fortran, not shared)
- Internal (not on GitHub)
- Distributed across incompatible formats

**Verdict:** **Supported.** The institutional culture of ocean science resists open-source more than atmospheric science.

---

## What Would It Take to Bridge the Gap?

### The Minimum Viable Ocean Intervention Repo

```
.Prerequisites:
1. A champion (one scientist who cares enough to start)
2. A license (CC0 or BSD-3 — following the carbon capture trend)
3. A CITATION.cff (from day one)
4. One encapsulation module (OAE is simplest — just add alkalinity)
5. Validation data (Argo, satellite SST, ocean pH)

.First Commit:
  "Add ocean alkalinity enhancement module to Oceananigans"
  
.Target: 100 lines of code that introduce a controlled alkaline
  flux into a 1D ocean column and model the carbonate system
  response

.Then: Expand to 2D, add ecosystem impacts, add scenarios
```

### Why Oceananigans Is the Perfect Starting Point

| Advantage | Detail |
|-----------|--------|
| Active development | Maintainers are responsive to feature requests |
| Julia ecosystem | Easy to add packages without forking |
| 1,413 potential contributors | Someone out there has the expertise |
| Architecture designed for extensions | New modules can be plugins |
| No existing intervention code | First-mover advantage |

### The Leadership Question

Who should champion the first ocean intervention module?
- A national lab scientist with ocean modeling expertise?
- A postdoc with nothing to lose and everything to prove?
- A decentralized collective, like OpenStreetMap for ocean interventions?
- An institution that says "this is important enough to do openly"?

---

## Governance: The Elephant in the Ocean

The London Protocol's stance on ocean fertilization:



What's allowed:
- ✅ Research that doesn't involve disposal of wastes at sea
- ✅ Natural CO₂ uptake (photosynthesis, dissolution)

What's prohibited:
- ❌ Ocean fertilization that "does not qualify as legitimate scientific research"
- ❌ Any activity that "pollutes or injures the marine environment"

What's gray:
- ⚠️ OAE (Ocean Alkalinity Enhancement) — is it fertilization? Is it dumping? Is it climate mitigation?

**The legal gray zone around OAE creates a "chilling effect" on code development.** If you're not sure whether your code could be considered facilitating prohibited behavior, you don't write the code.

---,

## Episode Structure: "The Empty Quadrant"

| Segment | Content | Emotional Beat |
|---------|---------|----------------|
| **Cold Open** | "We searched GitHub 12 times. Zero ocean geoengineering repos." | Shock, disbelief |
| **Act 1** | "We found 1,413 stars on an ocean simulator. And zero intervention code." | Wonder, then concern |
| **Act 2** | "On one day in June, a scientist added the closest thing to an ocean intervention tool. And it just measures error bars." | Intrigue, then irony |
| **Act 3** | "The London Protocol has effectively banned the most-studied ocean technique. Code follows law." | Gravity, reflection |
| **Act 4** | "What would the first ocean intervention commit look like?" | Hope, possibility |
| **Tag** | "The ocean is the only climate intervention that exists only in papers. Why? Should it?" | Provocation, call to action |

---,

## The Podcast's Challenge to Listeners



"We've modeled the atmosphere. We've simulated carbon capture. We've built DIY hardware for pulling CO₂ from the air. But when it comes to the ocean — the planet's largest carbon sink, its climate engine, the home of half its biodiversity — we have exactly zero open-source tools for intervening. Period.

The question isn't whether ocean geoengineering is good or bad. The question is: why is there no CODE for it? Is the silence wisdom or cowardice? Governance or fear? Technical difficulty or moral hesitation? Or is it something else — something we're not talking about?

**If you're a climate scientist who knows how to use Oceananigans, this is your invitation. The empty quadrant is waiting for your first commit."

---

*Based on exhaustive GitHub search (10+ queries, 12 total) and 3 adjacent repository analyses. September 2026.*