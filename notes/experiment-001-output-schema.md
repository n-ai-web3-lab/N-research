# Experiment 001: AI Output Schema

## Status
Draft

## Purpose
Define a structured, auditable output format for AI-generated
analysis of blockchain data that enables verification,
reproducibility, and human review.

## Design Requirements
- Machine-readable
- Human-auditable
- Deterministically referencable
- Non-executable

## Schema Overview

### Metadata
- experiment_id
- architecture_version
- timestamp
- model_identifier

### Input References
- blockchain
- network
- block_range
- transaction_hashes
- contract_addresses

### Observations
- detected_events
- state_changes
- anomalies

### Reasoning
- summary
- assumptions
- confidence_level

### Suggested Actions
- description
- risk_level
- requires_human_approval (always true)

### Limitations
- data_gaps
- uncertainty_sources

## Trust Guarantees
- No private keys
- No execution intent
- Advisory only

## Open Questions
- Should confidence be numeric or categorical?
- How much reasoning should be exposed?
- How to prevent prompt leakage?

## Next Steps
- Convert schema to JSON Schema
- Test against sample outputs
- Anchor outputs to IPFS
