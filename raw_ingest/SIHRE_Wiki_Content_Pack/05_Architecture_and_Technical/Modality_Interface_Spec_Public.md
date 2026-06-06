# Public-Safe Modality Interface Spec

## Purpose

Define a generic interface for SIHRE reasoning modalities without exposing implementation details.

## Generic modality contract

A modality should provide:

- input requirements
- output type
- confidence/uncertainty representation
- evidence provenance
- known limitations
- calibration status
- latency/cost estimate
- failure modes
- update hooks

## Example public-safe modality types

- Retrieval modality
- Graph reasoning modality
- Predictive modality
- Causal modality
- Uncertainty modality
- Verification modality
- Simulation modality
- Representation-learning modality
- Generative hypothesis modality

## Do not publish

- private algorithms
- exact feature sets
- exact thresholds
- proprietary scoring
- domain-sensitive mechanics
