---
eip: Meta-EIP-0001b
title: Genesis Hybrid Mint Architecture
subtitle: Pickle Punks × Bit Brains — Three-Step Identity, Ownership, and Permanence Model
author: Bit Brains Protocol
status: Draft
type: Meta
category: Architecture
created: 2026-02-02
requires: Meta-EIP-0001
---
# Meta EIP-0001b: Genesis Hybrid Mint Architecture  
## Pickle Punks × Bit Brains — Three-Step Identity, Ownership, and Permanence Model

## Abstract

This Meta EIP defines the Genesis Hybrid Mint Architecture of the Bit Brains protocol.
It formalizes a mandatory three-step minting process that separates ownership,
permanence, and identity into distinct layers, then binds them together at Genesis.

This specification introduces:
- A fixed Genesis identity ceiling of 10,000 numeric ENS identities
- A hybrid art model where 5,000 Genesis identities reference Pickle Punks artwork
- Mandatory pairing of ERC-721 NFTs with Ethscriptions
- ENS numeric subdomains under `bitbrains.eth` as the canonical identity layer

This EIP introduces no guarantees of rewards, yield, or future benefits.

---

## Motivation

Traditional NFT systems commonly collapse ownership, metadata, and identity into
a single mutable artifact. Over time, this creates structural fragility through:

- Metadata mutability
- Reliance on external storage
- Wallet rotation breaking continuity
- Ambiguous long-term identity

The Bit Brains protocol addresses these weaknesses by explicitly separating concerns.

The Genesis Hybrid Mint Architecture ensures:
- Ownership remains usable
- Permanence remains immutable
- Identity remains persistent and non-inflationary

No single layer is sufficient on its own.

---

## Genesis Identity Scope

The Bit Brains protocol defines a fixed Genesis identity ceiling:

- Exactly 10,000 Genesis identities
- The ceiling is absolute and non-expandable
- Identity-layer inflation is explicitly prohibited

Within this Genesis scope:
- 5,000 identities reference Pickle Punks artwork
- Pickle Punks function as hybrid art NFTs recognized by the Genesis protocol
- Remaining identities reference other Genesis-defined assets

This model allows artistic expression without fragmenting or inflating the canonical
identity layer.

---

## Specification: Three-Step Genesis Hybrid Mint

### Step One — ERC-721 NFT Mint (Ownership Layer)

The first step of the Genesis Mint is the creation of an ERC-721 NFT.

This layer establishes:
- On-chain ownership
- Wallet-native visibility
- Transferability under ERC-721 standards

The ERC-721 token is the ownership artifact of the Genesis asset.
This layer does not attempt to guarantee permanence or define long-term identity.

---

### Step Two — Ethscriptions Mint (Permanence Layer)

The second step is the minting of a paired Ethscription using calldata inscription
techniques.

The Ethscription:
- Contains the same visual payload as the ERC-721
- Is permanently embedded in Ethereum transaction history
- Cannot be altered, replaced, or rehosted
- Does not rely on external metadata or storage systems

The Ethscription exists solely to preserve immutable provenance.

Together, the ERC-721 and Ethscription form a Paired Genesis Asset:
- One layer optimized for usability
- One layer optimized for permanence

---

### Step Three — ENS Numeric Subdomain (Identity Layer)

The third and most critical step is the assignment of a numeric ENS subdomain under:

`<number>.bitbrains.eth`

Constraints:
- Numeric identifiers range strictly from 1 to 10,000
- Each identifier maps one-to-one with a Genesis identity
- Identifiers are finite, deterministic, and non-reusable

ENS is defined as the canonical identity layer of the Bit Brains protocol.

Wallet addresses are treated as replaceable endpoints.
ENS identity persists independently of wallet rotation or contract upgrades.

Genesis participants are expected to resolve their ENS subdomain to a wallet they control.

---

## Pickle Punks as Hybrid Art NFTs

Pickle Punks are defined as hybrid art NFTs within the Genesis framework.

They:
- Are artistically expressive ERC-721 assets
- Are paired with Ethscriptions for permanence
- Are referenced by Genesis Bit Brains identities
- Participate in the same ENS-anchored identity model

Art remains expressive.
Identity remains deterministic.

---

## Proof of Care (Non-Promissory)

The Bit Brains protocol makes no guarantees regarding rewards, yield, or future benefits.

The architecture allows continuity to be observed over time through:
- Sustained ENS resolution
- Preservation of paired Genesis assets
- Responsible protocol participation

Any future recognition is retrospective, conditional, and non-obligatory.

---

## Security Considerations

- ENS identity persistence mitigates wallet loss and rotation risks
- Ethscriptions mitigate metadata mutability and storage failure risks
- Fixed identity ceiling prevents identity-layer inflation

---

## Non-Guarantee Statement

Participation in the Genesis Hybrid Mint conveys structure, not entitlement.

This EIP does not guarantee:
- Rewards
- Yield
- Value appreciation
- Future protocol participation

---

## Conclusion

The Genesis Hybrid Mint Architecture establishes a durable protocol foundation by
separating ownership, permanence, and identity into explicit layers.

Genesis participants are not purchasers of promises.
They are early stewards of protocol structure.

---

End of Meta EIP-0001b
