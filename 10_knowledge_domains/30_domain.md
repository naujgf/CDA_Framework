# Domain Knowledge Domain

| Attribute | Value |
|----------|-------|
| Domain | Domain |
| Identifier | KD-30 |
| Version | 1.0.0 |
| Status | Stable |
| Layer | CDA Standard |
| Parent | Knowledge Domains |

---

# Purpose

The Domain Knowledge Domain defines the concepts, terminology, rules and relationships that exist within the problem space addressed by the software project.

It captures **the reality the software models**, independent of architecture, technology or implementation.

The Domain Knowledge Domain establishes a shared understanding of the business or operational environment in which the software exists.

---

# Primary Question

> **What reality does this software model?**

Every artifact belonging to the Domain Knowledge Domain should contribute to answering this question.

---

# Objectives

The Domain Knowledge Domain exists to:

- Define the fundamental concepts of the business domain.
- Establish a common language for stakeholders.
- Describe relationships between domain concepts.
- Capture business rules and invariants.
- Provide a stable conceptual model that guides architecture and implementation.
- Reduce ambiguity across the project.

---

# Core Concepts

The Domain Knowledge Domain is organized around five conceptual areas.

## Concepts

The primary entities and ideas that exist within the domain.

---

## Relationships

How domain concepts interact and relate to one another.

---

## Business Rules

The rules, constraints and invariants that govern the domain.

---

## Processes

The significant business workflows and lifecycle transitions that occur within the domain.

---

## Ubiquitous Language

The canonical vocabulary shared by all stakeholders.

---

# Knowledge Responsibilities

The Domain Knowledge Domain is responsible for documenting the following categories of knowledge.

## Domain Concepts

Define the fundamental concepts that exist within the problem space.

Typical knowledge includes:

- Entities
- Value Objects
- Aggregates
- Events
- Actors
- Resources

These represent business concepts rather than software classes.

---

## Relationships

Describe how domain concepts relate to each other.

Examples include:

- Ownership
- Composition
- Associations
- Dependencies
- Cardinality

Relationships describe the business reality, not the database structure.

---

## Business Rules

Document the rules that govern domain behavior.

Examples include:

- Validation rules
- Eligibility rules
- Lifecycle constraints
- Invariants
- Policies

Business rules should remain independent of implementation.

---

## Domain Processes

Describe significant business workflows and lifecycle transitions.

Typical knowledge includes:

- Business processes
- State transitions
- Event flows
- Responsibilities

These represent business operations rather than software workflows.

---

## Ubiquitous Language

Maintain the canonical terminology used across the project.

The same concept should always be referred to using the same name.

This vocabulary should be shared by business experts, developers, testers and stakeholders.

---

# Characteristics

Knowledge contained within this domain should exhibit the following characteristics.

## Technology Independent

The domain exists independently of software implementation.

---

## Business Centric

The domain reflects the real-world problem space rather than technical solutions.

---

## Stable

Domain concepts typically evolve more slowly than software implementations.

---

## Consistent

The same concepts and terminology should be used throughout the project.

---

## Expressive

The documentation should accurately represent the language used by domain experts.

---

# Relationships

## Depends On

- Foundation
- Requirements

The domain provides the conceptual model required to satisfy project requirements.

---

## Provides Context To

- Architecture
- Components
- API
- Data
- Implementation
- Decision Records
- Testing

---

# Reference Artifacts

The CDA Standard recommends the following artifacts for representing Domain knowledge.

## Required

| Artifact | Purpose |
|----------|---------|
| Domain Index | Entry point for Domain documentation. |
| Domain Model | Defines the primary concepts and relationships. |

---

## Recommended

| Artifact | Purpose |
|----------|---------|
| Business Rules | Captures domain constraints and invariants. |
| Domain Processes | Describes significant workflows. |
| Ubiquitous Language | Defines canonical terminology. |
| Context Map | Defines relationships between bounded contexts (when applicable). |

---

## Optional

| Artifact | Purpose |
|----------|---------|
| State Diagrams | Describe lifecycle transitions. |
| Event Catalog | Documents domain events. |
| Decision Tables | Formalize business rules. |
| Domain Glossary | Supplements shared terminology. |
| Personas | Represents domain actors. |

Projects may organize these artifacts according to their needs.

The CDA Standard defines knowledge responsibilities rather than mandatory document structures.

---

# Out of Scope

The Domain Knowledge Domain should not contain:

- Software architecture
- Component decomposition
- API contracts
- Database schemas
- Class diagrams
- Framework selection
- Deployment strategies
- Source code
- Infrastructure
- Technical implementation details

These belong to downstream knowledge domains.

---

# Evolution

The Domain Knowledge Domain evolves as the understanding of the business evolves.

Typical reasons for updates include:

- New business concepts.
- Regulatory changes.
- Business process evolution.
- Discovery of previously unknown domain knowledge.
- Refinement of terminology.

Changes to the domain should be reflected consistently across dependent knowledge domains.

---

# Conformance

A project conforms to the Domain Knowledge Domain if it:

- Documents the required knowledge responsibilities.
- Maintains a consistent ubiquitous language.
- Separates business concepts from software implementation.
- Captures domain rules independently of technical solutions.
- Represents the problem space rather than the solution.

Conformance is evaluated based on the quality and completeness of the documented knowledge rather than the number or names of documents.

---

# Implementation Guidance

This specification defines **what knowledge belongs** to the Domain Knowledge Domain.

It intentionally does **not** prescribe a mandatory document structure.

Reference templates for implementing this knowledge domain are provided separately in the `20_templates` section of the CDA repository.

Concrete software projects remain free to organize, merge or split documents according to their needs, provided the knowledge responsibilities defined by this specification are fulfilled.