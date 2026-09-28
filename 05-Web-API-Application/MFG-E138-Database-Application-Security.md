---
docType: guide
answerType: guide
guideType: pentest
knowledgeId: MFG-E138
sector: manufacturing_industrial
phase: Web / API / Application / Infrastructure
assetTags: ["data"]
safety: controlled
---

# MFG-E138: Database Application Security

## Question

How should an authorized manufacturing-sector VAPT auditor assess **Database Application Security**?

## Description

Standardized manufacturing VAPT guidance for the **Web / API / Application / Infrastructure** domain/phase. This unit is reusable methodology, not authorization to test a particular organization.

## Content

### Overview

Confirm scope, ownership, business function, environment (production/test/lab), dependencies and safety constraints before assessment. Use the least disruptive technique that can answer the security question.

### Assessment Objectives

1. **Authentication/Session** — identify the applicable control, observation or test and document the result.
2. **Authorization/Object Access** — identify the applicable control, observation or test and document the result.
3. **Input Validation** — identify the applicable control, observation or test and document the result.
4. **Business Logic** — identify the applicable control, observation or test and document the result.
5. **File/Data Handling** — identify the applicable control, observation or test and document the result.
6. **Configuration/Logging** — identify the applicable control, observation or test and document the result.

### Manufacturing Context

Consider relationships among enterprise IT, identity, ERP/business applications, manufacturing operations, engineering/IP, OT/ICS, IIoT/edge, cloud, remote access, suppliers and sensitive data.

### Scope & Preconditions

| Requirement | Minimum expectation |
|---|---|
| Authorization | Written authorization and explicit asset scope |
| Ownership | Business/technical owner identified |
| Environment | Production/test/lab status recorded |
| Accounts | Test accounts preferred where authentication is assessed |
| Data | Minimize collection and protect evidence |
| Safety | controlled; OT actions require additional safety controls |

### Evidence

- Asset identifier and environment.
- Relevant URL/IP/hostname/logical identifier where permitted.
- Observed technology/configuration.
- Authentication or authorization context where applicable.
- Screenshot, log, request/response or configuration excerpt when needed.
- Timestamp and tester action.
- Business/operational context.

### Expected Output

- Assessment coverage.
- Observations and findings with evidence.
- Technical, business and operational impact where supported.
- Remediation or compensating control.
- Retest requirement where applicable.

### Safety / Stop Conditions

- Stop if an action may affect production availability, safety, physical process control or data integrity.
- No denial-of-service, destructive exploitation, uncontrolled malware, intentional data deletion or unsafe OT manipulation unless separately authorized and safety-controlled.
- For OT/ICS, prefer passive/read-only validation and lab/digital-twin validation for disruptive actions.
- Escalate instability, alarms, process changes or safety concerns.

### Common Pitfalls

- Treating a software version as proof of a vulnerability.
- Assuming every manufacturer has the same architecture.
- Confusing exposure with compromise.
- Ignoring business/operational context.
- Testing production OT like ordinary IT.
- Storing client evidence or secrets in this reusable repository.

### Related Knowledge

Use the catalog to retrieve related units by asset, phase, technology and business function.

### Standards / References

- OWASP WSTG
- OWASP Top 10
- OWASP API Security
