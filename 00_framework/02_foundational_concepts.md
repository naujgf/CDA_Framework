---

document_id: FW-002
title: Foundational Concepts
version: 2.0
status: Draft
cda_version: 2.0
owner: CDA Working Group
last_updated: 2026-07-20

relationships:
derives_from:
constrained_by:
- FW-003
references:
- FW-001
supersedes:
-----------

# Foundational Concepts

## Purpose

Define the fundamental concepts and terminology used throughout the Capability Documentation Architecture (CDA).

These concepts establish the common vocabulary required to understand the framework. They describe *what* the core entities are, while the Framework Axioms define *how* they behave and relate to one another.

---

# Scope

## Defines

* Core CDA terminology.
* Fundamental software knowledge concepts.
* The conceptual entities referenced by all Knowledge Domains.

## Does NOT define

* Framework rules.
* Ownership constraints.
* Documentation practices.
* Knowledge Domain specifications.

---

# Software Knowledge

**Software Knowledge** is any persistent information required to understand, justify, construct, verify, operate, or evolve a software system.

Software knowledge exists independently of the documents, repositories, tools, or technologies used to represent it.

Examples include business objectives, requirements, architectural structures, interface agreements, implementation strategies, testing approaches, and design decisions.

---

# Knowledge Item

A **Knowledge Item** is the smallest meaningful unit of software knowledge that can be owned, referenced, maintained, and evolved independently.

A Knowledge Item may consist of a statement, definition, rule, model, diagram, specification, decision, or any other discrete piece of information.

Knowledge Items are conceptual entities rather than physical documents.

---

# Knowledge Domain

A **Knowledge Domain** is a conceptual category that groups software knowledge according to its nature and purpose.

Each Knowledge Domain represents a distinct category of software knowledge and defines the conceptual boundary within which that knowledge belongs.

Knowledge Domains organize knowledge independently of documentation structure, implementation technology, or project organization.

---

# Ownership

**Ownership** is the relationship between a Knowledge Domain and the software knowledge for which it is the authoritative source.

Ownership identifies where a piece of knowledge is defined and maintained.

Ownership is a conceptual property and is independent of where the corresponding documentation is physically stored.

---

# Reference

A **Reference** is a relationship through which one Knowledge Domain uses knowledge owned by another without duplicating or redefining it.

References preserve consistency by allowing knowledge to be reused while maintaining a single authoritative definition.

---

# Boundary

A **Boundary** defines the limits of a Knowledge Domain by distinguishing the knowledge that belongs to the domain from the knowledge that belongs elsewhere.

Boundaries provide conceptual separation between Knowledge Domains and establish clear ownership responsibilities.

---

# Participant

A **Participant** is any independent entity that produces, consumes, exchanges, or acts upon software knowledge or system behavior.

Depending on context, a participant may represent:

* a software component;
* a service;
* an application;
* an external system;
* a user;
* an organization;
* an automated agent;
* an AI agent;
* any other independently acting entity.

Participants interact through explicit or implicit contracts.

---

# Capability

A **Capability** is a coherent ability provided by a software system that delivers value to one or more stakeholders through the collaboration of multiple software elements.

Capabilities represent *what* a system enables rather than *how* that ability is implemented.

Multiple Knowledge Domains collectively describe a capability from different perspectives.

---

# Document

A **Document** is a physical representation of one or more Knowledge Items.

Documents are implementation artifacts used to record software knowledge.

A document is not software knowledge itself; it is merely one possible representation of that knowledge.

The same Knowledge Item may be represented in different document formats without changing its meaning.

---

# Repository

A **Repository** is a physical organization of documentation artifacts.

Repositories provide storage and navigation but do not determine knowledge ownership.

The organization of files, folders, or documentation platforms is considered an implementation detail of the framework.

---

# Relationship

A **Relationship** describes an explicit connection between two conceptual entities within the framework.

Relationships express dependency, reference, derivation, constraint, or other meaningful associations while preserving the independent identity of each entity.

---

# Conceptual Hierarchy

The Capability Documentation Architecture organizes software knowledge according to the following conceptual hierarchy:

```text
Software Knowledge
        │
        ▼
Knowledge Domain
        │
        ▼
Knowledge Item
        │
        ▼
Document
        │
        ▼
Repository
```

This hierarchy separates conceptual entities from their physical representations.

Software knowledge exists independently of the documents and repositories used to record it.

---

# Summary

The concepts defined in this document provide the vocabulary used throughout CDA.

Subsequent framework documents build upon these concepts by defining the immutable principles, documentation practices, Knowledge Domains, and implementation guidance that collectively form the Capability Documentation Architecture.
