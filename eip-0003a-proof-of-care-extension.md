: 0003-A
Title: Proof of Care Expansion & Post-Epoch Three Addendum
Author: Alex Diaz (ONGOD)
Status: Draft
Type: Standards Track
Category: Core
Created: 2025-12-25
Requires: EIP-0003, Genesis Parameters, EIP-0004, Ethscriptions Rail EIP
---

## Abstract

This addendum extends EIP-0003 by defining post–Epoch Three specifications for Proof-of-Care expansion, ENS-based identity continuity, privacy-preserving attestations, and staged evolutionary readiness.

This document introduces no independent reward guarantees, settlement rules, or economic distributions. All reward settlement, evolution, and economic outcomes remain governed by the Bit Brains Genesis Parameters, the Ethscriptions Rail EIP, and governance-defined phases.

---

## Motivation

Following the completion of Epoch Three, the protocol requires:

- A scalable mechanism to continue measuring Proof of Care
- Persistent identity across epochs and evolutionary states
- Privacy-preserving participation attestations
- A non-breaking framework that prepares future evolution without executing it

Epochs Four and Five are continuity and qualification epochs, not settlement or evolution events. This addendum formalizes that distinction.

---

## Specification

### 1. Canonical Genesis Reference

This addendum inherits all Genesis constraints.

Genesis Parameters define the initial conditions of the protocol at inception.
They do not represent protocol invariants and may evolve through governance,
future EIPs, or community consensus without violating core protocol principles.

No language in this document overrides Genesis reward timing, supply constraints, participation rules, or evolutionary requirements.

---

### 1A. Dual-Asset Evolution Alignment

This addendum operates within the **Dual-Asset Evolution Invariant** defined by the Ethscriptions Rail EIP.

All Proof-of-Care measurement, continuity evaluation, and evolutionary readiness described herein apply to the **Paired Asset**, defined as the canonical ERC-721 NFT and its associated Ethscription artifact.

Nothing in this addendum SHALL be interpreted to permit:
- independent evolution of ERC-721 assets,
- independent qualification of Ethscription artifacts, or
- sequential or partial transformation of paired assets.

Evolutionary eligibility assessed during Epochs Four and Five is satisfied only when dual-asset staking conditions are met, as defined by the applicable EIPs.

---

### 2. ENS as Canonical Identity Layer

Ethereum Name Service (ENS) SHALL serve as the canonical identity layer for:

- Proof-of-Care attribution
- Continuity tracking across epochs
- Reward eligibility resolution (when rewards are enabled)
- Governance-defined permissions and coordination

ENS identity persists across:
- Epoch transitions
- Asset evolution
- Protocol phases

ENS resolution is required for any future reward claims, permissions, or protocol-recognized actions.

---

### 3. Proof of Care Measurement via Website Interface

The Bit Brains website functions as a coordination and measurement layer, not a custodian.

It aggregates participation signals including:
- Sustained uptime
- Device- or environment-based attestations
- Contribution or compute signals (where applicable)

These signals are used exclusively for:
- Continuity verification
- Eligibility qualification
- Governance-defined analysis

No reward distribution, settlement, or evolution is triggered by this interface alone.

---

### 4. Privacy via Zero-Knowledge Attestations

Proof-of-Care signals SHALL be abstracted using zero-knowledge techniques.

The protocol proves participation consistency without revealing:
- Raw biometric data
- Device identifiers
- Behavioral fingerprints
- Personally identifying signals

Zero-knowledge attestations function as continuity and alignment proofs, not direct payout or execution instructions.

---

### 5. Post-Epoch Three Continuity Phase

Epochs Four and Five serve as extended continuity and qualification epochs.

During these epochs:
- Proof-of-Care measurement continues
- Long-term alignment and participation are evaluated
- Eligibility is finalized for:
  - BIT reward settlement
  - Evolutionary pathways
  - Phase 2 participation

No rewards are distributed at the conclusion of Epoch Three.
All settlement follows Genesis Parameters and governance-defined completion rules.

---

### 6. Evolutionary Readiness (Non-Settlement)

This addendum prepares — but does not execute — evolution.

Evolutionary states referenced include:
- Brains → Genesis ERC-721 assets with ENS identity
- Cerebrals → Amplified or delegated participation extensions
- Brainiacs → Advanced representations of sustained continuity

All evolution remains:
- Non-destructive
- Identity-preserving
- Gated by Proof of Care, continuity, dual-asset staking, and governance

No minting, transformation, or state transition occurs under this addendum.

---

### 7. Treasury-Backed Rewards (Deferred)

Rewards originate from the protocol treasury.

Reward logic is:
- Epoch-aware
- Governance-defined
- Subject to future EIPs

No fixed percentages, guarantees, or settlement triggers are introduced in this document.

Distribution timing and conditions are defined exclusively by:
- Genesis Parameters
- Applicable reward EIPs (e.g., EIP-0004)
- Governance decisions

---

## Rationale

This addendum ensures:

- Clear separation between measurement and settlement
- No premature reward assumptions
- Privacy-first participation
- Forward-compatible evolution
- Alignment with Genesis Parameters and the Dual-Asset Evolution model

---

## Backwards Compatibility

This addendum introduces no breaking changes.

It activates only after Epoch Three and does not alter:
- Genesis reward timing
- Supply constraints
- Prior Proof-of-Care commitments
- Existing staking behavior

---

## Conclusion

EIP-0003-A formalizes post–Epoch Three continuity without violating Genesis principles or dual-asset evolution invariants.

It measures alignment, preserves identity, and prepares future evolution while leaving rewards, settlement, and transformation governed by Genesis Parameters and subsequent EIPs.
