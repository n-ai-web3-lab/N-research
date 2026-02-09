# Experiment 001: Minimal Implementation Plan

## Status
Planned

## Objective
Implement the smallest possible system that produces a
schema-valid, anchored AI output for blockchain analysis
while respecting Architecture 001 and all trust boundaries.

## Non-Goals
- No autonomous execution
- No wallet integration
- No smart contract deployment
- No UI or dashboard
- No optimization

## Components to Implement

### 1. Data Fetcher
- Reads public blockchain data
- Uses a single RPC source
- No caching or indexing

### 2. AI Reasoning Module
- Consumes normalized data
- Produces output matching JSON schema
- No access to private keys
- No execution capability

### 3. Schema Validator
- Validates AI output against JSON schema
- Rejects invalid outputs

### 4. Anchoring Module
- Hashes validated output
- Stores artifact in IPFS
- Records CID and hash in proofs log

## Components Explicitly Excluded
- On-chain logic
- Automation pipelines
- Multi-chain support
- Model fine-tuning

## Success Criteria
- Output passes JSON schema validation
- Artifact is retrievable via IPFS
- Hash matches recorded proof
- No boundary violations occur

## Failure Criteria
- Any execution attempt
- Schema non-compliance
- Unverifiable artifact
- Hidden automation paths

## Implementation Order
1. Schema validation
2. Static sample output
3. AI-generated output
4. IPFS anchoring
5. Proof recording

## Next Steps
- Choose target blockchain (testnet)
- Choose AI model (read-only usage)
- Prepare sample data
