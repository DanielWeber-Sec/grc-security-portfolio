# IAM Risk Model

## Objective

This document demonstrates how Identity and Access Management (IAM) risks are identified, assessed, and translated into structured risks, governance decisions, and ISO 27001-aligned controls.

---

## Context

IAM is a critical control layer that determines who can access which systems and data.

Failures in IAM directly lead to:

- Unauthorized access
- Privilege escalation
- Insider threats
- Compliance violations

---

## Risk Evaluation Model

Risk Score = Likelihood (1–5) × Impact (1–5)

---

## Risk Evaluation Approach

... dein bestehender Content ...

## Management Decision Example

Risk: Missing MFA on critical systems  
Residual Risk: High  

Options:

1. Accept risk  
2. Implement MFA (cost: medium)  
3. Restrict access (impact: high)  

Decision:

→ Implement MFA for all privileged accounts  

Rationale:

High impact + regulatory relevance (ISO 27001 A.5 / A.8)
## Key Risk Scenarios

---

###  1. Excessive Privileges

**Description**  
Users or service accounts have more permissions than required.

**Risks**
- Unauthorized data access  
- Increased impact of compromised accounts  
- Insider misuse  

**Assessment**

| Factor      | Rating |
|------------|--------|
| Impact     | High   |
| Likelihood | Medium |
| Risk Score | 15     |

**Business Impact**  
Compromise of high-value systems due to excessive permissions.

---

###  2. Missing Joiner-Mover-Leaver Process

**Description**  
User access is not updated when employees join, change roles, or leave.

**Risks**
- Orphaned accounts  
- Unauthorized continued access  
- Compliance violations  

**Assessment**

| Factor      | Rating |
|------------|--------|
| Impact     | High   |
| Likelihood | High   |
| Risk Score | 20     |

**Business Impact**  
Former employees retain access to internal systems and sensitive data.

---

###  3. Weak Authentication Mechanisms

**Description**  
Systems rely on weak authentication (e.g., no MFA).

**Risks**
- Account takeover  
- Unauthorized system access  

**Assessment**

| Factor      | Rating |
|------------|--------|
| Impact     | High   |
| Likelihood | High   |
| Risk Score | 20     |

**Business Impact**  
Attackers gain access to critical systems via compromised credentials.

---

###  4. Lack of Access Reviews

**Description**  
User permissions are not regularly reviewed.

**Risks**
- Privilege creep  
- Uncontrolled access growth  

**Assessment**

| Factor      | Rating |
|------------|--------|
| Impact     | Medium–High |
| Likelihood | High        |
| Risk Score | 15–20       |

**Business Impact**  
Unnecessary access accumulates over time, increasing risk exposure.

---

## Example Risk Mapping

| Risk ID | Description | Likelihood | Impact | Score | Control |
|--------|------------|-----------|--------|------|--------|
| R-01 | Excessive admin privileges | 3 | 5 | 15 | RBAC, Access Reviews |
| R-02 | Missing MFA on critical systems | 4 | 5 | 20 | MFA Enforcement |

---

## Control Mapping (ISO 27001 aligned)

- Access Control Policy  
- User Access Management  
- Privileged Access Management  
- Authentication Controls (MFA)  
- Access Review Procedures  
- Logging and Monitoring  

---

## Example Scenario

A compromised user account with excessive privileges gains access to a production system.

Because no MFA is implemented and access reviews are missing, the attacker is able to:

- escalate privileges  
- access sensitive data  
- remain undetected  

**Result**  
Full system compromise due to combined IAM control failures.

---

## Governance Perspective

IAM requires coordination between:

- HR (identity lifecycle)
- IT (account provisioning)
- Security (policies & monitoring)
- Management (risk ownership)

---

## Conclusion

IAM is not just a technical topic.

It is a governance-critical domain that directly impacts:

- business risk
- compliance
- operational security
