# SIHRE Framework — Project Instructions

## What This Is

Obsidian vault + knowledge base for the **SIHRE (Self-Improving Heterogeneous Reasoning Ensemble)** framework. Goal: gather, organize, and refine all research and writing needed to get SIHRE published as a credible academic contribution.

## Key Distinction

- **SIHRE** = public, domain-general framework (publishable)
- **NeuroFusion-13** = proprietary trading implementation (never publish)
- Always enforce this boundary. When in doubt, classify as internal.

## Vault Layout

- `raw_ingest/` — Drop zone for unprocessed files. **Immutable.** Never delete or modify files here.
- `SIHRE_Wiki/` — Organized output. Numbered folders 00-13 plus 99_Archive. Created and maintained by the `/ingest` skill.
- `SIHRE Framework/` — Legacy content (research reports, whitepapers). Ingest into SIHRE_Wiki/ when ready.
- `INDEX.md` — Legacy vault index. Will be superseded by `SIHRE_Wiki/MASTER_INDEX.md`.

## Skills

| Skill | When to use |
|---|---|
| `/ingest` | Process new files from `raw_ingest/` into `SIHRE_Wiki/` |

## File Conventions

Every organized file in `SIHRE_Wiki/` gets YAML frontmatter:

```yaml
---
tags: [sihre, <section>, <topic>]
status: draft | review | final | published
source: original | deep-research | external | ingested
classification: public-safe | public-after-review | internal-only | private-sensitive
created: YYYY-MM-DD
updated: YYYY-MM-DD
original_path: raw_ingest/<filename> (if ingested)
---
```

## Workflow

1. Paul drops files into `raw_ingest/`
2. Invoke `/ingest` to classify and organize them into `SIHRE_Wiki/`
3. Tracking artifacts (MIGRATION_MAP, PUBLIC_PRIVATE_MAP, MASTER_INDEX, etc.) are auto-generated in `SIHRE_Wiki/`
4. Incremental runs process only new files not yet in the migration map
