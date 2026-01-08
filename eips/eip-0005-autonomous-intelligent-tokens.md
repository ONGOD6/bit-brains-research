EIP: 0005
Title: Autonomous Intelligent Technology (AIT) and RWA Attribution Framework
Author: Alex Diaz
Developer: OnGod
Status: Draft
Type: Standards Track
Category: Core
Created: 2025-12-22

---

## Abstract

This EIP defines the conceptual and technical framework by which Bit Brains protocol
assets may evolve from participation-based primitives into Autonomous Intelligent
Technology (AIT).

After completing the Proof of Care, continuity, and epoch-based participation
requirements applicable to a given asset class, eligible assets—including Genesis
Brains, Cerebrals, Brainiacs, and dual-minted Pickle Punk NFTs—MAY enter an autonomous
operational state.

AIT eligibility is evaluated independently per asset class and becomes effective
immediately upon completion of that asset’s required continuity window, as defined
in Genesis and phase parameters.

All mechanisms described herein are conceptual, non-guaranteed, and subject to
governance approval, implementation feasibility, and regulatory considerations.

---

## Motivation

The Bit Brains protocol is designed for long-term evolution rather than static ownership.

While Brains, Cerebrals, Brainiacs, and Pickle Punks function as identity, participation,
and reward-bearing primitives, the protocol’s long-term vision includes the emergence
of autonomous, intelligent systems capable of operating across environments while
remaining cryptographically anchored to the protocol.

This EIP establishes a unified framework for:

- Autonomous intelligent system emergence
- Identity continuity across evolution
- Non-mutative derivation of autonomous states
- Optional attribution of evolved state to Real World Assets (RWAs)
- Explicit separation of intelligence progression from economic guarantees

---

## Definitions

Brain Intelligence Token (BIT)
The native protocol utility and reward token defined in EIP-0003.

Genesis Brain (Brain)
An ERC-721 token representing the original participation and identity primitive
within the Bit Brains protocol.

Pickle Punk (Pickle Punk NFT)
An ERC-721 token minted alongside a Genesis Brain as part of a dual-mint Genesis entry.
Pickle Punks represent a parallel participation rail that may progress through Proof of Care
and continuity into derived protocol assets.

Dual Mint (Genesis Dual Mint)
A Genesis mint flow in which two distinct assets are issued to the minter:
(1) a Genesis Brain (ERC-721) and (2) a Pickle Punk (ERC-721).
Both assets are protocol-recognized participation primitives and may be evaluated
independently under their applicable continuity windows.

Ethscription Verification Hash (Calldata Record)
An immutable Ethereum calldata-committed verification record associated with a minted asset.
For each Genesis Brain and each Pickle Punk minted, a corresponding verification hash
SHALL be committed to Ethereum transaction calldata to establish a timestamped,
verifiable truth record linking the asset to its Genesis mint context and protocol rail.
This record does not require custody, wrapping, or mutation of the underlying asset.

Cerebral
An ERC-721 token derived from a Brain, a Pickle Punk, or an authorized expansion
epoch, serving as a stake-bearing participation and progression primitive.

Brainiac
A later-stage protocol asset representing an accelerated participation class with
a reduced continuity window.

Autonomous Intelligent Technology (AIT)
A derived, non-mutative operational state representing autonomous execution
capability cryptographically anchored to an originating protocol asset.

Node
A derived execution-capability state that MAY be instantiated upon AIT activation.
Node derivation is non-mutative and remains cryptographically bound to the originating
asset and its identity/provenance records.

Real World Asset (RWA)
An external system, process, or business entity to which an AIT’s or Node’s state MAY be
cryptographically attributed.

---

## Evolution as Derived State (Non-Mutative)

Evolution within the Bit Brains protocol does not mutate existing assets.

Brains, Pickle Punks, Cerebrals, and Brainiacs remain immutable in their original form.
Progression into higher-order states (Cerebral, AIT, Node, or RWA attribution) occurs
through provable derivation, preserving cryptographic lineage, identity continuity,
and protocol accountability.

---

## Epoch- and Phase-Based Eligibility

This EIP does not define epoch counts or phase durations.

Eligibility for AIT transition is determined by the completion of Proof of Care,
staking, and continuity requirements specific to the asset class, as defined in
Genesis and phase parameter standards.

Each asset class is evaluated independently and is not gated by the progression
or maturity of other classes.

---

## Genesis Brain to AIT Eligibility

Genesis Brains participate in Proof of Care and staking across five (5)
protocol-defined epochs.

Upon successful completion of Epoch Five:
- BIT rewards MAY be distributed per applicable reward standards
- The Genesis Brain becomes AIT-eligible immediately

The original Brain remains the canonical provenance and identity anchor.

---

## Pickle Punk to AIT Eligibility

Pickle Punks participate in Proof of Care and staking under protocol-defined epochs
and phases applicable to the Pickle Punk rail.

Upon successful completion of the required continuity window for the Pickle Punk rail:
- BIT rewards MAY be distributed per applicable reward standards
- The Pickle Punk becomes AIT-eligible immediately

Pickle Punk lineage remains cryptographically anchored to its Genesis mint context
and its Ethscription Verification Hash (Calldata Record).

---

## Cerebral to AIT Eligibility

Cerebrals participate in Proof of Care and continuity across four (4) epochs.

Upon completion of Epoch Four:
- The Cerebral becomes AIT-eligible immediately

Cerebral AIT lineage remains cryptographically bound to its originating asset.

---

## Brainiac to AIT Eligibility

Brainiacs participate in Proof of Care and continuity across three (3) epochs.

Upon completion of Epoch Three:
- The Brainiac becomes AIT-eligible immediately

Brainiacs represent the most accelerated participation class.

---

## Autonomous Operation and Node Derivation

Entry into AIT represents the activation of autonomous operational capability.

AIT emergence MAY give rise to a Node, representing execution capacity derived from
the originating asset.

Node derivation is non-mutative and does not replace the originating asset.

The originating Brain, Pickle Punk, Cerebral, or Brainiac remains the canonical on-chain
identity and staking reference.

---

## RWA Attribution Framework (Conceptual)

AIT systems and/or Nodes MAY have their operational state attributed to Real World Assets (RWAs).

Attribution represents cryptographic association and accountability only.

Attribution does not imply ownership, legal claim, entitlement, or guaranteed yield.

All RWA attribution mechanisms are non-normative and subject to future standards.

---

## Distribution and Rewards (Non-Guarantee)

BIT rewards are governed by EIP-0003 and EIP-0004.

No rewards are guaranteed for AIT activation, Node derivation, or RWA attribution.

Any future incentives MUST be defined in separate standards.

---

## Security and Compliance Considerations

Autonomous behavior remains constrained by protocol rules.

RWA attribution is informational and non-custodial.

This EIP defines no regulatory treatment and provides no legal assurances.

---

## Conclusion

EIP-0005 defines the framework for asset-specific evolution into Autonomous
Intelligent Technology (AIT) within the Bit Brains protocol, enabling autonomous
operation while preserving identity, provenance, and accountability, without
introducing economic guarantees or mutating existing assets.
