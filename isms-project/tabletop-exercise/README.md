# Tabletop Exercise – Ransomware Incident (Automotive Supplier)

---

## Context

This tabletop exercise is part of a simplified ISMS implementation aligned with ISO 27001 principles.

It is designed to validate the effectiveness of defined risk treatment measures and incident response capabilities by simulating a realistic ransomware attack scenario.

---

## Scenario Overview

A targeted ransomware attack impacts the internal IT environment of a mid-sized automotive supplier.

The attack originates from a phishing email leading to credential compromise. Due to insufficient network segmentation and delayed patching, the attacker achieves lateral movement and deploys ransomware across multiple systems.

---

## Objectives

The exercise aims to evaluate:

- Incident detection and escalation processes
- Technical containment and eradication capabilities
- Decision-making under pressure (management level)
- Internal and external communication workflows
- Business continuity and recovery effectiveness

---

## Scope

Systems in scope:

- Customer CRM system
- File servers (shared drives)
- Identity and access management (Active Directory)
- Production planning systems

---

## Initial Situation (T0)

- Users report inaccessible files
- Ransom note detected on shared drives
- Suspicious login activity outside business hours
- EDR alerts indicating lateral movement

---

## Attack Progression

| Time | Event |
|------|------|
| T0 | Phishing email received |
| T+2h | Credential compromise |
| T+6h | Lateral movement |
| T+8h | Domain-wide access |
| T+10h | Ransomware deployed |

---

## Key Decision Points

Participants must decide:

- System isolation vs. full network shutdown
- Ransom payment vs. recovery strategy
- Internal and external communication timing
- Production continuation vs. shutdown

---

## Roles and Responsibilities

| Role | Responsibility |
|------|--------------|
| IT Security | Incident coordination |
| IT Operations | System containment and recovery |
| Management | Strategic decisions |
| Legal & Compliance | Regulatory obligations |
| Communications | Stakeholder communication |

---

## Business Impact Analysis

| Area | Impact |
|------|-------|
| Operations | Production delays |
| Financial | Revenue loss and recovery costs |
| Legal | Potential compliance violations |
| Reputation | Loss of customer trust |

---

## Business Continuity Measures

- Use of offline backups
- Manual fallback procedures
- Prioritization of critical processes
- Alternative communication channels

---

## Key Controls Evaluated

- Patch management
- Network segmentation
- Access control (least privilege)
- Monitoring and detection
- Backup and recovery

---

## Lessons Learned

- Delayed patching increased risk exposure
- Lack of segmentation enabled rapid spread
- Backup processes must be regularly tested
- Clear roles and escalation paths are critical

---

## Link to Risk Assessment

This scenario is directly linked to identified risks:

- Ransomware due to outdated patching
- Insufficient network segmentation
- Weak access control mechanisms
