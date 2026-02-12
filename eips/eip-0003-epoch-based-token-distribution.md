# EIP-0003 — Token Supply Cap and Emission Constraints Standard (Final)

EIP: 0003  
Title: Token Supply Cap and Emission Constraints Standard  
Author: Alex Diaz  
Status: Draft (Locked Constraints)  
Type: Standards Track  
Category: Economic  
Created: 2025-12-28  
Related: EIP-0012, EIP-0013, EIP-0014  

---

# 1. Purpose

This EIP defines the constitutional supply cap and emission constraint rules for the protocol’s native token:

**BITS — Brain Intelligence Technology Services**

All emission mechanics, contracts, and governance actions MUST operate within the boundaries defined in this EIP.

---

# 2. Fixed Total Supply Cap (Normative)

The total token supply is permanently capped at:

**1,000,000,000 BITS**

The supply cap MUST NOT be exceeded.

Governance may not increase total supply without a constitutional amendment.

---

# 3. Emission Activation Rule (Normative)

BITS emissions MUST NOT occur prior to DAO activation.

- Protocol Launch: March 1, 2026  
- BITS Token Launch + DAO Activation: March 1, 2027  
- Emission Start Date: March 1, 2027  

There is no pre-DAO emission authority.

Any previously referenced “Year-1 emissions” prior to DAO activation are deprecated and non-authoritative.

---

# 4. Emission Allocation Ceiling (Normative)

A maximum of **50% of total supply** may be distributed through emissions:

**Maximum emission allocation: 500,000,000 BITS**

This allocation does not expand the total supply cap.

---

# 5. Annual Emission Ceiling (Normative)

Beginning March 1, 2027:

**Annual emission ceiling: 12,500,000 BITS per year**  
Equivalent to **1.25% of total supply annually**

No mechanism may cause annual emissions to exceed this ceiling.

---

# 6. Emission Schedule (Normative)

The canonical emission structure is:

- 40-year linear emission beginning March 1, 2027  
- 12,500,000 BITS maximum per program year  
- Total emissions not to exceed 500,000,000 BITS  

Governance MAY reduce emission rates for any year.

---

# 7. Suballocations Within the Annual Ceiling (Normative)

The annual emission ceiling may be partitioned into suballocations, provided:

- Total emissions in any year do not exceed 12,500,000 BITS  
- Lifetime emissions do not exceed 500,000,000 BITS  

Suballocations may include:

- Genesis Continuity Dividend (EIP-0012)  
- Node Service & Infrastructure Emissions  
- Other governance-approved reward programs  

Suballocations do not create additional mint authority.

---

# 8. Governance Authority (Normative)

After DAO activation (March 1, 2027):

END DAO governance may propose adjustments to emission parameters, including:

- Reducing annual emission levels  
- Modifying emission cadence  
- Adjusting suballocation structure  

Any change must:

- Remain within the fixed total supply cap  
- Remain within lifetime emission allocation boundaries  
- Follow the governance thresholds defined in EIP-0013  

The supply cap remains constitutionally protected.

---

# 9. Interpretation Rule

This EIP MUST NOT be interpreted as:

- Guaranteeing annual emissions  
- Requiring full annual distribution  
- Mandating specific suballocations  
- Creating entitlement expectations  

Emission authority is bounded, not mandatory.

---

End of EIP-0003
