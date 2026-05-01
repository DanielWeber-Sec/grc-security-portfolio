# Cloud Security & Misconfiguration Risk Model

## Objective

This document demonstrates how cloud security risks, especially misconfigurations, are identified, assessed, and translated into structured risks, governance decisions, and ISO 27001-aligned controls.

---

## Context

Cloud environments (AWS, Azure, GCP) introduce a shared responsibility model.

Many critical incidents are not caused by sophisticated attacks, but by:

- Misconfigured services  
- Excessive permissions  
- Lack of visibility  
- Missing monitoring  

Cloud security failures often result in immediate external exposure.

---

## Risk Evaluation Model

Risk Score = Likelihood (1–5) × Impact (1–5)

Additional factors:

- Exposure (public / internal)  
- Data sensitivity  
- Attack surface  
- Automation maturity  

---

## Key Risk Scenarios

---

### 🌍 1. Publicly Exposed Storage / Services

**Description**  
Cloud storage (e.g., S3 buckets, Blob storage) or services are publicly accessible.

**Risks**
- Data leakage  
- Unauthorized downloads  
- Reputation damage  

**Assessment**

| Factor      | Rating |
|------------|--------|
| Impact     | High   |
| Likelihood | High   |
| Risk Score | 20     |

**Business Impact**  
Sensitive data becomes publicly accessible on the internet.

---

### 🔑 2. Excessive Cloud IAM Permissions

**Description**  
Users or services have overly broad permissions (e.g., admin roles).

**Risks**
- Privilege escalation  
- Full account compromise  
- Lateral movement  

**Assessment**

| Factor      | Rating |
|------------|--------|
| Impact     | High   |
| Likelihood | High   |
| Risk Score | 20     |

**Business Impact**  
Compromised credentials lead to full cloud environment takeover.

---

### 🧱 3. Misconfigured Network Security (Security Groups / Firewall)

**Description**  
Security groups or firewall rules allow unrestricted access (e.g., 0.0.0.0/0).

**Risks**
- Direct exposure of services  
- Brute force attacks  
- Exploitation of vulnerabilities  

**Assessment**

| Factor      | Rating |
|------------|--------|
| Impact     | High   |
| Likelihood | Medium–High |
| Risk Score | 15–20       |

**Business Impact**  
Critical services are exposed to the public internet.

---

### 📡 4. Missing Logging and Monitoring

**Description**  
Cloud logs (e.g., CloudTrail, Azure Monitor) are not enabled or not reviewed.

**Risks**
- Attacks go undetected  
- No forensic capability  
- Delayed response  

**Assessment**

| Factor      | Rating |
|------------|--------|
| Impact     | High   |
| Likelihood | High   |
| Risk Score | 20     |

**Business Impact**  
Security incidents remain unnoticed, increasing damage.

---

### 🔄 5. Lack of Configuration Management

**Description**  
No standardized or automated configuration baseline (e.g., Infrastructure as Code).

**Risks**
- Drift from secure baseline  
- Inconsistent environments  
- Repeated misconfigurations  

**Assessment**

| Factor      | Rating |
|------------|--------|
| Impact     | Medium–High |
| Likelihood | High        |
| Risk Score | 15–20       |

**Business Impact**  
Security posture degrades over time without visibility.

---

## Example Risk Mapping

| Risk ID | Description | Likelihood | Impact | Score | Control |
|--------|------------|-----------|--------|------|--------|
| R-20 | Public S3 bucket exposure | 4 | 5 | 20 | Access Restrictions, Monitoring |
| R-21 | Excessive IAM permissions | 4 | 5 | 20 | Least Privilege, IAM Policies |

---

## Control Mapping (ISO 27001 aligned)

- Access Control (IAM)  
- Network Security Controls  
- Logging and Monitoring  
- Configuration Management  
- Asset Management  

Cloud-specific practices:

- Least privilege IAM  
- Secure defaults  
- Continuous monitoring  
- Infrastructure as Code (IaC)  
- CSPM (Cloud Security Posture Management)  

---

## Example Scenario

A cloud storage bucket is accidentally configured as public.

The bucket contains sensitive internal documents.

An attacker discovers the bucket via automated scanning tools.

Because:

- no access restrictions are enforced  
- no monitoring is in place  

the attacker is able to:

- download sensitive data  
- remain undetected  

**Result**  
Data breach caused by simple misconfiguration.

---

## Governance Perspective

Cloud security requires alignment between:

- Cloud Engineering (implementation)  
- Security (policies & controls)  
- DevOps (automation & deployment)  
- Management (risk ownership)  

---

## Conclusion

Cloud security is not only about infrastructure.

It is about managing:

- configuration risks  
- access risks  
- visibility  

Misconfigurations are one of the fastest ways to create critical security incidents.

A structured, risk-based approach is essential.
