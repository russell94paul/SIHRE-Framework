---
tags: [sihre, naming, update-report]
created: 2026-05-24
updated: 2026-05-24
---

# SIHRE Naming Update Report

**Date:** 2026-05-24
**Scope:** All Markdown files in `C:\Users\PaulRussell\Documents\SIHRE-Framework\` (excluding `raw_ingest/`)
**Backup:** `C:\Users\PaulRussell\Documents\SIHRE-Framework\backup_before_sihre_naming_update\`

## Summary

- **Files scanned:** ~90 (all .md files outside raw_ingest/)
- **Files edited:** 30
- **Files already consistent:** 43
- **Files skipped (templates/trackers with no positioning text):** ~17
- **Public-safety issues found and fixed:** 10 (modality counts, NeuroFusion refs, trading refs removed from public-facing files)
- **Public-safety issues flagged for manual review:** 2 (research docs classified public-after-review that need redaction before release)
- **Classification errors fixed:** 1 (Deep_Research_Meta_Orchestrator_Signal_13.md reclassified from public-after-review to private-sensitive)

## Files Edited

### Public Website (02_Public_Website/) — 7 files

| File | Changes |
|---|---|
| **Homepage_Draft.md** | One-liner and short description replaced with canonical versions |
| **Landing_Page_Copy.md** | Hero and subhero replaced with canonical one-liner and expanded description |
| **About_SIHRE.md** | Opening description replaced; added "What does 'self-improving' mean?" section |
| **FAQ.md** | Self-improving answer expanded with safety-boundary caveat; added "evaluation feedback" |
| **Executive_One_Pager.md** | "What it is" replaced with canonical one-liner + expanded description |
| **Press_Kit.md** | One-liner and short description replaced with canonical versions |
| **Newsletter_Issue_1.md** | Description replaced with canonical expanded description |

### Start Here (00_Start_Here/) — 5 files

| File | Changes |
|---|---|
| **Glossary.md** | Self-improvement definition expanded with full canonical + safety caveat |
| **Naming_and_Positioning.md** | "Positioning sentence" renamed to "One-line description"; added expanded description and self-improving definition sections |
| **README_Index.md** | Canonical positioning sentence updated |
| **SIHRE_Vault_Index.md** | Removed NeuroFusion-13/HRE-13 branding, modality counts, trading references; "Recursive self-improvement" → "Bounded self-improvement" |
| **SIHRE_Wiki_Content_Pack_Index.md** | "coordinating" → "governing" in canonical positioning |

### Public Framework (01_Public_Framework/) — 2 files

| File | Changes |
|---|---|
| **Public_Private_Boundary.md** | Added canonical one-liner blockquote at top |
| **Non_Goals.md** | Added canonical one-liner; softened "guarantee of correctness"; added self-improving definition section |

### Whitepaper & Publication (03_) — 2 files

| File | Changes |
|---|---|
| **SIHRE_Canonical_Paper_Title.md** | Removed "Signal 13" and "financial markets" references; added canonical one-liner and self-improving definition |
| **Publication/Academic/paper-title.md** | Same changes as Canonical_Paper_Title.md (legacy copy) |

### Meta-Orchestrator (05_) — 1 file

| File | Changes |
|---|---|
| **Deep_Research_Meta_Orchestrator_Signal_13.md** | Reclassified from `public-after-review` to `private-sensitive` (contains extensive NeuroFusion-13, trading, and quant details) |

### Research (07_) — 2 files

| File | Changes |
|---|---|
| **NeuroFusion_Architecture_Research_Overview.md** | Legacy naming block (KFEI/NeuroFusion-12/CNSTI) replaced with canonical SIHRE naming |
| **Deep_Research_Gemini_Ensemble_Architecture.md** | Softened 8 overclaiming phrases ("guarantees" → "designed to", "true epistemological supremacy" → "broad epistemological coverage", etc.) |

### Deep Research Prompts (08_) — 1 file

| File | Changes |
|---|---|
| **SIHRE_Deep_Research_Prompts_All_Seven.md** | Terminology block updated to canonical naming format |

### IP & Attribution (09_) — 1 file

| File | Changes |
|---|---|
| **Author_Attribution_Plan.md** | Attribution phrase replaced with canonical one-liner |

### Product & Monetization (10_) — 5 files

| File | Changes |
|---|---|
| **SIHRE_Monetization_Strategy.md** | 3 positioning sentences replaced with canonical one-liner |
| **SIHRE_Monetization_Model.md** | Expanded description and control-plane language updated to canonical |
| **SIHRE_Pitch_Deck_Outline.md** | Slides 4 and 10 updated to canonical one-liner |
| **Monetization_Roadmap.md** | Added canonical one-liner to commercial thesis section |

### Legacy Files — 3 files

| File | Changes |
|---|---|
| **INDEX.md** | Removed NeuroFusion-13/HRE-13 line; replaced one-liner; "Recursive" → "Bounded" self-improvement |
| **SIHRE Framework/Research Reports/README.md** | Legacy naming block replaced with canonical |
| **SIHRE Framework/Research Reports/deep-research-prompts.md** | Terminology block updated to canonical naming format |
| **Monetization/High-Level Options (Needs Deep Research).md** | 2 positioning sentences replaced with canonical |

## Key Replacements Made

| Category | Old Phrase | New Phrase |
|---|---|---|
| One-liner | Various weaker variants | "SIHRE is a meta-orchestrated framework for governing heterogeneous reasoning systems under uncertainty, drift, and non-stationarity." |
| Expanded | Various weaker variants | "SIHRE is a framework for coordinating multiple reasoning modalities through a meta-orchestrator that manages trust, uncertainty, verification, memory, and adaptation over time." |
| Self-improving | "Bounded updates to memory, expert trust, routing preferences, and research priorities" | Full canonical definition with safety-boundary caveat |
| Naming | "Brand: NeuroFusion-13 \| Academic: HRE-13" | Removed from public-facing files |
| Naming | "Signal 13 governs the ensemble" | "the meta-orchestrator governs the ensemble" |
| Overclaiming | "guarantees that no single mathematical blind spot can compromise" | "is designed so that no single mathematical blind spot dominates" |
| Overclaiming | "true epistemological supremacy" | "broad epistemological coverage" |
| Overclaiming | "radical departure" | "significant departure" |
| Overclaiming | "Recursive self-improvement" | "Bounded self-improvement" |
| Domain safety | "financial markets, changing environments" | "changing environments, drift, partial observability" |
| Domain safety | "trading, robotics, healthcare, cyber" | "robotics, healthcare, cyber, and other domains" |

## Files Skipped (No Changes Needed)

Files already consistent with canonical language — 43 total. Key examples:
- **SIHRE_Whitepaper_Public_Draft.md** — already has correct title, meta-orchestrated positioning, and well-written bounded self-improvement definition
- All 02_Public_Website files not listed above (Architecture_Page, Applications_Page, Meta_Orchestrator_Page, Whitepaper_Page, Blog_Post_Announcement)
- All 12_Trackers_and_Templates files (templates only, no positioning text)
- All 13_Future_Roadmap files
- All 11_Governance_Risk_and_Safety files
- Most 09_IP_and_Attribution files (templates)
- Most private-sensitive research files (internal content, no public-facing issues)

## Recommended Follow-Up

1. **Manual redaction needed:** `Deep_Research_Ensemble_Architecture_State_of_Art.md` and `Deep_Research_Gemini_Ensemble_Architecture.md` are classified `public-after-review` but contain extensive NeuroFusion-13, modality counts, and trading content. Must be redacted before any public release.
2. **Consider reclassifying:** Both files above may be better reclassified as `private-sensitive` (like the Meta_Orchestrator_Signal_13.md was).
3. **raw_ingest/ files:** Not modified per instructions. If content from raw_ingest/ is re-ingested into SIHRE_Wiki/, it will need the same canonical language applied.
