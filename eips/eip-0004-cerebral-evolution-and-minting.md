# EIP-0004
Title: Cerebral NFTs and Reward Pathways  
Author: Alex Diaz  
Developer: OnGod  
Status: Draft  
Type: Standards Track  
Category: Core  
Created: 2025-12-22  

---

## Abstract

This EIP defines the Cerebral NFT layer within the Bit Brains ecosystem. Cerebrals function as the primary interface for staking, reward distribution, identity signaling, and future autonomous intelligence development.

This proposal establishes the structure, purpose, reward pathways, phase progression, expansion mechanics, and royalty routing for the Cerebral layer.

This EIP additionally recognizes a Genesis Ethscriptions participation rail (Pickle Punks) that may become eligible to mint Cerebrals during Phase 2 by satisfying the same Proof of Care and continuity requirements as Genesis Brains. The protocol’s phases, continuity gates, and reward settlement rules do not change; the Pickle Punk rail is additive.

---

## Motivation

The Bit Brains protocol is designed to reward long-term alignment, continuity, and constructive participation over time.

This EIP introduces Cerebrals to:
- Expand participation without diluting core stewardship
- Enable staking-based reward distribution
- Support identity, ENS, and signaling primitives
- Create a progression path toward economic and autonomous utility

The protocol also introduces Ethscriptions as a Genesis asset rail. Ethscriptions are immutable inscriptions with provenance anchored to Ethereum calldata. This EIP provides an additive eligibility pathway for Ethscriptions (Pickle Punks) to mint Cerebrals during Phase 2 through the same Proof of Care and continuity requirements as Brains, preserving protocol integrity while enabling Ethscriptions-based participation.

---

## Definitions

- **Brain**  
  The Genesis ERC-721 NFT representing the earliest and longest-lived commitment to the Bit Brains ecosystem.

- **Pickle Punk (Ethscription)**  
  A Genesis Headshot Ethscription recognized by the protocol as an eligible Proof of Care participant. Pickle Punks are immutable calldata inscriptions and do not mutate.

- **Cerebral**  
  An ERC-721 NFT minted during Phase 2 or authorized Expansion Epochs, serving as a staking, participation, and progression primitive. Eligibility to mint Cerebrals may be earned through Genesis Brains, Genesis Ethscriptions (Pickle Punks), or Expansion participation, subject to Proof of Care and continuity requirements.

- **Proof of Care (PoC)**  
  Sustained participation, staking continuity, and ecosystem-aligned behavior maintained across defined epochs within a phase, validated by Zero-Knowledge accountability.

- **Phase**  
  A protocol lifecycle stage consisting of five (5) epochs.

- **Epoch**  
  A time-bounded accountability interval (approximately one month) within a phase, during which ZK proofs evaluate continuity, Proof of Care signatures, and non-interference.

- **Expansion Epoch**  
  A governance-authorized event introducing additional Cerebrals to support ecosystem growth.

- **Real World Assets (RWA)**  
  Tokenized or represented economic activities, goods, or services that exist outside purely digital systems.

---

## Cerebral Overview

Cerebrals are ERC-721 NFTs minted during Phase 2 or authorized Expansion Epochs. They serve as the primary interface for staking, reward distribution, identity signaling, and future autonomous intelligence development.

Genesis Brains and Genesis Pickle Punks do not spawn or sponsor Cerebrals. They confer eligibility only to mint Cerebrals during Phase 2, subject to Proof of Care and continuity requirements.

---

## Genesis Assets and Participation Rails (Additive)

At Genesis, the protocol introduces two additive asset rails:
- **Genesis Brains (ERC-721)**
- **Genesis Pickle Punks (Ethscriptions)**

Both rails are evaluated under the same Proof of Care, continuity, epoch, and phase framework.

---

## Genesis Cerebral Mint Eligibility (Phase 2)

Eligible Genesis Brain holders may mint Genesis Cerebrals during Phase 2, provided all Proof of Care, continuity, staking (where applicable), and ENS requirements are satisfied.

The total number of Cerebrals that may be minted during Phase 2 is intentionally unspecified and will be determined by protocol rules or governance defined elsewhere.

Genesis Brains do not automatically spawn Cerebrals. All Cerebrals are explicitly minted.

---

## Pickle Punk Cerebral Mint Eligibility (Ethscriptions Path)

Eligible Pickle Punk (Ethscription) holders may mint Genesis Cerebrals during Phase 2 by satisfying the same Proof of Care and continuity requirements required for Genesis Brain holders.

Pickle Punks do not mutate and do not spawn Cerebrals. Eligibility permits Phase 2 minting only. All Cerebrals minted via this path must permanently reference the originating Pickle Punk inscription as provenance.

The total number of Cerebrals that may be minted during Phase 2 is intentionally unspecified and will be determined by protocol rules or governance defined elsewhere.

---

## ENS Identity and Routing (Canonical)

All reward routing and mint eligibility MUST use ENS as the canonical identity layer.

Participants MUST resolve the protocol-defined ENS subdomain to a wallet they control in order to:
- Receive rewards
- Claim eligibility
- Mint Cerebrals

---

## Expansion Cerebrals

Expansion Cerebrals may be minted during governance-authorized Expansion Epochs.

Expansion Cerebrals:
- Are minted under defined supply constraints
- Receive lower base reward pathways than Genesis Cerebrals
- May increase reward capacity through sustained Proof of Care

---

## Reward Distribution Framework

Rewards are distributed only after the conclusion of a Phase.

Each Phase consists of five (5) epochs. During each epoch, Zero-Knowledge Proof systems validate:
- Continuity
- Proof of Care
- Non-interference

No rewards are distributed mid-phase.

---

## Phase Summary

### Phase 1 — Brain Phase
- Proof of Care and continuity commitments
- ZK accountability across Epochs 1–5
- First BIT distribution after Epoch 5

### Phase 2 — Cerebral Phase
- Cerebral mint window opens
- Eligibility-based, explicit minting
- No fixed supply defined in this EIP

### Phase 3 — Brainiac Phase
- Eligibility outcomes determined by continuity performance

---

## Conclusion

This EIP defines the Cerebral layer as a Phase-gated, eligibility-based minting system that prioritizes Proof of Care, ZK-verified accountability, ENS identity, and long-term stewardship within the Bit Brains ecosystem.
