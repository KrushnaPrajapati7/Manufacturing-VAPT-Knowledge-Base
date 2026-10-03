---
docType: knowledge_unit
knowledgeId: E010
sector: manufacturing_industrial
phase: Foundation
topic: Assessment Lifecycle and Knowledge Retrieval
safety: controlled
status: working-rebuild
---

# E010: Assessment Lifecycle and Knowledge Retrieval

## Assessment Question

**How should a manufacturing VAPT engagement progress from authorization to final retest, and how should the knowledge base preserve traceability and retrieval context?**

## Purpose

E010 is the Foundation lifecycle and retrieval map. It explains how the assessment modules fit together and what metadata each knowledge unit should expose for human and AI/RAG use.

It is not a generic penetration-testing checklist.

## 1. Assessment Lifecycle

Authorize → Understand → Prepare → Discover → Enumerate → Assess → Validate → Correlate → Report → Remediate → Retest → Close

The lifecycle can branch or stop when authorization, operational readiness or safety conditions are not satisfied.

## 2. Gate 1 — Authorization

Use E001.

Confirm:

- authorization;
- scope;
- ROE;
- permitted/restricted/prohibited actions;
- third-party boundaries;
- escalation;
- evidence rules.

No authorization means no testing.

## 3. Gate 2 — Environment Understanding

Use E002–E005.

Establish:

- manufacturing environment;
- asset context;
- business process;
- trust boundaries;
- external dependencies.

Do not begin with scanner output and work backward into architecture.

## 4. Gate 3 — Safety and Readiness

Use E006 and E008.

Confirm:

- OT relevance;
- production status;
- safety relevance;
- operational owner;
- test window;
- monitoring;
- recovery;
- emergency stop.

If a required gate fails, stop or change the planned method.

## 5. Assessment Phases

The later repository phases implement the lifecycle:

1. Reconnaissance
2. Scanning and Enumeration
3. Vulnerability Assessment
4. Identity and Access
5. Web/API/Application
6. Internal OT/ICS
7. Engineering, IIoT and Cloud
8. Network, Remote Access and Supply Chain
9. Data, Privacy and IP
10. Monitoring and Detection
11. Validation and Business Impact
12. Reporting and Remediation

The phases should be selected according to scope and engagement objectives; not every engagement requires every phase.

## 6. Validation Rule

For each candidate issue:

Detect → Validate → Interpret → Correlate → Decide

A scanner result, open port, banner or version match is not automatically a vulnerability.

## 7. Finding Traceability

Each important finding should connect, as applicable:

E001 Authorization → E002 Environment → E003 Asset → E004 Process → E005 Boundary → E006 Safety → Evidence → E009 Risk Decision → Remediation → Retest

Not every finding requires every link.

## 8. Knowledge-Unit Metadata

Each reusable knowledge unit should expose consistent metadata such as:

- knowledge ID;
- sector;
- phase;
- topic;
- assessment type;
- asset tags;
- safety classification;
- source references;
- prerequisites;
- related knowledge IDs;
- version/status.

Metadata should improve retrieval. It should not be used as decorative padding.

## 9. RAG Retrieval Requirements

For AI retrieval, a useful unit should answer a clear question and contain enough context to be understandable without copying the entire repository.

Retrieval should be able to distinguish:

- manufacturing context;
- IT versus OT;
- assessment phase;
- asset type;
- safety relevance;
- evidence requirement;
- finding logic;
- remediation/retest;
- authoritative sources.

Avoid creating multiple nearly identical files solely to increase document count.

## 10. Offensive and Defensive Retrieval

A useful AI query should be able to retrieve both:

**Offensive:** What path or capability could an attacker obtain?

**Defensive:** What control, telemetry or response capability should detect or prevent it?

The answer should preserve safety and authorization constraints.

## 11. Lifecycle Stop Conditions

Stop or escalate when:

- authorization becomes uncertain;
- scope changes without approval;
- production state changes;
- safety conditions change;
- unexpected operational effects occur;
- monitoring/recovery assumptions fail;
- activity becomes more intrusive than approved;
- third-party authorization is absent;
- evidence-handling requirements cannot be satisfied.

## 12. Reporting and Retest

Every material finding should preserve:

- affected asset;
- condition;
- evidence;
- validation;
- attack path;
- manufacturing relevance;
- limitations;
- remediation;
- retest method.

A successful retest should answer the original security question and provide evidence of closure.

## 13. Foundation Exit Criteria

The Foundation is ready for the Reconnaissance phase only when:

- E001–E010 have distinct purposes;
- duplicate generic methodology has been removed;
- authorization and safety gates are explicit;
- manufacturing context is established;
- assets and owners can be represented;
- process dependencies can be traced;
- trust boundaries can be described;
- evidence can be handled safely;
- findings can be reasoned from evidence;
- lifecycle and retrieval metadata are usable;
- sources are traceable;
- no client information is present.

## Sources

- NIST SP 800-115.
- NIST SP 800-82 Rev. 3.
- NIST IR 8183 Rev. 1.
- ISA-95.
- CISA ICS Recommended Practices.
- MITRE ATT&CK for ICS.

**Boundary:** E010 owns the lifecycle and knowledge-retrieval model. Detailed technical procedures belong to later phase documents.
