---
document_id: FW-001
title: Framework Index
version: 1.4
status: Approved
cda_version: 1.4
owner: CDA Working Group
last_updated: 2026-07-17

relationships:
  derives_from:
  constrained_by:
  references:
  supersedes:
---

# Framework Index

## Purpose

Provide the entry point to the Capability Documentation Architecture (CDA) framework and guide readers to the documents that define the framework itself.

## Scope of This Document

### Defines

- The structure of the Framework module.
- The purpose of each framework document.
- The recommended reading order for understanding CDA.

### Does NOT define

- The philosophy of the framework.
- Documentation conventions.
- Foundation concepts.
- Project-specific documentation.

---

# Framework Documents

| Order | Document | Purpose |
|------:|----------|---------|
| 00 | `00_index.md` | Entry point to the framework module. |
| 01 | `01_cda_overview.md` | Introduces CDA, its objectives, and its scope. |
| 02 | `02_axioms.md` | Defines the immutable principles that govern the framework. |
| 03 | `03_documentation_conventions.md` | Specifies the standards for writing, organizing and maintaining documentation. |
| 04 | `04_templates.md` | Contains reusable document templates used throughout CDA. |
| 05 | `05_framework_backlog.md` | Tracks proposed, approved, blocked and rejected framework improvements. |
| 06 | `06_framework_changelog.md` | Records the evolution of the framework across released versions. |

---

# Reading Order

Readers new to CDA should follow this sequence:

1. CDA Overview
2. CDA Axioms
3. Documentation Conventions
4. Templates
5. Framework Backlog
6. Framework Changelog

---

# Module Evolution

The Framework module evolves independently from projects that use CDA.

Changes to the framework are proposed, reviewed and approved through the Framework Backlog and become part of an official CDA release when incorporated into the Framework Changelog.

Project documentation should reference the framework version it conforms to using the `cda_version` metadata field.

---

# Related Modules

After understanding the framework itself, continue with:

- `10_foundation/`
- `20_requirements/`
- `30_domain/`
- `40_architecture/`
- `50_components/`
- `60_api/`
- `70_data/`
- `80_implementation/`
- `90_decision_records/`
- `100_testing/`