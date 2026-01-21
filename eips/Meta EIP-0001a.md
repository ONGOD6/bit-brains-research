EIP-0001a
Title: Bit Brains Protocol Lifecycle and Evolution
Author: Alex Diaz
Developer: OnGod
Status: Draft
Type: Standards Track
Category: Meta
Created: 2025-12-27
Requires: EIP-0001, EIP-0005, EIP-0006, EIP-0007, Ethscriptions Rail EIP

---

## Abstract

This EIP defines the canonical lifecycle of assets within the Bit Brains protocol.

The lifecycle describes how protocol assets progress from Genesis mint through
dual-asset staking, Proof of Care, Autonomous Intelligent Technology (AIT)
activation, Node derivation, and optional Real World Asset (RWA) attribution.

All lifecycle progression occurs at the level of a **Paired Asset**, composed of a
canonical ERC-721 NFT and its corresponding Ethscription artifact. No asset evolves,
qualifies, or transforms independently.

This EIP is descriptive and structural. It does not define economic guarantees,
reward formulas, or implementation details.

---

## Motivation

The Bit Brains protocol is designed around time, continuity, and care as first-class
primitives.

While individual EIPs define Genesis parameters, Proof of Care mechanics, and AIT
recognition, a unified lifecycle reference is required to clearly describe how
assets evolve across phases and rails.

This EIP provides that reference while enforcing a **dual-asset, non-fragmented
evolution model** that preserves provenance, identity, and long-term alignment.

---

## Lifecycle Principles

- Assets evolve through **continuity**, not mutation
- Time is a security primitive
- Identity persists across all stages
- Evolution is **paired and atomic**
- Autonomy is earned, bounded, and revocable
- No lifecycle stage implies economic entitlement

---

## Canonical Lifecycle Unit

All lifecycle stages described in this EIP apply to a **Paired Asset**, defined as:

- One canonical ERC-721 NFT (Brain, Cerebral, Brainiac, or successor), and
- Its corresponding Ethscription artifact serving as immutable calldata provenance

The ERC-721 NFT and Ethscription artifact SHALL always evolve, qualify, and transform
together. Partial, sequential, or independent evolution is explicitly disallowed.

---

## Canonical 12-Step Protocol Lifecycle

### Step 1 — Genesis Asset Mint (Dual-Asset)
A protocol participant mints a Genesis asset:

- Genesis Brain (ERC-721), or
- Pickle Punk (ERC-721)

At Genesis or via a protocol-defined process, the corresponding Ethscription artifact
is created or linked, forming a Paired Asset.

---

### Step 2 — Immutable Verification Record
For each Genesis ERC-721 asset, an immutable verification record is committed to
Ethereum transaction calldata via Ethscription, establishing timestamped and
verifiable Genesis provenance.

---

### Step 3 — ENS Identity Assignment
Each Paired Asset is assigned a canonical ENS subdomain under:

<index>.bitbrains.eth

ENS serves as the persistent identity anchor across the entire lifecycle, including
staking, Proof of Care, AIT activation, and Node derivation.

---

### Step 4 — Phase One Dual-Asset Staking (Genesis Brains)
Genesis Brains MAY stake and participate in Proof of Care across five (5)
protocol-defined epochs.

A position is Qualifying only when:
- the ERC-721 NFT is staked, AND
- the paired Ethscription artifact is concurrently staked or registered,
as defined by the applicable EIPs.

---

### Step 5 — Zero-Knowledge Continuity Verification
Zero-knowledge proofs attest that the Paired Asset satisfied:
- concurrent staking requirements,
- Proof of Care participation, and
- continuity across the full epoch window,

without revealing private or behavioral data.

---

### Step 6 — Phase One Settlement Eligibility
Upon completion of Epoch Five:
- BIT rewards MAY be distributed, and
- the Paired Asset becomes eligible for AIT activation.

Settlement and rewards are governed exclusively by Genesis Parameters and
governance-defined rules.

---

### Step 7 — Autonomous Intelligent Technology (AIT) Activation
Eligible Paired Assets MAY be recognized as operating in an AIT state.

AIT activation is:
- non-mutative,
- ZK-verified,
- identity-preserving, and
- applied to the Paired Asset as a single unit.

---

### Step 8 — Node Derivation
AIT activation MAY give rise to a Node representing autonomous execution capacity.

Node derivation:
- does not replace or mutate the originating ERC-721 asset,
- requires proof of Paired Asset eligibility, and
- is materialized only at protocol-defined milestones.

---

### Step 9 — Phase Two Continuity (Cerebrals)
Cerebrals participate in Proof of Care across four (4) epochs and become
AIT-eligible immediately upon completion of their continuity window, subject to
dual-asset staking requirements.

---

### Step 10 — Phase Three Continuity (Brainiacs)
Brainiacs participate in Proof of Care across three (3) epochs and become
AIT-eligible immediately upon completion of their continuity window, subject to
dual-asset staking requirements.

---

### Step 11 — Real World Asset (RWA) Attribution (Optional)
AIT-enabled Paired Assets or Nodes MAY have their operational state
cryptographically attributed to Real World Assets (RWAs).

Attribution represents accountability and association only and does not confer
ownership or financial claims.

---

### Step 12 — Ongoing Protocol Participation
Originating Paired Assets MAY continue staking and participating in the Bit Brains
protocol while derived Nodes operate in external execution or business tiers.

Paired Asset identity, continuity, and accountability persist indefinitely.

---

## Scope and Non-Guarantees

- Not all assets are required to reach all lifecycle stages
- Lifecycle progression does not imply economic entitlement
- Governance MAY define additional lifecycle extensions
- No lifecycle stage overrides Genesis Parameters or dual-asset invariants

---

## Conclusion

EIP-0001a establishes the canonical lifecycle of the Bit Brains protocol.

By defining a unified, dual-asset evolutionary path grounded in identity,
continuity, and care, this EIP enables protocol expansion without sacrificing
verifiability, safety, or long-term alignment.
