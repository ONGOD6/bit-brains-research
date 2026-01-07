EIP: 0003-A
Title: Proof of Care Expansion & Post-Epoch Three Addendum
Author: Alex Diaz (ONGOD)
Status: Draft
Type: Standards Track
Category: Core
Created: 2025-12-25
Requires: EIP-0003, Genesis Parameters, EIP-0004
---

## Abstract

This addendum extends EIP-0003 by defining post–Epoch Three specifications for Proof-of-Care expansion, ENS-based identity continuity, privacy-preserving attestations, and staged evolutionary readiness.

This document introduces no independent reward guarantees or distributions. All reward settlement, evolution, and economic outcomes remain governed by the Bit Brains Genesis Parameters and governance-defined phases.

---

## Motivation

Following the completion of Epoch Three, the protocol requires:

- A scalable mechanism to continue measuring Proof of Care
- Persistent identity across epochs and evolutions
- Privacy-preserving participation attestations
- A non-breaking framework for future evolutionary mechanics

Epochs Four and Five are continuity and qualification epochs, not settlement events. This addendum formalizes that distinction.

---

## Specification

### 1. Canonical Genesis Reference

This addendum inherits all Genesis constraints.

Genesis parameters define the initial conditions of the protocol at inception.
They do not represent protocol invariants and may evolve through governance,
future EIPs, or community consensus without violating core protocol principles.

No language in this document overrides Genesis reward timing, supply constraints, or participation rules.

---

### 2. ENS as Canonical Identity Layer

- Ethereum Name Service (ENS) SHALL serve as the canonical identifier for:
  - Proof-of-Care attribution
  - Continuity tracking across epochs
  - Reward eligibility resolution (when rewards are enabled)
- ENS identity persists across:
  - Epoch transitions
  - Asset evolution
  - Protocol phases
- ENS resolution is required for any future reward claims or permissions.

---

### 3. Proof of Care Measurement via Website Interface

- The Bit Brains website functions as a coordination and measurement layer, not a custodian.
- It aggregates participation signals including:
  - Sustained uptime
  - Device- or environment-based attestations
  - Compute or contribution signals (where applicable)
- Data is used for:
  - Continuity verification
  - Eligibility qualification
  - Governance-defined analysis

No reward distribution is triggered by this interface alone.

---

### 4. Privacy via Zero-Knowledge Attestations

- Proof-of-Care signals SHALL be abstracted using zero-knowledge techniques.
- The protocol proves participation consistency without revealing:
  - Raw biometric data
  - Device identifiers
  - Behavioral fingerprints
- ZK attestations function as depth and continuity signals, not direct payout instructions.

---

### 5. Post-Epoch Three Continuity Phase

Epochs Four and Five:

- Continue Proof-of-Care measurement
- Evaluate sustained alignment and participation
- Finalize eligibility for:
  - BIT reward settlement
  - Evolutionary pathways
  - Phase-2 participation

No rewards are distributed at the end of Epoch Three.
All settlement follows Genesis Parameters and governance-defined completion rules.

---

### 6. Evolutionary Readiness (Non-Settlement)

This addendum prepares — but does not execute — evolution:

- Brains → Genesis ERC-721 assets with ENS identity
- Cerebrals → Delegated or amplified participation extensions
- Brainiacs → Advanced representations of long-term continuity

All evolution remains:
- Non-destructive
- Identity-preserving
- Gated by Proof of Care, continuity, and governance

---

### 7. Treasury-Backed Rewards (Deferred)

- Rewards originate from the protocol treasury
- Reward logic is epoch-aware and governance-defined
- No fixed percentages or guarantees exist
- Distribution timing is defined exclusively by:
  - Genesis Parameters
  - Relevant reward EIPs (e.g., EIP-0004)

This addendum introduces no independent reward triggers.

---

## Rationale

This structure ensures:

- Clear separation between measurement and settlement
- No premature reward assumptions
- Privacy-first participation
- Forward-compatible evolution
- Alignment with Genesis and future EIPs

---

## Backwards Compatibility

This addendum introduces no breaking changes.

It activates only after Epoch Three and does not alter:
- Genesis reward timing
- Supply constraints
- Prior Proof-of-Care commitments

---

## Conclusion

EIP-0003-A formalizes post-Epoch-Three continuity without violating Genesis principles.

It measures alignment, preserves identity, and prepares evolution while leaving rewards, settlement, and expansion governed by Genesis Parameters and future EIPs.
