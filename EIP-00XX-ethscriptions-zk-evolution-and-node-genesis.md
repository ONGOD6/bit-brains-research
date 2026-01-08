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

The Ethscriptions Rail is an additive and experimental pathway that allows calldata-provenance assets to participate in Proof of Care and continuity with the goal of evolving into Autonomous Intelligent Technology (AIT) and ultimately a Node identity verified by an ERC-721 mint.

This proposal is descriptive and structural. It does not define economic guarantees, yield formulas, or market expectations.

---

## Motivation

The Bit Brains protocol is designed to reward long-term alignment, continuity, and care rather than short-term activity or frequent on-chain mutation.

In addition to the canonical NFT rail (Brains, Cerebrals, and Brainiacs), the protocol intentionally allows Ethscriptions to participate as an experimental evolution rail. This design serves two purposes:

1. To explore whether calldata-provenance assets can evolve into Autonomous Intelligent Technology through verifiable care and continuity, and
2. To provide an additional incentive layer for participants who originally entered the protocol through Brains, Cerebrals, or Brainiacs to continue progressing toward full Node actualization.

The Ethscriptions Rail does not dilute or replace the NFT rail. Instead, it adds an additional pathway that converges at the same Node recognition point, reinforcing long-term participation and protocol stewardship.

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

ZK proofs act as the canonical truth layer for progression and are used to demonstrate that continuity and Proof of Care requirements have been satisfied for the full duration of an epoch.

No ERC-721 mint and no Ethscription issuance occurs unless a milestone state is reached and successfully verified.

---

## Evolutionary States

Ethscriptions Rail assets progress through the following states:

### State 0 — Dormant (ZK Verifiable)
The asset exists but is not registered in the Bit Brains protocol.

### State 1 — Registered (ZK Verifiable)
The asset is registered for an epoch under Bit Brains protocol rules. Registration status is proven via ZK proof.

### State 2 — Proof of Care Proven (ZK Verifiable)
Continuity and Proof of Care requirements for the epoch are satisfied and proven via ZK proof.

### State 3 — AIT Activated (ZK Verifiable)
The asset achieves Autonomous Intelligent Technology activation status, proven via ZK proof.

### State 4 — Node Recognized (ZK Verifiable + Mint Event)
A Node is recognized only when a valid ZK proof attests to the correctness and truthfulness of the full required state history and eligibility constraints.

Upon successful verification:

1. A **Node ERC-721** is minted as the canonical asset verification of Node status, and  
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
- the proof has not been replayed, and
- no conflicting Node genesis exists.

Uniqueness constraints may be enforced through ZK proofs, on-chain checks, or a combination of both.

---

## Relationship to the NFT Rail

The Ethscriptions Rail is explicitly additive.

Brains, Cerebrals, and Brainiacs remain the primary entry assets to the Bit Brains protocol. The Ethscriptions Rail provides an additional experimental incentive layer that encourages continued participation, long-term alignment, and progression toward Node status.

Both rails converge on the same Bit Brains invariants:
- epoch-based continuity,
- Proof of Care gating,
- ZK-verified state transitions, and
- immutable Node genesis via ERC-721 mint and Ethscription record.

---

## Security Considerations

This model minimizes attack surface by:
- reducing unnecessary on-chain state changes,
- relying on cryptographic proofs for eligibility,
- limiting mint authority to verified milestone events, and
- preserving immutable historical records for auditability.

---

## Status

Draft — Reserved Protocol
