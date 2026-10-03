---
docType: knowledge_unit
knowledgeId: E004
sector: manufacturing_industrial
phase: Foundation
topic: Manufacturing Business Process Model
safety: controlled
status: working-rebuild
---

# E004: Manufacturing Business Process Model

## Assessment Question

**What manufacturing activity is being supported, what can go wrong if a security control fails, and which business or production outcome is affected?**

## Purpose

A technical vulnerability becomes meaningful only when its role in the manufacturing process is understood.

E004 connects technical systems to production activities without pretending that the assessor can independently determine process-engineering or safety consequences.

ISA-95 defines models and terminology for enterprise and manufacturing-control functions and describes Level 3 manufacturing operations management and its interface with Level 4 business functions.

## 1. Process Model

For each relevant process, use:

Business Objective → Manufacturing Operation → Process Step → Equipment → Control/IT System → Data → Human Decision → Output

Possible outputs include:

- product;
- quality result;
- production record;
- inventory movement;
- maintenance event;
- shipment;
- compliance record.

## 2. Process Categories

Depending on the facility, map:

- production planning;
- material handling;
- production execution;
- machine operation;
- quality control;
- laboratory testing;
- maintenance;
- calibration;
- packaging;
- warehouse/logistics;
- traceability;
- reporting;
- engineering change;
- supplier integration.

Do not assume every category exists.

## 3. Security-Relevant Properties

### Availability
Can the process continue if the system is unavailable?

### Integrity
Could incorrect data or commands cause an incorrect manufacturing outcome?

### Confidentiality
Could unauthorized disclosure expose IP, recipes, designs or sensitive production information?

### Authenticity
Can the process distinguish authorized users, devices and commands?

### Traceability
Can the organization determine who performed an action and when?

## 4. Attack-Path Thinking

Map:

Initial Access → Compromised Asset → Manufacturing Function → Process Capability → Business/Operational Effect

Example:

Compromised engineering workstation → engineering access → unauthorized configuration capability → possible process effect.

The example is a threat model, not permission to perform the action.

## 5. Process Dependencies

Record dependencies such as:

- identity services;
- DNS;
- time synchronization;
- databases;
- historians;
- MES;
- ERP;
- network infrastructure;
- backup;
- remote access;
- vendor support;
- cloud services.

A dependency is not automatically a vulnerability.

## 6. Offensive Questions

- Which system provides meaningful control over the process?
- Which credentials provide process capability?
- Which interfaces can influence process data?
- Can an attacker move from business systems toward production?
- Can a compromised engineering system affect a process?
- Can a supplier pathway influence a process?

## 7. Defensive Questions

- Would unauthorized process changes generate an alert?
- Are engineering changes logged?
- Are important operator actions attributable?
- Are production-data integrity events monitored?
- Can operations detect abnormal commands?
- Can affected process state be reconstructed?

MITRE ATT&CK for ICS includes process-oriented objectives such as Impair Process Control and Inhibit Response Function, which can help structure attack hypotheses.

## 8. Evidence

Useful evidence:

- process descriptions;
- sanitized process-flow diagrams;
- system dependency maps;
- approved architecture;
- configuration records;
- audit logs;
- interviews with process/operations owners;
- controlled observations.

Avoid collecting unnecessary proprietary recipes, production quantities or engineering IP.

## 9. Finding Logic

Do not report:

“System X is connected to MES, therefore it is critical.”

Instead establish:

Condition → Process Dependency → Security Requirement → Attack Capability → Evidence → Potential Effect

A process dependency may be verified, suspected, undocumented or unavailable for assessment.

## 10. Exit Criteria

The assessor can explain:

- what the process does;
- which systems support it;
- which systems can influence it;
- which data matters;
- which people/roles matter;
- what dependencies exist;
- what security failure could affect the process;
- what the organization can detect and recover.

## Sources

- ISA-95 — Enterprise-Control System Integration.
- NIST IR 8183 Rev. 1 — Manufacturing Profile.
- NIST SP 800-82 Rev. 3.
- MITRE ATT&CK for ICS.

**Boundary:** E004 owns process context. It does not own detailed asset inventory (E003), network trust boundaries (E005), or risk decisions (E009).
