---
eip: 0014
title: BITS (Brain Intelligence Technology Services) — Token Technical Specification
status: Draft
type: Standards Track
category: ERC
author: Alex Diaz
created: 2026-02-12
requires: 20, 2612
---

# BITS (Brain Intelligence Technology Services)
## Token Technical Specification

This document specifies the canonical ERC-20 token design for **BITS** and the required
control surfaces to support END DAO governance, capped supply integrity, and long-term emissions.

BITS is the native token referenced by **EIP-0013 (END DAO Governance & Revenue Framework)**.

---

# 1. Abstract

BITS is an ERC-20 token with a permanent supply cap and strictly bounded mint authority.

BITS supports:

- A fixed maximum supply (hard cap)
- Deterministic emissions governed by END DAO
- Optional on-protocol burns (utility-driven, not mandatory)
- Compatibility with standard wallets, exchanges, and tooling

This specification defines the minimum on-chain interfaces, roles, and invariants required for a compliant BITS deployment.

---

# 2. Motivation

The Bit Brains ecosystem requires a token that can serve as:

- The reward emission unit for node participation and service incentives
- The governance participation unit for END DAO
- The infrastructure utility token for future BaaS / SaaS / NaaS rails

This token must enforce:

- Non-inflation beyond the cap
- Clear separation of treasury control vs emission distribution mechanics
- Governance-bounded configurability without constitutional rewrite

---

# 3. Definitions

- **BITS**: The native ERC-20 token, “Brain Intelligence Technology Services”.
- **Cap**: The immutable maximum total supply of BITS.
- **Emission Controller**: A contract authorized to mint within defined bounds to execute emissions.
- **END DAO**: Ethereum Node Development DAO, the governance authority that may update bounded parameters.
- **Treasury**: A DAO-controlled address or contract receiving protocol revenues and allocations.

---

# 4. Token Metadata (Normative)

- Name: **BITS**
- Symbol: **BITS**
- Decimals: **18** (MUST be 18)

---

# 5. Supply Cap & Allocation (Normative)

## 5.1 Total Supply Cap

- The maximum supply of BITS MUST be **1,000,000,000 BITS**.
- The cap MUST be immutable after deployment.
- No contract or governance action MAY raise the cap.

## 5.2 Allocation Model (Reference)

EIP-0013 defines the constitutional allocation model (20 / 10 / 20 / 50).

This EIP requires:

- Any minting MUST remain within the global cap.
- Emission schedules MUST be executed by verifiable on-chain contracts.

---

# 6. Core Interfaces (Normative)

BITS MUST implement ERC-20 and SHOULD implement ERC-2612 permit.

## 6.1 ERC-20

- totalSupply()
- balanceOf(address)
- transfer(address,uint256)
- allowance(address,address)
- approve(address,uint256)
- transferFrom(address,address,uint256)

## 6.2 ERC-2612 (Recommended)

- permit(...)
- nonces(address)
- DOMAIN_SEPARATOR()

---

# 7. Roles & Authorities (Normative)

## 7.1 Admin Role

An Admin role MAY exist for setup purposes but MUST NOT:

- Mint arbitrarily
- Increase total supply beyond cap
- Bypass emission bounds

Admin MAY:

- Set the Emission Controller address
- Set the Treasury address
- Configure bounded operational parameters

All critical authority SHOULD transition to END DAO governance.

---

## 7.2 Emission Controller

The Emission Controller is the ONLY entity allowed to mint BITS post-initialization.

It MUST:

- Enforce the global cap
- Enforce annual or epoch emission ceilings
- Be a smart contract (not an EOA)

If upgradeable, upgrades MUST be governed by END DAO via timelock.

---

## 7.3 END DAO Governance Authority

END DAO governance controls:

- Emission rate adjustments within constitutional bounds
- Reward distributor addresses
- Treasury configuration
- Emergency pause mechanisms (if implemented)

Governance thresholds MUST align with EIP-0013 (70 / 70 / 75).

---

# 8. Emission Model Controls (Normative)

Invariant:

> totalSupply() MUST NEVER exceed the immutable cap.

Reference model from EIP-0013:

- 40-year linear emission
- 12,500,000 BITS per year
- 500,000,000 BITS reward allocation

Implementations MUST NOT exceed those bounds without Tier-3 constitutional amendment.

---

## 8.1 Enforceable Bound Patterns

Emission Controller MUST implement at least one of:

**Pattern A — Per-Year Ceiling**
- Hard yearly mint limit

**Pattern B — Per-Second Rate + Cumulative Cap**
- Rate-based emission control

**Pattern C — Fixed Emission Schedule**
- Predefined schedule table

The chosen mechanism MUST be transparent and verifiable.

---

## 8.2 Emission Recipients

Minted emissions SHOULD be routed to a Reward Distributor contract.

Possible recipients:

- Staking vaults
- Node reward modules
- Service incentive programs

Recipient updates MUST be governance-controlled.

---

# 9. Burn Mechanics (Optional)

If enabled, BITS MAY support:

- burn(uint256)
- burnFrom(address,uint256)

Burn MUST:

- Reduce totalSupply()
- Never increase the cap
- Never allow bypass re-minting

Burn should support utility, not speculative marketing.

---

# 10. Transfer Behavior (Normative)

BITS MUST:

- Be freely transferable
- Not impose transfer taxes
- Not impose buy/sell taxes
- Not enforce arbitrary blacklists

Emergency pause MAY exist but MUST be governance-controlled and time-bounded.

---

# 11. Treasury & Revenue Separation

BITS token mechanics are separate from protocol revenue.

Protocol revenue:

- May be held in Treasury
- May be used for buybacks, grants, liquidity, infrastructure
- Does NOT guarantee redistribution to token holders

NFT revenue routing is defined in EIP-0013.

---

# 12. Security Considerations

Recommended:

- Cap enforcement on every mint
- Role separation
- Event logging for mint and burn
- Timelocked governance upgrades
- Independent security audits

---

# 13. Reference Architecture (Non-Normative)

Typical deployment stack:

- BITS ERC-20 (cap + permit)
- Emission Controller
- Reward Distributor
- END DAO Governor + Timelock

---

# 14. Backwards Compatibility

BITS is ERC-20 compliant and compatible with wallets and exchanges.

ERC-2612 improves UX but is optional.

---

# 15. Copyright

CC0-1.0
