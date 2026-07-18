---
document_id: FW-006
title: Framework Changelog
version: 1.4
status: Approved
cda_version: 1.4
owner: CDA Working Group
last_updated: 2026-07-17

relationships:
  derives_from:
  constrained_by:
  references:
    - FW-005
  supersedes:
---

# Framework Changelog

## Purpose

Record the official release history of the Capability Documentation Architecture (CDA).

Each release summarizes the framework changes that became part of the official specification.

The changelog provides a historical record of the framework's evolution and serves as the authoritative source for released versions.

## Scope of This Document

### Defines

- Framework release history.
- Released framework changes.
- Framework version progression.

### Does NOT define

- Proposed changes.
- Future work.
- Project changelogs.
- Framework rationale.

---

# Release Policy

Only released framework changes appear in this document.

Every entry represents a completed framework release.

Changes under discussion or awaiting approval remain in the Framework Backlog until implemented.

---

# Versioning

CDA follows semantic versioning principles.

- **Major** versions introduce changes to the conceptual foundation of the framework, such as modifications to the CDA Axioms.

- **Minor** versions introduce new modules, conventions, specifications or other backward-compatible improvements.

- **Patch** versions correct errors, improve wording or make editorial refinements without changing the framework's meaning.

---

# Release History

## Version 1.4

Release Date: 2026-07-17

### Added

- Canonical Framework module.
- CDA Overview.
- CDA Axioms.
- Documentation Conventions.
- Framework Backlog.
- Framework Changelog.
- Standard metadata specification.
- Stable document identifier convention.
- Standard document lifecycle.
- Repository module numbering convention.

### Changed

- Framework documents reconstructed as the canonical source of truth.
- `framework_version` metadata field renamed to `cda_version`.
- Framework governance formalized through the Framework Backlog.
- Repository adopted as the authoritative source for CDA.

### Removed

- `04_templates.md`.
- Template explanations from the framework documentation.

Templates are now maintained as reusable framework assets rather than framework documentation.

---

# Relationship to the Framework Backlog

The Framework Backlog represents proposed and future improvements.

Once a proposal has been approved and implemented in an official release, its outcome is recorded in this changelog.

The backlog and changelog together provide complete traceability for the framework's evolution.

---

# Maintaining the Changelog

The changelog should only be updated when publishing a new framework release.

Historical release entries should never be modified.

If a correction is required, it should be introduced in a subsequent release rather than editing previous release records.