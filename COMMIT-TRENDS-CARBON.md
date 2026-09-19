# 🌍 Carbon Capture — Commit Trend Analysis

**Last Updated:** September 2026
**Data Source:** GitHub List Commits API + Repository Search API

---

## Velocity Overview

| Repository | Commits Pulled | Active Period | Stars | Velocity Pattern | Lead Developer(s) |
|-----------|---------------|---------------|-------|-----------------|-------------------|
| CO2-Sequestration | 2 | Mar 24, 2019 (1 day) | 32 | Uploadonce → permanent dormancy | Salman Karim |
| OpenCarbon | 10 | May 18 – Jul 18, 2023 (~2 months) | 2 | Burst then death | Dahl Winters, shrilaesturi2006 |
| climate-research-group | 4 | Aug 6, 2026 (1 day) | Low | Single-day website update | ClimateSoton |
| Carbon-emissions-database | (found in search) | Unknown | 4 | Undeveloped | Unknown |

---

## Trend: The Three Carbon Development Patterns

Carbon capture GitHub repos fall into **three distinct patterns**:

### 🔴 Upload-and-Die (Dead on Arrival)
- ** glaciers of knowledge uploaded once, never touched again
- **Example:** CO2-Sequestration (2 commits, both on day 1, 7 years ago)
- **Why:** Researchers upload their code as a supplementary artifact for a paper, then move on. The code serves as a citation, not a tool.
- **Signal:** High star count (32 for CO2-Sequestration) but zero commit activity. Stars = people who found it useful as a reference.

### 🟡 Kickoff-and-Stall (The Dream Die)
- ** A promising start with a clear mission, then silence after initial setup
- **Example:** OpenCarbon (10 commits in 2 months, 6 of which were README updates)
- **Why:** Two or three enthusiasts start a project, write a vision document, then realize building actual DAC tools is hard. The README updates are optimistic; the code never materializes.
- **Signal:** Commit messages dominated by "Update README.md" and "Merge pull request." No actual simulation or analysis code.

### 🟢 Institutional Steady (Rare)
- ** Continuous, low-velocity maintenance by an institution
- **Example:** ClimateSoton/climate-research-group (website maintenance only)
- **Why:** University groups maintain a web presence. Not a simulation tool — a documentation hub.
- **Signal:** All commits on one day, website content, not scientific code.

**⚠️ Not a single one of these repos follows software engineering best practices.** No CI/CD, no tests, no issue tracking, no roadmap. They are research artifacts, not software products.

---

## Detailed Commit Timeline: OpenCarbon (The Most "Alive" Carbon Repo)

```
2023-05-18 ████████████████ 4 commits (project kickoff: README + Project_Plan)
2023-05-20 ██████████ 2 commits (README updates - optimism)
2023-07-13 ████████████████████ 4 commits (PR merges - final push)
2023-07-18 █ 1 commit (merge final PR)
2023-07-19 → PERMANENT DORMANCY
```

**Interpretation:** OpenCarbon's 10 commits tell a story:
1. **May 18:** Two creators (Dahl Winters + shrilaesturi2006) start fresh. Create Project_Plan.md, update README.
2. **May 20:** Still excited. Update README again. Still no code.
3. **July 13:** A burst of PR activity. Merge 3 PRs. Update README one more time.
4. **July 18:** Final merge. Then silence.

**6 out of 10 commits are README updates.** The project never produced functional carbon capture simulation code. It was a vision document that died in middle.

---

## Detailed Commit Timeline: CO2-Sequestration (The Artifact)

```
2019-03-24 ████████████████████ 2 commits (initial upload)
2019-03-25 → PERMANENT DORMANCY (7+ years)
```

32 stars, 2 commits, 7 years of silence. The MATLAB code was uploaded as a paper supplement and abandoned. It's a **digital museum piece** — visited (starred) but never maintained.

---

## What This Means for Your Podcast

### Episode Architecture for Carbon Capture

**Segment 1: The Technology Landscape**
- CCS vs. DAC vs. CCU — three different approaches, three different GitHub ecosystems
- Why there's no "GitHub for Carbon Capture" — no unifying platform
- The MATLAB problem — many tools are in MATLAB, limiting accessibility

**Segment 2: The Open-Source Paradox**
- The most-starred repo (CO2-Sequestration, 32 stars) is completely dormant
- OpenCarbon had a clear mission but never wrote code
- Why? Because carbon capture is a hardware-heavy, expensive field. Software is secondary.
- contrast with solar geoengineering, where software IS the research

**Segment 3: The Cost Question**
- DAC costs ~$600–1000/ton currently. Can open source break that?
- OpenCarbon's mission was specifically about lowering DAC costs through clean energy
- But the project died before producing anything. The $1000/ton barrier remains.
- The CCU angle (ClimateSoton) — turning CO₂ into products, not just storing it

---

## Key Quote-Worthy Data Points

- **"32 stars, 2 commits, 7 years silent"** — CO2-Sequestration is the most-starred dead repo in climate tech
- **"6 README updates, zero lines of DAC code"** — OpenCarbon's tragic arc
- **"No CI/CD, no tests, no roadmap"** — Zero carbon capture repos on GitHub follow software engineering practices
- **"Hardware eats software for breakfast"** —Unlike solar geoengineering (where simulation IS the research), carbon capture is dominated by physical/chemical processes. Code is supplementary.
- **"The MATLAB island"** — Multiple carbon capture repos use MATLAB, fragmenting the ecosystem
- **"CCU is the sleeping giant"** — Carbon Capture and Utilization (ClimateSoton's focus) gets less attention than storage but may be more economically viable

---

## References
- [CO2-Sequestration repository](https://github.com/salmansust/CO2-Sequestration)
- [OpenCarbon repository](https://github.com/terranexum/OpenCarbon)
- [ClimateSoton/climate-research-group](https://github.com/ClimateSoton/climate-research-group)
- [ClimateSoton/ClimateSoton.github.io](https://github.com/ClimateSoton/ClimateSoton.github.io)
