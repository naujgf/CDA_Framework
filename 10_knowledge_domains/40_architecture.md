# Architecture Knowledge Domain

| Attribute  | Value             |
| ---------- | ----------------- |
| Domain     | Architecture      |
| Identifier | KD-40             |
| Version    | 1.0.0             |
| Status     | Stable            |
| Layer      | CDA Standard      |
| Parent     | Knowledge Domains |

---

# Purpose

The Architecture Knowledge Domain defines the high-level organization of the software solution.

It describes how the solution is structured into major architectural elements, how those elements interact, and the architectural principles that guide the overall design.

The Architecture Knowledge Domain translates the business intent captured in previous knowledge domains into a coherent solution structure while remaining independent of implementation details.

---

# Primary Question

> **How is the solution organized?**

Every artifact belonging to the Architecture Knowledge Domain should contribute to answering this question.

---

# Objectives

The Architecture Knowledge Domain exists to:

* Define the overall structure of the solution.
* Identify the major architectural building blocks.
* Describe interactions between architectural elements.
* Communicate architectural styles and patterns.
* Capture system-wide architectural decisions.
* Provide a stable blueprint for component design and implementation.

---

# Core Concepts

The Architecture Knowledge Domain is organized around five conceptual areas.

## Structure

Defines the major architectural elements and their organization.

---

## Interactions

Defines how architectural elements collaborate.

---

## Boundaries

Defines the separation of responsibilities between architectural areas.

---

## Architectural Principles

Defines the rules that govern the architecture.

---

## Architectural Views

Defines different perspectives used to communicate the architecture.

---

# Knowledge Responsibilities

The Architecture Knowledge Domain is responsible for documenting the following categories of knowledge.

## System Structure

Describe the major structural elements of the solution.

Typical knowledge includes:

* Systems
* Subsystems
* Layers
* Services
* Modules
* Containers

The focus is on architectural organization rather than internal implementation.

---

## Architectural Relationships

Describe how architectural elements communicate and depend on one another.

Examples include:

* Dependencies
* Communication paths
* Data flow
* Control flow
* Integration points

---

## Architectural Style

Document the architectural style adopted by the project.

Examples include:

* Layered Architecture
* Hexagonal Architecture
* Clean Architecture
* Event-Driven Architecture
* Microservices
* Modular Monolith

The selected style should explain the overall organization of the solution rather than technology choices.

---

## Architectural Principles

Document the principles that guide architectural decisions.

Examples include:

* Separation of concerns
* Loose coupling
* High cohesion
* Dependency inversion
* Scalability
* Resilience
* Security by design

---

## Architectural Views

Provide different perspectives of the solution.

Typical views include:

* System Context
* Container View
* Logical View
* Deployment View
* Integration View

Projects may adopt additional viewpoints as needed.

---

# Characteristics

Knowledge contained within this domain should exhibit the following characteristics.

## High-Level

Focuses on the overall organization of the solution rather than implementation details.

---

## Technology-Aware

Architecture may reference technologies where they influence structural decisions, but should not document implementation details.

---

## Stable

Architecture should evolve more slowly than individual components.

---

## Coherent

Architectural decisions should support the project's requirements and domain model.

---

## Communicative

Architecture should provide a clear mental model of the solution for all technical stakeholders.

---

# Relationships

## Depends On

* Foundation
* Requirements
* Domain

Architecture translates business understanding into a solution structure.

---

## Provides Context To

* Components
* API
* Data
* Implementation
* Decision Records
* Testing

---

# Reference Artifacts

The CDA Standard recommends the following artifacts for representing Architecture knowledge.

## Required

| Artifact            | Purpose                                     |
| ------------------- | ------------------------------------------- |
| Architecture Index  | Entry point for Architecture documentation. |
| System Architecture | Defines the overall solution structure.     |

---

## Recommended

| Artifact                 | Purpose                                  |
| ------------------------ | ---------------------------------------- |
| System Context Diagram   | Shows the system within its environment. |
| Container Diagram        | Defines major runtime building blocks.   |
| Integration Architecture | Describes communication between systems. |
| Architectural Principles | Documents guiding architectural rules.   |

---

## Optional

| Artifact             | Purpose                                                       |
| -------------------- | ------------------------------------------------------------- |
| Deployment View      | Describes physical deployment topology.                       |
| Logical View         | Represents logical organization.                              |
| Sequence Diagrams    | Illustrates significant architectural interactions.           |
| Network Topology     | Documents infrastructure communication.                       |
| Technology Landscape | Summarizes major technologies where architecturally relevant. |

Projects may organize these artifacts according to their needs.

The CDA Standard defines knowledge responsibilities rather than mandatory document structures.

---

# Out of Scope

The Architecture Knowledge Domain should not contain:

* Component internals
* Class diagrams
* Package structures
* Source code
* Algorithms
* Database schemas
* API endpoint definitions
* Configuration files
* Infrastructure scripts
* Deployment automation

These belong to downstream knowledge domains.

---

# Evolution

The Architecture Knowledge Domain evolves as the solution grows and architectural needs change.

Typical reasons for updates include:

* Significant changes in system structure.
* Introduction of new architectural styles.
* New integration patterns.
* Scalability or resilience improvements.
* Major technology shifts affecting architectural organization.

Architectural changes should be traceable through Architecture Decision Records when appropriate.

---

# Conformance

A project conforms to the Architecture Knowledge Domain if it:

* Documents the required knowledge responsibilities.
* Clearly defines the major architectural elements of the solution.
* Describes relationships between architectural elements.
* Separates architecture from implementation details.
* Maintains architectural consistency with the Foundation, Requirements and Domain knowledge.

Conformance is evaluated based on the quality and completeness of the documented knowledge rather than the number or names of documents.

---

# Implementation Guidance

This specification defines **what knowledge belongs** to the Architecture Knowledge Domain.

It intentionally does **not** prescribe a mandatory document structure.

Reference templates for implementing this knowledge domain are provided separately in the `20_templates` section of the CDA repository.

Concrete software projects remain free to organize, merge or split documents according to their needs, provided the knowledge responsibilities defined by this specification are fulfilled.
