# Rationale: Protocol-Ready Small Business

This document is **non-normative**.

It explains the motivation and design rationale behind the
**Protocol Ready Small Business (PRSB)** specification. Nothing in this
document introduces requirements, constraints, or guarantees beyond what
is defined in `SPEC.md`.

---

## Background

Modern small businesses increasingly depend on platform-mediated systems
for discovery, payments, reputation, and customer interaction. These systems
often bundle identity, communication, commerce, and incentives into closed,
permissioned environments.

While convenient, such dependency introduces structural risks:
- External control over identity and visibility
- Opaque or non-portable reputation signals
- Incentive misalignment between platforms and operators
- Fragility under policy, pricing, or algorithm changes

PRSB emerges from the observation that these risks are not primarily
technological, but architectural.

---

## The Sovereign Node Model (Conceptual)

PRSB is informed by a conceptual model in which a small business behaves as a
**sovereign node** within an open protocol environment.

In this model:
- Identity is held by cryptographic keys, not platform accounts
- Business artifacts are signed, versioned, and portable
- Payments occur over open settlement protocols rather than proprietary rails
- Discovery is derived from shared schemas and public artifacts, not ranking systems

This framing is descriptive, not prescriptive. PRSB does not require a business
to operate exclusively in this manner, nor does it claim superiority over other
models.

---

## On Advertising, Platforms, and Intermediation

PRSB intentionally avoids defining mechanisms related to:
- Advertising systems
- Algorithmic distribution
- Platform-native reputation or influence metrics
- Intermediated marketplaces

This is not a prohibition. It is a scope decision.

The specification focuses on **what can be represented and verified without
platform dependence**, leaving questions of marketing, growth, and customer
acquisition to external systems or implementations.

---

## Reputation as an Emergent Property

In platform-centric systems, reputation is typically:
- Centrally computed
- Opaque in methodology
- Non-portable across contexts

PRSB does not define reputation systems.

Instead, it defines **verifiable artifacts** (e.g., signed catalogs, delivery
records, dispute logs) from which reputation *may* be inferred externally.

Any interpretation of trust, reliability, or quality derived from these
artifacts is outside the scope of PRSB and intentionally left to implementers,
markets, or observers.

---

## Why PRSB Is Constraint-First

PRSB is designed around constraints rather than outcomes because:
- Outcomes vary by business context
- Incentives change over time
- Protocol longevity depends on minimal assumptions

By limiting itself to artifact structure and interface boundaries, PRSB aims
to remain usable across:
- Jurisdictions
- Industries
- Regulatory environments
- Economic conditions

---

## Relationship to Implementations

PRSB does not attempt to replace platforms, businesses, or existing workflows.

Implementations may:
- Use PRSB artifacts internally
- Expose them publicly
- Combine them with platform-based systems
- Ignore portions of the specification

The specification remains valid regardless of implementation success or failure.

---

## Closing Note

This rationale document exists to make the design posture explicit, not to
promote a particular operating model.

The normative definition of PRSB is contained exclusively in `SPEC.md`.
All exclusions and boundaries are enumerated in `NON_GOALS.md`.
