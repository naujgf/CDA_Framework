---
document_id: FW-003
title: CDA Axioms
version: 1.4
status: Approved
cda_version: 1.4
owner: CDA Working Group
last_updated: 2026-07-17

relationships:
  derives_from:
  constrained_by:
  references:
    - FW-004
  supersedes:
---

# CDA Axioms

## Purpose

Define the fundamental principles upon which the Capability Documentation Architecture (CDA) is built.

These axioms represent the immutable foundation of the framework. Every convention, guideline, module specification and future evolution of CDA should remain consistent with them.

## Scope of This Document

### Defines

- The fundamental principles of CDA.
- The philosophical foundation of the framework.

### Does NOT define

- Documentation conventions.
- Writing standards.
- Module specifications.
- Implementation guidelines.

---

# What is an Axiom?

An axiom is a foundational principle that is accepted as true within the framework.

Unlike conventions or implementation rules, axioms are intended to remain stable across framework versions and guide every design decision made within CDA.

---

# CDA Axioms

## Axiom 1 — Every Document Answers One Primary Question

Each document exists to answer one clearly defined question.

Documents should have a single primary responsibility. Additional information is included only when it directly supports that responsibility.

This principle minimizes ambiguity, reduces duplication and makes documentation easier to navigate.

---

## Axiom 2 — Abstraction Flows Downward

Documentation progresses from abstract concepts toward concrete implementation.

Higher-level documents define intent.

Lower-level documents define realization.

A document should never require knowledge from a more detailed document in order to understand its purpose.

---

## Axiom 3 — Stable Knowledge Lives Above Volatile Knowledge

Knowledge that changes infrequently belongs in higher-level modules.

Knowledge that changes frequently belongs in lower-level modules.

This separation minimizes maintenance effort and reduces unnecessary documentation changes.

---

## Axiom 4 — Intent Precedes Solution

Documentation explains why before explaining how.

Business goals, capabilities and architectural intent should always be understood before implementation details.

---

## Axiom 5 — Capabilities Precede Features

The framework organizes documentation around capabilities rather than implementation artifacts.

Capabilities represent enduring business or technical responsibilities, while features and implementations evolve over time.

---

## Axiom 6 — Every Significant Decision Must Be Traceable

Architectural and design decisions should be discoverable and understandable.

The framework should enable readers to understand not only what decisions were made, but also why they were made.

---

## Axiom 7 — Documentation Serves Humans and AI Equally

Documentation must be written to maximize clarity, consistency and discoverability for both human readers and AI systems.

The framework assumes that software documentation is consumed collaboratively by people and intelligent tools.

---

# Relationship Between Axioms and Conventions

The axioms define *what must always remain true*.

Documentation conventions define *how those principles are applied*.

Framework evolution may introduce new conventions, templates or modules, but they should always remain consistent with these axioms.

---

# Framework Evolution

Changes to these axioms should be extremely rare.

If an axiom requires modification, the change should be treated as a major framework evolution because it affects the conceptual foundation of CDA.
