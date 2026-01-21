EIP: 0005
Title: Autonomous Intelligent Technology (AIT) and RWA Attribution Framework
Author: Alex Diaz
Developer: OnGod
Status: Draft
Type: Standards Track
Category: Core
Created: 2025-12-22
Requires: EIP-0001, EIP-0002, EIP-0003, EIP-0004, Ethscriptions Rail EIP

---

## Abstract

This EIP defines the canonical framework by which Bit Brains protocol assets
may evolve from participation-based primitives into **Autonomous Intelligent
Technology (AIT)** and, where applicable, into **Node execution capability**.

AIT activation and Node derivation are evaluated **only at the Paired Asset
level**, composed of a canonical ERC-721 asset and its corresponding
Ethscription artifact.

All evolution is:
- non-mutative,
- dual-asset gated,
- continuity-dependent, and
- cryptographically verifiable.

This EIP defines **capability activation**, not economic guarantees, reward
entitlements, or execution mandates.

---

## Motivation

The Bit Brains protocol is designed for long-horizon evolution rather than
static ownership or extractive participation.

While Genesis assets function as identity, participation, and stewardship
primitives, the protocol’s long-term vision includes the emergence of
autonomous, intelligent systems that operate across environments while
remaining cryptographically anchored to protocol identity and accountability.

This EIP establishes a unified framework for:
- autonomous intelligence emergence,
- dual-asset identity continuity,
- non-mutative capability derivation,
- optional attribution to Real World Assets (RWAs), and
- strict separation of intelligence activation from economic guarantees.

---

## Definitions

- **ERC-721 Asset**  
  A canonical Bit Brains protocol NFT (Brain, Cerebral, Brainiac, Pickle Punk,
  or successor).

- **Ethscription Artifact**  
  An immutable calldata-provenance artifact committed to Ethereum via the
  Ethscriptions mechanism, paired one-to-one with an ERC-721 Asset.

- **Paired Asset**  
  The inseparable protocol participation unit composed of:
  1) an ERC-721 Asset, and  
  2) its associated Ethscription Artifact.

  All Proof-of-Care evaluation, continuity accumulation, AIT activation,
  Node derivation, and RWA attribution apply exclusively to the Paired Asset.

- **Autonomous Intelligent Technology (AIT)**  
  A non-mutative operational capability state activated for a Paired Asset
  after satisfying continuity, Proof-of-Care, and dual-staking requirements.

- **Node**  
  A derived execution-capability state that MAY be instantiated upon AIT
  activation, cryptographically bound to the originating Paired Asset.

- **Real World Asset (RWA)**  
  An external system, process, or organization to which an AIT or Node state
  MAY be cryptographically attributed for accountability purposes only.

---

## Evolution as Derived Capability (Non-Mutative)

Evolution within the Bit Brains protocol **does not mutate assets**.

ERC-721 tokens and Ethscription artifacts remain immutable in their original
form. Higher-order states (AIT and Node) are derived capabilities proven via
zero-knowledge verification and lineage integrity.

The originating Paired Asset remains the sole canonical identity anchor.

---

## Dual-Asset Evolution Invariant (Canonical)

AIT activation and Node derivation SHALL occur **only** when:

1. The ERC-721 Asset is staked or maintained in good standing, AND  
2. The paired Ethscription Artifact is concurrently staked, registered, or
   otherwise maintained in protocol-defined good standing.

If either component becomes non-compliant, the Paired Asset is ineligible
for AIT activation, Node derivation, or continuity accumulation.

No asset may evolve independently.

---

## Epoch- and Phase-Based Eligibility

This EIP does not define epoch counts or phase durations.

Eligibility for AIT activation is determined by:
- Proof-of-Care completion,
- continuity satisfaction,
- and sustained dual-asset qualification,

as defined by Genesis Parameters and applicable phase standards.

All eligibility is evaluated **per Paired Asset**, not per component.

---

## AIT Eligibility by Asset Class (Paired Assets)

### Genesis Brain Paired Asset

- Participates in Proof-of-Care across five (5) epochs
- Upon completion of Epoch Five:
  - Rewards MAY be settled per EIP-0003
  - The Paired Asset becomes AIT-eligible

### Pickle Punk Paired Asset

- Participates in Proof-of-Care under its defined continuity window
- Upon completion:
  - Rewards MAY be settled per EIP-0003
  - The Paired Asset becomes AIT-eligible

### Cerebral Paired Asset

- Participates across four (4) epochs
- Upon completion:
  - The Paired Asset becomes AIT-eligible

### Brainiac Paired Asset

- Participates across three (3) epochs
- Upon completion:
  - The Paired Asset becomes AIT-eligible

---

## Autonomous Operation and Node Derivation

AIT activation represents recognition of autonomous operational capability.

Upon AIT activation, a **Node MAY be instantiated** as an execution-capable
representation of the Paired Asset.

Node derivation:
- is non-mutative,
- does not replace the originating asset,
- and remains cryptographically bound to the Paired Asset’s lineage.

Node minting, where applicable, MUST occur as a **dual mint**
(ERC-721 Node + paired Ethscription), as defined by the Ethscriptions Rail EIP.

---

## RWA Attribution Framework (Conceptual)

AIT-enabled Paired Assets or Nodes MAY have their operational state
cryptographically attributed to Real World Assets (RWAs).

Attribution:
- establishes accountability and association only,
- implies no ownership or legal claim,
- conveys no guaranteed yield or entitlement.

All RWA attribution mechanisms are non-normative and subject to future EIPs.

---

## Distribution and Rewards (Non-Guarantee)

No rewards are guaranteed for:
- AIT activation,
- Node derivation, or
- RWA attribution.

All reward logic is governed exclusively by EIP-0003, Genesis Parameters,
and governance-defined settlement rules.

---

## Security and Compliance Considerations

- Autonomous behavior remains bounded by protocol rules
- Dual-asset requirements reduce spoofing and lineage attacks
- RWA attribution is non-custodial and informational only
- This EIP defines no regulatory treatment or compliance guarantees

---

## Conclusion

EIP-0005 establishes the canonical framework for Paired Asset evolution into
Autonomous Intelligent Technology (AIT) and Node capability within the
Bit Brains protocol.

It preserves identity, provenance, and accountability while enabling
autonomous operation — without mutating assets, fragmenting evolution,
or introducing economic guarantees.

---

## Copyright

CC0-1.0
