EIP: 0004  
Title: Genesis NFTs and Core Participation Assets  
Author: Alex Diaz  
Developer: OnGod  
Status: Draft  
Type: Standards Track  
Category: Core  
Created: 2025-12-22  
Requires: EIP-0001, EIP-0003, Genesis Parameters, Ethscriptions Rail EIP  

---

## Abstract

This EIP defines the Genesis participation assets of the  
Bit Brains protocol.

Genesis participation is established through **ERC-721 NFTs**,  
each minted with an associated **secondary Ethscription artifact**  
that serves as immutable calldata provenance.

Together, the ERC-721 asset and its paired Ethscription form a  
single protocol-recognized **Paired Asset**, which acts as the  
canonical unit of identity, eligibility, and long-term evolution.

This EIP defines **what exists at Genesis**, not how or when  
future evolution, activation, or staking mechanics occur.

---

## Motivation

The Bit Brains protocol is designed around clarity, continuity,  
and long-term extensibility.

Early-stage protocols often introduce parallel participation  
systems prematurely, increasing complexity and weakening  
identity guarantees.

This EIP enforces a strict Genesis boundary by defining:
- exactly which assets exist at inception, and
- how those assets are structurally composed on-chain.

Genesis defines **existence and identity**, not activation,  
evolution, or economic behavior.

---

## Genesis Asset Set

At Genesis, the Bit Brains protocol recognizes  
**3,000 total Genesis ERC-721 NFTs**, composed of:

- **1,500 Genesis Brains (ERC-721)**  
- **1,500 Genesis Pickle Punks (ERC-721)**  

Each Genesis ERC-721 NFT is minted **simultaneously** with a  
corresponding **Ethscription artifact**.

These paired components collectively form **Genesis Assets**.

---

## Canonical Paired Asset Definition

Each Genesis Asset consists of:

1. A canonical **ERC-721 NFT**, and  
2. A corresponding **Ethscription artifact**, committed as  
   immutable Ethereum calldata at mint time.

Together, these components form a **Paired Asset**.

The Paired Asset is the **only protocol-recognized identity unit**  
for participation, continuity tracking, and future evolution.

Neither component is recognized independently.

---

## Participation Scope (Genesis Phase)

During Genesis and initial protocol phases:

- Only **Paired Assets derived from Genesis ERC-721 NFTs** exist  
- No alternative assets, wrappers, derivatives, or representations  
  participate in protocol mechanics
- Ethscription artifacts are **non-operative** and **non-qualifying**
  until explicitly activated by later standards

Participation eligibility, staking, Proof-of-Care evaluation, and  
continuity tracking are defined exclusively by Genesis Parameters  
and subsequent EIPs.

---

## Explicit Non-Features

This EIP explicitly does **not** define or activate:

- Independent Ethscription participation rails  
- Secondary staking systems  
- Autonomous Intelligent Technology (AIT) mechanics  
- Node mechanics or execution layers  
- Reward formulas or emission schedules  
- Activation criteria for secondary artifacts  

All such mechanisms MUST be defined in future EIPs.

---

## Dual-Mint Invariant (Canonical)

The Bit Brains protocol defines a **dual-mint invariant**  
for all core asset classes, including:

- Brains  
- Cerebrals  
- Brainiacs  
- Nodes (where applicable)

For each such asset:
- An **ERC-721 NFT** and
- A **paired Ethscription artifact**

MUST be minted together as a single, inseparable unit.

This invariant ensures:
- immutable provenance,
- long-term extensibility,
- and non-fragmented asset evolution.

---

## Forward Compatibility

At later stages of protocol development, Paired Assets MAY  
become eligible for:

- dual-asset staking,
- Proof-of-Care evaluation,
- Autonomous Intelligent Technology (AIT) activation, and
- Node recognition.

Such activation:
- is **explicitly deferred**,
- requires future EIPs, and
- MUST enforce concurrent qualification of both paired components.

No activation, evolution, or staking behavior is enabled by  
this EIP.

---

## Security Considerations

By defining Genesis participation at the Paired Asset level  
while keeping secondary artifacts non-operative, the protocol:

- minimizes attack surface,
- preserves clear ownership semantics,
- prevents premature system complexity, and
- maintains cryptographic extensibility guarantees.

---

## Copyright

Copyright and related rights waived via CC0.
