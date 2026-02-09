# Experiment 001: Anchoring Strategy

## Status
Draft

## Purpose
Define how outputs of Experiment 001 are made tamper-evident
and time-bound without placing AI reasoning or authority on-chain.

## Anchoring Goals
- Prove existence at a point in time
- Enable independent verification
- Avoid centralized trust
- Preserve off-chain flexibility

## Artifacts to Anchor
- AI output JSON (schema-compliant)
- Input reference list
- Experiment metadata

## Artifacts NOT to Anchor
- AI prompts
- Model weights
- Internal reasoning traces
- Execution suggestions

## Anchoring Method
1. Generate AI output artifact
2. Validate against JSON schema
3. Compute cryptographic hash
4. Store artifact in IPFS
5. Record CID and hash in proofs log

## On-Chain Usage
- Optional hash anchoring
- No interpretation of contents
- No dependency on AI semantics

## Verification Process
- Retrieve artifact via CID
- Recompute hash
- Compare with recorded hash
- Confirm schema validity

## Failure Handling
- Invalid schema → reject artifact
- Hash mismatch → discard artifact
- Missing CID → unverifiable result

## Trust Assumptions
- IPFS availability is probabilistic
- Hash functions are collision-resistant
- Verification is public and repeatable

## Open Questions
- When is on-chain anchoring justified?
- How often should artifacts be anchored?
- Should multiple storage backends be used?

## Next Steps
- Integrate anchoring with proofs directory
- Define artifact naming conventions
- Prepare minimal implementation
