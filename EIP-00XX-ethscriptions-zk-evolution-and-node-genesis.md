00XX
Title: Ethscriptions Rail — Dual-Asset ZK-Gated Evolution and Node Genesis
Author: Alex Diaz
Developer: OnGod
Status: Draft
Type: Standards Track
Category: Core
Created: 2026-01-08
Requires: EIP-0001, EIP-0004, ZK Proof Verification Layer
---

## Abstract

This EIP defines the Ethscriptions participation rail within the Bit Brains protocol and specifies a **dual-asset, ZK-gated evolutionary model** in which protocol state transitions are proven via zero-knowledge proofs and materialized on-chain only at defined milestone events.

The Ethscriptions Rail operates as a **paired asset system**, where a canonical ERC-721 NFT and its corresponding Ethscription artifact form a single evolutionary unit. Participation, staking, reward eligibility, Autonomous Intelligent Technology (AIT) activation, and Node genesis require **concurrent staking and verification of both assets**.

All evolution occurs atomically at the paired-asset level. No asset may evolve, qualify, or transform independently.

This proposal is descriptive and structural. It does not define economic guarantees, yield formulas, or market expectations.

---

## Motivation

The Bit Brains protocol is designed around continuity, verifiable stewardship, and non-fragmented evolution.

Allowing ERC-721 assets or Ethscription artifacts to progress independently would weaken protocol guarantees, introduce ambiguity in lineage, and undermine long-term intelligence attribution.

Accordingly, the protocol enforces **dual-asset evolution**, where calldata provenance (Ethscriptions) and programmable ownership (ERC-721 NFTs) advance together under a unified eligibility model.

This approach preserves:
- immutable provenance,
- non-custodial ownership,
- cryptographic verifiability, and
- atomic Node genesis.

---

## Definitions

- **Ethscription Asset:** A calldata-provenance artifact committed to Ethereum via the Ethscriptions mechanism.
- **ERC-721 Asset:** A canonical Bit Brains NFT (Brain, Cerebral, Brainiac, or successor).
- **Paired Asset:** The inseparable evolutionary unit composed of an ERC-721 asset and its corresponding Ethscription artifact.
- **Epoch:** A Bit Brains–defined continuity window used to evaluate long-term alignment.
- **Continuity:** Time-based participation requirements enforced across an epoch.
- **Proof of Care (PoC):** Verifiable participation signals required for progression.
- **AIT State:** Autonomous Intelligent Technology activation state recognized by the Bit Brains protocol.
- **Node State:** A recognized execution and identity state derived from a qualified Paired Asset.
- **ZK Proof Protocol:** The Bit Brains verification layer used to prove eligibility, continuity, and Proof of Care without revealing sensitive information.

---

## Dual-Asset Evolution Invariant (Canonical)

All Bit Brains protocol evolution, including Proof of Care evaluation, AIT activation, and Node genesis, SHALL be governed by a **Dual-Asset Evolution Invariant**.

A position is considered **Qualifying** only when BOTH of the following assets are concurrently staked and in good standing:

1. The canonical **ERC-721 NFT**, and  
2. Its **paired Ethscription artifact** serving as immutable calldata provenance.

The ERC-721 asset and Ethscription artifact together form a single **Paired Asset**.

No protocol-defined evolution, reward eligibility, continuity accumulation, AIT activation, or Node recognition SHALL occur unless the Paired Asset remains concurrently staked for the full required continuity window.

If either asset is unstaked, invalid, or noncompliant, the position becomes **Non-Qualifying**.

---

## Activation Constraint (Canonical)

The Ethscriptions Rail is defined at Genesis but remains **Non-Qualifying** until completion of the following canonical NFT phases:

1. **Brain Phase**
2. **Cerebral Phase**
3. **Brainiac Phase**

Ethscriptions MAY be created, held, and paired at any time.

However, an Ethscription SHALL NOT independently qualify for:
- staking,
- Proof of Care evaluation,
- continuity tracking,
- reward eligibility,
- AIT activation, or
- Node recognition.

Qualification is achieved **only** when the paired ERC-721 asset reaches the applicable phase AND both assets are concurrently staked under the Dual-Asset Evolution Invariant.

---

## Canonical Model: ZK-Gated Dual-Asset Evolution

All evolutionary state transitions within the Bit Brains protocol are evaluated at the level of the **Paired Asset** and validated via zero-knowledge proofs.

ZK proofs attest that the ERC-721 asset and its paired Ethscription artifact have:
- remained concurrently staked,
- satisfied continuity requirements for the full epoch, and
- met Proof of Care conditions.

No evolution, AIT activation, or Node recognition SHALL be materialized on-chain unless a ZK proof verifies the complete Paired Asset state history.

---

## Evolutionary States (Post-Activation Only)

All states described below apply to the **Paired Asset as a single evolutionary unit** and not to the ERC-721 asset or Ethscription independently.

### State 0 — Dormant (ZK Verifiable)
The Paired Asset exists but is not registered within the Bit Brains protocol.

### State 1 — Registered (ZK Verifiable)
The Paired Asset is registered for an epoch under protocol rules. Registration status is proven via ZK proof.

### State 2 — Proof of Care Proven (ZK Verifiable)
Continuity and Proof of Care requirements for the epoch are satisfied and proven via ZK proof.

### State 3 — AIT Activated (Paired Asset, ZK Verifiable)
The Paired Asset achieves Autonomous Intelligent Technology activation status, proven via ZK proof.

### State 4 — Node Recognized (Paired Asset, ZK Verifiable + Mint Event)
A Node is recognized only when a valid ZK proof attests to the correctness and truthfulness of the full required Paired Asset state history and eligibility constraints.

Upon successful verification:

1. A **Node ERC-721** is minted as the canonical verification of Node status, and  
2. A **new Ethscription** is issued as the immutable calldata record of Node genesis.

---

## Canonical Minting Rule

ERC-721 mints and Ethscription issuance occur only at the following milestone levels:

1. **Brain** — ERC-721 mint + Ethscription  
2. **Cerebral** — ERC-721 mint + Ethscription  
3. **Brainiac** — ERC-721 mint + Ethscription  
4. **Node Genesis** — ERC-721 mint + Ethscription  

All mint events represent the **simultaneous evolution of the ERC-721 asset and its paired Ethscription artifact** and SHALL NOT be executed independently.

All other evolutionary progress is proven exclusively via ZK proofs and does not result in on-chain minting.

---

## Uniqueness and Anti-Replay Constraints

Node minting MUST enforce protocol-defined uniqueness constraints.

A valid ZK proof MUST attest that:
- the Paired Asset lineage has not previously produced a Node under the applicable rules,
- the proof has not been replayed, and
- no conflicting Node genesis exists.

---

## Relationship to the NFT Rail

The Ethscriptions Rail is not independent of the NFT Rail.

Both rails converge on the same Bit Brains invariants:
- epoch-based continuity,
- Proof of Care gating,
- dual-asset staking,
- ZK-verified state transitions, and
- immutable Node genesis.

The ERC-721 asset and Ethscription artifact SHALL always evolve as a **single Paired Asset**.

---

## Status

Draft — Reserved Protocol
