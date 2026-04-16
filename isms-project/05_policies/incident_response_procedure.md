## Incident Response Procedure

---

### Objective

This procedure defines the operational steps for handling security incidents.

It complements the Incident Response Policy by translating high-level principles into actionable tasks and responsibilities during an incident.

---

### Incident Classification

Incidents are classified based on their impact and urgency:

| Severity | Description | Example |
|----------|------------|--------|
| Low      | Limited impact, isolated issue | Single endpoint infection |
| Medium   | Noticeable disruption | Partial system outage |
| High     | Significant business impact | Multiple systems affected |
| Critical | Severe disruption of operations | Ransomware, production downtime |

---

### Response Timeline

The following target timelines apply under normal conditions:

| Phase        | Target Time |
|--------------|------------|
| Detection    | Immediate |
| Assessment   | < 1 hour |
| Containment  | < 4 hours |
| Recovery     | < 24 hours |

Actual timelines may vary depending on incident complexity and available information.

---

### Roles During Incident

| Role                     | Responsibility |
|--------------------------|----------------|
| IT Operations            | Technical containment and recovery |
| Incident Response Lead   | Coordination and prioritization |
| Security Lead / CISO     | Strategic decisions and escalation |
| Management               | Business impact decisions |
| Legal / Compliance       | Regulatory evaluation |
| Communication            | Internal and external communication |

---

### Step-by-Step Procedure

#### 1. Detection

- identify abnormal system behavior through monitoring or user reports  
- validate whether the event qualifies as a security incident  

---

#### 2. Initial Assessment

- determine scope and affected systems  
- estimate potential business impact  
- classify incident severity  

---

#### 3. Containment

- isolate affected systems from the network  
- disable compromised accounts  
- prevent further spread across systems  

Containment is prioritized over immediate recovery to limit overall impact.

---

#### 4. Investigation

- analyze logs and system behavior  
- identify root cause and attack vector  
- determine whether data exposure occurred  

At this stage, information may be incomplete and subject to change.

---

#### 5. Recovery

- restore systems from verified backups  
- validate system integrity before reconnecting  
- gradually resume operations  

Production systems are prioritized (target RTO: 4 hours where applicable).

---

#### 6. Communication

- inform internal stakeholders (management, affected teams)  
- prepare external communication if required  
- coordinate with legal regarding regulatory obligations  

---

#### 7. Escalation

Escalation is required if:

- multiple critical systems are affected  
- data exposure is suspected  
- business operations are significantly disrupted  

→ escalation to Crisis Management Team  

---

#### 8. Post-Incident Review

- document timeline, actions, and decisions  
- identify gaps in response and controls  
- integrate findings into risk management and process improvements  

---

### Decision-Making Principles

During the response, decisions are guided by:

- prioritization of business-critical systems  
- containment of further damage before recovery  
- balancing speed and system integrity  
- operating under incomplete information  

---

### Practical Consideration

In real incidents, response activities do not always follow a strict sequence.

Parallel actions, changing priorities, and uncertainty are typical and require continuous reassessment.
