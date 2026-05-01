# Cloud Security & Misconfiguration Risk Model

## Objective

This document demonstrates how cloud-specific risks, especially misconfigurations, are identified, assessed, and translated into structured risks, governance decisions, and ISO 27001-aligned controls.

---

## Context

Cloud environments introduce new risks due to:

- Dynamic infrastructure  
- Shared responsibility models  
- High complexity and scalability  

Misconfigurations are one of the leading causes of cloud security incidents.

Effective cloud security focuses on:

- Secure configuration of services  
- Access control and identity management  
- Monitoring and detection  
- Infrastructure as Code (IaC) governance  

---

## Risk Evaluation Model

Risk Score = Likelihood (1–5) × Impact (1–5)

Additional factors:

- Internet exposure  
- Privilege level  
- Data sensitivity  

---

## Key Risk Scenarios

---

### 1. Publicly Exposed Storage (e.g., S3 Bucket)

**Description**  
Sensitive data is exposed due to misconfigured access settings.

**Risks**

- Data leakage  
- Regulatory violations  
- Reputation damage  

**Assessment**

| Factor      | Rating |
|------------|--------|
| Impact     | High   |
| Likelihood | High   |
| Risk Score | 20     |

**Business Impact**  
Sensitive customer or company data becomes publicly accessible.

---

### 2. Overprivileged Cloud IAM Roles

**Description**  
Cloud identities have excessive permissions.

**Risks**

- Privilege escalation  
- Unauthorized access  
- Full environment compromise  

**Assessment**

| Factor      | Rating |
|------------|--------|
| Impact     | High   |
| Likelihood | Medium–High |
| Risk Score | 15–20 |

**Business Impact**  
Attackers can control cloud infrastructure after initial compromise.

---

### 3. Missing Logging & Monitoring

**Description**  
Insufficient logging in cloud environments.

**Risks**

- Undetected attacks  
- Delayed incident response  

**Assessment**

| Factor      | Rating |
|------------|--------|
| Impact     | High   |
| Likelihood | Medium |
| Risk Score | 12     |

**Business Impact**  
Security incidents remain unnoticed until damage is done.

---

## Example Risk Mapping

| Risk ID | Description                      | Likelihood | Impact | Score | Control                     |
|--------|----------------------------------|-----------|--------|-------|-----------------------------|
| R-20   | Public S3 bucket                 | 4         | 5      | 20    | Secure Configuration        |
| R-21   | Overprivileged IAM roles         | 4         | 4      | 16    | Least Privilege             |

---

## Control Mapping (ISO 27001 aligned)

- Access Control (IAM / Least Privilege)  
- Secure Configuration Management  
- Logging & Monitoring  
- Infrastructure as Code Governance  

---

## Example Scenario

A cloud storage service is misconfigured and publicly accessible.

An attacker discovers the service via automated scanning.

Because access restrictions are missing:

- sensitive data is exposed  
- data can be downloaded without authentication  

Because logging is insufficient:

- access is not detected  

**Result**

Data breach due to misconfiguration and lack of monitoring.

---

## Management Decision Example

Risk: Publicly exposed cloud storage  
Residual Risk: High  

Options:

1. Accept risk  
2. Restrict public access  
3. Implement automated configuration checks  

Decision:

→ **Restrict access and implement continuous configuration monitoring**

Rationale:

High impact on confidentiality + regulatory exposure  
(ISO 27001 A.5 / A.8)

---

## Governance Perspective

Cloud security requires coordination between:

- Security (policies & controls)  
- Cloud / DevOps (implementation)  
- Management (risk prioritization)  

---

## Conclusion

Cloud misconfiguration risks can lead to immediate and severe security incidents.

Proper governance enables:

- secure-by-default configurations  
- continuous monitoring  
- scalable security controls  

Cloud security is not a tool problem, but a governance and process challenge.
