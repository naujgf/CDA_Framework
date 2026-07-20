# Contracts Knowledge Domain

## Definition

The **Contracts Knowledge Domain** represents the category of software knowledge that defines the explicit agreements governing communication between independent participants of a software system.

A contract specifies the externally observable behavior that one participant promises to another. It defines the information that may be exchanged, the expectations both parties must satisfy, the guarantees that must be honored, and the rules that preserve compatibility while allowing each participant to evolve independently.

Contracts describe *agreements*, never *implementations*.

---

# Primary Question

> **What agreements enable independent participants to collaborate safely and predictably?**

---

# Purpose

The purpose of the Contracts Knowledge Domain is to establish stable collaboration boundaries between independently evolving responsibilities.

By explicitly defining agreements separately from implementations, contracts reduce coupling, improve interoperability, simplify evolution, and allow systems to change internally without affecting their consumers.

Every observable interaction within a software system should be governed by an explicit or implicit contract.

---

# Owns

The Contracts Knowledge Domain owns knowledge describing:

* Interface definitions
* Communication agreements
* Service contracts
* Consumer-provider expectations
* Request and response models
* Command and query definitions
* Event definitions
* Message schemas
* Protocol specifications
* Function signatures
* Extension point definitions
* File format specifications
* Validation rules exposed through interfaces
* Error models
* Compatibility guarantees
* Versioning policies
* Interaction constraints
* Authentication and authorization requirements that form part of an external agreement

---

# Never Owns

The Contracts Knowledge Domain never owns knowledge describing:

* Business objectives
* Functional requirements
* Business concepts
* Component responsibilities
* Architectural structure
* Internal algorithms
* Data persistence
* Source code
* Deployment
* Infrastructure
* Test implementations
* Decision rationale

---

# Relationships

## Depends On

* Components
* Data

Contracts define agreements between responsibilities and therefore depend on clearly identified participants and shared information models.

---

## Enables

* Implementation
* Testing

Implementations realize contracts.

Testing verifies conformance to contracts.

---

## References

* Decision Records

Design decisions affecting contracts should be justified through Decision Records rather than embedded within contract definitions.

---

# Boundary Principle

> **The Contracts Knowledge Domain owns every explicit agreement that enables independently evolving participants to collaborate without requiring knowledge of each other's internal implementation.**

---

# Design Principles

The Contracts Knowledge Domain follows these principles:

1. A contract describes externally observable behavior.
2. Contracts remain independent from implementation details.
3. Every contract has one or more providers and one or more consumers.
4. Contracts define guarantees, expectations, and constraints.
5. Implementations may evolve without changing contracts, provided contract guarantees remain satisfied.
6. Versioning and compatibility are properties of contracts, not implementations.
7. Contracts describe collaboration, not execution.

---

# Examples

## Belongs in this Domain

* REST API specifications
* GraphQL schemas
* Protocol Buffers
* OpenAPI documents
* AsyncAPI specifications
* JSON Schemas
* Avro schemas
* Interface definitions
* Public SDK contracts
* Plugin interfaces
* CLI specifications
* File format specifications
* Event definitions
* Protocol specifications
* Error models
* Version compatibility rules

---

## Does Not Belong in this Domain

* Controller implementations
* Service implementations
* Database schemas
* SQL queries
* Business rules
* Internal algorithms
* Dependency injection
* Infrastructure configuration
* Deployment scripts
* Unit tests
* Integration tests

---

# Rationale

Contracts constitute an irreducible category of software knowledge because agreements between independent participants cannot be derived from any other Knowledge Domain.

Architecture defines the system's structure.

Components define responsibilities.

Data defines information.

Implementation realizes behavior.

Testing verifies behavior.

Decision Records justify behavior.

None of these domains define the agreements that govern collaboration between independently evolving participants.

Without Contracts, software participants cannot communicate reliably while remaining independently evolvable.

---

# Ownership Rule

When classifying documentation, ask:

> **Does this document define an agreement that another independent participant is expected to follow?**

If the answer is **yes**, the document belongs to the Contracts Knowledge Domain.

If the document explains how that agreement is implemented internally, it belongs to the Implementation Knowledge Domain instead.
