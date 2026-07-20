# API Knowledge Domain

| Attribute  | Value             |
| ---------- | ----------------- |
| Domain     | API               |
| Identifier | KD-60             |
| Version    | 1.0.0             |
| Status     | Stable            |
| Layer      | CDA Standard      |
| Parent     | Knowledge Domains |

---

# Purpose

The API Knowledge Domain defines the contracts through which software components, systems and external consumers interact.

It specifies the capabilities exposed by the solution, the structure of requests and responses, communication patterns, and interaction rules while remaining independent of implementation details.

The API Knowledge Domain ensures that integrations are stable, well-defined and technology-agnostic.

---

# Primary Question

> **How do systems communicate?**

Every artifact belonging to the API Knowledge Domain should contribute to answering this question.

---

# Objectives

The API Knowledge Domain exists to:

* Define interaction contracts between systems and components.
* Specify exposed capabilities.
* Describe communication patterns.
* Document exchanged information.
* Promote interoperability and consistency.
* Enable independent evolution of providers and consumers.

---

# Core Concepts

The API Knowledge Domain is organized around five conceptual areas.

## Contracts

Defines the agreements between providers and consumers.

---

## Operations

Defines the capabilities exposed through an API.

---

## Messages

Defines the structure of exchanged information.

---

## Protocols

Defines the communication mechanisms used to realize the contracts.

---

## Versioning

Defines how APIs evolve while preserving compatibility.

---

# Knowledge Responsibilities

The API Knowledge Domain is responsible for documenting the following categories of knowledge.

## API Catalog

Describe every externally or internally exposed API.

Typical knowledge includes:

* Purpose
* Consumers
* Providers
* Scope
* Ownership

Each API should have a clearly defined responsibility.

---

## Operations

Document the capabilities offered by each API.

Examples include:

* Commands
* Queries
* Endpoints
* Procedures
* Events
* Streams

Operations describe what consumers can accomplish rather than how they are implemented.

---

## Message Contracts

Describe the structure of exchanged information.

Typical knowledge includes:

* Requests
* Responses
* Events
* Commands
* Payloads
* Errors

The focus is on contractual compatibility.

---

## Communication Patterns

Describe how participants interact.

Examples include:

* Request/Response
* Publish/Subscribe
* Event Streaming
* Command Processing
* Asynchronous Messaging
* Bidirectional Communication

Communication patterns should be independent of specific technologies whenever possible.

---

## Versioning and Compatibility

Document the evolution strategy of APIs.

Typical knowledge includes:

* Versioning policy
* Compatibility guarantees
* Deprecation strategy
* Breaking change policy

---

# Characteristics

Knowledge contained within this domain should exhibit the following characteristics.

## Contract-First

APIs should be defined as contracts before implementation.

---

## Technology-Agnostic

The API describes interactions independently of implementation frameworks.

---

## Consistent

Naming, structures and behaviors should be predictable across APIs.

---

## Stable

API contracts should evolve carefully to minimize disruption.

---

## Consumer-Oriented

APIs should be documented from the perspective of their consumers.

---

# Relationships

## Depends On

* Foundation
* Requirements
* Domain
* Architecture
* Components

APIs expose the capabilities implemented by components.

---

## Provides Context To

* Data
* Implementation
* Testing
* Decision Records

---

# Reference Artifacts

The CDA Standard recommends the following artifacts for representing API knowledge.

## Required

| Artifact    | Purpose                                                |
| ----------- | ------------------------------------------------------ |
| API Index   | Entry point for API documentation.                     |
| API Catalog | Defines the available APIs and their responsibilities. |

---

## Recommended

| Artifact           | Purpose                          |
| ------------------ | -------------------------------- |
| API Specifications | Define contracts and operations. |
| Message Models     | Describe exchanged payloads.     |
| Error Catalog      | Standardize error handling.      |
| Versioning Policy  | Documents API evolution rules.   |

---

## Optional

| Artifact             | Purpose                                           |
| -------------------- | ------------------------------------------------- |
| Sequence Diagrams    | Illustrate interaction flows.                     |
| Event Catalog        | Documents published and consumed events.          |
| Authentication Guide | Explains authentication and authorization models. |
| Consumer Guide       | Helps external consumers integrate with the API.  |

Projects may organize these artifacts according to their needs.

The CDA Standard defines knowledge responsibilities rather than mandatory document structures.

---

# Out of Scope

The API Knowledge Domain should not contain:

* Business requirements
* Internal component implementation
* Database schemas
* Source code
* Framework-specific controllers
* Network infrastructure
* Deployment configuration
* Client implementations
* Server implementations

These belong to other knowledge domains.

---

# Evolution

The API Knowledge Domain evolves as interaction capabilities change.

Typical reasons for updates include:

* New operations.
* New consumers.
* New communication patterns.
* API version releases.
* Contract evolution.
* Deprecation of obsolete interfaces.

API evolution should prioritize backward compatibility whenever practical.

---

# Conformance

A project conforms to the API Knowledge Domain if it:

* Documents the required knowledge responsibilities.
* Defines clear interaction contracts.
* Specifies message structures and communication patterns.
* Documents API evolution and compatibility policies.
* Separates contracts from implementation details.

Conformance is evaluated based on the quality and completeness of the documented knowledge rather than the number or names of documents.

---

# Implementation Guidance

This specification defines **what knowledge belongs** to the API Knowledge Domain.

It intentionally does **not** prescribe a mandatory document structure.

Reference templates for implementing this knowledge domain are provided separately in the `20_templates` section of the CDA repository.

Concrete software projects remain free to organize, merge or split documents according to their needs, provided the knowledge responsibilities defined by this specification are fulfilled.
