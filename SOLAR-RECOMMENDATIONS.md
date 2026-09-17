# ☀️ Solar Geoengineering — Research Recommendations & Next Steps

---

## Immediate Actions

### 1. Contact WRF Maintainers
- **Target:** Anthony Islas (NCAR), weiwangncar
- **Ask:** Has the EOT solar radiation correction been validated against observational data? Are SRM-specific experiments recommended?
- **Approach:** Issue comment on the EOT fix commit requesting a follow-up suitable for SRM users

### 2. Revive ClimateMARGO Community
- **Target:** Fons van der Plas
- **Ask:** What prompted the August 2026 README update? Are there plans for new features?
- **Approach:** Open an issue expressing interest in contributing or a forum discussion

### 3. Fork GCCS-Core as a Genuine Climate Control Model
- **Target:** The GCCS-Core concept
- **Action:** This repo has infrastructure but no code. A fork with actual solar radiation management simulation code could fill a critical gap
- **Challenge:** The name is grandiose; a rename would be needed for credibility

### 4. Archive OOCC_2021 as a Historical Artifact
- **Target:** jlehtomaa
- **Action:** The governance model deserves preservation and possibly a modern rewrite. Consider forking with updated governance frameworks (e.g., the 2022 NASEM report recommendations)

---

## Longer-Term Research Direction

### The "SRM-FRAC" Proposal
Propose a **Solar Radiation Management Faithful Repo Attendance Counter** — a lightweight metric that tracks:
- Recent commits to solar-relevant physics code
- Number of active contributors to SGE-relevant repos
- Frequency of solar radiation scheme updates in major climate models
- Maintenance status of governance models

**Why?** The current ecosystem has no way to measure "are people actually building SGE code?" Stars measure popularity. Forks measure interest. Commits measure *action*.

### The "WRF-SGE Extension" Concept
Could WRF benefit from an official SGE module? Something like:
- A `wrf-sra` (Solar Radiation Adjustment) experimental physics suite
- Pre-configured namelists for α=1.0, 1.01, 1.02 solar constant perturbation experiments
- Community documentation on how to interpret WRF output for SRM attribution

**Precedent:** WRF already has specialized physics suites (MP, TP, Cum) maintained by different groups. An SRE physics group could follow the same model.

---

## Open Questions for the Episode

1. ** responsibility for invalidated results:** If WRF's solar radiation fix changes past SRM simulation results, who re-runs the experiments? Is there an SRE replicability crisis?

2. ** The single-maintainer bottleneck:** 4 of 6 solar repositories have exactly 1 contributor. What happens when the maintainer burns out? Is there a succession plan?

3. ** Governance code preservation:** Is there a version-control equivalent of the "private archive" for dead governance code? Who maintains the knowledge of what OOCC_2021 tried to do?

4. ** The naming problem:** "GCCS-Core" (Global Climate Control System) vs. "OOCC_2021" (obscure acronym) vs. "ClimateMARGO" ( MARGO = Mitigation, Adaptation, Geoengineering Optimization). How does naming affect whether policymakers take SGE research seriously?
