EIP: 0001a
Title: Bit Brains Protocol Lifecycle and Evolution
Author: Alex Diaz
Developer: OnGod
Status: Draft
Type: Standards Track
Category: Meta
Created: 2025-12-27
Requires: EIP-0001, EIP-0005, EIP-0006, EIP-0007

---

## Abstract

This EIP defines the canonical lifecycle of assets within the Bit Brains protocol.

The lifecycle describes how protocol assets progress from Genesis mint through
staking, Proof of Care, Autonomous Intelligent Technology (AIT) activation,
node derivation, and optional Real World Asset (RWA) attribution.

This EIP is descriptive and structural. It does not define economic guarantees,
reward formulas, or implementation details.

---

## Motivation

The Bit Brains protocol is designed around time, continuity, and care as first-class
primitives.

While individual EIPs define Genesis parameters, Proof of Care, and AIT mechanics,
a unified lifecycle reference is required to clearly describe how assets evolve
through the protocol.

This EIP provides that reference.

---

## Lifecycle Principles

- Assets evolve through **continuity**, not mutation
- Time is a security primitive
- Identity persists across all stages
- Autonomy is earned, bounded, and revocable
- No lifecycle stage implies economic entitlement

---

## Canonical 12-Step Protocol Lifecycle

### Step 1 — Genesis Asset Mint
A protocol participant independently mints a Genesis asset:
- Genesis Brain (ERC-721), or
- Pickle Punk (ERC-721)

Each asset is minted through its own supply and mint flow.

---

### Step 2 — Immutable Verification Record
For each Genesis asset minted, an immutable verification record is committed to
Ethereum transaction calldata, establishing a timestamped and verifiable
Genesis truth.

---

### Step 3 — ENS Identity Assignment
Each minted asset is assigned a canonical ENS subdomain under:

<index>.bitbrains.eth

ENS serves as the persistent identity anchor for the asset lifecycle.

---

### Step 4 — Phase One Staking (Genesis Brains)
Genesis Brains may stake and participate in Proof of Care across five (5)
protocol-defined epochs.

---

### Step 5 — Zero-Knowledge Continuity Verification
Zero-knowledge proofs attest that staking, Proof of Care, and continuity
requirements were satisfied without revealing private data.

---

### Step 6 — Phase One Settlement
Upon completion of Epoch Five:
- BIT rewards MAY be distributed
- Genesis Brains become eligible for AIT activation

---

### Step 7 — Autonomous Intelligent Technology (AIT) Activation
Eligible assets may be recognized as operating in an AIT state.

AIT activation is non-mutative and preserves the originating asset as the
canonical provenance anchor.

---

### Step 8 — Node Derivation
AIT activation MAY give rise to a Node representing autonomous execution capacity.

Node derivation does not replace or mutate the originating asset.

---

### Step 9 — Phase Two Continuity (Cerebrals)
Cerebrals participate in Proof of Care across four (4) epochs and become
AIT-eligible immediately upon completion of their continuity window.

---

### Step 10 — Phase Three Continuity (Brainiacs)
Brainiacs participate in Proof of Care across three (3) epochs and become
AIT-eligible immediately upon completion of their continuity window.

---

### Step 11 — Real World Asset (RWA) Attribution (Optional)
AIT-enabled assets or Nodes MAY have their operational state cryptographically
attributed to Real World Assets (RWAs).

Attribution represents accountability and association only.

---

### Step 12 — Ongoing Protocol Participation
Originating assets may continue staking and participating in the Bit Brains
protocol while derived Nodes operate in external execution or business tiers.

---

## Scope and Non-Guarantees

- Not all assets are required to reach all lifecycle stages
- Lifecycle progression does not imply economic entitlement
- Governance may define additional lifecycle extensions

---

## Conclusion

EIP-0001a establishes the canonical lifecycle of the Bit Brains protocol.

By defining a shared evolutionary path grounded in identity, continuity, and care,
this EIP enables protocol growth without sacrificing safety, accountability,
or long-term alignment.
