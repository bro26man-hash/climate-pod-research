# 🌊 Ocean Intervention — Open-Source Project Discoveries

## Branch: `ocean-intervention`
*Last updated by podcast research, Sept 2026*

---

## 1. The Big Finding: The Empty Quadrant

The most significant discovery from this research round is what **isn't** on GitHub. After exhaustive searches for ocean geoengineering, ocean alkalinity enhancement, ocean fertilization, and related terms, **GitHub returned zero results** for ocean-based geoengineering projects.

Compare that to:
- ☀️ Solar geoengineering: ~10–15 repos (mostly legacy, some active)
- 🌍 Carbon capture: ~20+ repos (hardware, material-science, system-level)
- 🌊 Ocean intervention: **≈ 0 dedicated repositories**

This gap is itself the story.

---

## 2. Nearest-Proximity Projects

While no dedicated ocean geoengineering repositories exist, a few projects touch on ocean-adjacent topics:

### 🐋 Team50-Labs/NebuGrid-OpenSource — **0 ⭐**
**URL:** https://github.com/Team50-Labs/NebuGrid-OpenSource
**Last updated:** Aug 2026
**Focus:** Fog-harvesting & drip irrigation for arid coastal environments

**Commit history:** `988b673` (Aug 28, 2026) — Initial commit — README update.

**Podcast angle:** Not ocean geoengineering per se, but an ocean-adjacent climate adaptation project. Fog harvesting is surface-ocean-water interaction — a trivial form of "marine intervention," but with no deliberate climate forcing.

---

### 🔬 api-evangelist/clairity — **unlisted stars**
**URL:** https://github.com/api-evangelist/clairity
**Last updated:** Sep 16, 2026
**Focus:** API profile of Clairity Technology Inc. (LA-based climate-tech company)

A public-API catalog entry, not research code. Tracks how one LA-based climate-tech firm exposes its data. Clairity's work includes direct air capture — no ocean component.

---

### 🔬 api-evangelist/spiritus — **unlisted stars**
**URL:** https://github.com/api-evangelist/spiritus
**Last updated:** Sep 16, 2026
**Focus:** API profile of Spiritus Technologies (climate-tech company)

Same pattern — a metadata profile, not research code. Spiritus builds low-carbon industrial products.

---

## 3. Why Is Ocean Geoengineering Missing from GitHub?

Based on the absence of repositories and filtering further searches, several structural factors emerge:

| Factor | Explanation |
|--------|-------------|
| **Experimental complexity** | Ocean experiments require ship time, deployment infrastructure, and clean-water access — not someone's laptop |
| **Governance sensitivity** | Ocean fertilization and alkalinization are regulated under CBD, London Protocol, and national laws — researchers may avoid public code |
| **Institutional siloing** | Ocean geoengineering research is concentrated in a handful of institutions (WHOI, Scripps, GEOMAR) that publish in journals, not on GitHub |
| **Liberty & liability risk** | Unlike solar geoengineering (stratospheric injection) or carbon capture (point-source capture), ocean intervention has direct ecological impact — code could be misused |
| **Open-source culture mismatch** | Ocean science still runs on MATLAB, Fortran, and proprietary modeling platforms — the GitHub-native developer community hasn't penetrated this space |

---

## 4. What *Would* an Open-Source Ocean Intervention Repo Look Like?

If the GitHub community were to build the missing ocean quadrant, the most likely starting points are:

1. **Ocean Alkalinity Enhancement (OAE) modeling** — Python notebooks for modeling basalt dissolution kinetics in seawater pH adjustment
2. **Iron fertilization impact simulators** — Agent-based models of phytoplankton bloom dynamics, adapted from existing ocean biogeochemistry frameworks
3. **Seaweed/macroalgae cultivation optimizers** — Open toolkits for kelp farm planning, carbon sequestration accounting
4. **Marine ethic & governance frameworks** — Open-source regulatory analysis tools, not just code

The closest existing analogues are marine biogeochemistry models like **CESM2's ocean biogeochemistry module** or **NEMO-PISCES**, but these are institutional Fortran monoliths, not GitHub-native projects.

---

## 5. The "Ocean Data" Adjacent Landscape

While code is absent, ocean *data* infrastructure exists:
- **CMIP6 ocean datasets** — accessible via tools like `xarray` and `ESMValTool`
- **NOAA ocean observation APIs** — public, but not geoengineering-specific
- **Global Ocean Biogeochemistry (GLODAP) model** — legacy, not on GitHub as an independent repo

The data exists. What's missing is the open-source layer that would allow community experimentation with ocean intervention scenarios.

---

## 6. Commit Trend Summary (Ocean)

| Finding | Detail |
|---------|--------|
| Dedicated ocean geoengineering repos | **Zero** found across all search queries |
| Nearest-adjacent activity | Team50-Labs/NebuGrid: 1 commit, Aug 2026 |
| API/metadata profiles only | Clairity & Spiritus: Sep 2026, no code |
| GitHub search queries returning nothing | "ocean geoengineering", "ocean alkalinity", "ocean fertilization", "alkalinization" |

**Bottom line for the episode:** Ocean geoengineering is the missing quadrant of open-source climate tech. The next great podcast angle: what would it take to build an open-source community around ocean intervention modeling — and would we *want* to?
