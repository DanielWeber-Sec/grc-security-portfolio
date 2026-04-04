# Tabletop Exercise – Ransomware Incident (Automotive Supplier)

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
- Active Directory / Identity Management
- Production planning systems

Out of scope:

- OT systems (only indirectly impacted)

---

## Initial Situation (T0)

- Multiple employees report inaccessible files
- Ransom note detected on shared drives
- Unusual login activity during off-hours
- EDR alerts triggered (lateral movement behavior)

---

## Attack Progression (Simulated)

| Time | Event |
|------|------|
| T0 | Initial compromise via phishing |
| T+2h | Credential abuse and lateral movement |
| T+6h | Domain-wide access achieved |
| T+8h | Ransomware deployment triggered |
| T+10h | Systems encrypted, operations impacted |

---

## Key Decision Points

Participants must actively decide:

### 1. Containment Strategy
- Immediate network shutdown vs. controlled isolation
- Trade-off: speed vs. business disruption

### 2. Ransom Payment
- Legal, ethical, and operational considerations
- Backup availability vs. recovery time

### 3. Communication
- When to inform:
  - Employees
  - Customers
  - Regulators
- Risk of reputational damage vs. transparency

### 4. Production Impact
- Continue limited operations vs. full shutdown
- Dependency on IT systems

---

## Roles and Responsibilities

| Role | Responsibility |
|------|--------------|
| IT Security | Incident coordination, technical response |
| IT Operations | System isolation, recovery |
| Management | Strategic decisions, risk acceptance |
| Legal & Compliance | Regulatory obligations |
| Communications | Internal & external messaging |

---

## Incident Response Phases

### Detection
- EDR alerts and anomaly detection
- Initial triage and validation

### Containment
- Isolation of infected systems
- Blocking lateral movement
- Account lockdown

### Eradication
- Malware removal
- Patch vulnerabilities
- Remove persistence mechanisms

### Recovery
- Restore systems from backups
- Validate integrity
- Resume operations

---

## Business Impact Analysis

| Area | Impact |
|------|-------|
| Operations | Production delays |
| Financial | Revenue loss, recovery costs |
| Legal | Potential compliance violations |
| Reputation | Customer trust damage |

---

## Business Continuity Measures

- Backup restoration strategy (offline backups)
- Manual fallback processes for critical operations
- Prioritization of core business functions
- Alternative communication channels

---

## Key Controls Evaluated

- Patch management
- Network segmentation
- Access control (least privilege)
- Monitoring & detection (EDR, logging)
- Backup & recovery processes

---

## Lessons Learned

- Delayed patching significantly increased impact
- Lack of segmentation enabled lateral movement
- Backup strategy must be tested regularly
- Incident response roles must be clearly defined

---

## Link to Risk Assessment

This scenario directly relates to identified risks:

- Ransomware infection due to outdated patching
- Insufficient network segmentation
- Weak access control mechanisms

The tabletop exercise validates the effectiveness of defined mitigation strategies.
