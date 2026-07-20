---

document_id: FW-006
title: Framework Changelog
version: 2.0
status: Approved
cda_version: 2.0
owner: CDA Working Group
last_updated: 2026-07-20

relationships:
derives_from:
constrained_by:
references:
- FW-005
supersedes: FW-006 v1.4
-----------------------

# Framework Changelog

## Purpose

Record the official release history of the Capability Documentation Architecture (CDA).

Each release documents the changes incorporated into the official specification of the CDA Reference Knowledge Model and provides the authoritative history of the framework's evolution.

---

# Scope

## Defines

* Official framework releases.
* Released framework changes.
* Framework version progression.
* Historical evolution of the reference model.

## Does NOT define

* Proposed changes.
* Future work.
* Project-specific changelogs.
* Design rationale for unreleased changes.

---

# Relationship to the Framework

The Framework Backlog records proposed changes.

The Framework Changelog records changes that have been approved, implemented, and published as part of an official CDA release.

Together they provide complete traceability of the framework's evolution.

---

# Release Policy

Only officially released changes appear in this document.

Every release represents a stable version of the Capability Documentation Architecture.

Changes under discussion remain in the Framework Backlog until they are approved and incorporated into an official release.

---

# Versioning Policy

CDA follows Semantic Versioning principles.

## Major Releases

Major versions introduce changes to the conceptual foundation of the framework.

Examples include:

* modifications to Foundational Concepts;
* modifications to Core Axioms;
* changes to Knowledge Domain boundaries;
* changes affecting conceptual ownership or the reference knowledge model.

These releases may require existing CDA implementations to be reviewed or updated.

---

## Minor Releases

Minor versions introduce new capabilities while preserving conceptual compatibility.

Examples include:

* new Documentation Practices;
* additional templates;
* new governance mechanisms;
* new Knowledge Domains that do not alter existing ownership boundaries;
* backward-compatible improvements to the framework.

---

## Patch Releases

Patch versions introduce editorial improvements without changing the meaning of the framework.

Examples include:

* wording improvements;
* examples;
* formatting;
* typo corrections;
* clarifications.

---

# Release History

## Version 2.0

Release Date: 2026-07-20

### Added

* Foundational Concepts as a new foundational framework document.
* Reference Knowledge Model as the conceptual definition of CDA.
* Knowledge Item as the fundamental unit of software knowledge.
* Knowledge Domain as the authoritative owner of software knowledge.
* Explicit ownership boundaries between Knowledge Domains.
* Knowledge reuse through references as a core architectural principle.
* Governance model for evolving the conceptual framework.

### Changed

* Repositioned CDA from a documentation framework to a Reference Knowledge Model for Software Knowledge.
* Reorganized the framework into four foundational documents:

  * Overview
  * Foundational Concepts
  * Core Axioms
  * Documentation Practices
* Replaced document-centric principles with knowledge-centric principles.
* Redefined the Core Axioms around software knowledge ownership, boundaries, references, and conceptual organization.
* Updated Documentation Practices to reflect conceptual ownership rather than document organization.
* Expanded framework governance to classify changes by type and impact.

### Removed

* Documentation-centric interpretation of CDA.
* Document ownership as an implicit organizing principle.
* Capability-oriented organization as a universal framework principle.

---

## Version 1.4

Release Date: 2026-07-17

### Added

* Canonical Framework module.
* CDA Overview.
* CDA Axioms.
* Documentation Conventions.
* Framework Backlog.
* Framework Changelog.
* Standard metadata specification.
* Stable document identifier convention.
* Standard document lifecycle.
* Repository module numbering convention.

### Changed

* Framework documents reconstructed as the canonical source of truth.
* `framework_version` metadata field renamed to `cda_version`.
* Framework governance formalized through the Framework Backlog.
* Repository adopted as the authoritative source for CDA.

### Removed

* `04_templates.md`.
* Template explanations from the framework documentation.

Templates are maintained as reusable framework assets rather than framework documentation.

---

# Maintaining the Changelog

The changelog should be updated only when publishing an official framework release.

Released entries represent historical records and should not be modified.

If a correction to a previous release is required, it should be documented in a subsequent release rather than altering historical records.

---

# Evolution

As CDA evolves, this changelog provides the authoritative record of how the reference knowledge model has changed over time.

Every released version should correspond to one or more completed Framework Evolution items recorded in the Framework Backlog.
