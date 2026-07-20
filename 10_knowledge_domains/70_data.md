# Data Knowledge Domain

| Attribute  | Value             |
| ---------- | ----------------- |
| Domain     | Data              |
| Identifier | KD-70             |
| Version    | 1.0.0             |
| Status     | Stable            |
| Layer      | CDA Standard      |
| Parent     | Knowledge Domains |

---

# Purpose

The Data Knowledge Domain defines the information managed by the software solution.

It describes the structure, meaning, relationships, lifecycle and governance of information independently of storage technologies or implementation details.

The Data Knowledge Domain provides a consistent understanding of the information exchanged, processed and persisted throughout the system.

---

# Primary Question

> **What information is managed?**

Every artifact belonging to the Data Knowledge Domain should contribute to answering this question.

---

# Objectives

The Data Knowledge Domain exists to:

* Define the information managed by the system.
* Describe relationships between information entities.
* Establish shared data definitions.
* Document information lifecycle and ownership.
* Promote consistency across APIs, components and implementations.
* Remain independent of storage technologies.

---

# Core Concepts

The Data Knowledge Domain is organized around five conceptual areas.

## Information Model

Defines the information managed by the solution.

---

## Relationships

Defines how information entities relate to one another.

---

## Lifecycle

Defines how information is created, modified, retained and removed.

---

## Ownership

Defines responsibility for creating and maintaining information.

---

## Governance

Defines rules that ensure information quality, consistency and integrity.

---

# Knowledge Responsibilities

The Data Knowledge Domain is responsible for documenting the following categories of knowledge.

## Information Model

Describe the information entities managed by the solution.

Typical knowledge includes:

* Information entities
* Attributes
* Identifiers
* Relationships
* Cardinality

The focus is on information semantics rather than physical storage.

---

## Information Definitions

Document the meaning of information.

Examples include:

* Business definitions
* Attribute descriptions
* Allowed values
* Validation rules
* Units of measurement

Every important piece of information should have an unambiguous definition.

---

## Information Lifecycle

Describe how information evolves over time.

Typical knowledge includes:

* Creation
* Updates
* Archival
* Deletion
* Retention
* Versioning

Lifecycle describes information behavior rather than database operations.

---

## Ownership

Document who owns each information entity.

Examples include:

* Producing components
* Consuming components
* Source of truth
* Stewardship

Ownership promotes consistency across the solution.

---

## Information Governance

Document rules that maintain information quality.

Typical knowledge includes:

* Naming conventions
* Validation rules
* Privacy classifications
* Sensitivity levels
* Integrity constraints
* Data quality expectations

Governance applies regardless of storage technology.

---

# Characteristics

Knowledge contained within this domain should exhibit the following characteristics.

## Technology Independent

Information definitions should not depend on storage technologies.

---

## Consistent

The same information should have the same meaning across the solution.

---

## Traceable

Information should be traceable to business concepts and requirements.

---

## Durable

Information definitions should evolve more slowly than implementation technologies.

---

## Shared

Information models should provide a common understanding across teams.

---

# Relationships

## Depends On

* Foundation
* Requirements
* Domain
* Architecture
* Components
* API

The Data Knowledge Domain defines the information exchanged through APIs and managed by components.

---

## Provides Context To

* Implementation
* Testing
* Decision Records

---

# Reference Artifacts

The CDA Standard recommends the following artifacts for representing Data knowledge.

## Required

| Artifact          | Purpose                             |
| ----------------- | ----------------------------------- |
| Data Index        | Entry point for Data documentation. |
| Information Model | Defines the managed information.    |

---

## Recommended

| Artifact           | Purpose                                |
| ------------------ | -------------------------------------- |
| Data Dictionary    | Defines entities and attributes.       |
| Relationship Model | Documents information relationships.   |
| Lifecycle Model    | Describes information evolution.       |
| Governance Guide   | Documents ownership and quality rules. |

---

## Optional

| Artifact               | Purpose                                         |
| ---------------------- | ----------------------------------------------- |
| Canonical Data Model   | Defines enterprise-wide information structures. |
| Reference Data Catalog | Documents controlled vocabularies.              |
| Privacy Classification | Defines sensitivity levels.                     |
| Retention Policy       | Documents information retention requirements.   |

Projects may organize these artifacts according to their needs.

The CDA Standard defines knowledge responsibilities rather than mandatory document structures.

---

# Out of Scope

The Data Knowledge Domain should not contain:

* Database schemas
* SQL scripts
* Table definitions
* Indexes
* ORM mappings
* Migration scripts
* Storage engines
* Cache implementations
* Database configuration
* Physical persistence strategies

These belong to the Implementation Knowledge Domain.

---

# Evolution

The Data Knowledge Domain evolves as business information changes.

Typical reasons for updates include:

* New information entities.
* Changes in business terminology.
* Regulatory requirements.
* New governance policies.
* Information lifecycle refinement.

Changes should preserve consistency across APIs, Components and the Domain model.

---

# Conformance

A project conforms to the Data Knowledge Domain if it:

* Documents the required knowledge responsibilities.
* Defines information independently of storage technologies.
* Maintains consistent information definitions across the solution.
* Documents ownership and lifecycle of managed information.
* Separates information semantics from implementation details.

Conformance is evaluated based on the quality and completeness of the documented knowledge rather than the number or names of documents.

---

# Implementation Guidance

This specification defines **what knowledge belongs** to the Data Knowledge Domain.

It intentionally does **not** prescribe a mandatory document structure.

Reference templates for implementing this knowledge domain are provided separately in the `20_templates` section of the CDA repository.

Concrete software projects remain free to organize, merge or split documents according to their needs, provided the knowledge responsibilities defined by this specification are fulfilled.
