---
EIP: 0006
Title: Proof of Care Continuity and Staking Enforcement
Author: Alex Diaz
Developer: OnGod
Status: Draft
Type: Standards Track
Category: Core
Created: 2025-12-26
Requires: EIP-0001, EIP-0002, EIP-0003, EIP-0004
---

## Abstract

This EIP defines the continuity enforcement rules for Proof of Care (PoC) and staking within the Bit Brains Protocol.

It establishes mandatory continuity requirements across epochs and phases, specifies disqualification and eligibility rules, and defines how interruptions in participation affect rewards, progression, and advancement into higher protocol states.

This EIP applies uniformly across all Genesis participation primitives, including Brains, Pickle Punks (Ethscriptions), and derived Cerebrals, without altering the underlying epoch or reward mechanics defined in earlier standards.

---

## Motivation

The Bit Brains protocol prioritizes long-term alignment over short-term participation.

Without explicit continuity enforcement, participants could extract rewards by temporarily participating at critical moments without maintaining sustained care. This EIP ensures that Proof of Care is not symbolic but continuous, measurable, and enforceable.

Continuity is treated as a protocol invariant rather than an optional behavior.

---

## Definitions

- **Continuity**  
  Uninterrupted satisfaction of Proof of Care requirements across a defined sequence of epochs.

- **Proof of Care (PoC)**  
  Verifiable behaviors demonstrating sustained, constructive participation as defined in EIP-0002.

- **Epoch**  
  A fixed-duration accountability window during which PoC is evaluated.

- **Phase**  
  A group of five (5) consecutive epochs forming a reward settlement boundary.

- **Genesis Participant**  
  A protocol-recognized participation primitive introduced at Genesis, including Brains and Pickle Punks.

- **Staking Asset**  
  An asset that is required to remain staked to maintain continuity, as defined by protocol rules.

---

## Continuity Requirement (Global)

Continuity is mandatory for:

- Reward eligibility
- Advancement between phases
- Cerebral mint eligibility
- Autonomous Intelligent Token (AIT) eligibility
- RWA attribution eligibility

Failure to maintain continuity during a required window results in delayed or reduced eligibility.

---

## Continuity Windows

Continuity is evaluated over explicit windows defined by protocol phase rules.

### Phase-Level Continuity

- Each Phase consists of five (5) epochs
- Full continuity requires uninterrupted PoC across all five epochs
- Partial continuity MAY be recognized for reduced outcomes as defined in later EIPs

---

## Staking and Continuity Enforcement

### Brains

- Brains MUST remain staked continuously during required continuity windows
- Unstaking during a required window breaks continuity
- Breaking continuity disqualifies the Brain from full eligibility for that Phase

### Pickle Punks (Ethscriptions)

- Pickle Punks do not stake
- Continuity is enforced through:
  - Proof of Care signals
  - Identity persistence (ENS)
  - Epoch participation validation

Failure to satisfy continuity requirements disqualifies the Pickle Punk from progression outcomes for that window.

---

## Continuity Failure and Recovery

- Continuity failure does NOT permanently disqualify a participant
- Failed windows MUST be reattempted in full
- Progression resumes only after continuity is re-established across a complete window

Continuity failures do not slash rewards and do not redistribute locked rewards.

---

## Impact on Rewards

- Rewards accrue only during epochs where continuity is maintained
- Rewards associated with incomplete continuity windows remain locked
- Locked rewards MAY become claimable once continuity is successfully re-established

Rewards are never redistributed to other participants.

---

## Interaction with Cerebral Minting

- Genesis Cerebral mint eligibility requires full continuity across the defined eligibility window
- Partial continuity MAY reduce mint quantity or delay mint eligibility
- Continuity enforcement applies equally to:
  - Brain-derived Cerebrals
  - Pickle Punk–derived Cerebrals

---

## Interaction with AIT Eligibility

- AIT eligibility requires uninterrupted continuity across protocol-defined windows
- Continuity failure delays, but does not eliminate, AIT eligibility
- All AIT lineage remains bound to the originating asset via ENS and immutable metadata

---

## Non-Custodial Enforcement

Continuity enforcement does not require:

- Custody of participant funds
- Forced transactions
- Automatic slashing

All enforcement occurs through eligibility gating and reward locking.

---

## Security Considerations

Continuity enforcement mitigates:

- Opportunistic participation
- Epoch boundary exploitation
- Reward extraction without sustained care

No enforcement mechanism may introduce discretionary or subjective judgment.

---

## Governance Considerations

Changes to continuity windows, enforcement severity, or recovery rules require governance approval and MUST be defined in subsequent EIPs.

---

## Conclusion

This EIP establishes continuity as a core invariant of the Bit Brains Protocol.

By enforcing uninterrupted Proof of Care across defined windows, the protocol ensures that rewards, progression, and autonomous evolution remain aligned with long-term stewardship rather than short-term participation.

---

## Copyright

Copyright and related rights waived via CC0.
