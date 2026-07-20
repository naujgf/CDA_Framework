---

document_id: FW-000
title: Framework Index
version: 2.0
status: Approved
cda_version: 2.0
owner: CDA Working Group
last_updated: 2026-07-20

relationships:
derives_from:
constrained_by:
references:
supersedes: FW-001 v1.4
-----------------------

# Framework Index

## Purpose

Provide the entry point to the Capability Documentation Architecture (CDA) framework and guide readers through the documents that define the framework, its theoretical foundations, and its implementation guidelines.

The Framework module contains the normative definition of CDA as a **Reference Knowledge Model for Software Knowledge**. It defines the concepts, principles, and rules that govern the organization and ownership of software knowledge independently of technologies, documentation tools, or development methodologies.

---

# Scope of This Document

## Defines

* The structure of the Framework module.
* The purpose of each framework document.
* The recommended reading order for understanding CDA.
* The relationship between the framework documents.

## Does NOT define

* Individual Knowledge Domains.
* Project-specific documentation.
* Software architecture.
* Business requirements.
* Implementation details.

---

# Framework Documents

| Order | Document                          | Purpose                                                                                                                                                               |
| ----: | --------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|    00 | `00_index.md`                     | Entry point to the Framework module.                                                                                                                                  |
|    01 | `01_cda_overview.md`              | Introduces CDA, its vision, scope, terminology, and positioning as a Reference Knowledge Model.                                                                       |
|    02 | `02_foundational_concepts.md`     | Defines the fundamental concepts used throughout the framework, including Software Knowledge, Knowledge Domains, Ownership, Boundaries, References, and Participants. |
|    03 | `03_axioms.md`                    | Defines the immutable principles and axioms governing the framework.                                                                                                  |
|    04 | `04_documentation_conventions.md` | Specifies standards for writing, organizing, and maintaining documentation while preserving knowledge ownership.                                                      |
|    05 | `05_templates.md`                 | Contains reusable document templates used throughout CDA.                                                                                                             |
|    06 | `06_framework_backlog.md`         | Tracks proposed, approved, deferred, and rejected framework improvements.                                                                                             |
|    07 | `07_framework_changelog.md`       | Records the evolution of the framework across released versions.                                                                                                      |

---

# Recommended Reading Order

Readers new to CDA should follow this sequence:

1. CDA Overview
2. Foundational Concepts
3. CDA Axioms
4. Documentation Conventions
5. Templates
6. Framework Backlog
7. Framework Changelog

Each document builds upon the concepts introduced by the previous ones, progressing from theory to practical application.

---

# Framework Responsibilities

The Framework module defines the rules that govern CDA itself.

Specifically, it defines:

* the conceptual model;
* the vocabulary;
* the core principles;
* the ownership model;
* documentation conventions;
* reusable templates;
* the evolution process of the framework.

The Framework module intentionally does **not** define the knowledge owned by individual Knowledge Domains. Those definitions belong to their respective modules.

---

# Module Evolution

The Framework evolves independently from projects that adopt CDA.

Changes are proposed, reviewed, and approved through the Framework Backlog and become part of an official CDA release when incorporated into the Framework Changelog.

Projects adopting CDA should specify the framework version they conform to using the `cda_version` metadata field.

---

# Related Modules

Once the Framework has been understood, continue with the Knowledge Domains:

* `10_foundation/`
* `20_requirements/`
* `30_domain/`
* `40_architecture/`
* `50_components/`
* `60_contracts/`
* `70_data/`
* `80_implementation/`
* `90_testing/`
* `100_decision_records/`

---

# Maintenance

The Framework module should evolve conservatively.

Changes affecting terminology, ownership rules, Knowledge Domains, or foundational concepts should be considered framework-level changes and follow the official framework evolution process before being adopted by projects.
