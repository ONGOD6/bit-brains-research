EIP: 0002
Title: Epoch Proof-of-Care (EPO) for Genesis Participants
Author: Alex Diaz
Developer: OnGod
Status: Draft
Type: Standards Track
Created: 2025-12-21
Requires: EIP-0001, EIP-0011, Genesis Parameters
---

## Abstract

This EIP defines the Epoch Proof-of-Care (EPO) mechanism for Genesis
participation primitives within the Bit Brains protocol.

Epochs provide discrete, time-based evaluation windows during which
participation and care are measured to determine eligibility, continuity,
and potential progression under protocol rules.

This mechanism prioritizes patience, sustained alignment, and simplicity
over extraction-driven or speculative incentive structures.

This EIP applies uniformly to all recognized Genesis participation
primitives, including ERC-721 NFTs and their associated Ethscription
artifacts, while deferring reward settlement and evolution outcomes to
Genesis Parameters and subsequent EIPs.

---

## Motivation

Many decentralized systems reward passive ownership or short-term
optimization rather than sustained care.

Bit Brains requires a mechanism that:
- Rewards patience and long-term participation
- Provides recurring accountability through time
- Prevents permanent influence capture
- Remains simple, explainable, and auditable at early stages

Epoch Proof-of-Care establishes these properties without introducing
derivative cycles, productivity flywheels, or premature complexity.

---

## Canonical Genesis Reference

This EIP inherits and defers to the Bit Brains Genesis Parameters.

Genesis parameters define the initial conditions of the protocol at
inception. They do not represent protocol invariants and may evolve
through governance, future EIPs, or community consensus without
violating core protocol principles.

Nothing in this EIP guarantees rewards, settlement timing, or permanent
influence.

---

## Definitions

- **Genesis Participant**  
  A protocol-recognized participation primitive introduced at Genesis,
  including ERC-721 assets and their associated secondary Ethscription
  artifacts, together forming a dual-pathway on-chain record of Genesis
  participation on Ethereum.

- **Brain (AIT-capable)**  
  A Genesis ERC-721 NFT whose participation may, through Proof-of-Care
  and continuity, activate **Autonomous Intelligence Technology (AIT)
  capability**, as defined in EIP-0011.

- **Pickle Punk**  
  A Genesis ERC-721 NFT with an associated Ethscription artifact serving
  as an immutable calldata-based provenance record, participating in
  Epoch Proof-of-Care under protocol-defined rules.

- **Epoch**  
  A fixed-duration accounting period during which Proof-of-Care is
  measured and eligibility or continuity status is evaluated.

- **Proof-of-Care (PoC)**  
  A composite set of verifiable behaviors demonstrating sustained,
  constructive engagement during an epoch.

---

## Epoch Applicability

Epoch Proof-of-Care applies to **all Genesis Participants**.

Genesis Participants:
- may be staked under protocol-defined rules,
- are evaluated uniformly for Proof-of-Care and continuity, and
- may produce differentiated outcomes as defined in subsequent EIPs.

Participation in EPO does not guarantee rewards, progression, or
economic influence. All outcomes are contingent on Genesis Parameters,
Proof-of-Care continuity, and governance-defined thresholds.

---

## Epoch Duration

Epochs are fixed-duration evaluation windows.

- Epoch length is approximately **one (1) month**
- Epochs repeat continuously
- Evaluation occurs at each epoch boundary

Epoch duration is parameterized and MAY be adjusted in future EIPs,
provided such changes remain consistent with the stewardship principles
defined in EIP-0001.

---

## Epoch Lifecycle

Each epoch proceeds through the following phases:

1. **Initialization**  
   Epoch parameters are fixed and the prior epoch state is finalized.

2. **Active Phase**  
   Genesis Participants engage with the protocol and Proof-of-Care
   signals are accumulated.

3. **Finalization**  
   Proof-of-Care signals are evaluated and continuity or eligibility
   status is recorded.

4. **Transition**  
   Continuity status is carried forward and the next epoch begins.

No reward settlement is required or implied at individual epoch
boundaries.

---

## Proof-of-Care Signals

Proof-of-Care is a composite signal composed of multiple verifiable
behaviors that may evolve over time.

Examples include:
- Sustained participation across consecutive epochs
- Adherence to continuity commitments
- Actions that support network health, alignment, and non-interference

Asset ownership alone does not constitute Proof-of-Care. Care must be
demonstrated through continued participation over time.

---

## Influence, Eligibility, and Rewards

Epoch Proof-of-Care determines **eligibility and continuity**, not
automatic reward distribution.

- Influence is renewable through continued Proof-of-Care
- Influence decays in the absence of participation
- Reward eligibility accrues through sustained alignment

Reward settlement, where applicable, occurs only at governance-defined
phase boundaries and is specified in Genesis Parameters and subsequent
reward EIPs.

---

## Simplicity and Patience

The Bit Brains protocol intentionally prioritizes simplicity in its
initial design.

Rather than introducing multiple incentive loops or productivity
amplifiers, the system rewards patience through sustained participation
across epochs.

Additional mechanisms are intentionally deferred to future EIPs once the
core Epoch Proof-of-Care mechanics are validated.

---

## Rationale

Epoch-based evaluation introduces accountability through time.
Proof-of-Care introduces alignment through action.
Simplicity preserves legitimacy and long-term adaptability.

Epoch Proof-of-Care establishes a neutral, auditable eligibility layer
upon which reward settlement and evolution may later occur.

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
