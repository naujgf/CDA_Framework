---
document_id: FW-004
title: Documentation Conventions
version: 1.4
status: Approved
cda_version: 1.4
owner: CDA Working Group
last_updated: 2026-07-17

relationships:
  derives_from:
    - FW-003
  constrained_by:
  references:
  supersedes:
---

# Documentation Conventions

## Purpose

Define the standards for writing, organizing, versioning and maintaining documentation within the Capability Documentation Architecture (CDA).

These conventions ensure that documentation remains consistent, predictable and scalable across projects.

## Scope of This Document

### Defines

- Document structure.
- Naming conventions.
- Numbering conventions.
- Metadata specification.
- Writing conventions.
- Relationship conventions.
- Document lifecycle.

### Does NOT define

- Framework philosophy.
- Framework axioms.
- Module specifications.
- Project-specific conventions.

---

# Relationship to the Axioms

The CDA Axioms define **what must always remain true**.

The Documentation Conventions define **how those principles are applied** when creating documentation.

Conventions may evolve over time provided they remain consistent with the framework axioms.

---

# Standard Document Structure

Every document follows the same high-level structure.

1. YAML metadata
2. Document title
3. Purpose
4. Scope of This Document
5. Main content
6. Optional examples
7. Optional references

This structure provides consistency across the framework while allowing each document to define its own content.

---

# Metadata Specification

Every document begins with the following metadata.

```yaml
document_id:
title:
version:
status:
cda_version:
owner:
last_updated:

relationships:

  derives_from:

  constrained_by:

  references:

  supersedes:
```

Metadata provides document identity, versioning and traceability.

---

# Scope Section

Every document includes a scope section composed of two parts.

## Defines

Lists the concepts that are intentionally covered by the document.

## Does NOT define

Lists related concepts that are intentionally excluded.

The purpose of this section is to eliminate ambiguity and reduce overlap between documents.

---

# Naming Conventions

Documentation files follow these rules.

- lowercase only
- words separated by underscores
- singular nouns
- descriptive names
- no abbreviations
- `.md` extension

Examples

```
01_product_scope.md

03_system_context.md

05_domain_event.md
```

---

# Numbering Conventions

## Module Numbering

Top-level modules use increments of ten.

```
00_framework

10_foundation

20_requirements

30_domain

40_architecture

50_components

60_api

70_data

80_implementation

90_decision_records

100_testing
```

This allows future modules to be inserted without renumbering the repository.

---

## Document Numbering

Documents inside each module use sequential numbering.

```
00_index.md

01_...

02_...

03_...
```

Documents may be renumbered within a module if required.

---

# Document Identifier Convention

Every document has a stable identifier independent of its filename.

Examples

```
FW-001

FD-001

RQ-001

DM-001

AR-001

CP-001

API-001

DT-001

IM-001

DR-001

TS-001
```

Identifiers remain stable even if documents are renamed.

---

# Writing Conventions

Documentation should be:

- concise
- explicit
- technology-agnostic whenever possible
- written in active voice
- unambiguous
- free from unnecessary repetition

Each document should answer one primary question.

Information should appear only once within the documentation architecture whenever practical.

---

# Relationship Conventions

Relationships provide traceability between documents.

Relationship metadata is included only when it adds value.

Not every document requires relationships.

Relationship strategy is defined separately by each module as appropriate.

Supported relationship types are:

- derives_from
- constrained_by
- references
- supersedes

---

# Document Lifecycle

Every document progresses through the following lifecycle.

```
Draft

↓

Review

↓

Approved

↓

Deprecated

↓

Archived
```

Approved documents should only be modified through the Framework Evolution process.

---

# Versioning

Projects declare the version of CDA they implement using the `cda_version` metadata field.

Framework releases are versioned independently from the software projects that adopt them.

---

# Traceability

Documentation should enable readers to navigate naturally from:

Business intent

↓

Requirements

↓

Domain

↓

Architecture

↓

Components

↓

Implementation

↓

Testing

without duplication of information.

---

# Evolution

Documentation conventions may evolve between framework versions.

However, every change must remain consistent with the CDA Axioms.

Changes to these conventions are managed through the Framework Evolution process.
