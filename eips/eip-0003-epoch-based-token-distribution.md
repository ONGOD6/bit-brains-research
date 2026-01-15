EIP: 0003
Title: Token Supply Cap and Emission Constraints Standard
Author: Alex Diaz
Developer: OnGod
Status: Draft
Type: Standards Track
Category: Economic
Created: 2025-12-28
Requires: EIP-0001, Genesis Parameters

---

## Abstract

EIP-0003 defines the fixed maximum token supply and the constraints under which any future emissions MAY occur within the Bit Brains protocol.

This EIP establishes a hard-capped total supply, prohibits inflationary minting, and constrains all token distribution to governance-defined phases and eligibility rules.

This specification does not guarantee emission schedules, reward amounts, or distribution timing. All emissions, if any, remain subject to Proof-of-Care, continuity, and governance-defined settlement conditions.

This revision additionally defines:
- a revised Year-1 Genesis Brain staking emission schedule (20M / 15M / 10M; 45M total)
- a mint-time 12-month liquidity preference constraint (30% fee if made liquid within 12 months)
- a **maximum 6% continuity bonus pool per phase**, distributed **only among reward holders who continue staking their rewards** after mint maturity

---

## Motivation

Token systems frequently fail due to inflationary drift, unclear issuance authority, and premature extraction.

This EIP enforces a strict upper bound on supply while intentionally separating participation eligibility from emission guarantees, ensuring that no asset class, participant count, or Genesis condition can implicitly expand supply or force distribution.

This revision further strengthens sustainability by:
- tapering Year-1 staking emissions after early participation
- enforcing a mint-time 12-month holding preference for reward liquidity
- rewarding only those who maintain continuity by restaking earned rewards

---

## Canonical Genesis Reference

This EIP inherits and defers to the Bit Brains Genesis Parameters.

Genesis parameters define the initial conditions of the protocol at inception. They do not represent protocol invariants and may evolve through governance, future EIPs, or community consensus without violating core protocol principles.

Nothing in this EIP guarantees rewards, fixed schedules, or emission certainty.

---

## Total Supply (Invariant)

Maximum Supply: 200,000,000 tokens  
Inflation: Prohibited  
Supply Expansion: Not permitted under any circumstance  

This maximum supply is absolute and SHALL NOT be exceeded.

---

## Emission Constraints (Non-Guaranteed)

- Token emissions, if any, MUST occur within governance-defined phases and budgets.
- Emissions MUST remain bounded within the hard cap.
- Emissions MAY be constrained by epoch completion, Proof-of-Care, and continuity rules.
- Emissions MAY be delayed, reduced, or halted entirely.

This EIP defines constraints, not guaranteed schedules.

---

## Treasury-Held Supply Segmentation (Accounting Only)

Category                                  Tokens       % of Supply  
Governance-Controlled Emission Reserve     60,000,000   30%  
Treasury Reserve                          40,000,000   20%  
Team Allocation                           30,000,000   15%  
Proof-of-Care Incentive Reserve           40,000,000   20%  
Ecosystem Growth Reserve                  30,000,000   15%  
TOTAL SUPPLY                              200,000,000  100%  

All reserves are treasury-controlled. No reserve implies guaranteed distribution.

### Emission Reserve Internal Budgeting

The Governance-Controlled Emission Reserve (60,000,000) MAY be internally allocated by governance as follows:

- Year-1 Genesis Brain staking emissions: 45,000,000
- Preserved continuity and bonus reserve: 15,000,000

No internal allocation implies entitlement.

---

## Year-1 Genesis Brain Staking Emissions (Revised)

### Phase 1
- Duration: Months 1–5
- Allocation: 20,000,000 tokens

### Phase 2
- Duration: Months 6–9
- Allocation: 15,000,000 tokens

### Phase 3
- Duration: Months 10–12
- Allocation: 10,000,000 tokens

Total Year-1 staking emissions: 45,000,000 tokens.

---

## Liquidity Preference Constraint (Mint-Time 12-Month Rule)

### Definition

The 12-month maturity window begins at the mint timestamp of the staking position or associated reward-mint epoch.

### Rule

Any reward that becomes liquid within twelve (12) months from mint is subject to a **30% liquidity preference fee**.

Rewards made liquid after twelve (12) months MAY incur **0%** liquidity preference fee.

### Enforcement

- Enforced at the claim/withdrawal layer
- MUST NOT be implemented as a transfer-level token tax
- Fees route to treasury

---

## 12-Month Continuity Bonus  
### (Maximum 6% Pool — Distributed Only to Reward Restakers)

### Definition

Governance MAY authorize a **maximum continuity bonus pool equal to six percent (6%) of a phase’s base reward allocation**.

This pool:
- is a **hard maximum**, not a guarantee
- is distributed **only among participants who continue staking their earned rewards**
- is not available to participants who withdraw or make rewards liquid

If **no participants qualify** by restaking rewards for a phase, that phase’s continuity bonus pool MUST NOT be distributed and remains in treasury or preserved reserves.

---

### Eligibility (All Required)

A participant is eligible for the continuity bonus pool if ALL are true:

1. The participant earned rewards in the applicable phase.
2. The participant maintained continuous staking through the 12-month mint maturity window.
3. The participant **continues staking their earned rewards** at the time of bonus settlement.
4. The participant remains in good standing under Proof-of-Care rules.

---

### Pro-Rata Distribution Rule (Authoritative)

The continuity bonus pool is split **only among eligible reward restakers**, proportional to their share of restaked rewards.

Let:
- `B_phase` = maximum authorized bonus pool (≤ 6% of phase rewards)
- `R_u` = restaked rewards held by participant `u`
- `R_restaked_total` = total restaked rewards across all eligible participants

Then:

`Bonus_u = B_phase × (R_u / R_restaked_total)`

Participants who do not restake rewards receive **no share** of the pool.

---

### Maximum Bonus Pool Budgets

| Phase | Base Rewards | Max Bonus Pool (6%) |
|------|-------------:|--------------------:|
| Phase 1 | 20,000,000 | 1,200,000 |
| Phase 2 | 15,000,000 | 900,000 |
| Phase 3 | 10,000,000 | 600,000 |
| TOTAL | 45,000,000 | 2,700,000 |

These values represent **absolute caps**, not promised distributions.

---

### Constraints

- Bonuses are paid from preserved reserves
- No increase to total supply
- One-time only
- Non-compounding
- MUST NOT be described as APY or yield

---

## Security and Economic Considerations

- Fixed supply prevents inflation
- Continuity incentives reward behavior, not entitlement
- Liquidity penalties discourage premature extraction
- Bonus pools self-adjust based on participation
- Treasury remains solvent even under maximum allocation

---

## Copyright

CC0-1.0
