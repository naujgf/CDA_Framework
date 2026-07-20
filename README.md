# Capability Documentation Architecture (CDA)

> A Reference Knowledge Model for Software Systems

---

# What is CDA?

The **Capability Documentation Architecture (CDA)** is a reference knowledge model that organizes software knowledge into a finite set of independent Knowledge Domains.

Unlike traditional documentation frameworks, CDA does **not** prescribe document templates, folder structures, or writing styles.

Instead, it answers a more fundamental question:

> **What kinds of knowledge exist in a software system, and who owns them?**

CDA provides a conceptual model for classifying software knowledge independently of technologies, documentation formats, methodologies, or development processes.

It can be implemented using Markdown repositories, documentation platforms, knowledge graphs, wikis, AI retrieval systems, or any other documentation technology.

---

# Why CDA Exists

Modern software documentation is often organized around artifacts:

* Requirements documents
* API documentation
* Architecture diagrams
* ADRs
* Wikis
* Confluence pages
* Source code comments

These artifacts frequently overlap, duplicate information, and blur ownership boundaries.

As systems evolve, documentation becomes inconsistent because multiple documents attempt to describe the same knowledge from different perspectives.

CDA approaches the problem differently.

Instead of organizing documentation around artifacts, CDA organizes knowledge around **ownership**.

Every piece of software knowledge belongs to exactly one Knowledge Domain.

This creates clear ownership, eliminates duplication, improves consistency, and enables documentation to evolve alongside the software system.

---

# Core Principle

The central principle of CDA is:

> **Every piece of software knowledge has exactly one authoritative owner.**

Knowledge may be referenced by multiple domains.

Knowledge may influence multiple domains.

Knowledge may appear in many views.

But it is **owned by one and only one Knowledge Domain**.

This principle provides the foundation for consistency, traceability, maintainability, and AI-assisted knowledge retrieval.

---

# Knowledge Domains

CDA partitions software knowledge into a set of irreducible Knowledge Domains.

Each domain:

* owns a unique category of software knowledge,
* answers one irreducible question,
* defines explicit ownership boundaries,
* explicitly states what it does **not** own.

Current Knowledge Domains:

1. Foundation
2. Requirements
3. Domain
4. Architecture
5. Components
6. Contracts
7. Data
8. Implementation
9. Testing
10. Decision Records

---

# The Philosophy Behind CDA

CDA is based on several fundamental principles.

## Knowledge First

Documentation is an implementation.

Knowledge is the model.

CDA models software knowledge independently of the documents that describe it.

---

## Ownership Over Location

Knowledge ownership is more important than where documents are stored.

Whether documentation lives in Git, Confluence, Notion, SharePoint, or a knowledge graph is an implementation detail.

Ownership remains unchanged.

---

## One Source of Truth

Every knowledge item has a single authoritative owner.

Other domains reference that knowledge instead of duplicating it.

---

## Explicit Boundaries

Every Knowledge Domain defines both:

* what it owns;
* what it never owns.

These positive and negative boundaries minimize overlap and ambiguity.

---

## Technology Independence

The model is independent of:

* programming languages,
* frameworks,
* cloud providers,
* architectural styles,
* development methodologies,
* documentation tools.

CDA applies equally to monoliths, microservices, embedded systems, AI agents, distributed platforms, and future software paradigms.

---

## Stable Concepts, Evolving Implementations

Technologies change.

Programming languages evolve.

Frameworks become obsolete.

The underlying categories of software knowledge remain stable.

CDA models those enduring concepts rather than temporary implementation choices.

---

# What CDA Is Not

CDA is **not**:

* a documentation template;
* a folder structure;
* a software architecture framework;
* a software development methodology;
* an enterprise architecture framework;
* a project management methodology;
* a documentation generator;
* a replacement for architecture documentation;
* a replacement for requirements engineering.

Instead, CDA provides a conceptual foundation upon which any of those approaches can be built.

---

# Intended Audience

CDA is intended for:

* Software Architects
* Technical Leads
* Engineering Managers
* Platform Teams
* System Designers
* Documentation Engineers
* AI-assisted engineering teams
* Organizations seeking long-term knowledge management

---

# Repository Structure

This repository is organized according to the CDA Knowledge Domains.

Each domain owns the documentation describing its corresponding category of software knowledge.

The repository intentionally mirrors the conceptual model defined by CDA.

---

# Relationship with Existing Frameworks

CDA complements—not replaces—existing engineering practices.

For example:

* ISO/IEC/IEEE 42010 defines how architecture descriptions are structured.
* arc42 provides a template for architecture documentation.
* C4 provides architectural visualization.
* ADRs capture design rationale.
* DDD models business domains.

CDA provides the knowledge model that allows these artifacts to coexist without overlapping ownership.

---

# Guiding Question

Whenever new documentation is created, ask:

> **Which Knowledge Domain is the authoritative owner of this knowledge?**

The answer determines where the knowledge belongs.

---

# Status

CDA is an evolving research project exploring software knowledge classification and ownership.

The model is being refined through theoretical analysis, practical application, and comparison with existing software engineering literature.

---

# License

Specify the license applicable to this repository (for example, MIT, Apache-2.0, or another license of your choice).

---

# Contributing

Contributions are welcome.

When proposing changes, contributors should preserve the core principles of CDA:

* unique ownership,
* explicit boundaries,
* non-overlapping Knowledge Domains,
* technology independence,
* conceptual consistency,
* one authoritative source for every category of software knowledge.
