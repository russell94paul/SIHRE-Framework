---
name: ingest
description: Process files from raw_ingest/ into the organized SIHRE_Wiki/ structure. Classifies content, copies files to correct numbered folders, generates tracking artifacts (migration map, public/private map, duplicates report, missing docs). Treats raw_ingest/ as immutable read-only source.
allowed-tools: Read, Write, Edit, Glob, Grep, Bash, Agent, TaskCreate, TaskUpdate, TaskList
---

# SIHRE Wiki Ingest Skill

Organize unprocessed Markdown files from `raw_ingest/` into the structured `SIHRE_Wiki/` output folder.

## Core Rules

1. **`raw_ingest/` is immutable.** Never delete, move, or modify files in `raw_ingest/`. Read only.
2. **`SIHRE_Wiki/` is the organized output.** All organized content goes here.
3. **Copy, never move.** Files are copied from `raw_ingest/` into `SIHRE_Wiki/`.
4. **Preserve all Markdown content** unless fixing obvious broken frontmatter or duplicated titles.
5. **Public/private separation is mandatory.** Never mix internal strategy into public framework folders.

## When Invoked

### Step 1 — Scan raw_ingest/

Recursively inspect all files in `raw_ingest/`. For each file:

- Read its content
- Infer its purpose from filename + content
- Classify it into a target folder (see Target Structure below)
- Classify its sensitivity (see Classification Guidance below)
- Note if it overlaps with or duplicates an existing file

