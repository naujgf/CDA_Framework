---

document_id: FW-001
title: CDA Overview
version: 2.0
status: Approved
cda_version: 2.0
owner: CDA Working Group
last_updated: 2026-07-20

relationships:
derives_from:
constrained_by:
- FW-002
- FW-003
references:
supersedes: FW-002 v1.4
-----------------------

# CDA Overview

## Purpose

Introduce the Capability Documentation Architecture (CDA), explain the problems it addresses, define its scope, and establish the conceptual foundation required to understand the remainder of the framework.

---

# Scope

## Defines

* What CDA is.
* Why CDA exists.
* The objectives of the framework.
* The principles behind the knowledge model.
* The intended audience.
* The overall structure of the framework.

## Does NOT define

* Foundational concepts.
* Core axioms.
* Documentation practices.
* Knowledge Domain specifications.
* Project-specific documentation.

---

# What is CDA?

The **Capability Documentation Architecture (CDA)** is a **Reference Knowledge Model for Software Knowledge**.

Rather than defining how documentation should be written, CDA defines how software knowledge is classified, organized, owned, and related.

The framework provides a conceptual model that identifies the fundamental categories of software knowledge, establishes clear ownership boundaries between them, and enables software knowledge to evolve without ambiguity or unnecessary duplication.

Documentation repositories, knowledge bases, wikis, Markdown files, documentation portals, and AI retrieval systems are implementations of the model rather than the model itself.

CDA is independent of programming languages, software architectures, development methodologies, organizational structures, and documentation technologies.

---

# Why CDA Exists

Software systems generate many different kinds of knowledge throughout their lifecycle.

Business objectives, requirements, domain models, architectures, interface agreements, implementation details, testing strategies, and design decisions are often documented independently, resulting in duplicated information, inconsistent terminology, unclear ownership, and fragmented understanding.

Traditional documentation approaches typically organize information according to documents or folders rather than according to the knowledge itself.

CDA addresses this problem by treating software knowledge as a structured system with explicit categories, clear ownership boundaries, and well-defined relationships.

---

# Framework Objectives

The objectives of CDA are to:

* Provide a common conceptual model for organizing software knowledge.
* Define clear ownership boundaries between different categories of knowledge.
* Reduce ambiguity and unnecessary duplication.
* Improve traceability throughout the software lifecycle.
* Separate stable knowledge from volatile knowledge.
* Enable documentation to evolve without losing conceptual consistency.
* Support knowledge consumption by both humans and intelligent systems.
* Remain independent of documentation technologies and software development methodologies.

---

# Fundamental Principles

The framework is built upon several guiding ideas.

## Software Knowledge Is the Primary Asset

Software systems are ultimately understood through knowledge rather than through source code alone.

Documentation exists to represent software knowledge, but software knowledge exists independently of any document, repository, or documentation technology.

---

## Knowledge Is Organized by Concept Rather Than by Document

CDA organizes software knowledge into conceptual categories known as **Knowledge Domains**.

Each domain represents a distinct category of software knowledge and establishes a clear conceptual boundary for that knowledge.

Documents are simply one possible representation of knowledge and do not determine its ownership.

---

## Every Category of Knowledge Has an Authoritative Owner

Each category of software knowledge belongs to exactly one Knowledge Domain.

Other domains may reference that knowledge, but they do not redefine or duplicate it.

This principle establishes a single source of truth throughout the framework.

---

## Knowledge Evolves Independently of Its Representation

Software knowledge may be represented through Markdown files, diagrams, databases, documentation portals, knowledge graphs, or AI retrieval systems.

The conceptual model defined by CDA remains unchanged regardless of how that knowledge is stored or presented.

---

## The Framework Evolves Through Governance

CDA evolves through a controlled and transparent process.

Framework improvements are proposed, reviewed, approved, and incorporated into official releases while preserving the stability of the underlying conceptual model.

---

# Intended Audience

CDA is intended for:

* Software architects.
* Technical leaders.
* Software engineers.
* Documentation engineers.
* Enterprise architects.
* AI-assisted software development workflows.
* Teams building long-lived software systems.
* Organizations seeking consistent software knowledge management.

---

# Framework Structure

The framework is organized into two complementary parts.

## Framework

The Framework defines the conceptual foundation of CDA, including:

* Overview
* Foundational Concepts
* Core Axioms
* Documentation Practices
* Templates
* Framework Governance

---

## Knowledge Domains

The Knowledge Domains define the major categories of software knowledge:

* Foundation
* Requirements
* Domain
* Architecture
* Components
* Contracts
* Data
* Implementation
* Testing
* Decision Records

Each Knowledge Domain answers one irreducible question about a software system and collectively they form a complete model of software knowledge.

---

# Relationship with Projects

CDA is independent of any individual software project.

Projects adopt a particular version of the framework and organize their software knowledge according to its concepts, axioms, and Knowledge Domains.

Individual repositories may implement CDA using different documentation structures or technologies while remaining conceptually consistent with the framework.

Projects indicate the framework version they conform to through the `cda_version` metadata field.

---

# Relationship with Documentation

CDA does not prescribe a particular documentation technology or repository structure.

Instead, it provides the conceptual model that documentation should represent.

Documents, directories, repositories, knowledge bases, and documentation platforms are implementation choices that exist to capture and communicate software knowledge.

---

# Next Reading

After understanding the purpose and scope of CDA, continue with:

1. Foundational Concepts
2. Core Axioms
3. Documentation Practices
4. Foundation Knowledge Domain
