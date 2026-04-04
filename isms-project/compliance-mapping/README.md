# Compliance & Control Mapping

---

## Objective

The objective of this module is to demonstrate how security requirements from multiple frameworks can be translated into a coherent set of practical controls.

Rather than treating standards and regulations as isolated documents, this mapping takes a control-oriented view and highlights where different frameworks overlap, reinforce each other, or require specific interpretation.

The goal is to show how compliance requirements can be operationalized into implementable governance and security measures.

---

## Context

Organizations rarely operate against a single standard only.

In practice, security programs often need to align with multiple sources at the same time, including:

- ISO 27001
- BSI IT-Grundschutz
- KRITIS-related expectations
- General regulatory and organizational requirements

This creates a need for structured mapping, so that overlapping requirements can be addressed efficiently and consistently.

---

## Scope

This mapping focuses on core security control domains relevant for a mid-sized automotive supplier with:

- production-dependent business operations
- external supplier connectivity
- internal IT infrastructure
- customer-related data processing

The mapping is intentionally designed around practical control areas that are directly relevant for ISMS implementation, governance, audit preparation, and risk treatment.

---

## Approach

The mapping follows a unified control logic:

1. Identify a core control objective
2. Translate that objective into practical implementation language
3. Map the control against multiple frameworks
4. Highlight regulatory relevance and operational impact

This approach avoids duplicate implementation work and helps create a single, business-aligned control view.

---

## Mapping Logic

The control mapping is structured around the following principles:

- focus on control objectives, not document silos
- identify overlaps between standards
- use framework references as anchors, not as isolated end goals
- connect requirements to realistic implementation examples

This makes the mapping usable for:

- ISMS implementation
- control design
- audit preparation
- management reporting
- framework alignment discussions

---

## Example Control Mapping

| Control ID | Control Name | Control Objective | ISO 27001 Reference | BSI IT-Grundschutz Reference | KRITIS Relevance | Implementation Example |
|------------|--------------|------------------|---------------------|------------------------------|------------------|------------------------|
| CM-01 | Access Control | Restrict system access to authorized users only | A.5.15 | ORP.4.A1 | High | Role-based access control, regular access reviews |
| CM-02 | Identity Management | Ensure proper onboarding, change, and removal of user access | A.5.16 / A.5.18 | ORP.4.A3 | High | Joiner-mover-leaver process, periodic recertification |
| CM-03 | Patch Management | Reduce exposure to known vulnerabilities through timely updates | A.8.8 | OPS.1.1.A1 | High | Centralized patching, defined patch cycles, exception handling |
| CM-04 | Vulnerability Management | Identify and track technical weaknesses systematically | A.8.8 / A.8.9 | OPS.1.1.A5 | Medium | Vulnerability scans, remediation plans, ownership tracking |
| CM-05 | Network Segmentation | Limit attack propagation and isolate critical assets | A.8.20 | NET.1.1.A1 | High | Segmentation between office IT, production-related systems, and supplier connections |
| CM-06 | Logging & Monitoring | Detect suspicious or unauthorized activities | A.8.15 / A.8.16 | DER.1.A1 | High | Central logging, alerting, log retention, event correlation |
| CM-07 | Incident Response | Ensure structured handling of security incidents | A.5.24 to A.5.27 | DER.2.A1 | High | Defined IR process, escalation paths, incident documentation |
| CM-08 | Backup & Recovery | Ensure recoverability of critical systems and data | A.8.13 | CON.3.A1 | High | Offline backups, restore testing, recovery procedures |
| CM-09 | Supplier Security | Manage third-party and supply-chain security risks | A.5.19 / A.5.20 / A.5.21 | OPS.2.3.A1 | High | Supplier assessments, contractual security clauses, periodic reviews |
| CM-10 | Business Continuity | Maintain essential processes during disruptions | A.5.29 / A.5.30 | CON.10.A1 | High | Fallback procedures, continuity planning, defined recovery priorities |
| CM-11 | Security Awareness | Reduce user-related risk through training and awareness | A.6.3 | ORP.3.A1 | Medium | Awareness campaigns, phishing simulations, mandatory training |
| CM-12 | Privileged Access Management | Reduce misuse of elevated access rights | A.5.17 / A.8.2 | ORP.4.A8 | High | Admin account separation, approval workflows, logging of privileged actions |
| CM-13 | Encryption & Data Protection | Protect sensitive data in storage and transmission | A.8.24 / A.8.25 | CON.1.A1 | High | Encryption of laptops, protected file transfer, restricted access to sensitive data |
| CM-14 | Asset Management | Maintain transparency over systems, devices, and owners | A.5.9 / A.5.10 / A.5.11 | OPS.1.1.A3 | Medium | Asset inventory, owner assignment, lifecycle management |
| CM-15 | Change Management | Ensure security-relevant changes are controlled and documented | A.8.32 | OPS.1.1.A6 | Medium | Formal change approval, rollback plans, documentation requirements |

---

## Interpretation

The mapping shows that many requirements across ISO 27001, BSI IT-Grundschutz, and KRITIS-related expectations converge around the same underlying control domains.

This means that a well-structured ISMS does not need to reinvent controls for each framework separately. Instead, a unified control design can often satisfy multiple expectations simultaneously, provided that implementation depth and evidence are sufficient.

This is especially relevant for organizations that need to balance:

- compliance demands
- business continuity requirements
- operational feasibility
- audit readiness

---

## Practical Value

This mapping provides value in several areas:

### 1. Control Harmonization

It helps avoid duplicate work by identifying where different frameworks point to the same control objective.

### 2. Implementation Planning

It supports prioritization by connecting control requirements to actual implementation examples.

### 3. Audit Preparation

It enables a structured view of how one implemented control can support multiple audit or compliance discussions.

### 4. Governance Communication

It creates a clearer language for management and stakeholders by translating framework references into understandable control topics.

---

## Example Use Cases

This mapping can be used to support:

- preparation of an ISMS implementation roadmap
- internal audit planning
- security control gap analysis
- framework comparison workshops
- prioritization of control implementation in risk treatment plans

---

## Relation to Other ISMS Components

This module directly complements other parts of the ISMS project:

- **Risk Assessment**  
  Risks identified in the register are linked to concrete control domains

- **Security Policies**  
  Policies define governance expectations around selected controls

- **Tabletop Exercise**  
  Incident and continuity exercises validate whether selected controls are effective in practice

- **Statement of Applicability (SoA)**  
  The SoA determines which controls are applicable, while this mapping shows how those controls relate to broader framework expectations

---

## Conclusion

The purpose of this control mapping is not to reproduce full standards documentation.

Its purpose is to demonstrate the ability to interpret, align, and operationalize security requirements across multiple frameworks in a practical and business-oriented way.

This reflects a core capability in Information Security Governance, GRC, and ISMS-related roles.

---

## Supporting File

A more detailed control mapping is maintained in the accompanying spreadsheet:

[control-mapping.xlsx](control-mapping.xlsx)
