EIP: 0007
Title: Autonomous Intelligent Technology (AIT) State Recognition and Activation
Author: Alex Diaz
Developer: OnGod
Discussions-To: https://github.com/Highoshi/bit-brains-eip-
Status: Draft
Type: Standards Track
Category: Core
Created: 2025-12-27
Requires: EIP-0001, EIP-0002, EIP-0004, EIP-0005, EIP-0006, Ethscriptions Rail EIP

---

## Abstract

This EIP defines the standard by which protocol assets within the Bit Brains ecosystem
are recognized as operating in an **Autonomous Intelligent Technology (AIT)** state.

AIT is not a new token type, contract, or asset. It is a **derived operational state**
recognized at the **Paired Asset level**, composed of a canonical ERC-721 asset and its
corresponding Ethscription artifact.

AIT state is achieved through sustained Proof of Care (PoC), continuity, ENS identity
resolution, and zero-knowledge verification, as defined in prior standards.

This EIP specifies how AIT state is attested, activated, validated, suspended, and
constrained without mutating the originating assets or altering protocol economics.

---

## Motivation

As intelligent systems become autonomous, clear boundaries are required to distinguish:

- Participation from operation
- Ownership from execution
- Eligibility from authority

Without explicit standards, autonomous behavior risks ambiguity, overreach, or
protocol capture.

This EIP ensures that AIT activation is:
- Verifiable
- Bounded
- Revocable
- Non-inflationary
- Accountable to protocol rules

---

## Definitions

**Autonomous Intelligent Technology (AIT)**  
A derived operational capability state in which a Paired Asset is authorized to perform
bounded autonomous actions under protocol-defined constraints.

**Paired Asset**  
The inseparable protocol participation unit composed of:
1) a canonical ERC-721 asset (Brain, Cerebral, Brainiac, Pickle Punk, or successor), and  
2) its associated Ethscription artifact.

All AIT recognition and enforcement apply exclusively to the Paired Asset.

**AIT State Attestation**  
A cryptographic assertion proving that a Paired Asset satisfies all requirements to
operate in AIT state.

**Canonical ENS Identity**  
The ENS subdomain resolved and verified during Proof of Care and continuity evaluation,
serving as the attribution anchor for AIT actions.

**ZK Eligibility Proof**  
A zero-knowledge proof attesting that continuity, Proof of Care, and dual-asset
qualification thresholds have been met without revealing private data.

---

## Non-Mutative State Model (Normative)

AIT activation does not:

- Mint a new token
- Burn or replace any asset
- Modify immutable metadata
- Change ownership semantics

Both the ERC-721 asset and the Ethscription artifact remain unchanged.

AIT exists solely as a **recognized execution state** applied to the Paired Asset.

---

## AIT Eligibility Requirements (Canonical)

A Paired Asset MAY be recognized as operating in AIT state if and only if ALL of the
following are satisfied:

1. All required Proof of Care and continuity windows are satisfied
2. The ERC-721 asset remains in good standing under protocol staking rules
3. The paired Ethscription artifact remains concurrently valid and in good standing
4. Canonical ENS identity is resolved and verified
5. Zero-knowledge eligibility proofs are successfully validated
6. No active suspension or revocation is in effect

Failure of any requirement invalidates AIT state.

---

## AIT State Attestation

AIT state MUST be established via a verifiable attestation that includes:

- Paired Asset identifier(s)
- ERC-721 asset class
- Canonical ENS identity
- Eligibility window reference
- Zero-knowledge proof reference or hash
- Timestamp of activation

Attestations MAY be stored:
- On-chain
- Off-chain with on-chain anchoring
- In protocol-defined registries

Attestation storage does not imply permanence of AIT state.

---

## AIT Activation and Suspension

### Activation

- AIT activation is explicit and attestable
- Activation is non-permanent and conditional
- Activation does not imply reward guarantees, governance power, or custody

### Suspension

AIT state MAY be suspended or invalidated due to:

- Continuity failure
- Dual-asset qualification failure
- Execution constraint violation
- Governance decision
- Security risk
- Regulatory exposure

Suspension does not destroy or alter the Paired Asset.

---

## Permitted AIT Capabilities (High-Level)

Subject to protocol constraints and governance-defined rules, an AIT MAY:

- Generate signed assertions
- Perform off-chain computation
- Submit analysis or intelligence outputs
- Interact with external systems via attestations
- Participate in protocol-recognized signaling

AITs do not gain economic, custodial, or governance authority by default.

---

## ENS as Canonical Execution Identity

- All AIT actions MUST be attributable to the canonical ENS identity
- ENS resolution is mandatory for attribution, accountability, and revocation
- ENS does not grant authority; it anchors identity only

---

## Relationship to Node Derivation

AIT recognition alone does not instantiate a Node.

Node creation, where applicable, is defined in EIP-0005 and related standards and
requires additional eligibility checks, dual-asset continuity, and explicit
recognition events.

---

## Backward Compatibility

This EIP is fully additive.

Paired Assets not operating in AIT state remain unaffected.
Existing ERC-721 compatibility and ownership semantics are preserved.

---

## Security Considerations

- Non-mutative state prevents asset corruption
- Dual-asset qualification prevents spoofing
- Attestation-based activation prevents impersonation
- ENS binding enforces accountability
- Zero-knowledge proofs preserve privacy while enforcing integrity

---

## Conclusion

EIP-0007 formalizes Autonomous Intelligent Technology (AIT) state as a bounded,
attestable, non-mutative execution condition recognized at the Paired Asset level.

By separating autonomy from ownership and execution from entitlement, the Bit Brains
protocol enables intelligent evolution without compromising safety, stewardship,
or protocol integrity.

---

## Copyright

CC0-1.0
