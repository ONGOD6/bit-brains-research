---
EIP-0003: Finalize Token Supply and Distribution Standard
Author: Bit Brains Protocol
Developer: On God
- Define fixed 200M max supply with no inflation
- Introduce hard-capped 3-phase emissions (60M total)
- Specify canonical allocations for treasury, team, ecosystem growth,
  and NFT staking / Proof of Care rewards
- Add optional extensions for exit penalties, NFT royalties, and ENS-based routing
discussions-to: TBD
status: Draft
type: Standards Track
category: Economic
created: 2025-12-28
---

## Abstract

EIP-0003 defines the fixed token supply, allocation, and phased emission schedule for the Bit Brains Protocol. This specification establishes a hard-capped maximum supply, a three-phase emissions program that terminates permanently after Phase 3, and explicit allocations for protocol treasury, team, ecosystem growth, and eligibility-based rewards tied to NFT staking and Proof of Care continuity participation.

At Genesis, the protocol introduces multiple on-chain participant asset types, including Genesis Brain NFTs and Pickle Punk Headshot Ethscriptions. While multiple assets may participate in Proof of Care and continuity mechanisms, token emissions remain strictly capped and are distributed solely according to protocol-defined eligibility criteria, not asset count or asset class.

## Motivation

Token launches frequently suffer from unclear allocation, inflationary drift, and premature liquidity extraction. EIP-0003 addresses these failures by enforcing a fixed maximum supply, capped emissions with no extensions, and treasury-held incentive pools aligned with long-term participation and protocol continuity.

Additionally, by explicitly recognizing multiple Genesis participant asset types while keeping emissions strictly capped, this EIP prevents misinterpretation that additional Genesis assets expand token supply or create discretionary minting authority.

## Specification

### Total Supply

- **Maximum supply:** **200,000,000 tokens**
- **Inflation:** None
- **Additional emissions:** Not permitted beyond Phase 3

### Phase Emissions (Hard-Capped)

Emissions occur across three complete phases with no mid-phase unlocks and no emissions after Phase 3.

- **Phase 1:** 20,000,000 tokens
- **Phase 2:** 20,000,000 tokens
- **Phase 3:** 20,000,000 tokens

**Total phase emissions:** **60,000,000 tokens (30%)**

There is no Phase 4 and no discretionary minting authority.

### Genesis Participants and Eligibility

At Genesis, the protocol recognizes a fixed set of **Genesis Participants (GP)**, defined as the union of:

- **1,500 Genesis Brain NFTs**
- **1,500 Pickle Punk Headshot Ethscriptions**

Total Genesis Participants: **3,000**

Genesis Participants MAY participate in Proof of Care and continuity mechanisms; however, participation alone does not guarantee token emissions. Eligibility for rewards is determined by protocol-defined rules, including staking status, continuity requirements, and identity resolution (e.g. ENS-based routing), as specified in subsequent standards.

### Allocation (Fully Accounted)

All tokens are accounted for within the fixed supply. Tokens intended for time-based distribution are held in vaults/escrows at genesis and released according to protocol rules.

| Category | Tokens | % of Supply |
|---|---:|---:|
| **Phase Emissions Vault (Treasury-held; released across 3 phases)** | 60,000,000 | 30% |
| Treasury Reserve | 40,000,000 | 20% |
| Team Allocation | 30,000,000 | 15% |
| NFT Staking / Proof of Care Rewards (Treasury-held) | 40,000,000 | 20% |
| Ecosystem Growth Treasury | 30,000,000 | 15% |
| **TOTAL SUPPLY** | **200,000,000** | **100%** |

### Allocation Notes

**Phase Emissions Vault (30%, Treasury-held)**  
A dedicated vault containing 60,000,000 tokens reserved at genesis and released only according to the Phase 1–3 emission schedule. No tokens may be emitted beyond Phase 3.

**Treasury Reserve (20%)**  
Held to support protocol solvency, stabilization mechanisms, governance-approved initiatives, and optional buyback or burn programs if adopted by governance.

**Team Allocation (15%)**  
Reserved for contributors and operators. Vesting or lock schedules, if applicable, MUST be defined by subsequent standards or governance resolutions.

**NFT Staking / Proof of Care Rewards (20%, Treasury-held)**  
A dedicated pool reserved for rewards distributed to eligible participants who satisfy protocol-defined staking, Proof of Care, and continuity requirements. Eligibility MAY include multiple Genesis asset types but does not expand the emissions cap or alter the fixed supply.

**Ecosystem Growth Treasury (15%)**  
Reserved for ecosystem expansion, including developer grants, partnerships, infrastructure, and adoption incentives.

## Optional Extensions (Non-Normative)

The following mechanisms MAY be adopted via subsequent standards or governance but are not required by this EIP:

### Progressive Downstream Exit Penalty

A phased penalty MAY apply to early exits or withdrawals:

- Phase 1: 30%
- Phase 2: 20%
- Phase 3: 10%

Penalties route to the Treasury Reserve.

### NFT Secondary Royalties

A baseline secondary royalty MAY be applied:

- 3% total (1% Founder, 1% Artist, 1% Treasury)

### ENS-Based Reward Routing

Reward eligibility and routing MAY require ENS resolution as the canonical identity layer, with optional zero-knowledge proofs for eligibility verification. ENS-based routing MAY apply to Genesis Participants, including both NFTs and Ethscriptions, subject to protocol-defined eligibility requirements.

## Security and Economic Considerations

- Fixed supply prevents inflationary dilution.
- Hard-capped emissions reduce liquidity shock risk.
- Treasury-held incentive pools prevent uncontrolled distribution.
- Explicit accounting improves auditability and governance clarity.
- Explicit Genesis participant definitions prevent misinterpretation that additional Genesis assets expand supply or emissions.

## Copyright

Copyright and related rights waived via CC0.
