# Implementation Knowledge Domain

| Attribute | Value |
|----------|-------|
| Domain | Implementation |
| Identifier | KD-80 |
| Version | 1.0.0 |
| Status | Stable |
| Layer | CDA Standard |
| Parent | Knowledge Domains |

---

# Purpose

The Implementation Knowledge Domain defines how the software solution is realized.

It documents the technologies, frameworks, project structure, configuration, deployment and implementation practices that transform the architectural design into a working software system.

The Implementation Knowledge Domain captures the technical realization of the solution while remaining separate from the rationale behind architectural decisions.

---

# Primary Question

> **How is the solution realized?**

Every artifact belonging to the Implementation Knowledge Domain should contribute to answering this question.

---

# Objectives

The Implementation Knowledge Domain exists to:

- Describe how the solution is implemented.
- Document implementation technologies.
- Define project organization.
- Capture deployment and runtime configuration.
- Promote consistency across implementations.
- Enable reproducible software delivery.

---

# Core Concepts

The Implementation Knowledge Domain is organized around five conceptual areas.

## Technology Stack

Defines the technologies used to implement the solution.

---

## Project Structure

Defines how the implementation is organized.

---

## Configuration

Defines how the software is configured across environments.

---

## Build and Deployment

Defines how the software is packaged and delivered.

---

## Operational Practices

Defines implementation conventions and engineering practices.

---

# Knowledge Responsibilities

The Implementation Knowledge Domain is responsible for documenting the following categories of knowledge.

## Technology Stack

Document the technologies used to realize the solution.

Typical knowledge includes:

- Programming languages
- Frameworks
- Libraries
- Databases
- Messaging platforms
- Runtime environments

Technology choices should reflect the architectural requirements of the solution.

---

## Project Structure

Describe the organization of the implementation.

Examples include:

- Repository structure
- Modules
- Packages
- Services
- Build organization
- Dependency management

The goal is to help contributors understand how the implementation is organized.

---

## Configuration

Document how the solution is configured.

Typical knowledge includes:

- Environment variables
- Configuration files
- Feature flags
- Secrets management
- Profiles
- Runtime parameters

Configuration should support reproducible deployments.

---

## Build and Deployment

Describe how the solution is built and deployed.

Examples include:

- Build process
- Packaging
- CI/CD pipelines
- Deployment environments
- Infrastructure dependencies
- Release process

---

## Engineering Practices

Document implementation conventions adopted by the project.

Examples include:

- Coding standards
- Branching strategy
- Dependency management
- Logging conventions
- Error handling
- Observability practices

These practices promote consistency across the implementation.

---

# Characteristics

Knowledge contained within this domain should exhibit the following characteristics.

## Technology Specific

Implementation documentation should accurately reflect the technologies used by the project.

---

## Practical

Documentation should enable contributors to build, configure and operate the solution.

---

## Reproducible

A contributor should be able to recreate the implementation environment using the documented knowledge.

---

## Maintainable

Implementation documentation should evolve together with the software.

---

## Operational

The focus is on delivering and operating working software.

---

# Relationships

## Depends On

- Foundation
- Requirements
- Domain
- Architecture
- Components
- API
- Data

Implementation realizes every previous Knowledge Domain.

---

## Provides Context To

- Testing
- Decision Records

---

# Reference Artifacts

The CDA Standard recommends the following artifacts for representing Implementation knowledge.

## Required

| Artifact | Purpose |
|----------|---------|
| Implementation Index | Entry point for Implementation documentation. |
| Technology Stack | Documents the technologies used by the solution. |

---

## Recommended

| Artifact | Purpose |
|----------|---------|
| Project Structure | Describes repository organization. |
| Configuration Guide | Documents runtime configuration. |
| Deployment Guide | Explains deployment procedures. |
| Development Guide | Helps contributors work on the project. |

---

## Optional

| Artifact | Purpose |
|----------|---------|
| Coding Standards | Documents implementation conventions. |
| Build Guide | Explains build procedures. |
| Environment Setup | Defines local development setup. |
| Operations Guide | Documents runtime operations. |
| Infrastructure Guide | Describes implementation infrastructure. |

Projects may organize these artifacts according to their needs.

The CDA Standard defines knowledge responsibilities rather than mandatory document structures.

---

# Out of Scope

The Implementation Knowledge Domain should not contain:

- Business objectives
- Functional requirements
- Domain concepts
- Architectural rationale
- Component responsibilities
- API contracts
- Information models
- Decision rationale
- Test results

These belong to other Knowledge Domains.

---

# Evolution

The Implementation Knowledge Domain evolves as the software implementation changes.

Typical reasons for updates include:

- Adoption of new technologies.
- Framework upgrades.
- Repository restructuring.
- Deployment improvements.
- New engineering practices.
- Infrastructure modernization.

Implementation documentation should evolve continuously alongside the software.

---

# Conformance

A project conforms to the Implementation Knowledge Domain if it:

- Documents the required knowledge responsibilities.
- Accurately reflects the implementation.
- Documents technologies, configuration and deployment.
- Supports reproducible software delivery.
- Separates implementation details from architectural rationale.

Conformance is evaluated based on the quality and completeness of the documented knowledge rather than the number or names of documents.

---

# Implementation Guidance

This specification defines **what knowledge belongs** to the Implementation Knowledge Domain.

It intentionally does **not** prescribe a mandatory document structure.

Reference templates for implementing this knowledge domain are provided separately in the `20_templates` section of the CDA repository.

Concrete software projects remain free to organize, merge or split documents according to their needs, provided the knowledge responsibilities defined by this specification are fulfilled.