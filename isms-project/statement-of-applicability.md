# Statement of Applicability (SoA)

## Objective
Define applicable ISO 27001 controls and justify their inclusion based on identified risks.

## Scope
Mid-sized automotive supplier with focus on production systems, office IT, and supplier integration.

---

## Control Selection Overview

| Control Area              | Included | Justification                                      |
|---------------------------|----------|----------------------------------------------------|
| Access Control            | Yes      | Protection of sensitive systems and data           |
| Backup & Recovery         | Yes      | Mitigation of ransomware and system failures       |
| Incident Management       | Yes      | Required for structured incident handling          |
| Supplier Security         | Yes      | Strong dependency on external suppliers            |
| Asset Management          | Yes      | Identification of critical systems                 |
| Cryptography              | No       | Not critical in current simplified scenario        |
| Physical Security         | No       | Out of scope for this project                      |

---

## Mapping to Implemented Controls

| Control Area        | Implementation                              |
|--------------------|----------------------------------------------|
| Access Control     | access-control-policy.md                     |
| Backup             | backup-policy.md                             |
| Incident Response  | incident-response-policy.md                  |
| Supplier Security  | Risk Assessment + contractual measures       |

---

## Summary

The selected controls reflect the main risk drivers:
- Production downtime
- Human error (phishing)
- Supplier dependencies

The SoA ensures alignment between identified risks and implemented controls.
