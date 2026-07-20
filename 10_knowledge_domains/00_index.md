# Knowledge Domains

## Purpose

The Knowledge Domains define the categories of knowledge that should be captured when documenting a software project using the CDA Standard.

Each domain specification defines:

- Purpose
- Primary Question
- Core Concepts
- Knowledge Responsibilities
- Relationships
- Reference Artifacts
- Conformance

---

## Core Knowledge Domains

## Problem Space

    Foundation
    Requirements
    Domain

### Solution Space

    Architecture
    Components
    API
    Data
    Implementation

### Cross-Layer Knowledge Domains

    Decision Records
    Testing

---

## Reading Order

Projects should normally be understood in the following order:

1. Foundation
2. Requirements
3. Domain
4. Architecture
5. Components
6. API
7. Data
8. Implementation
9. Decision Records
10. Testing

# CDA Knowledge Domains at a Glance

The Capability Documentation Architecture (CDA) organizes software knowledge into distinct Knowledge Domains. Each domain has a single responsibility, answers a single primary question, and follows a guiding principle that defines its boundaries.

| Knowledge Domain     | Primary Question                                       | Guiding Principle                                            |
| -------------------- | ------------------------------------------------------ | ------------------------------------------------------------ |
| **Foundation**       | **Why does this project exist?**                       | Describe **purpose**, not functionality.                     |
| **Requirements**     | **What must the system accomplish?**                   | Describe **intent**, not design.                             |
| **Domain**           | **What reality does the system model?**                | Describe **the business**, not the software.                 |
| **Architecture**     | **How is the solution organized?**                     | Describe **structure**, not implementation.                  |
| **Components**       | **What building blocks compose the solution?**         | Describe **responsibilities**, not code.                     |
| **API**              | **How do systems communicate?**                        | Describe **contracts**, not implementations.                 |
| **Data**             | **What information is managed?**                       | Describe **information**, not storage technology.            |
| **Implementation**   | **How is the solution realized?**                      | Describe **realization**, not historical decisions.          |
| **Decision Records** | **Why were significant decisions made?**               | Describe **decision rationale**, not implementation details. |
| **Testing**          | **How do we verify the solution fulfills its intent?** | Describe **verification**, not debugging.                    |

## Knowledge Flow

Each Knowledge Domain builds upon the previous one, progressively transforming business intent into a complete software solution while maintaining clear separation of concerns.

```text
Foundation
    │
    ▼
Requirements
    │
    ▼
Domain
    │
    ▼
Architecture
    │
    ▼
Components
    │
    ▼
API
    │
    ▼
Data
    │
    ▼
Implementation
    │
    ▼
Testing
```

> **Decision Records** span the entire lifecycle, documenting the rationale behind significant decisions that influence one or more Knowledge Domains.

This progression is intentional. Each Knowledge Domain answers one fundamental question while deliberately avoiding concerns that belong to downstream domains. This separation enables documentation that is easier to understand, maintain, evolve, and consume by both humans and AI systems.

## Knowledge Domain Summary

| Knowledge Domain | Primary Question                                   | Owns               | Never Describes    |
| ---------------- | -------------------------------------------------- | ------------------ | ------------------ |
| Foundation       | Why does this project exist?                       | Purpose            | Functionality      |
| Requirements     | What must the system accomplish?                   | Intent             | Design             |
| Domain           | What reality does the system model?                | Business Reality   | Software           |
| Architecture     | How is the solution organized?                     | Structure          | Implementation     |
| Components       | What building blocks compose the solution?         | Responsibilities   | Code               |
| API              | How do systems communicate?                        | Contracts          | Implementations    |
| Data             | What information is managed?                       | Information        | Storage Technology |
| Implementation   | How is the solution realized?                      | Realization        | Rationale          |
| Testing          | How do we verify the solution fulfills its intent? | Verification       | Debugging          |
| Decision Records | Why was this decision made?                        | Decision Rationale | Outcomes           |
