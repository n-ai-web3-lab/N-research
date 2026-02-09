# Experiment 001: On-Chain vs Off-Chain Boundary

## Status
Draft

## Purpose
Define which components of Experiment 001 may interact with
on-chain systems and which must remain strictly off-chain to
preserve security, decentralization, and user sovereignty.

## On-Chain Allowed (Strictly Limited)
- Smart contract rule enforcement
- Deterministic validation of inputs
- User signature verification
- Execution of explicitly approved actions

## On-Chain Forbidden (Never Allowed)
- AI reasoning or inference
- Model identifiers or prompts
- Probabilistic confidence scores
- Suggested actions or opinions

## Off-Chain Required
- AI analysis and planning
- Data aggregation and normalization
- Natural language explanations
- Risk interpretation

## Justification
AI outputs are non-deterministic and probabilistic.
Placing them on-chain would:
- Break determinism
- Introduce governance risk
- Create false authority

## Trust Model
- Blockchain: rule enforcer
- AI: untrusted advisor
- User: final authority

## Attack Scenarios Prevented
- AI output replay attacks
- Prompt injection affecting contracts
- AI model replacement without notice
- Hidden automation paths

## Open Questions
- What minimal hashes, if any, may be anchored on-chain?
- How should off-chain data availability be guaranteed?
- Can zero-knowledge proofs play a role here?

## Next Steps
- Decide anchoring strategy
- Map boundary to Architecture 001
- Prepare minimal implementation plan
