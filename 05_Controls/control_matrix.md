# AI Control Matrix

| Control ID | Risk addressed | Control | Type | Owner | Evidence | Frequency |
|---|---|---|---|---|---|---|
| C-01 | Unauthorized actions | System-level read-only permissions; no transaction capability | Preventive | Technology / Security | Permission test results | Before release + change events |
| C-02 | Prompt injection | Adversarial prompt-injection red-team testing | Preventive / Detective | Security | Test report and remediation log | Pre-release + material changes |
| C-03 | PII exposure | Data minimization and restricted log access | Preventive | Privacy / Security | Access review, data-flow record | Continuous + periodic review |
| C-04 | Hallucination | Curated accuracy benchmark and sampled conversation review | Preventive / Detective | Business Owner / Risk | Evaluation results, QA samples | Pre-release + ongoing |
| C-05 | Over-reliance | Human escalation for out-of-scope queries and dissatisfaction | Corrective | Customer Experience | Escalation records | Continuous |
| C-06 | Security / misuse | Input/output filtering and anomaly detection | Preventive / Detective | Security | Alerts and test results | Continuous |
| C-07 | Drift | Knowledge-base version and change control | Preventive | Technology / Business Owner | Change records | On every material update |
| C-08 | Incident harm | Containment, customer remediation and root-cause process | Corrective | AI Risk Owner | Incident records | Event-driven |
| C-09 | Third-party risk | Vendor governance and assurance evidence | Preventive / Detective | Procurement / Risk | Vendor assessment | Pre-contract + periodic |
| C-10 | Regulatory exposure | Separate legal/compliance review for RBI and DPDP applicability | Preventive | Legal / Compliance | Review record | Before release + regulatory change |

## Control design principle

Controls are layered. A single safeguard should not be treated as sufficient for a high-impact failure mode where multiple independent controls are practical.
