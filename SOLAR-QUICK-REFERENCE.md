# ☀️ Solar Geoengineering — Quick Reference Card
## Climate Pod Research | September 2026

---

## The Six Repos At-a-Glance

| Repo | Stars | Language | Last Commit | Pattern | SRM Relevance |
|------|-------|----------|-------------|---------|--------------|
| **wrf-model/WRF** | 1,763 | Fortran | Jun 8, 2026 | Steady institutional | ★★★★☆ (physics foundation) |
| **PCMDI/pcmdi_metrics** | 133 | Python | Sep 17, 2026 | Burst release | ★★★★☆ (evaluation infrastructure) |
| **NOAA-GFDL/MDTF-diagnostics** | 80 | Python/R | Aug 14, 2026 | POD-driven | ★★★☆☆ (process evaluation) |
| **ClimateMARGO/ClimateMARGO.jl** | 73 | Julia | Aug 17, 2026 | Ghost dormant | ★★★☆☆ (optimization theory) |
| **yanpefnsc/orbital-climate-simulator** | 2 | Python | Sep 16, 2026 | Rapid prototype | ★★☆☆☆ (operational concept) |
| **hausfath/srm-forever** | 0 | Python/Markdown | Aug 26, 2026 | Single-day launch | ★★☆☆☆ (economic theory) |

## Key Dates Timeline

```
May 12 ─── WRF: MYNN-SFC submodule update
May 20 ─── WRF: New PBL scheme (ShinHong) + TEMPO messaging
May 26 ─── WRF: CDXWRF module fix + GFL README
May 28 ─── WRF: ★ SOLAR RADIATION FIX (EOT calculation correction)
Jun  5 ─── WRF: ★ Aerosol-aware physics DEPRECATED (tempo_aerosolaware off)
Jun  8 ─── WRF: v4.8.0 released
Jun 19 ─── MDTF: ★ 5 commits on precip-buoyancy POD (same file)
Aug 17 ─── ClimateMARGO: ★ Ghost revival (2 README updates, 0 code)
Aug 26 ─── srm-forever: ★ 4 commits — Weitzman discounting model launched
Sep  3 ─── PCMDI: Dask SVD memory optimization
Sep  4 ─── PCMDI: ★ v4.2.1 released — 10 commits, roundoff fix
Sep 15 ─── Orbital-Sim: ★ 12 commits begin — drone fleet prototype
Sep 16 ─── Orbital-Sim: ★ Streamlit dashboard + documentation sprint
Sep 17 ─── PCMDI: Final v4.2.1 patch merged
```

## The Three Development Patterns

### 1. Steady Institutional (WRF, MDTF)
- Multiple contributors across organizations
- Consistent weekly pace
- Phased releases with documentation
- **Podcast framing:** "The establishment"

### 2. Burst Release (PCMDI)
- Weeks of preparation
- Single-day delivery blitz
- Precision fixes with downstream impact
- **Podcast framing:** "The precision gatekeepers"

### 3. Rapid Prototype (srm-forever, Orbital-Sim)
- Single developer
- Single-day sprint
- Proof-of-concept focus
- **Podcast framing:** "The rebels"

### Ghost Pattern (ClimateMARGO)
- Years of silence
- README-only revival
- Single contributor
- **Podcast framing:** "The haunted library"

## Five Talking Points for the Episode

1. **The solar radiation fix** (WRF, May 28) — the most SRM-relevant code change, in the most popular atmospheric model
2. **The aerosol deprecation** (WRF, Jun 5) — they're moving away from aerosol physics, not toward it
3. **The roundoff fix** (PCMDI, Sep 4) — a 0.004°C signal could be hidden by floating-point rounding
4. **The precip-buoyancy POD** (MDTF, Jun 19) — 5 commits on one file, the ocean's closest friend
5. **The zero-star theory** (srm-forever, Aug 26) — Weitzman discounting coded by one person, discovered by nobody

## What's Missing (The Episode's Thesis)

- ❌ No SRM scenario module for WRF
- ❌ No SRM metrics in PCMDI
- ❌ No Marine Cloud Brightening code
- ❌ No real-time SRM monitoring tools
- ❌ No SRM risk assessment frameworks
- ✅ Evaluation infrastructure: mature
- ✅ Atmospheric models: sophisticated
- ✅ Economic theory: elegant
- ❌ Community connecting the above: **doesn't exist**

---

*Quick reference for on-air discussion. For full analysis, see PROJECT-DISCOVERIES-SOLAR.md and COMMIT-TRENDS-SOLAR.md.*