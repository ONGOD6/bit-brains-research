EIP: 0006
Title: Genesis Parameters, Independent Minting, and Verification Rails
Author: Alex Diaz
Developer: OnGod
Status: Draft
Type: Standards Track
Category: Core
Created: 2025-12-22

---

## Abstract

This EIP defines the Genesis parameters of the Bit Brains protocol, including
initial asset supplies, independent minting architecture, identity assignment,
and immutable verification rails.

Genesis parameters define what exists at protocol inception. They do not define
future behavior, incentives, or guarantees, and may evolve through governance
without violating core protocol principles.

---

## Genesis Supply Parameters

At Genesis, the Bit Brains protocol introduces two independent ERC-721 NFT
collections with separate mint flows and equal standing at the protocol layer.

### Genesis Brains

- Total Supply: 1,500
- Public Allocation: 1,400
- Team / Treasury Allocation: 100

### Pickle Punks

- Total Supply: 1,500
- Public Allocation: 1,400
- Team / Treasury Allocation: 100

Genesis Brains and Pickle Punks are distinct collections.
Minting one does not require minting the other.

---

## Independent Genesis Minting

Genesis participation is established through **independent minting** of protocol
assets.

Participants MAY choose to mint:
- A Genesis Brain
- A Pickle Punk
- Both assets through separate mint actions

There is no bundled or forced issuance of multiple NFTs.
Each asset stands on its own mint, supply, and participation path.

---

## Per-Asset Dual Record Structure

For each Genesis asset minted—whether a Genesis Brain or a Pickle Punk—the protocol
creates a **dual record**:

1. One ERC-721 NFT
2. One immutable verification record committed to Ethereum transaction calldata

This dual record structure applies independently to each asset mint.

---

## Ethscription Verification Rail (Calldata Truth Layer)

For every Genesis Brain and every Pickle Punk minted, the protocol SHALL commit an
immutable verification record to Ethereum transaction calldata.

This verification record (Ethscription Verification Hash):

- Establishes a timestamped, verifiable truth that the asset was minted within the
  Bit Brains Genesis context
- Is immutable once committed
- Does not require custody, wrapping, or mutation of the ERC-721 NFT
- Does not alter ownership semantics
- Exists independently of off-chain indexing or metadata

Verification records MAY be referenced by future protocol advancements but SHALL
never be modified or revoked.

---

## ENS Identity Assignment

Upon minting, each Genesis ERC-721 NFT is assigned a canonical ENS subdomain under:

<index>.bitbrains.eth

This ENS identity:

- Persists throughout the asset lifecycle
- Serves as the canonical routing identity for rewards
- Anchors Proof-of-Care, continuity, and accountability
- Supports lineage, derivation, and zero-knowledge proofs

ENS resolution is a required protocol primitive for participation and rewards.

---

## Phase and Epoch References

Genesis Brains and Pickle Punks participate in Proof-of-Care and continuity under
protocol-defined phases and epochs as defined in subsequent standards.

Genesis parameters reference the following asset-specific continuity windows:

- Genesis Brains: five (5) epochs
- Cerebrals: four (4) epochs
- Brainiacs: three (3) epochs

Eligibility for Autonomous Intelligent Technology (AIT) activation is evaluated
independently per asset class and becomes effective immediately upon completion
of the applicable continuity window, as defined in EIP-0005.

---

## Zero-Knowledge Proof Commitment

The protocol commits that Proof-of-Care, staking continuity, and eligibility
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
including Genesis supplies, independent minting of protocol assets, ENS identity
assignment, and immutable calldata-based verification rails upon which all future
participation, evolution, and intelligence standards are built.
