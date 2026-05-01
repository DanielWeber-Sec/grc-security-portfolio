```txt
████████╗███████╗ ██████╗██╗  ██╗███╗   ██╗██╗ ██████╗ █████╗ ██╗     
╚══██╔══╝██╔════╝██╔════╝██║  ██║████╗  ██║██║██╔════╝██╔══██╗██║     
   ██║   █████╗  ██║     ███████║██╔██╗ ██║██║██║     ███████║██║     
   ██║   ██╔══╝  ██║     ██╔══██║██║╚██╗██║██║██║     ██╔══██║██║     
   ██║   ███████╗╚██████╗██║  ██║██║ ╚████║██║╚██████╗██║  ██║███████╗
   ╚═╝   ╚══════╝ ╚═════╝╚═╝  ╚═╝╚═╝  ╚═══╝╚═╝ ╚═════╝╚═╝  ╚═╝╚══════╝

 ██████╗ ██████╗ ███╗   ██╗████████╗███████╗██╗  ██╗████████╗
██╔════╝██╔═══██╗████╗  ██║╚══██╔══╝██╔════╝╚██╗██╔╝╚══██╔══╝
██║     ██║   ██║██╔██╗ ██║   ██║   █████╗   ╚███╔╝    ██║   
██║     ██║   ██║██║╚██╗██║   ██║   ██╔══╝   ██╔██╗    ██║   
╚██████╗╚██████╔╝██║ ╚████║   ██║   ███████╗██╔╝ ██╗   ██║   
 ╚═════╝ ╚═════╝ ╚═╝  ╚═══╝   ╚═╝   ╚══════╝╚═╝  ╚═╝   ╚═╝   
```

# Technical Context

## Objective

This section demonstrates how technical security domains are translated into structured risks, governance decisions, and ISO 27001-aligned controls.

It extends the ISMS foundation by connecting policies and risk management with real-world technical security challenges.

---

## Scope

The following domains are covered:

- **Identity and Access Management (IAM)**  
- **Vulnerability Management**  
- **Cloud Security & Misconfiguration Risks**  

---

## Approach

Each document follows a consistent methodology:

1. Identify relevant technical risks  
2. Assess likelihood and impact  
3. Translate risks into structured governance decisions  
4. Map risks to ISO 27001-aligned controls  
5. Define practical risk treatment strategies  

---

## Key Idea

Technical risks are not isolated problems.

They must be translated into:

- Business risk  
- Governance decisions  
- Control requirements  
- Risk treatment actions  

---

## Example System Context

- Active Directory (IAM)  
- Cloud Environment (AWS)  
- Web Application (Customer Portal)  
- Database (Customer Data)  

Trust Boundaries:

- Internal Network  
- Public Internet  

---

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

---

## End-to-End Risk Scenario

### Scenario Overview

A compromised user account leads to a full system compromise across multiple layers.

---

### Step 1 – Initial Access (IAM Failure)

A user account without MFA is compromised.

- Weak authentication  
- Excessive privileges  

---

### Step 2 – Persistence

The attacker creates additional accounts and maintains access.

- No access reviews  
- No monitoring  

---

### Step 3 – Lateral Movement

The attacker moves across systems.

- Shared credentials  
- Overprivileged access  

---

### Step 4 – Exploitation (Vulnerability Failure)

Unpatched systems are exploited.

- Known vulnerabilities  
- Missing patching  

---

### Step 5 – Data Exfiltration

Sensitive data is extracted.

- No monitoring  
- No anomaly detection  

---

### Step 6 – Business Impact

- Data breach  
- Service disruption  
- Compliance violations  

---

## Governance Relevance

The purpose of this section is not to demonstrate deep technical engineering.

It shows how technical security risks can be translated into:

- Business risk  
- Governance decisions  
- Control requirements  
- Risk treatment actions  
- Audit-ready documentation  

---

## Positioning

This section highlights a hybrid skillset:

- Understanding of technical security domains  
- Ability to translate technical issues into risk-based decisions  
- Alignment with ISMS and compliance frameworks  
- Communication between technical teams and management  

The focus is:

**Technical credibility combined with governance expertise.**

---

## Summary

This section strengthens the ISMS project by adding technical depth.

It shows that security governance is not only about policies and documentation, but about understanding the technical realities behind the risks.

The goal is to make security decisions understandable, structured, and actionable.
