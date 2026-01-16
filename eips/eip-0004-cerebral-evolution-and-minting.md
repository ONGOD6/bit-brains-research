EIP: 0004  
Title: Genesis NFTs and Core Participation Assets  
Author: Alex Diaz  
Developer: OnGod  
Status: Draft  
Type: Standards Track  
Category: Core  
Created: 2025-12-22  
Requires: EIP-0001, EIP-0003  

---

## Abstract

This EIP defines the Genesis participation assets of the  
Bit Brains protocol.

Genesis participation is established exclusively through  
ERC-721 NFTs.

These assets form the foundational layer for identity,  
staking eligibility, Proof-of-Care alignment, and  
continuity participation.

This proposal intentionally limits scope to ERC-721  
Genesis assets and does not introduce alternative  
participation rails, derivative mechanisms, or active  
secondary systems.

---

## Motivation

The Bit Brains protocol is designed around clarity,  
continuity, and long-term extensibility.

Early-stage protocols often introduce parallel systems  
too early, increasing complexity and weakening identity  
guarantees.

This EIP enforces a strict Genesis boundary by defining  
exactly which assets exist at inception and how they  
participate.

Genesis defines **what exists**, not how all future  
evolution unfolds.

---

## Genesis Asset Set

At Genesis, the Bit Brains protocol recognizes  
**3,000 total Genesis NFTs**, composed of:

- **1,500 Genesis Brains (ERC-721)**
- **1,500 Genesis Pickle Punks (ERC-721)**

These assets are collectively referred to as  
**Genesis NFTs**.

Genesis NFTs are the **only assets eligible** for protocol  
participation during the initial phases.

---

## Participation Scope

Genesis NFTs enable:

- Protocol identity anchoring  
- ENS-based identification  
- Eligibility for staking  
- Participation in Proof-of-Care  
- Continuity tracking across phases  

No additional assets, wrappers, inscriptions, or  
derivative representations participate in Genesis  
mechanics.

---

## Exclusions and Non-Features

This EIP explicitly does **not** introduce:

- Alternative minting rails  
- Secondary participation assets  
- Node mechanics  
- Autonomous Intelligent Technology (AIT)  
- Economic guarantees or reward formulas  
- Time-based unlocks or emissions schedules  

Any such mechanisms, if introduced, must be defined  
in future EIPs.

---

## Dual Mint Clarification (Future-Scoped)

Each Genesis NFT is minted with a **secondary on-chain  
artifact** created in parallel.

This artifact is an **Ethscription**, represented as  
calldata committed to Ethereum.

The Ethscription:

- Has no active protocol function at Genesis  
- Does not confer participation rights  
- Does not affect staking or rewards  
- Does not operate as a participation rail  

Its sole purpose is to act as a **protocol safeguard  
and extensibility anchor**, reserved for future system  
development.

This capability is **explicitly inactive** during  
Genesis and the initial protocol phases.

---

## Forward Compatibility

At a later stage of protocol development, secondary  
artifacts may be utilized to support future evolution  
paths.

These paths may include progression toward  
Autonomous Intelligent Technology (AIT) or node-based  
systems.

No mechanics, guarantees, timelines, or activation  
criteria are defined in this EIP.

---

## Invariant

The Bit Brains protocol defines a **dual-mint invariant**  
for its core asset classes:

- Brains  
- Cerebrals  
- Brainiacs  

Each ERC-721 asset is minted with a corresponding  
secondary artifact.

This invariant ensures long-term extensibility without  
altering current protocol behavior.

---

## Security Considerations

By limiting Genesis participation to ERC-721 NFTs,  
the protocol reduces attack surface and preserves  
clear ownership and identity semantics.

Secondary artifacts remain non-operative until  
explicitly activated by future standards.

---

## Copyright

Copyright and related rights waived via CC0.
