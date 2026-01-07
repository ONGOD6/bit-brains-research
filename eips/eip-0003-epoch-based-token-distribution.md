EIP: 0003
Title: Token Supply Cap and Emission Constraints Standard
Author: Bit Brains Protocol
Developer: OnGod
Discussions-To: TBD
Status: Draft
Type: Standards Track
Category: Economic
Created: 2025-12-28
Requires: EIP-0001, Genesis Parameters
---

## Abstract

EIP-0003 defines the fixed maximum token supply and the constraints under which
any future emissions MAY occur within the Bit Brains protocol.

This EIP establishes a hard-capped total supply, prohibits inflationary minting,
and constrains all token distribution to governance-defined phases and eligibility
rules.

This specification does **not** guarantee emission schedules, reward amounts, or
distribution timing. All emissions, if any, remain subject to Proof-of-Care,
continuity, and governance-defined settlement conditions as defined in Genesis
Parameters and subsequent EIPs.

---

## Motivation

Token systems frequently fail due to inflationary drift, unclear issuance authority,
and premature extraction.

This EIP enforces a strict upper bound on supply while intentionally separating
**participation eligibility** from **emission guarantees**, ensuring that no asset
class, participant count, or Genesis condition can implicitly expand supply or force
distribution.

---

## Canonical Genesis Reference

This EIP inherits and defers to the Bit Brains Genesis Parameters.

Genesis parameters define the initial conditions of the protocol at inception.
They do not represent protocol invariants and may evolve through governance,
future EIPs, or community consensus without violating core protocol principles.

Nothing in this EIP guarantees rewards, fixed schedules, or emission certainty.

---

## Total Supply (Invariant)

- **Maximum Supply:** **200,000,000 tokens**
- **Inflation:** Prohibited
- **Supply Expansion:** Not permitted under any circumstance

This maximum supply is absolute and SHALL NOT be exceeded.

---

## Emission Constraints (Non-Guaranteed)

- Token emissions, if any, MUST occur within governance-defined phases
- Emissions MAY be constrained by epoch completion, Proof-of-Care, and continuity
- Emissions MAY be delayed, reduced, or halted entirely
- No emissions are permitted beyond governance-authorized phases

This EIP defines **constraints**, not schedules.

---

## Genesis Participants and Eligibility (Non-Expansive)

At Genesis, the protocol recognizes multiple participation primitives, including:

- **Genesis Brains** — ERC-721 NFTs with associated Ethscription provenance
- **Pickle Punks** — ERC-721 NFTs with associated Ethscription provenance

Genesis Participants:
- MAY participate in Proof-of-Care and continuity mechanisms
- DO NOT expand token supply
- DO NOT create per-asset emission entitlements
- DO NOT imply proportional reward guarantees

Eligibility for any token distribution is determined exclusively by:
- Proof-of-Care
- Continuity
- ENS-resolved identity
- Governance-defined settlement rules

---

## Treasury-Held Supply Segmentation (Accounting Only)

For accounting and governance clarity, the total supply MAY be segmented into
treasury-held pools. These pools do not imply guaranteed release.

| Category | Tokens | % of Supply |
|---|---:|---:|
| Governance-Controlled Emission Reserve | 60,000,000 | 30% |
| Treasury Reserve | 40,000,000 | 20% |
| Team Allocation | 30,000,000 | 15% |
| Proof-of-Care Incentive Reserve | 40,000,000 | 20% |
| Ecosystem Growth Reserve | 30,000,000 | 15% |
| **TOTAL SUPPLY** | **200,000,000** | **100%** |

All reserves are treasury-controlled and subject to governance constraints.

---

## Allocation Notes

**Governance-Controlled Emission Reserve**  
Tokens reserved for potential phased emissions. Release is optional, conditional,
and governance-controlled.

**Proof-of-Care Incentive Reserve**  
Tokens reserved for potential rewards tied to Proof-of-Care and continuity.
No entitlement exists absent governance-defined settlement.

**Team Allocation**  
Subject to vesting or lockups as defined by governance or future standards.

No reserve implies automatic distribution.

---

## ENS-Based Reward Routing

Where rewards are distributed, ENS MAY serve as the canonical identity layer for
routing, eligibility verification, and accountability.

ENS usage does not imply reward entitlement.

---

## Security and Economic Considerations

- Fixed supply prevents inflation
- Governance gating prevents forced emissions
- Treasury custody prevents unauthorized distribution
- Explicit non-entitlement language prevents misinterpretation
- Genesis participation does not expand supply or authority

---

## Copyright

Copyright and related rights waived via CC0.
