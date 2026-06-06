# Duplicates Report

## Exact Duplicates Found (skipped during ingest)

| File A | File B | Action |
|---|---|---|
| `raw_ingest/SIHRE_Monetization_Model.md` | `raw_ingest/SIHRE_Monetization_Artifacts/SIHRE_Monetization_Model.md` | Ingested file A only |
| `raw_ingest/SIHRE_Monetization_Deep_Research_Prompt.md` | `raw_ingest/SIHRE_Monetization_Artifacts/SIHRE_Monetization_Deep_Research_Prompt.md` | Ingested file A only |
| `raw_ingest/SIHRE_Pitch_Deck_Outline.md` | `raw_ingest/SIHRE_Monetization_Artifacts/SIHRE_Pitch_Deck_Outline.md` | Ingested file A only |

All three files in `raw_ingest/SIHRE_Monetization_Artifacts/` are byte-identical copies of files at the root of `raw_ingest/`. Only the root-level copies were ingested.

## Near-Duplicates (both preserved)

### 1. Ensemble Architecture — Two AI Research Tools

| File | Location | Source |
|---|---|---|
| `Deep_Research_Ensemble_Architecture_State_of_Art.md` | 07_Research_and_Prior_Art/ | ChatGPT Pro |
| `Deep_Research_Gemini_Ensemble_Architecture.md` | 07_Research_and_Prior_Art/ | Gemini |

Both cover Prompt 1 (ensemble architecture state of art) but from different research tools. ChatGPT version is more structured with clear sections; Gemini version is more comprehensive on modality fusion math and RRF formulas. Both preserved for cross-referencing.

### 2. Monetization Coverage Overlap

| File | Location | Focus |
|---|---|---|
| `SIHRE_Monetization_Strategy.md` | 10_Product_and_Monetization/ | Original high-level 10-path strategy |
| `SIHRE_Monetization_Model.md` | 10_Product_and_Monetization/ | Detailed profit scenarios and go-to-market |
| `Monetization_Roadmap.md` | 10_Product_and_Monetization/ | Phased timeline |

These overlap but serve different purposes. `Strategy` is the original brainstorm; `Model` adds financial scenarios; `Roadmap` is the timeline. Consider consolidating into one canonical monetization doc when mature.

### 3. Publication Checklists Overlap

| File | Location | Focus |
|---|---|---|
| `Publication_Checklist.md` | 03_Whitepaper_and_Publication/ | Pre-publication checklist |
| `Whitepaper_Release_Checklist.md` | 03_Whitepaper_and_Publication/ | Final release gate |
| `SIHRE_Publishing_Guide.md` | 03_Whitepaper_and_Publication/ | Full publishing strategy |

These have overlapping scope. `Publishing_Guide` is the most comprehensive; the checklists are derived subsets. Consider merging checklists into the guide when finalizing.
