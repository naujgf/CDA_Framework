---

document_id: FW-003
title: Core Axioms
version: 2.0
status: Approved
cda_version: 2.0
owner: CDA Working Group
last_updated: 2026-07-20

relationships:
derives_from:
- FW-002
constrained_by:
references:
- FW-004
supersedes: FW-003 v1.4
-----------------------

# Core Axioms

## Purpose

Define the immutable principles that govern the Capability Documentation Architecture (CDA).

These axioms establish the behavior of the concepts defined in the Foundational Concepts document. Every Knowledge Domain, documentation practice, template, and future evolution of the framework shall remain consistent with these principles.

---

# Scope

## Defines

* The immutable principles of CDA.
* The behavioral rules governing software knowledge.
* The conceptual constraints that apply across the framework.

## Does NOT define

* Foundational terminology.
* Documentation practices.
* Knowledge Domain specifications.
* Project-specific guidance.

---

# What is an Axiom?

An axiom is a foundational principle accepted as universally true within the framework.

Unlike documentation practices or implementation guidance, axioms describe properties of the knowledge model itself. They are intended to remain stable across framework versions and provide the foundation upon which all other framework elements are built.

---

# Core Axioms

## Axiom 1 — Every Knowledge Item Has Exactly One Authoritative Owner

Every Knowledge Item belongs to exactly one Knowledge Domain.

Although a Knowledge Item may be referenced by many domains, documents, or systems, only one Knowledge Domain is responsible for defining and maintaining its authoritative meaning.

This principle establishes a single source of truth for every piece of software knowledge.

---

## Axiom 2 — Knowledge Domains Have Explicit Boundaries

Every Knowledge Domain defines the limits of the software knowledge it owns.

A domain is responsible only for the knowledge within its conceptual boundary and must not redefine knowledge owned by another domain.

Clear boundaries minimize ambiguity, overlap, and duplication.

---

## Axiom 3 — Knowledge Is Reused Through References, Not Duplication

Knowledge owned by one domain may be used by many others through references.

References preserve consistency while allowing knowledge to be reused without creating competing definitions.

Duplication should never replace authoritative ownership.

---

## Axiom 4 — Knowledge Progresses from Intent to Realization

Software knowledge is organized as a progression from purpose toward implementation.

Higher levels describe intent, objectives, and conceptual models.

Lower levels progressively define structure, behavior, implementation, verification, and operation.

Each level provides the context necessary to understand the levels that follow.

---

## Axiom 5 — Stable Knowledge Is Separated from Volatile Knowledge

Knowledge that changes infrequently should remain independent from knowledge that changes frequently.

Separating stable knowledge from volatile knowledge reduces maintenance effort, improves long-term consistency, and minimizes the impact of change.

---

## Axiom 6 — Every Knowledge Domain Answers One Irreducible Question

Each Knowledge Domain exists to answer a single fundamental question about a software system.

That question cannot be completely answered by another Knowledge Domain without losing conceptual clarity or ownership.

This principle defines the purpose and independence of every Knowledge Domain within CDA.

---

## Axiom 7 — Knowledge Domains Are Technology Independent

Knowledge Domains describe categories of software knowledge rather than technologies, methodologies, programming languages, organizational structures, or documentation tools.

The conceptual model remains valid regardless of how software is developed, documented, or implemented.

---

## Axiom 8 — Significant Decisions Preserve Their Rationale

Architecturally or strategically significant decisions constitute software knowledge.

The rationale behind such decisions should be preserved so future readers can understand not only what was decided, but why the decision was made.

---

# Relationship Between Concepts, Axioms, and Practices

The framework is organized into three complementary layers:

1. **Foundational Concepts** define the vocabulary of CDA.
2. **Core Axioms** define the immutable behavior of those concepts.
3. **Documentation Practices** describe how the concepts and axioms are applied when documenting software systems.

Together, these layers form the conceptual foundation of the Capability Documentation Architecture.

---

# Framework Evolution

Changes to these axioms should be exceptionally rare.

Because the axioms define the conceptual foundation of CDA, modifying them constitutes a major evolution of the framework and may require corresponding changes to Knowledge Domains, documentation practices, templates, and existing implementations.

New axioms should be introduced only when they describe a universally applicable property of the knowledge model that cannot be derived from the existing principles.
