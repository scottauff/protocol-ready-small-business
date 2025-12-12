# Protocol Ready Small Business (PRSB)

The **Protocol Ready Small Business (PRSB)** specification defines formal constraints, interfaces, and templates for representing and coordinating **business-relevant workflows and artifacts** on sovereign, open protocols.

This repository contains the normative specification, related schemas, and reference documentation.

PRSB does **not** prescribe business models, adoption strategies, marketplaces, credential systems, reputation systems, or community frameworks.

---

## Specification Overview

PRSB provides:

- A **schema** for representing small business readiness constructs
- Interfaces for encoding transparency templates and structured business artifacts
- Conventions for documenting operational constraints
- Edge-case models for dispute resolution and interaction constraints

The specification is **implementation-agnostic** and **neutral** with respect to incentive models, governance structures, and commercial outcomes.

---

## Repository Structure

```
/
├── README.md
├── CONTRIBUTING.md
├── NON_GOALS.md
├── SPEC.md
├── CHANGELOG.md
└── GOVERNANCE/
├── NEUTRALITY.md
└── MAINTAINERS.md
```

- **SPEC.md** — normative specification text  
- **CONTRIBUTING.md** — guidelines for submitting specification improvements  
- **NON_GOALS.md** — explicit out-of-scope definitions  
- **GOVERNANCE/** — neutrality posture and maintainer constraints  

---

## Principles and Scope

The PRSB specification operates under the following constraints:

- **Protocol-native**: defines interfaces compatible with sovereign protocol systems
- **Constraint-first**: language focuses on invariants and requirements, not outcomes
- **Economically non-prescriptive**: does not mandate pricing, monetization, or settlement models
- **Authority-neutral**: does not define reputation systems, rankings, or canonical implementations

Explicit exclusions and non-objectives are documented in `NON_GOALS.md`.

---

## Contributing

Contributions may propose clarifications, schema refinements, documentation improvements, or edge-case analysis relevant to the specification.

All contributions are subject to the neutrality and non-alignment constraints defined in `GOVERNANCE/NEUTRALITY.md`.

See `CONTRIBUTING.md` for process details.

---

## Governance

Specification stewardship and maintainer scope are defined in `GOVERNANCE/MAINTAINERS.md`.

PRSB has no central authority, foundation, or representative body.

---

## Licensing

This specification and associated documents are released under the repository’s default open license.

---

## Notes on Usage

PRSB content is intended for use in:
- Protocol-native representations of business artifacts
- Interoperable communication between sovereign systems
- Independent implementations whose semantics are defined externally

PRSB is **not** a product, platform, service, or ecosystem.  
It is a formal specification that may be referenced, implemented, forked, or abandoned without permission.
