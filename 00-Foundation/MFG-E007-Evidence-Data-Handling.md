---
docType: knowledge_unit
knowledgeId: E007
sector: manufacturing_industrial
phase: Foundation
topic: Evidence and Data Handling
safety: controlled
status: working-rebuild
---

# E007: Evidence and Data Handling

## Assessment Question

**Can every important assessment conclusion be supported by sufficient, attributable and appropriately protected evidence without collecting unnecessary manufacturing data?**

## Purpose

E007 establishes evidence discipline for VAPT.

Manufacturing evidence can contain credentials, personal information, engineering drawings, PLC logic, recipes, production data, network architecture and proprietary information. The assessor should collect what is necessary to prove the assessment result—not everything technically available.

## 1. Evidence Chain

Use:

Assessment Question → Observation → Evidence → Interpretation → Finding → Remediation → Retest Evidence

Evidence must support the claim actually being made.

## 2. Evidence Types

Examples:

- screenshots;
- configuration extracts;
- logs;
- request/response pairs;
- packet metadata;
- firewall rules;
- authentication records;
- cloud configuration;
- vulnerability scanner output;
- command output;
- architecture diagrams;
- interviews;
- controlled test results.

Tool output is evidence only to the extent that it supports the conclusion.

## 3. Evidence Quality

Good evidence should be:

- attributable;
- time-associated;
- relevant;
- understandable;
- reproducible where practical;
- minimally collected;
- protected from unauthorized disclosure or alteration.

## 4. Manufacturing-Sensitive Evidence

Treat carefully:

- PLC logic;
- controller configuration;
- recipes;
- CAD/design files;
- production quantities;
- quality records;
- maintenance records;
- engineering credentials;
- network diagrams;
- remote-access configuration;
- packet captures;
- personal information;
- vendor confidential material.

Never copy client evidence into this reusable public knowledge base.

## 5. Evidence Minimization

Before collecting an item ask:

**What claim will this evidence prove?**

If there is no clear answer, collection may not be necessary.

Prefer a redacted configuration excerpt over a complete export when the complete export adds no evidentiary value.

## 6. Integrity

The engagement evidence process may define:

- hashes;
- timestamps;
- access control;
- chain of custody;
- versioning;
- retention;
- transfer method.

The KB should explain these concepts but must not prescribe one universal legal chain-of-custody process.

## 7. Finding Evidence

A finding should normally connect:

Condition → Expected Control/Requirement → Evidence → Security Consequence → Manufacturing Relevance

Avoid unsupported statements such as:

“This is critical because it is an OT device.”

## 8. Negative Evidence

Record important negative results.

Examples:

- test did not reproduce;
- exploit path was blocked;
- monitoring generated an alert;
- access was denied;
- scope prevented validation;
- evidence was insufficient.

Negative results prevent the report from overstating risk.

## 9. Evidence Confidence

Use practical labels:

- confirmed;
- strongly supported;
- partially supported;
- inconclusive;
- not tested.

Do not turn confidence into fake mathematical precision.

## 10. Offensive Questions

- What minimum evidence proves the attack path?
- Can the claim be demonstrated without destructive testing?
- Can the observation be reproduced?
- Is evidence accidentally exposing a secret?

## 11. Defensive Questions

- Would defenders have equivalent evidence?
- Which logs should contain the event?
- Was the event actually logged?
- Can investigators reconstruct the sequence?
- Are timestamps consistent enough to correlate activity?

## 12. Evidence Handling Procedure

1. Define the assessment question.
2. Identify minimum evidence.
3. Collect only authorized evidence.
4. Record source, time and context.
5. Redact unnecessary sensitive information.
6. Store in the controlled engagement location.
7. Link evidence to the finding.
8. Preserve required evidence for retest.
9. Dispose or retain according to engagement requirements.

## Finding Logic

Missing evidence does not prove absence of a control.

Examples:

- no screenshot → not automatically no control;
- no log found → determine whether logging exists and whether the event should generate a log;
- scanner output only → may be an indicator, not sufficient proof of vulnerability.

## Exit Criteria

For each material finding, the team can answer:

- What happened?
- Where?
- When?
- How was it observed?
- Why does it matter?
- What requirement/control is affected?
- What evidence supports it?
- What evidence limitation exists?
- What evidence will prove remediation?

## Sources

- NIST SP 800-115.
- NIST SP 800-82 Rev. 3.
- CISA ICS Recommended Practices, including control-system forensics and incident-response material.

**Boundary:** E007 owns evidence discipline. It does not own the full risk decision (E009) or assessment lifecycle (E010).
