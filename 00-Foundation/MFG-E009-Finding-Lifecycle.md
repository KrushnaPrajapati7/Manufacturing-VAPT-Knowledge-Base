---
docType: knowledge_unit
knowledgeId: E009
sector: manufacturing_industrial
phase: Foundation
topic: VAPT Risk and Finding Decision Model
safety: controlled
status: working-rebuild
---

# E009: VAPT Risk and Finding Decision Model

## Assessment Question

**How does the assessor convert technical evidence into a defensible manufacturing risk decision without overstating severity or confusing technical weakness with business impact?**

## Purpose

E009 provides the reasoning model used after technical observation.

It deliberately avoids a universal scoring formula. CVSS or another organizational model may be used when required, but manufacturing impact must still be interpreted in context.

NIST IR 8183 Rev. 1 provides a manufacturing-specific, voluntary, risk-based cybersecurity framework profile.

## 1. Finding Chain

Observation → Validation → Security Requirement → Exploit/Misuse Capability → Affected Asset → Manufacturing Dependency → Impact → Exposure → Finding → Remediation → Retest

Each link should be supported by evidence or clearly marked as an assumption or limitation.

## 2. Observation Is Not Automatically a Finding

Examples:

- open port → observation;
- detected version → observation;
- weak configuration → potential weakness;
- confirmed exploitable condition → vulnerability evidence;
- vulnerability affecting a critical production dependency → manufacturing relevance;
- vulnerability with no meaningful path or exposure → may require different treatment.

## 3. Impact Dimensions

Consider separately:

- confidentiality;
- integrity;
- availability;
- safety relevance;
- production continuity;
- product quality;
- traceability;
- engineering/IP;
- recovery effort;
- regulatory/customer dependency;
- propagation potential.

Do not claim safety impact without evidence and appropriate domain input.

## 4. Exposure Dimensions

Consider:

- internet exposure;
- enterprise exposure;
- OT-zone exposure;
- remote-access exposure;
- authentication requirement;
- privilege required;
- reachable assets;
- attack-path dependencies;
- monitoring/detection;
- compensating controls.

## 5. Manufacturing Risk Statement

A useful statement has the form:

A validated condition on [asset/function] allows [capability], which can affect [process/dependency] under [conditions]. Evidence is [confidence] and limitations are [limitations].

This is stronger than assigning a number without context.

## 6. Offensive Questions

- What can an attacker actually achieve?
- What prerequisite access is required?
- What trust boundary must be crossed?
- What privilege is needed?
- Can the capability persist?
- Can it reach another asset?
- Can it influence production or sensitive information?

MITRE ATT&CK for ICS can help describe adversary objectives such as Initial Access, Lateral Movement, Impair Process Control and Impact.

## 7. Defensive Questions

- Would the activity be detected?
- What control would stop it?
- What telemetry exists?
- Is the affected asset monitored?
- Can the organization contain the path?
- Can the process recover?

## 8. Decision States

Use explicit states:

- Confirmed finding;
- Validated weakness;
- Observation;
- Inconclusive;
- Not tested;
- Not applicable;
- Out of scope.

Do not force every observation into a vulnerability category.

## 9. Severity

If an engagement requires CVSS, use the applicable CVSS version and document the vector and assumptions.

Do not modify a standard score simply to make it represent manufacturing impact.

Instead provide a separate manufacturing impact statement or the organization's defined risk rating.

## 10. Root Cause

Where evidence permits, distinguish:

- configuration error;
- architecture/design issue;
- identity/access-control weakness;
- lifecycle issue;
- unsupported/obsolete technology;
- monitoring gap;
- governance/process deficiency;
- supplier dependency;
- implementation defect.

Do not claim root cause if the assessment did not establish it.

## 11. Remediation

Remediation should address the underlying control or design issue.

Possible classes:

- remove unnecessary exposure;
- restrict access;
- segment;
- strengthen authentication;
- reduce privilege;
- update/patch where operationally appropriate;
- compensate where patching is unsafe;
- improve monitoring;
- improve backup/recovery;
- change supplier access;
- improve lifecycle management.

OT remediation must consider operational constraints.

## 12. Retest Logic

A retest should answer the original security question.

Verify:

- original condition;
- relevant alternate path;
- intended control;
- monitoring behavior where relevant;
- no unacceptable operational side effect.

A screenshot of a changed setting is not automatically proof that the attack path is closed.

## 13. Finding Evidence Template

| Field | Required question |
|---|---|
| Asset | What is affected? |
| Condition | What was observed? |
| Requirement | What should happen? |
| Validation | How was it confirmed? |
| Capability | What can an unauthorized party do? |
| Dependency | What process relies on it? |
| Impact | What can reasonably result? |
| Exposure | Who can reach it and how? |
| Detection | Would the organization detect it? |
| Root cause | What caused the weakness? |
| Remediation | What should change? |
| Retest | How will closure be verified? |

## Exit Criteria

The finding is decision-ready when a reviewer can independently understand the evidence, attack path, manufacturing relevance, limitations and remediation.

## Sources

- NIST IR 8183 Rev. 1.
- NIST SP 800-82 Rev. 3.
- MITRE ATT&CK for ICS.

**Boundary:** E009 owns the finding/risk decision model. It does not own authorization, safety approval or evidence storage.
