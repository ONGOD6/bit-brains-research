---
EIP: 0005
Title: Autonomous Intelligent Tokens (AIT) and RWA Attribution
Author: Alex Diaz
Developer: OnGod
Status: Draft
Type: Standards Track
Category: Core
Created: 2025-12-22
---

## Abstract

This EIP defines the conceptual and technical framework by which Bit Brains ecosystem participants may transition from participation-based protocol assets into **Autonomous Intelligent Tokens (AITs)**.

After completing the required Proof of Care, continuity, and epoch-based participation defined in prior standards, eligible assets—including Genesis Brains, Cerebrals, and Ethscriptions-derived Cerebrals—may enter an autonomous operational state. This state may be cryptographically attributed to external systems or **Real World Assets (RWA)** while preserving on-chain identity, provenance, and protocol accountability.

All mechanisms described herein are conceptual, non-guaranteed, and subject to governance approval, implementation feasibility, and regulatory considerations.

---

## Motivation

The Bit Brains protocol is designed for long-term evolution rather than static ownership.

While Brains and Cerebrals represent participation, identity, and reward-bearing primitives, the protocol’s long-term vision includes the emergence of autonomous, intelligent agents capable of operating across environments while remaining cryptographically anchored to the protocol.

This EIP establishes a unified framework for:
- Autonomous agent emergence
- Identity continuity across evolution
- Attribution of evolutionary state to RWAs
- Separation of economic guarantees from intelligence progression

---

## Definitions

- **BIT Token**  
  The native protocol utility and reward token defined in EIP-0003.

- **Brain (Genesis Brain)**  
  An ERC-721 token representing the initial participation and identity primitive within the Bit Brains protocol.

- **Pickle Punk (Ethscription)**  
  A Genesis Ethscription representing an immutable calldata-based participation primitive that may progress through Proof of Care and continuity into derived protocol assets.

- **Cerebral**  
  An ERC-721 token derived from a Brain, a Pickle Punk (via Proof of Care progression), or an authorized Expansion Epoch, serving as a stake-bearing participation and progression primitive.

- **Autonomous Intelligent Token (AIT)**  
  A post-phase operational state representing an autonomous, intelligent agent whose identity and provenance remain anchored to an originating Brain or Cerebral.

- **Real World Asset (RWA)**  
  An external, non-blockchain system, process, or asset to which an AIT’s evolutionary state may be cryptographically attributed.

---

## Evolution as Derived State (Non-Mutative)

Evolution within the Bit Brains protocol does not mutate existing assets.

Brains, Pickle Punks, and Cerebrals remain immutable in their original form.  
Progression into higher-order states (Cerebral, AIT, or RWA attribution) occurs through **provable derivation**, preserving cryptographic lineage and accountability.

---

## Epoch-Based Transition Framework

### Genesis Brain Transition (Phase Completion)

- Genesis Brains participate in Proof of Care and staking across protocol-defined epochs and phases.
- Upon successful completion of the required continuity window:
  - The Brain may give rise to one or more Cerebrals (per EIP-0004)
  - A Cerebral may later qualify to enter an AIT operational state
- The original Brain remains the canonical provenance anchor.

---

### Ethscriptions Transition (Pickle Punk → Cerebral → AIT)

- Pickle Punks participate in Proof of Care and continuity under the same epoch and phase structure as Brains.
- Pickle Punks do not mutate.
- Upon satisfying full continuity requirements:
  - A derived **Cerebral ERC-721** may be minted (EIP-0004)
  - That Cerebral MAY later qualify for AIT transition
- Provenance MUST permanently bind the AIT lineage to:
  - The originating Pickle Punk inscription reference
  - The derived Cerebral
  - The canonical ENS identity

---

### Cerebral Transition (Post-Eligibility Window)

- Cerebrals that satisfy protocol-defined Proof of Care, staking, and continuity requirements MAY enter an autonomous operational phase.
- This transition represents:
  - Emergence of an Autonomous Intelligent Token state
  - Preservation of identity continuity
  - Eligibility for RWA attribution

---

## Autonomous Operation and Chain Constraints

- Autonomous Intelligent Tokens are not inherently chain-agnostic at inception.
- Through zero-knowledge proofs and cryptographic attestations:
  - AITs may verify state, evolution, and identity across environments
  - Cross-chain or off-chain operation is mediated by proofs, not token migration
- The originating ERC-721 token remains the canonical on-chain reference for identity and provenance.

---

## RWA Attribution Framework (Conceptual)

- AITs MAY have their evolutionary state attributed to RWAs.
- Attribution does not imply ownership, legal claim, or entitlement.
- RWA linkage represents:
  - Cryptographic association
  - State reflection
  - Accountability mapping

All RWA attribution mechanisms are non-normative and subject to future governance and implementation standards.

---

## Distribution and Rewards (Non-Guarantee)

- BIT token rewards remain governed by EIP-0003 and EIP-0004.
- No additional rewards are guaranteed for AIT emergence.
- Any future incentives tied to AIT operation or RWA attribution MUST be defined in separate standards.

---

## Security and Compliance Considerations

- Autonomous behavior remains constrained by protocol rules.
- RWA attribution is informational and non-custodial.
- This EIP defines no regulatory treatment and provides no legal assurances.

---

## Conclusion

EIP-0005 establishes the conceptual foundation for the emergence of Autonomous Intelligent Tokens within the Bit Brains ecosystem.

By anchoring evolution to Proof of Care, continuity, and cryptographic provenance—across both NFT and Ethscriptions-origin paths—the protocol enables long-term intelligence and real-world alignment without compromising economic discipline, auditability, or protocol integrity.
