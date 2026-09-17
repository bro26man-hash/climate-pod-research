# 03 — Ocean Intervention Episode: Research Overview

> **Episode Theme:** 🌊 Ocean-Based Geoengineering
> **Research Date:** 2026-09

---

## Episode Premise

Why is ocean geoengineering the empty quadrant of GitHub? This episode investigates ocean alkalinity enhancement, iron fertilization, seaweed cultivation, and the systemic reasons why open-source ocean climate research barely exists — and what it would take to change that.

---

## 🔍 Open-Source Ocean Intervention Projects Discovered

| Repo | Stars | Language | Last Update | Description |
|------|-------|----------|-------------|-------------|
| **CrayLabs/NCAR_ML_EKE** | 20 | Jupyter | Aug 2022 | ML at scale in HPC for ocean climate modeling (MOM6) |
| **Team50-Labs/NebuGrid-OpenSource** | 0 | — | Aug 2026 | Fog-harvesting & drip irrigation (coastal water tech) |
| **openair-collective/openair-sorbent-tester** | 3 | Python | Jan 2026 | (Relevant) Sorbent testing for marine DAC applications |
| **PSLmodels/Geo-DICE** | 2 | MATLAB | Aug 2018 | (Cross-cutting) DICE model includes ocean carbon feedback |

### Notable Absences

After extensive searching, **no dedicated ocean geoengineering repositories** were found for:
- Ocean alkalinity enhancement (OAE)
- Iron fertilization
- Seaweed/kelp cultivation monitoring
- Marine cloud brightening over oceans
- Ocean upwelling/downwelling simulation
- Deep ocean carbon storage modeling

---

## 📊 Commit Trend Analysis (Ocean Intervention)

### NCAR_ML_EKE (CrayLabs)
⭐ **20 stars | Jupyter Notebook | Dormant (2021–2022)**

| Commit | Author | Date | Summary |
|--------|--------|------|---------|
| `5b2d6cf` | Andrew Shao | Mar 30, 2022 | Fix notebook typos (#10) |
| `c4028e5` | Andrew Shao | Mar 28, 2022 | Refactor driver for colocated option (#9) |
| `aa0abc8` | Sam Partee | Mar 14, 2022 | Update MOM6 instructions and submodule |
| `6586405` | Andrew Shao | Feb 9, 2022 | Update README for compiling MOM6 |
| `962e6c6` | Andrew Shao | Feb 8, 2022 | Update MOM6 submodule |
| `b30698f` | Sam Partee | Jul 23, 2021 | Edit README |
| `b300602` | Sam Partee | Apr 13, 2021 | Create LICENSE |
| `90b0430` | Sam Partee | Apr 13, 2021 | Update README.md |

### Trend Insights
- **MITgcm's MOM6 ocean model:** This is the gold-standard ocean circulation model used in IPCC-class simulations — performance via ML at HPC scale
- **NCAR + Cray collaboration:** Supercomputing power meets ocean modeling — exactly the infrastructure needed for ocean geoengineering simulation
- **Active maintenance but no new features:** The 2021–2022 commits are all maintenance/docs, not new science — suggests the project reached a stable tool state
- **Two-complementor model:** Andrew Shao (ML/driver code) + Sam Partee (documentation/compilation) — complementary skills
- **Trend sign:** This is the closest thing to open-source ocean climate simulation, but it's an HPC infrastructure project, not a geoengineering tool

---

## 🌊 The Ocean Intervention Gap: Why Nothing Exists

This is the most significant finding across all three episode themes. The near-total absence of ocean geoengineering on GitHub is not an accident. Here's why:

### 1. Experimental Complexity
Ocean geoengineering experiments (like OAE or iron fertilization) require massive physical deployments — ships, monitoring equipment, controlled release sites. You can't simulate these on a laptop. The barrier to open-source participation is extraordinarily high.

### 2. Governance Sensitivity
Ocean interventions in international waters fall under UNCLOS (UN Convention on the Law of the Sea) and the London Protocol. Many nations and institutions view ocean geoengineering as legally and politically fraught. Researchers are understandably cautious about open-sourcing work that could be perceived as unauthorized deployment.

### 3. Institutional Siloing
Ocean research is dominated by a small number of well-funded institutions (WHOI, Scripps, GEOMAR, CSIRO) with proprietary data policies. The culture is less open-source than atmospheric science communities.

### 4. Simulations ≠ Experiments
Unlike SRM (where you can model radiative transfer on a laptop) or DAC (where you can test sorbents in a lab), most ocean interventions require actual ocean deployment to validate. The "simulation gap" is therefore much wider.

### 5. Funding Psychology
Ocean geoengineering carries the highest reputational risk for funders. No venture capital, no climate-tech accelerators, few philanthropic grants. Without funding, there's no lab, no GitHub repo, no community.

---

## 🎙️ Episode Talking Points

1. **The Empty Quadrant:** Ocean intervention has the least open-source presence of any climate tech domain. This episode should explore why — it's a story about risk, not just technology.
2. **ML + Ocean = The Bridge:** NCAR_ML_EKE shows that ML-driven ocean simulation is a viable entry point for open-source ocean climate work. MOM6 + ML could democratize ocean modeling.
3. **What Would Open-Source OAE Look Like?:** Ocean alkalinity enhancement is the most "open-source-able" ocean intervention — it's essentially a chemistry experiment at scale. A community could design and test alkalinity enhancement protocols in coastal waters.
4. **Governance as Code:** One potential angle is building open-source governance frameworks for ocean intervention — modeling the legal/ethical dimensions, not just the physical ones.
5. **Coastal Water Tech Start:** The fog-harvesting/drip irrigation niche (NebuGrid) could be an on-ramp for ocean-adjacent community science.

---

## ⚠️ Key Risks & Uncertainties
- Ocean geoengineering carries profound ecological risks that are poorly understood — open-source advocacy must not outpace scientific caution
- International law frameworks are still being developed; the legal landscape is uncertain
- Most ocean climate models are output-restricted by institutions; the data gap is as much policy as technology
- ML-driven ocean simulation (NCAR_ML_EKE) is promising but requires HPC access that community researchers don't have
