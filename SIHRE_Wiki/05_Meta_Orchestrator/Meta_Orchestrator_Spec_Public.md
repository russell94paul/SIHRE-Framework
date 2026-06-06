---
tags: [sihre, meta-orchestrator, spec, public]
status: draft
source: ingested
classification: public-after-review
created: 2026-05-23
updated: 2026-05-23
original_path: raw_ingest/SIHRE_Wiki_Content_Pack/05_Architecture_and_Technical/Meta_Orchestrator_Spec_Public.md
---
# SIHRE Meta-Orchestrator Public Specification

## Public definition

The SIHRE meta-orchestrator is a reasoning-governance layer that selects, sequences, weights, challenges, suppresses, or promotes heterogeneous reasoning modalities based on context, uncertainty, disagreement, evidence quality, historical reliability, and outcomes.

## Inputs

- Task context
- Evidence quality
- Domain context
- Expert outputs
- Uncertainty estimates
- Disagreement signals
- Drift signals
- Prior reliability
- Cost of error
- Governance constraints

## Outputs

- Expert routing plan
- Trust weights or rankings
- Verification request
- Simulation request
- Abstention or deferral
- Final synthesis
- Memory update
- Reliability update
- Research-action recommendation

## Public-safe non-details

This public specification intentionally omits exact algorithms, thresholds, formulas, and implementation policies.
