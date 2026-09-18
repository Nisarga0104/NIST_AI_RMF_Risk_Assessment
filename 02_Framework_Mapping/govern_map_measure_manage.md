# NIST AI RMF Function-by-Function Mapping

## 1. GOVERN

**Purpose in this assessment:** create the accountability structure that makes AI risk management repeatable.

### Portfolio implementation

- **Governance body:** AI Governance Committee comprising Risk, Legal/Privacy, Technology, Customer Experience, and Internal Audit.
- **Business accountability:** Head of Customer Experience is the Business Owner.
- **Risk accountability:** a named AI Risk Owner in the Risk function owns ongoing monitoring and escalation.
- **Policy connection:** the Responsible AI Policy in Project 3 provides the internal risk-classification mechanism.
- **Incident escalation:** customer harm, financially consequential factual error, or suspected security incident is escalated to the AI Risk Owner.
- **Third-party oversight:** the third-party LLM relationship requires documented vendor governance rather than reliance on vendor assurances alone.

### Evidence artifacts

- `04_Governance/governance_structure.md`
- `04_Governance/governance_decision.md`
- `05_Controls/control_matrix.md`

---

## 2. MAP

**Purpose in this assessment:** establish the system context, intended purpose, stakeholders, data, dependencies, and foreseeable risks.

### Intended purpose

Reduce customer wait times and deflect routine customer-service queries.

### Stakeholders

- Retail customers
- Customer-service staff
- RBI and other regulators
- Board and shareholders
- Risk, Legal/Privacy, Technology, and Internal Audit functions
- Third-party LLM provider

### System/data context

The agent uses:
- read-only customer account data;
- product/FAQ knowledge;
- session conversation history;
- a third-party LLM API;
- Northstar's internal customer-data platform.

### Foreseeable risks

1. Hallucination
2. Prompt injection
3. Privacy / PII exposure
4. Over-reliance and insufficient human oversight
5. Model/knowledge drift
6. Unauthorized transaction initiation

The last risk is intentionally constrained by the system's **read-only capability boundary**.

---

## 3. MEASURE

**Purpose in this assessment:** assess identified risks using documented qualitative judgments and define what should be monitored.

### Risk assessment method

Likelihood and impact are rated as Low / Medium / High, with Severe used for the potential impact of unauthorized transaction initiation. The exercise explicitly describes these as reasoned qualitative judgments rather than statistical probabilities.

### Monitoring themes

- Hallucination / factual-error rate
- Escalation appropriateness
- PII-handling compliance
- Prompt-injection indicators
- Knowledge-base freshness
- Disputed interaction reconstruction
- Subgroup / accuracy performance where applicable

### Measurement evidence

The risk register translates these themes into owners, controls, monitoring indicators, and residual-risk fields.

---

## 4. MANAGE

**Purpose in this assessment:** prioritize risks, implement treatment, accept residual risk explicitly, and determine whether deployment should proceed.

### Preventive treatment

- Read-only scope enforcement
- Input/output filtering
- Data minimization
- Pre-deployment adversarial testing
- Accuracy benchmarking

### Detective treatment

- Sampled conversation review
- Restricted audit logging
- Anomaly detection

### Corrective treatment

- Human escalation
- Incident response
- Knowledge-base and version management

### Deployment decision

The final assessment records **Approve with Conditions**, subject to the stated controls and completion of the separate RBI / regulatory review.

This is a risk-management judgment for the fictional case study, not a legal compliance conclusion.

---

## Continuous cycle

The repository treats NIST AI RMF as a lifecycle process:

**Govern → Map → Measure → Manage → Monitor → Reassess**

A material scope change — especially adding transaction authority — should trigger a new Map/Measure cycle rather than being treated as a minor feature update.
