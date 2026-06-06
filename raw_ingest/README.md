# raw_ingest — Drop Zone

Drop unprocessed files here for organization into the SIHRE Wiki.

## How it works

1. Drop any Markdown (or other) files into this folder
2. Run `/ingest` to classify and copy them into `SIHRE_Wiki/`
3. Original files here are **never deleted or modified** — this folder is the immutable source of record

## What gets processed

- Markdown files (`.md`)
- Any text-based research, notes, drafts, prompts, strategy docs
- Files in subfolders are scanned recursively

## What gets skipped

- This README
- Files already recorded in `SIHRE_Wiki/MIGRATION_MAP.md`

## After ingest

Each file gets:
- Proper YAML frontmatter (tags, status, source, classification)
- A descriptive filename (if the original was vague)
- Placement in the correct numbered `SIHRE_Wiki/` folder
- An entry in the migration map, master index, and public/private map
