# Foundation Knowledge Domain

| Attribute | Value |
|----------|-------|
| Domain | Foundation |
| Identifier | KD-10 |
| Version | 1.0.0 |
| Status | Stable |
| Layer | CDA Standard |
| Parent | Knowledge Domains |

---

# Purpose

The Foundation Knowledge Domain defines the stable, high-level knowledge that establishes the identity and context of a software project.

It provides the conceptual foundation upon which every other knowledge domain is built.

The information contained within this domain should remain relatively stable throughout the lifetime of a project and should be understandable by both technical and non-technical stakeholders.

Foundation describes **what the project is**, not **how it is implemented**.

---

# Primary Question

> **What is this software project?**

Every artifact belonging to the Foundation domain should contribute to answering this question.

---

# Objectives

The Foundation Knowledge Domain exists to:

- Establish the identity of the project.
- Define its purpose and long-term vision.
- Describe its scope and boundaries.
- Capture the enduring principles that guide the project.
- Establish a common language across stakeholders.
- Provide the conceptual context required by every other knowledge domain.

---

# Core Concepts

The Foundation domain is organized around five conceptual areas.

## Identity

Defines what the project is and why it exists.

---

## Scope

Defines the boundaries of the project.

---

## Principles

Defines the enduring beliefs that guide future decisions.

---

## Language

Defines the canonical terminology used throughout the documentation.

---

## Navigation

Defines how stakeholders discover and consume the project's documentation.

---

# Knowledge Responsibilities

The Foundation Knowledge Domain is responsible for documenting the following categories of knowledge.

## Project Identity

Capture the project's identity and long-term purpose.

Typical knowledge includes:

- Vision
- Mission
- Purpose
- Strategic objectives

---

## Project Scope

Define the boundaries of the project.

Typical knowledge includes:

- In scope
- Out of scope
- Assumptions
- Constraints
- Intended audience

---

## Guiding Principles

Capture the enduring principles that influence future decisions.

Examples include:

- Product philosophy
- Engineering philosophy
- Design philosophy
- Quality principles

These represent long-lived beliefs rather than implementation decisions.

---

## Shared Language

Define the canonical terminology used across the project.

Typical knowledge includes:

- Ubiquitous language
- Glossary
- Acronyms
- Business terminology

This responsibility ensures that all stakeholders interpret concepts consistently.

---

## Documentation Navigation

Provide guidance for discovering and consuming project documentation.

Typical knowledge includes:

- Documentation index
- Reading paths
- Audience guides
- Learning paths

---

# Characteristics

Knowledge contained within this domain should exhibit the following characteristics.

## Stable

Changes infrequently during the lifetime of the project.

## Conceptual

Describes the project rather than its implementation.

## Technology Independent

Independent of programming languages, frameworks, databases or infrastructure.

## Stakeholder Friendly

Understandable by both technical and non-technical audiences.

## Foundational

Provides context for every remaining knowledge domain.

---

# Relationships

## Provides Context To

- Requirements
- Domain
- Architecture
- Components
- API
- Data
- Implementation
- Decision Records
- Testing

---

## Depends On

None.

Foundation represents the highest abstraction level within the CDA Standard.

---

# Reference Artifacts

The CDA Standard recommends the following artifacts for representing Foundation knowledge.

## Required

| Artifact | Purpose |
|----------|---------|
| Documentation Index | Entry point for the Foundation documentation. |

---

## Recommended

| Artifact | Purpose |
|----------|---------|
| Project Vision | Defines the long-term aspiration of the project. |
| Product Scope | Defines the project boundaries. |
| Design Philosophy | Captures the principles guiding design decisions. |
| Guiding Principles | Defines enduring project beliefs. |

---

## Optional

| Artifact | Purpose |
|----------|---------|
| Glossary | Defines canonical terminology. |
| Ubiquitous Language | Establishes a shared vocabulary. |
| Reading Paths | Suggests documentation consumption paths. |
| Frequently Asked Questions | Answers recurring conceptual questions. |
| Project Background | Provides historical and business context. |

Projects may merge, split or omit these artifacts according to their size and complexity.

The CDA Standard defines **knowledge responsibilities**, not mandatory document structures.

---

# Out of Scope

The Foundation Knowledge Domain should not contain:

- Functional requirements
- User stories
- Business rules
- Domain models
- Architecture
- Component specifications
- API contracts
- Database schemas
- Infrastructure
- Implementation details
- Testing strategies

These belong to other knowledge domains.

---

# Evolution

The Foundation Knowledge Domain evolves slowly.

Typical reasons for updates include:

- Significant changes in product vision.
- Changes in project scope.
- Organizational strategy changes.
- Fundamental terminology revisions.

Routine implementation changes should not require modifications to Foundation documentation.

---

# Implementation Guidance

This specification defines **what knowledge belongs** to the Foundation domain.

It intentionally does **not** prescribe a mandatory document structure.

Reference templates for implementing this knowledge domain are provided separately in the `20_templates` section of the CDA repository.

Concrete software projects remain free to organize, merge or split documents according to their needs, provided the knowledge responsibilities defined by this specification are fulfilled.

# Conformance

A project conforms to the Foundation Knowledge Domain if it:

- Documents all required knowledge responsibilities.
- Maintains a navigable entry point for Foundation documentation.
- Separates Foundation knowledge from other knowledge domains.
- Keeps Foundation documentation implementation-independent.

The CDA Standard evaluates conformance based on the presence and quality of knowledge, not on the number or names of documents.