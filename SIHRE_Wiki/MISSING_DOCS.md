# Missing Docs

Gaps in the wiki based on the current 94-file inventory.

## Priority 1 — Critical for Publication

| Doc | Folder | Why | Status |
|---|---|---|---|
| SIHRE_Framework_Overview.md | 01_Public_Framework/ | Core public-safe definition of SIHRE | **MISSING** — highest priority |
| Verified_Reference_Bibliography.md | 03_Whitepaper_and_Publication/ | Clean, verified bibliography from deep research | **MISSING** — blocks publication |
| Citation verification pass | 03_Whitepaper_and_Publication/ | All Deep Research citation tokens need verification | **NOT STARTED** |
| IP decision (patent/trademark) | 09_IP_and_Attribution/ | Templates exist but decisions not recorded | **NOT STARTED** |

## Priority 2 — Structural Gaps

These folders have content but are missing key files.

| Doc | Folder | Why |
|---|---|---|
| SIHRE_Architecture_Overview.md | 04_Architecture/ | Public-safe architecture summary (Layered_Architecture exists but is from content pack) |
| SIHRE_Competitive_Landscape.md | 07_Research_and_Prior_Art/ | Extracted from deep research — how SIHRE differs from TradExpert, TRACE, Compound AI |
| SIHRE_Key_Papers.md | 07_Research_and_Prior_Art/ | Curated reading list from deep research citations |
| Benchmark_Suite_Design.md | 06_Evaluation_and_Benchmarks/ | Concrete benchmark proposal (prompt exists but not run) |

## Priority 3 — Content Pack Gaps Filled

These items from the original MISSING_DOCS have been filled by the content pack:

| Originally Missing | Now Exists As | Location |
|---|---|---|
| Glossary | Glossary.md | 00_Start_Here/ |
| Public/private boundary | Public_Private_Boundary.md | 01_Public_Framework/ |
| Homepage copy | Homepage_Draft.md | 02_Public_Website/ |
| About page | About_SIHRE.md | 02_Public_Website/ |
| FAQ | FAQ.md | 02_Public_Website/ |
| Applications page | Applications_Page.md | 02_Public_Website/ |
| Press kit | Press_Kit.md | 02_Public_Website/ |
| Blog announcement | Blog_Post_Announcement.md | 02_Public_Website/ |
| Citation/DOI checklist | Citation_and_DOI_Checklist.md | 03_Whitepaper_and_Publication/ |
| IP strategy | IP_Strategy_Memo.md | 09_IP_and_Attribution/ |
| Trademark checklist | Trademark_Checklist.md | 09_IP_and_Attribution/ |
| Offer ladder | Offer_Ladder.md | 10_Product_and_Monetization/ |
| Control plane PRD | SIHRE_Control_Plane_PRD.md | 10_Product_and_Monetization/ |
| Consulting audit template | Consulting_Audit_Template.md | 10_Product_and_Monetization/ |
| Author attribution | Author_Attribution_Plan.md | 09_IP_and_Attribution/ |
| Disclosure log | Disclosure_Log_Template.md | 09_IP_and_Attribution/ |
| Risk register | Risk_Register.md | 11_Governance_Risk_and_Safety/ |
| Redaction checklist | Redaction_Checklist.md | 11_Governance_Risk_and_Safety/ |
| Artifact tracker | Artifact_Status_Tracker.md | 12_Trackers_and_Templates/ |
| Research backlog | Research_Backlog.md | 12_Trackers_and_Templates/ |
| Deep research run log | Deep_Research_Run_Log.md | 12_Trackers_and_Templates/ |
| Roadmap | Comprehensive_Artifact_Backlog.md | 13_Future_Roadmap/ |
| Domain expansion | Domain_Specific_Expansion_List.md | 13_Future_Roadmap/ |

## Maintenance Recommendations

1. **Citation verification is the #1 blocker.** 16 files are classified "public-after-review" — all need citation tokens verified or removed before any public release.
2. **Write the SIHRE Framework Overview.** A clean, trading-free public definition is the highest-leverage single doc to write. Extract from whitepaper abstract + Non_Goals + Public_Safe_Examples.
3. **Consolidate monetization docs.** Three overlapping monetization files should eventually merge into one canonical doc.
4. **Consolidate publication checklists.** Three overlapping checklist files should merge into the Publishing Guide.
5. **Run the deep research prompts.** 18 prompts are queued and ready. Priority order: Competitive Landscape, Benchmark Suite, Meta-Orchestrator Deep Dive.
