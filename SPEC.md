# Protocol Ready Small Business (PRSB)
## Version 0.1 — Draft

PRSB defines constraints and interfaces for representing business-relevant artifacts
using sovereign, open protocols. PRSB is implementation-agnostic and does not
prescribe business outcomes, adoption strategy, governance models, or reputation logic.

See `NON_GOALS.md` for explicit exclusions.

---

## 1. Scope

A “protocol-ready small business” (as used in this specification) is a business whose
public-facing operational artifacts can be represented and verified using:
- sovereign identity keys (e.g., Nostr-compatible keypairs or equivalent)
- sovereign payment interfaces (e.g., Bitcoin/Lightning-compatible settlement)
- portable discovery artifacts (e.g., open catalog schemas)
- signed delivery and support artifacts (e.g., receipts, logs, and dispute records)

PRSB defines artifact formats and conformance constraints. Any interpretation of these
artifacts for trust, reputation, ranking, or recommendation is external to PRSB.

---

## 2. Identity Requirements

A conforming implementation MUST support:
1. A dedicated business signing key (public/private keypair).
2. Secure key backup and key rotation procedures (implementation-defined).
3. Use of the business key to sign business-relevant artifacts, including (as applicable):
   - announcements
   - catalog versions
   - deliverable provenance records
   - support and dispute artifacts

A conforming implementation MUST NOT require platform-controlled identity as the
sole method of authentication or provenance.

---

## 3. Payment Interface Requirements

A conforming implementation MUST support at least one sovereign settlement interface
suitable for the business context (e.g., Lightning invoice, LNURL-pay, or equivalent).

Where payments are used, a conforming implementation SHOULD provide a verifiable
payment reference artifact (implementation-defined) that can be associated with
deliverables and/or dispute records.

PRSB does not prescribe treasury policy, pricing, monetization, or performance claims
(e.g., “instant” or “final” settlement guarantees).

---

## 4. Discovery Requirements

A conforming implementation MUST provide a portable, machine-readable catalog artifact
for discovery and verification. At minimum, this SHOULD include:
- a versioned catalog schema (e.g., JSON)
- a stable retrieval mechanism (e.g., a publicly accessible endpoint or equivalent)
- optional mirroring into protocol-native discovery channels (implementation-defined)

PRSB does not prescribe use of any specific commerce platform and does not require
negative dependencies (“must not use X”) beyond the portability and verifiability
constraints above.

---

## 5. Transparency and Provenance Artifacts

A conforming implementation MUST support signed, timestamped artifacts for:
- fulfillment / delivery evidence (where applicable)
- support interactions (where applicable)
- service terms or SLA representations (where applicable)
- dispute records (where applicable)

Visibility of artifacts (public, private, selective disclosure) is implementation-defined
and may be constrained by privacy, security, regulatory, or contractual requirements.

PRSB does not define a global reputation system. Any reputation or trust signaling is
external and derived from artifacts according to implementation-specific rules.

---

## 6. Participation and Feedback (Optional)

A conforming implementation MAY support mechanisms for receiving structured feedback,
including:
- issue reports (e.g., UX friction)
- documentation corrections
- schema refinement proposals
- localization or translation contributions

If contributor acknowledgment or compensation occurs, it is voluntary and external to
PRSB. PRSB does not prescribe or guarantee payment, rewards, or incentive programs.

---

## 7. Operations Artifacts

A conforming implementation SHOULD document operational workflows in reproducible,
versioned form, including (as applicable):
- custody diagrams
- support protocols
- refund/dispute flows
- security audit steps
- vendor evaluation criteria

PRSB excludes marketing/growth and onboarding objectives; see `NON_GOALS.md`.
Operational artifacts may be published or retained privately according to
implementation constraints.

---

## 8. Dispute Artifacts

Where disputes are supported, a conforming implementation MUST represent disputes as
signed records that MAY include:
- escalation steps
- refund path or remediation steps
- payment reference linkage (where applicable)
- visibility scope (public/private/selective)

PRSB does not prescribe dispute resolution services, arbitration, escrow, or marketplace
intermediation.

---

## 9. Implementation Validation (Non-Normative)

For maturity, major clauses SHOULD be supported by at least one implementation example
and associated evidence artifacts (e.g., catalog sample, signed deliverable record,
support log, or dispute record).

Unvalidated clauses may be marked as experimental.

---

## 10. Versioning and Change Management

Specification changes SHOULD be tracked via:
- issue discussion and rationale
- versioned diffs
- review notes

Release announcements and signatures are implementation-defined. PRSB does not mandate
any specific broadcast channel.

---

## 11. Out of Scope

PRSB does not define:
- marketplaces, hiring systems, or credentialing
- global reputation metrics or social graphs
- governance bodies, representation, or advocacy
- marketing, growth, onboarding, or adoption strategies

See `NON_GOALS.md` for additional exclusions.
