# Testing Knowledge Domain

| Attribute | Value |
|----------|-------|
| Domain | Testing |
| Identifier | KD-90 |
| Version | 1.0.0 |
| Status | Stable |
| Layer | CDA Standard |
| Category | Cross-Layer Knowledge Domain |
| Parent | Knowledge Domains |

---

# Purpose

The Testing Knowledge Domain defines how the correctness, completeness and quality of the software solution are verified.

It documents the strategies, methods, evidence and criteria used to validate that the solution fulfills its intended purpose across all Knowledge Domains.

The Testing Knowledge Domain provides confidence that documented knowledge is realized correctly and continues to remain valid as the solution evolves.

---

# Primary Question

> **How do we verify the solution fulfills its intent?**

Every artifact belonging to the Testing Knowledge Domain should contribute to answering this question.

---

# Objectives

The Testing Knowledge Domain exists to:

- Define verification strategies.
- Establish acceptance criteria.
- Document validation methods.
- Provide evidence of correctness.
- Promote confidence in the solution.
- Support continuous quality assurance.

---

# Core Concepts

The Testing Knowledge Domain is organized around five conceptual areas.

## Verification

Defines how documented knowledge is verified.

---

## Validation

Defines how the solution is evaluated against business intent.

---

## Test Strategy

Defines the overall approach to verification.

---

## Test Coverage

Defines what is verified and to what extent.

---

## Evidence

Defines the artifacts demonstrating successful verification.

---

# Knowledge Responsibilities

The Testing Knowledge Domain is responsible for documenting the following categories of knowledge.

## Test Strategy

Describe the overall verification approach.

Typical knowledge includes:

- Testing philosophy
- Testing levels
- Quality objectives
- Verification scope
- Acceptance approach

The strategy should define how confidence in the solution is established.

---

## Verification Criteria

Document what constitutes successful verification.

Examples include:

- Acceptance criteria
- Pass/fail conditions
- Quality thresholds
- Compliance requirements
- Coverage objectives

Verification criteria should be measurable whenever practical.

---

## Test Specifications

Describe how specific capabilities are verified.

Typical knowledge includes:

- Test scenarios
- Test cases
- Expected outcomes
- Preconditions
- Verification procedures

The focus is on demonstrating correctness rather than describing implementation.

---

## Coverage

Document which knowledge has been verified.

Examples include:

- Requirements coverage
- Component coverage
- API coverage
- Data validation coverage
- Implementation coverage

Coverage should reflect the project's quality objectives rather than arbitrary metrics.

---

## Verification Evidence

Document the evidence supporting verification.

Examples include:

- Test reports
- Automated test results
- Manual validation records
- Compliance evidence
- Performance benchmarks

Evidence provides confidence that verification has been performed successfully.

---

# Characteristics

Knowledge contained within this domain should exhibit the following characteristics.

## Objective

Verification should rely on observable evidence.

---

## Repeatable

Verification activities should produce consistent results when repeated.

---

## Traceable

Verification should be traceable to the knowledge being validated.

---

## Comprehensive

Verification should address all relevant Knowledge Domains.

---

## Continuous

Verification should evolve alongside the software solution.

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
- Implementation

Testing verifies knowledge across every Core Knowledge Domain.

---

## Cross-Layer Responsibility

The Testing Knowledge Domain validates the correctness and completeness of every Core Knowledge Domain.

It is not limited to implementation testing and should provide verification strategies appropriate to each layer of knowledge.

---

# Reference Artifacts

The CDA Standard recommends the following artifacts for representing Testing knowledge.

## Required

| Artifact | Purpose |
|----------|---------|
| Testing Index | Entry point for Testing documentation. |
| Test Strategy | Defines the overall verification approach. |

---

## Recommended

| Artifact | Purpose |
|----------|---------|
| Acceptance Criteria | Defines success conditions. |
| Test Specifications | Describes verification procedures. |
| Coverage Matrix | Maps verification to Knowledge Domains. |
| Test Reports | Provides verification evidence. |

---

## Optional

| Artifact | Purpose |
|----------|---------|
| Performance Test Plan | Documents performance verification. |
| Security Test Plan | Documents security verification. |
| Compliance Verification | Demonstrates regulatory compliance. |
| Regression Strategy | Defines ongoing verification practices. |
| Quality Dashboard | Summarizes verification status. |

Projects may organize these artifacts according to their needs.

The CDA Standard defines knowledge responsibilities rather than mandatory document structures.

---

# Out of Scope

The Testing Knowledge Domain should not contain:

- Bug reports
- Root cause analyses
- Implementation fixes
- Architectural decisions
- Coding standards
- Feature requests
- Project planning

These belong to other Knowledge Domains.

---

# Evolution

The Testing Knowledge Domain evolves as the solution and its quality objectives evolve.

Typical reasons for updates include:

- New requirements.
- New verification strategies.
- Additional quality objectives.
- Expanded coverage.
- New compliance obligations.
- Improved automation.

Testing documentation should evolve continuously to maintain confidence in the solution.

---

# Conformance

A project conforms to the Testing Knowledge Domain if it:

- Documents the required knowledge responsibilities.
- Defines verification strategies for the Core Knowledge Domains.
- Provides measurable verification criteria.
- Maintains traceability between knowledge and verification.
- Documents evidence demonstrating successful validation.

Conformance is evaluated based on the quality and completeness of the documented verification knowledge rather than the quantity of executed tests.

---

# Implementation Guidance

This specification defines **what knowledge belongs** to the Testing Knowledge Domain.

It intentionally does **not** prescribe a mandatory document structure.

Reference templates for implementing this knowledge domain are provided separately in the `20_templates` section of the CDA repository.

Concrete software projects remain free to organize, merge or split documents according to their needs, provided the knowledge responsibilities defined by this specification are fulfilled.