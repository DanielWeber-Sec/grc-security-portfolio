# 04 – Statement of Applicability (SoA)

---

## Overview

This document defines the applicability and implementation status of selected ISO 27001 Annex A controls within the ISMS.

It provides justification for inclusion or exclusion and ensures traceability between identified risks and implemented controls.

---

## Scope

The SoA applies to the defined ISMS scope covering:

- development environment
- production-related systems
- supplier integrations

---

## Control Selection Approach

Controls are selected based on:

- identified risks
- business impact
- operational feasibility

The focus is on implementing controls that provide **effective and measurable risk reduction**, rather than maximum control coverage.

---

## Control Overview

| Control Domain      | Control                      | Applicable | Status      | Justification                                             |
| ------------------- | ---------------------------- | ---------- | ----------- | --------------------------------------------------------- |
| Access Control      | User Access Management       | Yes        | Implemented | Required to prevent unauthorized access to sensitive data |
| Access Control      | Privileged Access Management | Yes        | Partial     | Elevated access exists; stricter controls planned         |
| Cryptography        | Encryption of Data at Rest   | Yes        | Partial     | Applied in cloud systems, not consistently on-prem        |
| Operations Security | Backup Management            | Yes        | Implemented | Critical for recovery in case of ransomware               |
| Operations Security | Logging & Monitoring         | Yes        | Partial     | Logging exists but not centrally correlated               |
| Incident Management | Incident Response Process    | Yes        | Implemented | Defined process and responsibilities                      |
| Supplier Security   | Third-Party Risk Management  | Yes        | Planned     | Increasing supplier integration requires formalization    |
| Business Continuity | Disaster Recovery            | Yes        | Partial     | Backup exists, DR testing limited                         |

---

## Interpretation

The SoA demonstrates:

- alignment between risks and controls
- structured and risk-based decision-making
- prioritization based on business impact

---

## Outcome

The SoA provides:

- transparency in control selection
- traceability to identified risks
- a foundation for auditability and continuous improvement

It serves as a central artifact linking **risk assessment and control implementation**.
