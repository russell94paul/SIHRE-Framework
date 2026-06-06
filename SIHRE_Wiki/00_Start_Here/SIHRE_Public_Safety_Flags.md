---
tags: [sihre, public-safety, audit]
created: 2026-05-24
updated: 2026-05-24
---

# SIHRE Public Safety Flags

**Date:** 2026-05-24
**Purpose:** Identify files that contain content that must not appear in public-facing materials.

## Classification Errors Fixed

| File | Old Classification | New Classification | Reason |
|---|---|---|---|
| `SIHRE_Wiki/05_Meta_Orchestrator/Deep_Research_Meta_Orchestrator_Signal_13.md` | `public-after-review` | `private-sensitive` | Contains extensive NeuroFusion-13 details, Signal 13 references, quant trading strategies, risk management specifics, MiFID/DORA regulatory references, proprietary architecture |

## Files Requiring Manual Redaction Before Public Release

### 1. `SIHRE_Wiki/07_Research_and_Prior_Art/Deep_Research_Ensemble_Architecture_State_of_Art.md`

**Current classification:** `public-after-review`
**Recommended action:** Reclassify to `private-sensitive` OR create a redacted public version

Contains:
- "NeuroFusion-13" throughout (title and body)
- "13-signal" architecture references
- "four-signal architecture" with specific signal enumeration
- Specific modality counts
- Trading-specific content (ICT/Smart Money, FVGs, order blocks)
- NeuroSpect product references

### 2. `SIHRE_Wiki/07_Research_and_Prior_Art/Deep_Research_Gemini_Ensemble_Architecture.md`

**Current classification:** `public-after-review`
**Recommended action:** Reclassify to `private-sensitive` OR create a redacted public version

Contains:
- "NeuroFusion-13" throughout
- "13 distinct intelligence typologies"
- "13 modalities", "13 heterogeneous modalities"
- Extensive trading-specific content (quant trading, LightGBM, NeuroSpect)
- Overclaiming language softened in this update but trading content remains

## Files with Exact Modality Counts (Correctly Classified Internal)

| File | Classification | Content |
|---|---|---|
| `SIHRE_Wiki/04_Architecture/Deep_Research_Signal_Optimization_Technical_Design.md` | `private-sensitive` | Signal 1-13 enumerated with trading-specific details, "NeuroFusion-13" throughout |
| `SIHRE_Wiki/05_Meta_Orchestrator/Deep_Research_Meta_Orchestrator_Signal_13.md` | `private-sensitive` (fixed) | "twelve inputs/signals/modalities", Signal 13 as meta-orchestrator |
| `SIHRE_Wiki/07_Research_and_Prior_Art/Deep_Research_Extended_Signals_5_Through_13.md` | `private-sensitive` | Signals 5-13 detailed |
| `SIHRE_Wiki/07_Research_and_Prior_Art/Deep_Research_DSLM_Quant_Hybrid.md` | `private-sensitive` | Quant-specific signal details |
| `SIHRE_Wiki/07_Research_and_Prior_Art/Deep_Research_Knowledge_Graph_Trading.md` | `private-sensitive` | Trading knowledge graph architecture |

## Files Mentioning NeuroFusion (Correctly Classified)

| File | Classification | Context |
|---|---|---|
| `SIHRE_Wiki/07_Research_and_Prior_Art/NeuroFusion_Architecture_Research_Overview.md` | `internal-only` | Research overview, naming now shows SIHRE primary with NeuroFusion as proprietary implementation |
| `SIHRE_Wiki/README.md` | N/A (meta) | Correctly uses NeuroFusion-13 only in "never publish" boundary section |
| `SIHRE_Wiki/MASTER_INDEX.md` | N/A (meta) | References NeuroFusion in file titles marked "(private)" |
| `SIHRE Framework/Research Reports/README.md` | `internal-only` | Legacy research index, naming updated |
| `SIHRE Framework/Research Reports/deep-research-prompts.md` | `internal-only` | Prompt archive, naming updated |

## Files Mentioning Trading/Finance (Correctly Classified)

| File | Classification | Content Type |
|---|---|---|
| `Deep_Research_Novel_Quant_Trading_Technology.md` | `private-sensitive` | Quant trading technology research |
| `Deep_Research_Signal_Optimization_Technical_Design.md` | `private-sensitive` | Trading signal optimization |
| `Deep_Research_Meta_Orchestrator_Signal_13.md` | `private-sensitive` | Trading meta-orchestrator design |
| `Deep_Research_DSLM_Quant_Hybrid.md` | `private-sensitive` | DSLM + quant hybrid |
| `Deep_Research_Knowledge_Graph_Trading.md` | `private-sensitive` | Trading knowledge graphs |
| `Monetization/High-Level Options (Needs Deep Research).md` | `internal-only` | Business planning |
| `SIHRE_Wiki/10_Product_and_Monetization/*` | `internal-only` | Business/monetization planning |

## Public-Facing Files — Clean

All files in these public-facing directories are confirmed clean of:
- Modality counts
- SIHRE-13 references
- NeuroFusion details
- Trading/finance examples
- Alpha/strategy/execution logic
- Proprietary schemas or thresholds

Verified clean directories:
- `SIHRE_Wiki/02_Public_Website/` (12 files)
- `SIHRE_Wiki/01_Public_Framework/` (3 files)
- `SIHRE_Wiki/04_Architecture/Diagram_Pack_Mermaid.md`
- `SIHRE_Wiki/04_Architecture/Layered_Architecture.md`
- `SIHRE_Wiki/04_Architecture/Modality_Interface_Spec_Public.md`
- `SIHRE_Wiki/05_Meta_Orchestrator/Meta_Orchestrator_Spec_Public.md`
- `SIHRE_Wiki/06_Evaluation_and_Benchmarks/Evaluation_Framework.md`

## Recommended Actions

1. **Reclassify** `Deep_Research_Ensemble_Architecture_State_of_Art.md` to `private-sensitive`
2. **Reclassify** `Deep_Research_Gemini_Ensemble_Architecture.md` to `private-sensitive`
3. If public versions of these research docs are needed, create separate redacted copies with NeuroFusion/trading content removed and modality counts generalized
