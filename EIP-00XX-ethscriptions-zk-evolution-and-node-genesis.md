EIP: 00XX
Title: Ethscriptions Rail — ZK-Gated Evolution and Node Genesis
Author: Alex Diaz
Developer: OnGod
Status: Draft
Type: Standards Track
Category: Core
Created: 2026-01-08
Requires: EIP-0001, EIP-0004, ZK Proof Verification Layer
---

## Abstract

This EIP defines the Ethscriptions participation rail within the Bit Brains protocol and specifies a ZK-gated evolutionary model in which protocol state transitions are proven via zero-knowledge proofs and only materialized on-chain at defined milestone events.

Ethscriptions serve as immutable calldata records and are issued exclusively when ERC-721 milestone mints occur. All intermediate evolutionary states are validated via ZK proofs without requiring additional mints.

This proposal is descriptive and structural. It does not define economic guarantees, yield formulas, or market expectations.

---

## Motivation

The Bit Brains protocol prioritizes continuity, Proof of Care, and long-term alignment over frequent on-chain mutations.

Issuing on-chain assets for every state transition introduces unnecessary complexity, gas costs, and mutable upgrade vectors. This EIP establishes a model where:

- ZK proofs act as the canonical truth layer for evolution,
- ERC-721 mints occur only at meaningful milestone states, and
- Ethscriptions provide immutable, auditable protocol memory only when those milestones are reached.

This design preserves trust minimization while enabling rich, verifiable progression logic.

---

## Definitions

- **Ethscription Asset:** A calldata-provenance asset committed to Ethereum via the Ethscriptions mechanism.
- **Epoch:** A Bit Brains–defined continuity window used to evaluate long-term alignment.
- **Continuity:** Time-based participation requirement enforced across an epoch.
- **Proof of Care (PoC):** Verifiable participation signals required for progression.
- **AIT State:** Autonomous Intelligent Technology activation state recognized by the Bit Brains protocol.
- **Node State:** A recognized execution and identity state derived from a qualified asset.
- **ZK Proof Protocol:** The Bit Brains verification layer used to prove eligibility, continuity, and PoC without revealing sensitive information.

---

## Canonical Model: ZK-Gated Evolution

All evolutionary state transitions within the Ethscriptions Rail are validated via ZK proofs.

No ERC-721 mint and no Ethscription issuance occurs unless a milestone state is reached and verified.

ZK proofs are the authoritative truth mechanism for all non-minted states.

---

## Evolutionary States

Ethscriptions Rail assets progress through the following states:

### State 0 — Dormant (ZK Verifiable)
The asset exists but is not registered in the Bit Brains protocol.

### State 1 — Registered (ZK Verifiable)
The asset is registered or staked for an epoch under protocol rules. Registration status is proven via ZK proof.

### State 2 — Proof of Care Proven (ZK Verifiable)
Continuity and Proof of Care requirements for the epoch are satisfied and proven via ZK proof.

### State 3 — AIT Activated (ZK Verifiable)
The asset achieves Autonomous Intelligent Technology activation status, proven via ZK proof.

### State 4 — Node Recognized (ZK Verifiable + Mint Event)
A Node is recognized only when a valid ZK proof attests to the correctness and truthfulness of the full required state history and eligibility constraints.

Upon successful verification:

1. A **Node ERC-721** is minted, and  
2. A **new Ethscription** is issued as the immutable calldata record of Node genesis.

---

## Canonical Minting Rule

ERC-721 mints and Ethscription issuance occur only at the following milestone levels:

1. **Brain** — ERC-721 mint + Ethscription  
2. **Cerebral** — ERC-721 mint + Ethscription  
3. **Brainiac** — ERC-721 mint + Ethscription  
4. **Node Genesis** — ERC-721 mint + Ethscription  

All other evolutionary progress is proven exclusively via ZK proofs and does not result in on-chain minting.

---

## Canonical Ethscription Rule

Ethscriptions are issued only when an ERC-721 milestone mint occurs.

> No ERC-721 mint → no new Ethscription.

Ethscriptions encode immutable commitments including lineage references, verified state commitments, epoch completion attestations, and Node genesis proofs.

---

## Uniqueness and Anti-Replay Constraints

Node minting MUST enforce protocol-defined uniqueness constraints.

A valid ZK proof MUST attest that:
- the asset lineage has not previously produced a Node under the applicable rules,
- the proof has not been replayed,
- and no conflicting Node genesis exists.

Uniqueness constraints may be enforced through ZK proofs, on-chain checks, or a combination of both.

---

## Relationship to the NFT Rail

The Ethscriptions Rail does not replace the NFT rail.

Both rails converge on the same Bit Brains invariants:
- epoch-based continuity,
- Proof of Care gating,
- ZK-verified state transitions,
- and immutable milestone recording via Ethscriptions.

---

## Security Considerations

This model minimizes attack surface by:
- reducing unnecessary on-chain state changes,
- relying on cryptographic proofs for eligibility,
- and limiting mint authority to verifiable milestone events.

---

## Status

Draft — Reserved Protocol  
