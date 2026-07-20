---

document_id: FW-005
title: Framework Backlog
version: 2.0
status: Approved
cda_version: 2.0
owner: CDA Working Group
last_updated: 2026-07-20

relationships:
derives_from:
- FW-002
- FW-003
- FW-004
constrained_by:
references:
- FW-006
supersedes: FW-005 v1.4
-----------------------

# Framework Backlog

## Purpose

Maintain the list of proposed changes to the Capability Documentation Architecture (CDA).

The Framework Backlog provides the governance mechanism through which the CDA reference model evolves in a controlled, transparent, and traceable manner.

---

# Scope

## Defines

* How framework changes are proposed.
* The lifecycle of Framework Evolution items.
* The classification of framework changes.
* The status model used by the framework.
* The current backlog of framework proposals.

## Does NOT define

* Framework history.
* Framework releases.
* Knowledge Domain specifications.
* Project-specific backlogs.

---

# Relationship to the Framework

The Foundational Concepts and Core Axioms define the conceptual foundation of CDA.

The Framework Backlog records proposals that may evolve the framework while preserving that foundation.

Acceptance into the backlog does **not** imply acceptance into the framework.

Every proposal should be evaluated for consistency with the Foundational Concepts and Core Axioms before approval.

---

# Framework Evolution

Every proposed change to CDA begins as a **Framework Evolution (FE)** item.

An FE item represents a proposed improvement to the framework itself rather than to any individual software project.

Framework Evolution items remain in the backlog until they are implemented, rejected, or otherwise resolved.

---

# Types of Framework Changes

Framework Evolution items may affect different parts of the framework.

| Type                   | Description                                                                    |
| ---------------------- | ------------------------------------------------------------------------------ |
| Conceptual             | Introduces or modifies Foundational Concepts.                                  |
| Axiomatic              | Introduces or modifies Core Axioms.                                            |
| Knowledge Model        | Adds, removes, merges, or redefines Knowledge Domains or ownership boundaries. |
| Documentation Practice | Modifies recommended documentation practices.                                  |
| Template               | Updates reusable document templates.                                           |
| Governance             | Changes framework evolution or release processes.                              |
| Editorial              | Clarifies wording, formatting, or examples without changing meaning.           |

---

# Change Impact

Each Framework Evolution item should declare its expected impact.

Possible impact levels are:

* Editorial
* Minor
* Major
* Breaking

A proposal is considered **Breaking** if it changes:

* Foundational Concepts;
* Core Axioms;
* Knowledge Domain boundaries;
* ownership rules;
* framework terminology that affects existing implementations.

---

# Framework Evolution Lifecycle

Each Framework Evolution item progresses through the following lifecycle.

```text
Proposed
    ↓
Under Review
    ↓
Approved
    ↓
Implemented
```

Alternative outcomes are:

```text
Deferred

Rejected
```

### Status Definitions

* **Proposed** — The improvement has been identified but has not yet been reviewed.
* **Under Review** — The proposal is being evaluated.
* **Approved** — The proposal has been accepted for implementation.
* **Implemented** — The proposal has been incorporated into an official framework release.
* **Deferred** — The proposal remains valid but has been postponed.
* **Rejected** — The proposal will not become part of the framework.

---

# Framework Evolution Item Structure

Every Framework Evolution item should contain:

* Identifier
* Title
* Type
* Impact
* Status
* Description
* Rationale
* Dependencies (optional)

Example:

```text
FE-021

Title:
Introduce Knowledge Relationships

Type:
Knowledge Model

Impact:
Major

Status:
Proposed

Description:
...

Rationale:
...

Dependencies:
FE-018
```

---

# Current Framework Backlog

The following Framework Evolution items are currently tracked.

| ID     | Title                          | Type                   | Impact | Status      |
| ------ | ------------------------------ | ---------------------- | ------ | ----------- |
| FE-014 | Module Specification           | Knowledge Model        | Major  | Deferred    |
| FE-016 | Relationship Strategy          | Documentation Practice | Minor  | Deferred    |
| FE-020 | Remove Templates Specification | Governance             | Minor  | Implemented |

New items should use the next available Framework Evolution identifier.

---

# Governance

Framework Evolution items should be evaluated according to:

* conceptual consistency;
* alignment with the Foundational Concepts;
* consistency with the Core Axioms;
* impact on existing Knowledge Domains;
* compatibility with existing framework implementations.

Only approved items may be incorporated into an official CDA release.

---

# Relationship with Releases

The Framework Backlog represents the future evolution of CDA.

The Framework Changelog records the history of completed framework releases.

When a Framework Evolution item is implemented, its outcome should be recorded in the Framework Changelog together with the corresponding framework version.

---

# Evolution

The governance process defined by this document may itself evolve through future Framework Evolution items.

Changes to governance should preserve the stability, consistency, and long-term integrity of the Capability Documentation Architecture.
