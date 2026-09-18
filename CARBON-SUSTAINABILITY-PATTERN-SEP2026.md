# 🌍 The Burst-and-Freeze Pattern: Why Carbon Capture Can't Sustain
## Structural Diagnosis — September 2026

---

## The Data

Every carbon capture repository follows the same lifecycle:

```
CREATION → BURST → PEAK → SILENCE → DORMANCY
```

| Repo | Creation | Burst | Peak | Silence | Current |
|------|----------|-------|------|---------|---------|
| OpenAir-Cyan | May 2022 | May-Jul 2022 + Feb 2024 | OSHWA cert (Feb 2024) | Feb 2024 → now | ❌ Frozen |
| dac-moving-bed | Unknown | Jul 3, 2026 (8/day) | Complete system | Jul 2026 → now | ❌ Frozen |
| Carbon_Capture_ML | Feb 2023 | Feb 2023 (4/4 days) | Full survey | May 2024 → now | ⚠️ Quarterly |
| OpenCarbon | May 2023 | May-Jul 2023 | Full plan | Jul 2023 → now | ❌ Dormant |
| CC-and-Storage | Pre-2021 | Unknown | 85★ | Mar 2021 → now | ❌ Ghost |
| Open-Sust-Tech | Ongoing | Continuous | Still growing | N/A | ✅ **Active** |

**5 out of 6 repos are non-functional. The 6th is a directory, not a technology.**

---

## Root Cause Analysis

### 1. The Hardware Gap
DAC isn't just software — it's machines that suck CO₂ out of the air. You can model the chemistry in code, but you need fans, filters, and heat exchangers. Software repos can't test hardware.

### 2. The Expertise Bottleneck
DAC requires: thermodynamics + materials science + chemical engineering + control systems + software development. Finding one person who knows all five is rare. Finding five who will contribute to a GitHub repo is rarer still.

### 3. The Academic Incentive Mismatch
Academics publish papers. They don't maintain software. The incentive structure rewards new publications, not bug fixes.

### 4. The Corporate Displacement
Major DAC companies (Climeworks, Carbon Engineering, 44.01) develop internally. Their engineers use internal tools, not public repos.

### 5. The Funding Vacuum
Software maintenance requires sustained funding. Climate science grants fund research, not maintenance. The NSF doesn't have a "Code Sustainability" program line item.

---

## Why Open-Sustainable-Technology Survives (And They Don't)

| Factor | Directory | Technology |
|--------|-----------|------------------------|
| **Entry barrier** | Low (add a link) | High (domain expertise) |
| **Contribution model** | Distributed (many adds) | Centralized (specialist code) |
| **Maintenance need** | Minimal (link checking) | High (dependabot, testing) |
| **Value persistence** | Reference data doesn't expire | Code needs updates |
| **Community size** | Anyone can contribute | Few specialists |

**The lesson:** Low-barrier, distributed contribution models sustain. High-barrier, specialized models don't.

---

## The Fix? A Structural Proposal

### 1. The DAC Analogues to Bioinformatics
Bioinformatics survived because it created standardized data formats, centralized databases, automated pipelines, and community curation. Carbon capture needs equivalents:
- **Standardized sorbent formats** (like "SorbentBAM")
- **Centralized screening databases** (like "DAC-we、文明")
- **Automated simulation pipelines** (like "DAC-Bowtie")
- **Community standards bodies**

### 2. Maintenance as a Publication Category
Journals should recognize code maintenance as a research contribution. If maintaining a repo is as valuable as publishing a paper, academics will maintain repos.

### 3. Corporate Open-Source Programs
Companies like Climeworks should have "open-source days" where engineers contribute to public repos. The Linux Foundation has proven this model works.

### 4. DOI for Code
If every significant commit gets a DOI, maintenance becomes citable.

---

## Episode Discussion Prompts

1. "Is burst-and-freeze the natural lifecycle of climate tech on GitHub?"
2. "Should we raise the 'maintainer' flag — or lower the 'contributor' bar?"
3. "What would make YOU contribute to a DAC repository? Money? Credit? Fun?"
4. "Is the answer not more code, but better incentives?"
5. "What's the quote-unquote 'GitHub model' for ocean alkalinity enhancement?"

---

*Structural diagnosis based on commit pattern analysis across 6 repositories, September 2026.*