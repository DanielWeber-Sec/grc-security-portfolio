# IAM Risk Model

## Objective

This document demonstrates how Identity and Access Management (IAM) risks are identified, assessed, and translated into structured risks, governance decisions, and ISO 27001-aligned controls.

The goal is to ensure that access to systems and data is appropriate, controlled, and continuously validated.

---

## Context

IAM is a critical security domain because it directly controls who can access which systems and data.

Weak IAM practices are a leading cause of:

- Unauthorized access to sensitive information
- Privilege escalation and lateral movement
- Insider threats and misuse of access rights
- Compliance violations (e.g., ISO 27001, GDPR)

Effective IAM is therefore a cornerstone of any Information Security Management System (ISMS).

---

## Key Risk Scenarios

### 1. Excessive Privileges

**Description**  
Users or service accounts have more permissions than required.

**Risk**  
- Unauthorized access to sensitive data  
- Increased impact of compromised accounts  
- Higher risk of insider misuse  

**Example**  
A developer retains administrative access to production systems.

**Impact**  
High

**Likelihood**  
Medium

---

### 2. Missing Joiner-Mover-Leaver Process

**Description**  
User access is not properly updated when employees join, change roles, or leave the organization.

**Risk**  
- Orphaned accounts  
- Unauthorized continued access  
- Compliance violations  

**Example**  
A former employee still has access to internal systems via VPN.

**Impact**  
High

**Likelihood**  
High

---

### 3. Weak Authentication Mechanisms

**Description**  
Systems rely on weak authentication (e.g., no MFA).

**Risk**  
- Account takeover via phishing or credential stuffing  
- Unauthorized system access  

**Example**  
Critical applications are accessible with password-only authentication.

**Impact**  
High

**Likelihood**  
High

---

### 4. Lack of Access Reviews

**Description**  
User permissions are not regularly reviewed and validated.

**Risk**  
- Privilege creep over time  
- Accumulation of unnecessary access rights  

**Example**  
Users retain access to systems they no longer need.

**Impact**  
Medium–High

**Likelihood**  
High

---

## Risk Evaluation Approach

Risk scoring is based on:

- Likelihood (1–5)  
- Impact (1–5)  

Risk Score = Likelihood × Impact

Additional factors may include:

- Privilege level (standard vs. admin)
- System criticality
- Exposure (internal vs. external)

---

## Control Mapping (ISO 27001 aligned)

Relevant controls include:

- **Access Control Policy**
- **User Access Management**
- **Privileged Access Management**
- **Authentication Controls (e.g., MFA)**
- **Access Review Procedures**
- **Logging and Monitoring of Access Activities**

---

## Risk Treatment Strategy

### Preventive Controls
- Enforce least privilege (Role-Based Access Control)
- Implement Multi-Factor Authentication (MFA)
- Define and enforce Joiner-Mover-Leaver processes

### Detective Controls
- Regular access reviews
- Monitoring of privileged account activity
- Logging and SIEM integration

### Corrective Controls
- Immediate deprovisioning of unauthorized accounts
- Incident response for compromised identities
- Remediation of misconfigured access rights

---

## Governance Perspective

IAM is not only a technical topic but a governance challenge.

It requires coordination between:

- HR (identity lifecycle)
- IT (account provisioning)
- Security (policy and monitoring)
- Management (risk ownership)

Clear ownership, defined processes, and accountability are essential.

---

## Conclusion

Effective IAM reduces some of the most critical security risks.

By translating access-related issues into structured risks and controls, IAM becomes a key component of:

- Information Security Governance
- Risk Management
- Compliance (ISO 27001, GDPR, NIS2)

This approach enables proactive, risk-based decision-making instead of reactive access control.
