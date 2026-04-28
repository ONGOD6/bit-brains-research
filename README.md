⚠️ Status Note — Bit Brains Protocol Research

Bit Brains represents the original protocol design and research framework for
autonomous intelligent assets, Proof of Care, ENS-based identity, and long-term
protocol evolution.

The active implementation of these concepts has evolved into BITY Nodes,
which focuses on real-time human intelligence, prediction systems, and AI training.

This repository should be viewed as the foundational research and architectural
layer, not the current production system.

---

# Bit Brains — EIP Repository

## Authorship & Attribution

Author: Alex Diaz
Developer: ONGOD

This repository is authored and maintained by Alex Diaz, with protocol design,
development, and implementation led under the developer handle ONGOD.

---

## Overview

This repository contains the canonical Ethereum Improvement Proposal–style documents
(EIPs) for the Bit Brains protocol.

These documents define the economic, governance, identity, and protocol-level frameworks
that guide the design, evolution, and long-term stewardship of Bit Brains.

All proposals in this repository are intended to be read, discussed, reviewed, and
referenced prior to implementation.

---

## Epoch-to–Real World Asset Transformation

Bit Brains undergo a protocol-level transformation following the completion of the first
five epochs.

During the Genesis and Brain phases, assets exist in an observed and measured state:
minted, distributed, staked, and evaluated through Proof of Care. No external value inputs
or off-chain ownership claims are required.

After Epoch Five, Paired Assets (ERC-721 NFTs and their associated Ethscription
artifacts) activate as autonomous intelligent assets. At this stage, the protocol begins
responding to verified real-world participation through Proof of Care and continuity
signals.

---

## Real World Asset Convergence

ENS provides persistent cryptographic identity.
Proof of Care provides real-world participation input.

Together, they allow Bit Brains to function as autonomous, non-custodial assets that
evolve based on verifiable human and machine participation — without surveillance or
behavioral extraction.

This convergence enables long-term coordination between humans, machines, and protocols
while preserving privacy and sovereignty.

Bit Brains do not represent ownership of off-chain property or financial claims.
They are real-world–anchored assets whose behavior, rewards, and evolution are influenced
by verifiable participation and continuity.

---

## Proof of Care (Protocol-Level Overview)

Proof of Care is the canonical participation and qualification mechanism of the Bit Brains
protocol.

It defines how real-world contribution, continuity, and stewardship are recognized
without relying on surveillance, custodial control, or extractive behavioral tracking.

Core Principles:

- Participation is voluntary and opt-in
- Rewards are earned through sustained care, not speculation
- Identity is persistent but privacy-preserving
- Verification is cryptographic, not reputational

---

## Identity Anchor

All participants enter the protocol through a protocol-issued identity anchor.

- Each Brain, Cerebral, Brainiac, or successor asset is associated with an ENS subdomain
- The ENS record acts as a long-lived wallet identifier
- Rewards, participation history, and continuity are referenced through this identity layer

The ENS record does not expose personal data and does not function as a social profile.
It exists solely as a cryptographic coordination primitive.

---

## Zero-Knowledge Verification

Proof of Care verification is performed using zero-knowledge proofs.

These proofs allow the protocol to confirm that:

- Required participation conditions were met
- Required staking conditions were maintained
- No disqualifying actions occurred during the evaluation window

without revealing transactional history, balances, or behavioral details.

Eligibility is verified without observing user activity directly.

---

## Reward Eligibility

Reward issuance is contingent upon:

- Active participation during the relevant epoch
- Maintenance of required staking conditions
- Successful zero-knowledge verification at claim time

If assets are moved, partially withdrawn, or otherwise altered in violation of protocol
rules, rewards for that epoch are not issued.

---

## Scope and Disclosure

This repository defines Proof of Care at the protocol and standards level only.

The following are intentionally excluded and maintained as private intellectual property:

- Scoring models
- Heuristics
- App-level implementations
- Proprietary optimization logic

Formal specifications for Proof of Care mechanics are defined in EIP-0002 and related documents.

---

## EIP Index

Core:

- EIP-0001 — Economic Stewardship Framework
- EIP-0002 — Epoch-Based Proof-of-Care
- EIP-0003 — Epoch-Based Token Distribution
- EIP-0003-A — Proof of Care Expansion & Post-Epoch Three Addendum
- EIP-0004 — Cerebral Evolution and Minting
- EIP-00XX — Ethscriptions Rail: Dual-Asset ZK-Gated Evolution and Node Genesis

Genesis:

- GENESIS.md — Genesis Parameters and Initial Conditions

---

## Repository Scope

What This Repository Contains:

- Standards-track and informational EIPs defining Bit Brains protocol concepts
- Canonical economic, identity, and stewardship frameworks
- Formal specifications for epoch mechanics and Proof of Care
- Historical records of draft, accepted, and superseded proposals

What This Repository Defines:

This repository contains the canonical protocol-level specifications for Bit Brains, including:

- Smart contract architecture and execution logic
- NFT minting, staking, and reward mechanics
- Epoch-based state transitions and lifecycle rules
- Proof of Care and Proof of Stake alignment
- ENS-based identity anchoring and verification
- Website-facing frontend and backend logic required for protocol operation

---

## Current Status

This repository is in its early formation stage.

- EIPs are published as Draft unless otherwise noted
- No proposal should be considered final until explicitly marked as Accepted
- Specifications may evolve through governance and formal review

---

## Contributing

Contributions are welcome in the form of:

- Issues for clarification or discussion
- Pull requests proposing new EIPs or revisions
- Formal reviews focused on correctness, security, and coherence

All contributors are expected to engage constructively and respect the stewardship
principles defined in EIP-0001.

---

## License

Unless otherwise specified, all documents in this repository are released under
CC0 1.0 Universal (Public Domain).