Skip `raw_ingest/README.md` (that's the drop-zone instructions, not content).

### Step 2 — Ensure SIHRE_Wiki/ structure exists

Create the full folder tree if it doesn't exist:

```
SIHRE_Wiki/
  00_Start_Here/
  01_Public_Framework/
  02_Public_Website/
  03_Whitepaper_and_Publication/
  04_Architecture/
  05_Meta_Orchestrator/
  06_Evaluation_and_Benchmarks/
  07_Research_and_Prior_Art/
  08_Deep_Research_Prompts/
    Market_and_Monetization/
    Architecture_and_Meta_Orchestration/
    Evaluation_and_Benchmarks/
    IP_and_Publication/
    Governance_and_Safety/
    Academic_and_Prior_Art/
  09_IP_and_Attribution/
  10_Product_and_Monetization/
  11_Governance_Risk_and_Safety/
  12_Trackers_and_Templates/
  13_Future_Roadmap/
  99_Archive_or_Unsorted/
```

### Step 3 — Copy and restructure files

For each file classified in Step 1:

1. Determine the target path inside `SIHRE_Wiki/`
2. Rename the file if the original name is vague (use descriptive title-cased filenames)
3. Copy the content to the target path
4. Fix frontmatter if needed — ensure every file has:
   ```yaml
   ---
   tags: [sihre, <section-tag>, <topic-tags>]
   status: draft | review | final | published
   source: original | deep-research | external | ingested
   classification: public-safe | public-after-review | internal-only | private-sensitive
   created: YYYY-MM-DD
   updated: YYYY-MM-DD
   original_path: raw_ingest/<original-filename>
   ---
   ```
5. Do not alter the body content beyond fixing broken formatting
6. If a file fits multiple categories, place it in the most important one

### Step 4 — Generate tracking artifacts

After all files are placed, generate these files in `SIHRE_Wiki/`:

#### README.md
Root README explaining the entire SIHRE_Wiki structure, what each numbered folder contains, and how to navigate.

#### MASTER_INDEX.md
Links to all files organized by category. One entry per file with a short description.

#### PUBLIC_PRIVATE_MAP.md
Table classifying every file as:
- **Public-safe** — ready for website/whitepaper
- **Public-safe after review** — has citations, novelty claims, or benchmarks that need verification
- **Internal only** — monetization, pricing, product strategy, publication planning
- **Private / sensitive** — IP strategy, patents, trademarks, disclosure logs, proprietary logic

#### MIGRATION_MAP.md
Table with columns:
| Original Path | New Path | New Filename | Reason for Placement |

#### DUPLICATES_REPORT.md
If duplicate or overlapping files are detected, list them with recommendations. If none, create the file with "No duplicates detected."

#### MISSING_DOCS.md
List wiki pages or artifacts that should be created next based on gaps in coverage. Reference the folder structure to identify holes.

### Step 5 — Report

After completion, output a summary:

1. Final folder tree (actual files placed)
2. File-by-file placement table
3. Public/private classification table
4. Count of files processed, skipped, flagged
5. Top recommended missing docs to write next

---

## Target Structure — Folder Descriptions

### 00_Start_Here
Overview files, master indexes, naming conventions, glossary, knowledge map, navigation docs.

### 01_Public_Framework
Public-safe framework explanations: SIHRE definition, principles, non-goals, public/private boundary summaries, conceptual content safe for external audiences.

### 02_Public_Website
Website-ready content: homepage copy, About page, FAQ, applications page, landing page copy, press kit, blog announcement, newsletter drafts, executive one-pagers, public web pages.

### 03_Whitepaper_and_Publication
Whitepaper drafts, publishing guides, release checklists, citation/DOI checklists, publication strategy, arXiv/workshop planning, public paper assets.

### 04_Architecture
Architecture pages, layered architecture docs, Mermaid diagrams, modality interface specs, reference architecture docs, public architecture specs, architecture decision records.

### 05_Meta_Orchestrator
All meta-orchestrator-specific material: definitions, public specs, workflow diagrams, routing/trust concepts, meta-orchestrator research prompts.

### 06_Evaluation_and_Benchmarks
Evaluation framework docs, benchmark suite prompts, metrics, evaluation protocols, drift robustness, calibration, abstention, testing-related files.

### 07_Research_and_Prior_Art
Literature review, prior-art analysis, competitive landscape, taxonomy, academic venue strategy, research foundation files.

### 08_Deep_Research_Prompts
Prompts for future Deep Research runs. NOT finished research — only the prompts themselves.

Subfolders:
- `Market_and_Monetization/` — prompts about market sizing, pricing, competitive business analysis
- `Architecture_and_Meta_Orchestration/` — prompts about system design, orchestration, routing
- `Evaluation_and_Benchmarks/` — prompts about testing, metrics, benchmark design
- `IP_and_Publication/` — prompts about patent strategy, publication venues, citation analysis
- `Governance_and_Safety/` — prompts about risk, safety, auditability, compliance
- `Academic_and_Prior_Art/` — prompts about literature review, related work, taxonomy

### 09_IP_and_Attribution
IP strategy, trademark checklist, patent preparation, disclosure log, author attribution plan, claim register, citation register, public/private legal boundary docs.

### 10_Product_and_Monetization
Monetization roadmap, offer ladder, control-plane PRD, consulting audit templates, certification blueprint, pricing experiments, partner program, business model files.

### 11_Governance_Risk_and_Safety
Risk register, redaction checklist, reliability/governance docs, safety and risk prompts, auditability docs, public-safety materials.

### 12_Trackers_and_Templates
Artifact tracker, research backlog, decision log, meeting notes template, version history, content calendar, Deep Research run log, reusable templates.

### 13_Future_Roadmap
Comprehensive artifact backlog, suggested docs to generate next, future roadmap, domain expansion list, long-term planning docs.

### 99_Archive_or_Unsorted
Anything that does not clearly fit elsewhere. Review periodically and re-classify.

---

## Classification Guidance

### Public-safe
- Website copy
- Public framework explanations
- Glossary
- Public-safe diagrams
- Public whitepaper material
- Non-sensitive architecture descriptions
- General research positioning

### Public-safe after review
- Anything with citations (verify all references are real and correctly formatted)
- Anything making novelty claims (need academic defensibility check)
- Anything referencing benchmarks (need accuracy verification)
- Anything that may need public-safety review before publishing

### Internal only
- Monetization strategy
- Pricing models
- Product strategy and PRDs
- Roadmap documents
- Consulting offers and templates
- Partner strategy
- Publication planning and timeline
- Research workflow docs

### Private / sensitive
- IP strategy and patent preparation
- Trademark strategy and registration
- Disclosure logs
- Public/private boundary strategy docs
- Implementation-specific details
- Anything that could reveal proprietary logic (NeuroFusion routing, weights, thresholds)

---

## Incremental Runs

When the skill is invoked again after initial setup:

1. Scan `raw_ingest/` for files not yet in `MIGRATION_MAP.md`
2. Process only new files
3. Append to `MIGRATION_MAP.md`, `MASTER_INDEX.md`, `PUBLIC_PRIVATE_MAP.md`
4. Update `MISSING_DOCS.md` if gaps have been filled
5. Report only the delta (what was new and where it went)

---

## Naming Conventions

- Use title-cased descriptive filenames: `SIHRE_Framework_Overview.md`, not `overview.md`
- Replace vague names: `prompt-1-ensemble-architecture.md` → `Deep_Research_Ensemble_Architecture_State_of_Art.md`
- Preserve the original filename in frontmatter `original_path` field
- Use underscores for spaces in filenames

---

## SIHRE Context

- **SIHRE** = Self-Improving Heterogeneous Reasoning Ensemble
- **Brand name**: NeuroFusion-13 (trading implementation, PRIVATE)
- **Academic name**: HRE-13 (alternative)
- SIHRE is the **public, domain-general** framework
- NeuroFusion-13 is a **proprietary implementation** for trading — never include in public folders
- The 13 signals: VectorDB RAG, DSLM Hybrid, Quant Model, Knowledge Graph, Causal Engine, Conformal Predictor, Adversarial Debate, Synthetic Scenarios, Active Learning, Federated Network, Contrastive Regimes, Program Synthesis, Meta-Orchestrator
