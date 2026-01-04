EIP: 0002
Title: Epoch Proof-of-Care (EPO) for Genesis Participants
Author: Alex Diaz  
Developer: OnGod
Status: Draft
Type: Standards Track
Created: 2025-12-21
Requires: EIP-0001
---

## Abstract

This EIP defines the Epoch Proof-of-Care (EPO) mechanism for Genesis participation primitives within the Bit Brains protocol.

Epochs provide discrete, time-based evaluation windows during which participation and care are measured to determine influence, progression, and reward eligibility. The mechanism prioritizes patience, sustained alignment, and simplicity over complex incentive structures.

This EIP applies uniformly to all recognized Genesis participation primitives, including Brains and Ethscriptions, while allowing downstream standards to define differentiated outcomes.

---

## Motivation

Many decentralized systems reward passive ownership or short-term optimization rather than sustained care.

Bit Brains requires a mechanism that:
- Rewards patience and long-term participation
- Provides recurring accountability through time
- Prevents permanent influence capture
- Remains simple, explainable, and auditable at early stages

Epoch Proof-of-Care establishes these properties without introducing derivative cycles, productivity flywheels, or premature complexity.

---

## Definitions

- **Genesis Participant**  
  A protocol-recognized participation primitive introduced at Genesis, including Brains (ERC-721 NFTs) and Pickle Punks (Ethscriptions).

- **Brain (AIT-capable)**  
  An ERC-721 Genesis NFT whose influence emerges from epoch-based evaluation, accumulated Proof-of-Care, and temporal continuity.

- **Pickle Punk (Ethscription)**  
  An immutable calldata-based Genesis participation artifact that participates in Epoch Proof-of-Care and continuity evaluation.

- **Epoch**  
  A fixed-duration accounting period during which Proof-of-Care is measured and influence or eligibility is evaluated.

- **Proof-of-Care (PoC)**  
  A composite set of verifiable behaviors demonstrating sustained, constructive engagement during an epoch.

---

## Epoch Applicability

Epoch Proof-of-Care applies to all Genesis Participants.

- Brains participate in EPO as stake-bearing, reward-eligible primitives.
- Pickle Punks participate in EPO as non-staking participation primitives whose outcomes are defined in subsequent EIPs.

Participation in EPO does not guarantee rewards, progression, or economic influence. Outcomes are determined by protocol-defined rules layered atop this mechanism.

---

## Epoch Duration

Epochs are fixed-duration evaluation windows.

- Epoch length is approximately **one (1) month**
- Epochs repeat continuously
- Evaluation occurs at each epoch boundary

Epoch duration is parameterized and MAY be adjusted in future EIPs, provided such changes remain consistent with the stewardship principles defined in EIP-0001.

---

## Epoch Lifecycle

Each epoch proceeds through the following phases:

1. **Initialization**  
   Epoch parameters are fixed and the prior epoch state is finalized.

2. **Active Phase**  
   Genesis Participants engage with the protocol and Proof-of-Care signals are accumulated.

3. **Finalization**  
   Proof-of-Care signals are evaluated and eligibility, influence renewal, or progression status is determined.

4. **Transition**  
   Influence renewal, decay, or eligibility outcomes are applied and the next epoch begins.

---

## Proof-of-Care Signals

Proof-of-Care is a composite signal composed of multiple verifiable behaviors that may evolve over time.

Examples include:
- Sustained participation across consecutive epochs
- Adherence to continuity commitments
- Actions that support network health, alignment, and non-interference

Asset ownership or capital provision alone does not constitute Proof-of-Care.  
Care must be demonstrated through continued participation over time.

---

## Influence, Eligibility, and Rewards

Influence is earned, not permanent.

- Influence renews through continued Proof-of-Care
- Influence decays in the absence of participation
- Rewards follow influence and eligibility, not the reverse

Epoch boundaries ensure that influence remains renewable and contingent on patience and alignment.

Specific reward mechanisms, staking requirements, and progression outcomes are defined in subsequent EIPs.

---

## Simplicity and Patience

The Bit Brains protocol intentionally prioritizes simplicity in its initial design.

Rather than introducing multiple incentive loops or productivity amplifiers, the system rewards patience through sustained participation across epochs.

Additional mechanisms are intentionally deferred to future EIPs once the core Epoch Proof-of-Care mechanics are validated.

---

## Rationale

Epoch-based evaluation introduces accountability through time.  
Proof-of-Care introduces alignment through action.  
Simplicity preserves legitimacy and long-term adaptability.

Epoch rewards, where applicable, are allocated based on protocol-defined eligibility. Advancement and reward release are contingent upon satisfying Proof-of-Care criteria. In cases where Proof-of-Care is insufficient, rewards remain locked and progression is delayed until requirements are met. Rewards are neither slashed nor redistributed.

---

## Security Considerations

Potential risks include:
- Sybil participation
- Strategic epoch boundary behavior
- Manipulation of care signals

Mitigation strategies will be addressed in future EIPs.

---

## Copyright

Copyright and related rights waived via CC0.
