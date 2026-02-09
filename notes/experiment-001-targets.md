# Experiment 001: Target Selection and Justification

## Status
Final (Pre-Implementation)

## Purpose
Document and justify the selection of the blockchain network
and AI model used in Experiment 001 to ensure reproducibility,
auditability, and alignment with Architecture 001.

## Blockchain Selection

### Selected Blockchain
Ethereum (Testnet)

### Justification
- Mature tooling and documentation
- Public, well-understood data model
- Rich event and transaction metadata
- Strong ecosystem for future verification work

### Scope
- Read-only access
- No contract deployment
- No transaction execution

## AI Model Selection

### Selected Model
General-purpose LLM (read-only usage)

### Justification
- Capable of structured output
- No fine-tuning or training involved
- Used strictly for inference
- Replaceable without architectural changes

### Constraints
- No memory persistence
- No tool-based execution
- No access to private keys or secrets

## Reproducibility Notes
- Model identifier must be recorded in output metadata
- Blockchain network and block range must be explicit
- Outputs must be schema-valid and anchored

## Risks
- Model behavior may change over time
- RPC data availability may vary
- Results are advisory, not authoritative

## Alternatives Considered
- Other L1/L2 networks
- Smaller or specialized models

## Decision Summary
These selections prioritize safety, clarity, and auditability
over performance or automation.
