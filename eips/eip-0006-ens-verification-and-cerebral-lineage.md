EIP: 0006
Title: Genesis Parameters, Independent Minting, and Verification Rails
Author: Alex Diaz
Developer: OnGod
Status: Draft
Type: Standards Track
Category: Core
Created: 2025-12-22
Requires: EIP-0001, EIP-0002, EIP-0004, EIP-0005, Ethscriptions Rail EIP

---

## Abstract

This EIP defines the Genesis parameters of the Bit Brains protocol, including
initial asset supplies, independent minting architecture, identity assignment,
and immutable verification rails.

Genesis parameters define what exists at protocol inception. They do not define
future behavior, incentives, guarantees, or evolution outcomes, and may evolve
through governance without violating core protocol principles.

This EIP formalizes independent minting with paired verification, ensuring that
every Genesis asset is anchored by immutable calldata provenance while preserving
non-custodial ownership and long-term extensibility.

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

Genesis Brains and Pickle Punks are distinct collections with independent supply
constraints and minting processes.

---

## Independent Genesis Minting (Canonical)

Genesis participation is established through independent minting of protocol
assets.

Participants MAY choose to mint:
- a Genesis Brain,
- a Pickle Punk, or
- both assets through separate mint actions.

There is no bundled issuance requirement and no forced pairing between different
ERC-721 collections.

Each independent mint, however, produces a Paired Asset as defined below.

---

## Canonical Paired Asset Formation

For every Genesis mint — whether a Genesis Brain or a Pickle Punk — the protocol
creates a Paired Asset composed of:

1. One ERC-721 NFT, and
2. One immutable verification record committed to Ethereum transaction calldata
   (an Ethscription artifact).

The ERC-721 asset and its associated Ethscription artifact are inseparable at the
protocol level and together form the sole unit of participation, continuity, and
evolution.

Neither component is recognized independently for protocol qualification.

---

## Ethscription Verification Rail (Calldata Truth Layer)

For every Genesis ERC-721 NFT minted, the protocol SHALL commit a corresponding
immutable verification record to Ethereum transaction calldata.

This Ethscription verification artifact:

- Establishes a timestamped, verifiable Genesis truth
- Is immutable once committed
- Does not require custody, wrapping, or mutation of the ERC-721 NFT
- Does not alter ownership semantics
- Exists independently of off-chain indexing or metadata systems

Verification artifacts MAY be referenced by future protocol advancements but
SHALL never be modified, revoked, or replaced.

---

## ENS Identity Assignment

Upon minting, each Genesis ERC-721 NFT is assigned a canonical ENS subdomain under:

<index>.bitbrains.eth

This ENS identity:

- Persists throughout the asset lifecycle
- Serves as the canonical routing identity for rewards
- Anchors Proof-of-Care, continuity, and accountability
- Supports lineage tracking, derivation proofs, and zero-knowledge verification

ENS resolution is a required protocol primitive for participation and rewards.

---

## Phase and Epoch References

Genesis participation is evaluated under protocol-defined phases and epochs as
defined in subsequent standards.

Canonical continuity references include:

- Genesis Brains (Paired Assets): five (5) epochs
- Cerebrals (Paired Assets): four (4) epochs
- Brainiacs (Paired Assets): three (3) epochs

Eligibility for Autonomous Intelligent Technology (AIT) activation and Node
capability is evaluated only at the Paired Asset level, as defined in EIP-0005.

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

- Existing on-chain ERC-721 records remain valid
- Ethscription verification artifacts remain immutable
- ENS identity bindings remain intact
- Lineage and provenance guarantees are preserved

---

## Conclusion

EIP-0006 establishes the Genesis truth layer of the Bit Brains protocol,
formalizing independent minting, Paired Asset formation, ENS identity anchoring,
and immutable calldata-based verification rails upon which all Proof-of-Care,
evolution, AIT activation, and Node standards depend.

---

## Copyright

CC0-1.0
