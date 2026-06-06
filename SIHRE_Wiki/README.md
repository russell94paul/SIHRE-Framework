# SIHRE Wiki

**Self-Improving Heterogeneous Reasoning Ensemble (SIHRE)**

Organized knowledge base for the SIHRE framework — 94 content files across 14 sections.

## Structure

| Folder | Files | Purpose |
|---|---|---|
| `00_Start_Here/` | 6 | Overview, indexes, glossary, knowledge map, navigation |
| `01_Public_Framework/` | 3 | Public-safe framework explanations, non-goals, boundary rules |
| `02_Public_Website/` | 11 | Website content: homepage, about, FAQ, blog, press kit, newsletter |
| `03_Whitepaper_and_Publication/` | 7 | Whitepaper drafts, publishing guides, checklists, DOI planning |
| `04_Architecture/` | 4 | Architecture docs, diagrams, modality specs, technical design |
| `05_Meta_Orchestrator/` | 2 | Signal 13: meta-orchestrator specs and research |
| `06_Evaluation_and_Benchmarks/` | 1 | Evaluation framework, metrics, protocols |
| `07_Research_and_Prior_Art/` | 7 | Deep research outputs, literature review, prior art |
| `08_Deep_Research_Prompts/` | 18 | Prompts for future deep research (6 subfolders by topic) |
| `09_IP_and_Attribution/` | 5 | IP strategy, patents, trademarks, attribution, disclosure |
| `10_Product_and_Monetization/` | 10 | Monetization, pricing, PRD, consulting, certification, pitch deck |
| `11_Governance_Risk_and_Safety/` | 3 | Risk register, redaction checklist, reliability |
| `12_Trackers_and_Templates/` | 10 | Status trackers, registers, logs, templates |
| `13_Future_Roadmap/` | 4 | Artifact backlog, domain expansion, next docs |
| `99_Archive_or_Unsorted/` | 0 | Staging area for unclassified content |

## Key Distinction

- **SIHRE** = public, domain-general framework (publishable)
- **NeuroFusion-13** = proprietary trading implementation (never publish)

## Sensitivity Breakdown

| Classification | Count |
|---|---|
| Public-safe | 9 |
| Public-after-review | 16 |
| Internal-only | 58 |
| Private-sensitive | 11 |

## Tracking Artifacts

| File | Purpose |
|---|---|
| `MASTER_INDEX.md` | Links to all 94 files by category |
| `PUBLIC_PRIVATE_MAP.md` | Sensitivity classification for every file |
| `MIGRATION_MAP.md` | Source path → destination path for all files |
| `DUPLICATES_REPORT.md` | 3 exact dupes skipped, 3 near-dupe clusters noted |
| `MISSING_DOCS.md` | Gaps and next docs to create |

## Workflow

1. Drop files into `raw_ingest/`
2. Run `/ingest` to classify and copy into this structure
3. Tracking artifacts auto-update
4. Incremental runs process only new files not in MIGRATION_MAP
