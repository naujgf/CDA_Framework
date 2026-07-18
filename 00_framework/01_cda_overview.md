---
document_id: FW-002
title: CDA Overview
version: 1.4
status: Approved
cda_version: 1.4
owner: CDA Working Group
last_updated: 2026-07-17

relationships:
  derives_from:
  constrained_by:
  references:
    - FW-003
    - FW-004
  supersedes:
---

# CDA Overview

## Purpose

Introduce the Capability Documentation Architecture (CDA), explain the problems it addresses, define its scope, and provide the conceptual foundation required to understand the rest of the framework.

## Scope of This Document

### Defines

- What CDA is.
- Why CDA exists.
- The objectives of the framework.
- The core concepts behind the framework.
- The intended audience.

### Does NOT define

- Framework axioms.
- Documentation conventions.
- Module specifications.
- Project-specific documentation.

---

# What is CDA?

Capability Documentation Architecture (CDA) is a documentation framework designed to organize software knowledge into a structured, scalable and maintainable architecture.

Rather than treating documentation as a collection of disconnected files, CDA treats documentation as a knowledge system. Every document has a clear purpose, every module answers a specific set of questions, and the complete documentation forms a coherent architecture that can evolve alongside the software it describes.

CDA is technology-agnostic and can be applied to projects of different sizes, domains and implementation technologies.

---

# Why CDA Exists

Traditional documentation often suffers from common problems:

- Information is duplicated across documents.
- Documentation becomes outdated as projects evolve.
- Architectural decisions are difficult to trace.
- Knowledge is scattered throughout repositories.
- AI assistants receive inconsistent or incomplete context.
- New contributors struggle to understand where information belongs.

CDA addresses these problems by providing a consistent architectural model for documentation.

---

# Framework Objectives

The objectives of CDA are to:

- Organize documentation as a coherent knowledge architecture.
- Separate stable knowledge from implementation details.
- Improve traceability across the software lifecycle.
- Reduce duplication and ambiguity.
- Support incremental evolution of documentation.
- Provide predictable navigation for both humans and AI assistants.
- Enable documentation to scale together with the software it describes.

---

# Core Concepts

The framework is built around several fundamental concepts.

## Knowledge as a First-Class Asset

Knowledge is the primary asset managed by CDA.

Documentation is the medium through which knowledge is captured, organized and communicated.

The architecture exists to preserve the integrity, discoverability and evolution of that knowledge.

---

## Documentation as Architecture

Documentation is not viewed as a folder containing documents.

Instead, documentation is organized as an architecture composed of modules, relationships and well-defined responsibilities.

Each module addresses a distinct aspect of software knowledge.

---

## Capability-Oriented Organization

CDA organizes documentation according to capabilities rather than implementation artifacts.

This allows documentation to remain stable even when implementation technologies change.

---

## Evolution Through Governance

The framework itself evolves through a governed process.

Changes are proposed, reviewed, approved and incorporated into official framework releases.

This ensures that CDA remains consistent while continuously improving.

---

# Intended Audience

CDA is designed for:

- Software architects.
- Technical leads.
- Software engineers.
- Documentation engineers.
- AI-assisted development workflows.
- Teams building long-lived software systems.

---

# Framework Structure

The framework is currently organized into the following modules:

- 00 Framework
- 10 Foundation
- 20 Requirements
- 30 Domain
- 40 Architecture
- 50 Components
- 60 API
- 70 Data
- 80 Implementation
- 90 Decision Records
- 100 Testing

Each module answers a distinct set of questions and together they form a complete documentation architecture.

---

# Relationship with Projects

CDA is independent of any individual software project.

Projects adopt a specific version of the framework and organize their documentation according to its principles.

The framework evolves independently from the projects that use it.

Projects indicate the framework version they conform to through the `cda_version` metadata field.

---

# Next Reading

After understanding the purpose and scope of CDA, continue with:

1. CDA Axioms
2. Documentation Conventions
3. Foundation Module