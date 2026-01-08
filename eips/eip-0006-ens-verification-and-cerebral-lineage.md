EIP: 0006
Title: Genesis Parameters, Dual-Mint Architecture, and Verification Rails
Author: Alex Diaz
Developer: OnGod
Status: Draft
Type: Standards Track
Category: Core
Created: 2025-12-22

---

## Abstract

This EIP defines the Genesis parameters of the Bit Brains protocol, including
initial supply, dual-mint architecture, identity assignment, and immutable
verification rails.

Genesis parameters define what exists at protocol inception. They do not define
future behavior, incentives, or guarantees, and may evolve through governance
without violating core protocol principles.

---

## Genesis Supply Parameters

At Genesis, the Bit Brains protocol issues two parallel asset supplies.

### Genesis Brain Supply

- Total Genesis Brains: 1,500
- Public Allocation: 1,400
- Team / Treasury Allocation: 100

### Pickle Punk Supply

- Total Pickle Punks: 1,500
- Public Allocation: 1,400
- Team / Treasury Allocation: 100

Genesis Brains and Pickle Punks are distinct ERC-721 NFTs.
Neither asset is metadata of the other.

---

## Dual-Mint Architecture

Genesis participation is established through a dual-mint process.

For each Genesis entry, the protocol issues:

1. One Genesis Brain (ERC-721 NFT)
2. One Pickle Punk (ERC-721 NFT)

Both assets are protocol-recognized participation primitives and may progress
independently through Proof of Care, continuity, and evolution standards.

Dual minting does not imply dependency, ownership coupling, or behavioral linkage
between assets.

---

## Ethscription Verification Rail (Calldata Truth Layer)

For each Genesis Brain and each Pickle Punk minted, the protocol SHALL commit an
immutable verification record to Ethereum transaction calldata.

This Ethscription Verification Hash:

- Establishes a timestamped, verifiable truth that the asset was created within
  the Bit Brains Genesis context
- Is immutable and permanently recorded on Ethereum
- Does not require custody, wrapping, or mutation of the NFT
- Does not alter ownership semantics

Verification hashes MAY be referenced by future protocol advancements but SHALL
never be modified or revoked.

---

## ENS Identity Assignment

At Genesis mint, each participant receives an ENS subdomain under:

<index>.bitbrains.eth

The assigned ENS identity becomes the canonical reference for:

- Proof of Care signaling
- Staking participation
- Reward routing
- Lineage and derivation references
- Zero-knowledge accountability proofs

ENS resolution is a required protocol primitive.

---

## Phase and Epoch References

Genesis Brains, Pickle Punks, and any derived assets participate in protocol phases
and epochs as defined in subsequent standards.

Genesis parameters reference the following asset-specific continuity windows:

- Genesis Brains: five (5) epochs
- Cerebrals: four (4) epochs
- Brainiacs: three (3) epochs

Eligibility for Autonomous Intelligent Technology (AIT) activation is evaluated
independently per asset class and becomes effective immediately upon completion
of the applicable continuity window, as defined in EIP-0005.

---

## Zero-Knowledge Proof Commitment

The protocol commits that Proof of Care, staking continuity, and eligibility
determinations SHALL be verifiable via zero-knowledge proofs.

This EIP does not define proof systems, circuits, or implementations.

---

## Non-Invariants

Genesis parameters define initial conditions only.

They do not represent immutable protocol invariants and may be revised through
future governance, provided that:

- Existing on-chain records remain valid
- Verification rails remain immutable
- Identity and lineage guarantees are preserved

---

## Conclusion

EIP-0006 establishes the foundational truth layer of the Bit Brains protocol,
including Genesis supply, dual-mint architecture, ENS identity assignment, and
immutable calldata verification rails, upon which all future participation,
evolution, and intelligence standards are built.
