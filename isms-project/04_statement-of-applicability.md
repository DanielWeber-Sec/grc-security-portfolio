# Statement of Applicability (SoA)

---

## Overview

This document defines the applicability and implementation status of selected ISO 27001 Annex A controls within the ISMS.

It provides justification for inclusion or exclusion and ensures traceability between identified risks and implemented controls.

---

## Scope

The SoA applies to the defined ISMS scope covering the development environment and associated systems.

---

## Control Overview

| Control Domain | Control | Applicable | Status | Justification |
|---------------|--------|-----------|--------|--------------|
| Access Control | User Access Management | Yes | Implemented | Required to prevent unauthorized access to sensitive development data |
| Access Control | Privileged Access Management | Yes | Partial | Elevated access exists; stricter controls planned |
| Cryptography | Encryption of Data at Rest | Yes | Partial | Applied in cloud systems, not consistently on-prem |
| Operations Security | Backup Management | Yes | Implemented | Critical for recovery in case of ransomware |
| Operations Security | Logging & Monitoring | Yes | Partial | Logging exists but not centrally correlated |
| Incident Management | Incident Response Process | Yes | Implemented | Defined process and responsibilities |
| Supplier Security | Third-Party Risk Management | Yes | Planned | Increasing supplier integration requires formalization |
| Business Continuity | Disaster Recovery | Yes | Partial | Backup exists, DR testing limited |

---

## Interpretation

Controls are selected based on:

- relevance to identified risks  
- business impact  
- operational feasibility  

The focus is on implementing controls that provide measurable risk reduction.

---

## Notes

This SoA represents a simplified but realistic control selection aligned with ISO 27001 principles.# Statement of Applicability (SoA)

---

## Objective

The Statement of Applicability defines which ISO 27001 controls are:

- applicable  
- implemented  
- excluded  

and provides justification for each decision.

---

## Scope Reference

The SoA is aligned with the defined ISMS scope:

- Office IT  
- Production systems  
- Supplier interfaces  

---

## Control Selection Approach

Controls are selected based on:

- identified risks  
- business relevance  
- implementation feasibility  

The focus is on selecting controls that provide **effective risk reduction**, rather than maximum coverage.

---

## Selected Controls (Example)

| Control | Description | Status | Justification |
|--------|-------------|--------|--------------|
| Access Control | Management of user access rights | Implemented | Critical for protecting systems and data |
| Backup | Data backup and recovery procedures | Implemented | Ensures business continuity |
| Supplier Security | Third-party risk management | Implemented | High dependency on suppliers |
| Cryptography | Encryption mechanisms | Partially | Limited scope relevance |
| Physical Security | Physical access protection | Not Applicable | Out of defined ISMS scope |

---

## Interpretation

The SoA demonstrates:

- alignment between risks and controls  
- structured decision-making  
- understanding of ISO 27001 requirements  

It is not intended to be exhaustive, but to reflect a **realistic and justifiable control set**.

---

## Outcome

The SoA provides:

- transparency in control selection  
- traceability to identified risks  
- a foundation for further ISMS development  

It serves as a key artifact linking **risk assessment and control implementation**. 
