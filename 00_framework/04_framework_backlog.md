---
document_id: FW-005
title: Framework Backlog
version: 1.4
status: Approved
cda_version: 1.4
owner: CDA Working Group
last_updated: 2026-07-17

relationships:
  derives_from:
    - FW-003
    - FW-004
  constrained_by:
  references:
    - FW-006
  supersedes:
---

# Framework Backlog

## Purpose

Maintain the list of proposed, approved, blocked, implemented and rejected improvements to the Capability Documentation Architecture (CDA).

The Framework Backlog is the entry point for evolving the framework in a controlled and traceable manner.

## Scope of This Document

### Defines

- How framework improvements are managed.
- The lifecycle of framework evolution items.
- The status model used by the framework.
- The current backlog of framework improvements.

### Does NOT define

- Framework history.
- Framework releases.
- Project-specific backlogs.

---

# Framework Evolution

Every change to CDA begins as a Framework Evolution (FE) item.

Each item represents a proposed improvement to the framework itself rather than to any individual project.

Framework Evolution items remain in the backlog until they are either implemented or rejected.

---

# Framework Evolution Lifecycle

Each Framework Evolution item progresses through the following lifecycle.

```
Proposed

↓

Approved

↓

Implemented
```

Alternative outcomes are:

```
Blocked

Rejected
```

Meaning:

- **Proposed** – The improvement has been identified but not yet reviewed.
- **Approved** – The improvement has been accepted and scheduled.
- **Implemented** – The improvement has been incorporated into an official framework release.
- **Blocked** – The improvement depends on another unresolved item.
- **Rejected** – The proposal will not become part of CDA.

---

# Framework Evolution Item Structure

Every Framework Evolution item contains:

- Identifier
- Title
- Status
- Description
- Rationale
- Dependencies (optional)

Example:

```
FE-021

Title:
Example Improvement

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

The following items are currently tracked.

| ID | Title | Status |
|----|-------|--------|
| FE-014 | Module Specification | Blocked |
| FE-016 | Relationship Strategy | Blocked |
| FE-020 | Remove Templates Specification | Implemented |

Additional items should be appended using the next available Framework Evolution identifier.

---

# Governance

Framework Evolution items are discussed before implementation.

Only approved items may be incorporated into the framework.

Implementation should occur together with an update to the Framework Changelog.

---

# Relationship with Releases

The backlog represents the future of the framework.

The Framework Changelog records its past.

Once an item has been implemented, its outcome becomes part of the official framework history.
