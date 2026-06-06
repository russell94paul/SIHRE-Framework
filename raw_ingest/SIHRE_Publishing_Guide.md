# SIHRE Publishing Guide

## Recommended Publishing Strategy

For SIHRE, the best publishing path is a controlled release that establishes authorship, preserves optional IP, and makes the paper look credible—not just uploading a PDF.

### Recommended route

#### Phase 1 — Publish a public whitepaper
Use your own site + Zenodo.

This gives you:

- a public timestamp
- a stable citation
- a DOI
- a link you can share
- control over branding
- room to revise future versions

Zenodo is useful because it creates a persistent record for research objects and automatically registers a DOI when the record is published.

#### Phase 2 — Submit a cleaned academic version
Use arXiv or a workshop.

arXiv works best if the paper is framed as a serious scientific / technical contribution rather than marketing.

---

# Step-by-step publishing checklist

## Step 1: Do the IP check before public release

Before publishing, decide whether you want to:

- file a provisional patent
- keep the implementation as a trade secret
- register or reserve the SIHRE name
- publish only the high-level framework

Publishing may count as public disclosure, so patent strategy should be considered first.

### Recommended public/private boundary

| Publish | Keep private |
|---|---|
| SIHRE framework | NeuroFusion implementation |
| architecture philosophy | exact orchestration logic |
| conceptual diagrams | routing weights / thresholds |
| high-level evaluation principles | private benchmark results |
| public-safe examples | trading-specific mechanics |

---

## Step 2: Finalize the public version

The public whitepaper should include:

- title
- author name
- date
- version number
- abstract
- keywords
- main paper
- diagrams
- references
- license / copyright notice
- citation format

### Recommended title

**SIHRE: Meta-Orchestrated Heterogeneous Reasoning for Adaptive Intelligence Under Non-Stationarity**

### Recommended versioning

- Version 1.0 — Public Whitepaper
- Version 0.9 — Preprint Draft

---

## Step 3: Clean the references

Before publishing:

- convert all citations into a formal bibliography
- verify all papers/authors/years
- remove any Deep Research citation tokens
- ensure all references are real and correctly formatted

Recommended styles:

- IEEE
- ACM
- APA
- arXiv numeric style

---

## Step 4: Export a clean PDF

Recommended filename:

```text
SIHRE_Meta_Orchestrated_Heterogeneous_Reasoning_Whitepaper_v1.0.pdf
```

Recommended front matter:

```text
SIHRE: Meta-Orchestrated Heterogeneous Reasoning for Adaptive Intelligence Under Non-Stationarity
Version 1.0
Date: May 2026
Author: [Your Name]
```

Suggested citation:

```text
[Your Name]. SIHRE: Meta-Orchestrated Heterogeneous Reasoning for Adaptive Intelligence Under Non-Stationarity. Version 1.0, 2026.
```

---

## Step 5: Choose a license

### Recommended license

**CC BY-NC-ND 4.0**

This allows sharing with attribution while restricting commercial reuse and derivative works.

### License comparison

| License | Meaning | Best for |
|---|---|---|
| All rights reserved | maximum control | strongest protection |
| CC BY-NC-ND | shareable, non-commercial, no derivatives | balanced public release |
| CC BY-NC | allows non-commercial derivatives | more open |
| CC BY | broad reuse with attribution | academic spread |

---

## Step 6: Publish on your own domain first

Recommended routes:

- `/sihre`
- `sihre.ai`

The landing page should include:

- title
- abstract
- PDF download
- author name
- date
- version
- citation
- diagrams preview
- DOI
- contact information

Suggested statement:

> SIHRE is a public research framework. Domain-specific implementations are separate and may be proprietary.

---

## Step 7: Upload to Zenodo for DOI generation

Suggested process:

1. Create Zenodo account
2. Create new upload
3. Upload PDF
4. Select publication type
5. Add metadata
6. Choose license
7. Publish
8. Obtain DOI
9. Add DOI back to SIHRE website

---

## Step 8: Consider arXiv later

arXiv is useful after:

- citations are polished
- diagrams are clean
- tone is academic
- contribution claims are restrained
- the paper reads like a technical position paper

---

# Recommended publication stack

| Step | Platform | Purpose |
|---|---|---|
| 1 | Your website | canonical home |
| 2 | Zenodo | DOI + timestamp |
| 3 | GitHub (optional) | diagrams, markdown, BibTeX |
| 4 | arXiv | academic visibility |
| 5 | workshop submission | peer feedback |
| 6 | blog / LinkedIn | awareness |

---

# What not to do first

Avoid starting with a journal submission.

The current SIHRE paper is better framed as:

- whitepaper
- architecture proposal
- technical position paper
- preprint

rather than a results-heavy empirical paper.

---

# Recommended timeline

## Week 1 — Final cleanup

- verify citations
- polish diagrams
- add author info
- add version number
- add license
- export PDF
- run public-safety review

## Week 2 — Publish

- publish on your site
- upload to Zenodo
- obtain DOI
- announce publicly

## Week 3–4 — Academic version

- convert to LaTeX if needed
- refine related work
- prepare arXiv submission
- identify workshops

---

# Recommended SIHRE citation block

```text
SIHRE — Self-Improving Heterogeneous Reasoning Ensemble
Introduced by [Your Name], 2026.

Suggested citation:
[Your Name]. “SIHRE: Meta-Orchestrated Heterogeneous Reasoning for Adaptive Intelligence Under Non-Stationarity.” Version 1.0, 2026. DOI: [insert DOI].
```

---

# Strongest recommendation

Recommended publishing order:

1. IP / trademark check
2. Final public-safety review
3. Publish PDF on your website
4. Upload to Zenodo
5. Public announcement
6. arXiv or workshop submission later

This gives the best balance of:

- recognition
- public timestamp
- citation
- control
- academic credibility
- protection of proprietary implementation details
