---
docType: knowledge_unit
knowledgeId: E002
sector: manufacturing_industrial
phase: Foundation
topic: Manufacturing Environment Overview
safety: controlled
status: working-rebuild
---

# E002: Manufacturing Environment Overview

## Assessment Question

**What does the manufacturing environment contain, how does it operate, and which technical systems support the physical production process?**

## Purpose

E002 gives the assessor a usable mental model of the plant before technical testing begins. It prevents a manufacturing environment from being treated as an ordinary corporate network.

The objective is not to document every device. The objective is to understand enough of the environment to make safe, technically meaningful assessment decisions.

NIST SP 800-82 Rev. 3 describes OT as systems and devices that interact with or manage the physical environment and emphasizes their performance, reliability and safety requirements.

## 1. What the Assessor Must Understand

Establish, where applicable:

- what the facility produces;
- which production areas or lines are included;
- which processes are continuous, batch or discrete;
- which systems monitor or control those processes;
- where engineering and maintenance functions occur;
- where production data is collected;
- where business systems exchange information with manufacturing systems;
- which systems are safety-related;
- which systems are remotely administered;
- which dependencies can affect production or recovery.

Do not assume that a system is OT merely because it is physically located in a plant.

## 2. Manufacturing Technology Model

Use ISA-95 as a common manufacturing vocabulary, not as proof that every plant has the same architecture. ISA-95 describes five logical levels: Level 0 physical production, Level 1 sensing/manipulation, Level 2 monitoring/supervisory control, Level 3 manufacturing operations management, and Level 4 business planning/logistics.

| Level | Typical concern | Assessment question |
|---|---|---|
| 0 | Physical process | What physical process is affected? |
| 1 | Sensors/actuators | Which devices sense or manipulate the process? |
| 2 | PLC/DCS/SCADA/HMI | Which systems supervise or control it? |
| 3 | MES/MOM/historian/operations | Which systems coordinate manufacturing operations? |
| 4 | ERP/business systems | Which business functions exchange data with manufacturing? |

This model is a logical aid. Modern environments may be distributed, virtualized, cloud-connected or vendor-managed.

## 3. Environment Discovery

Build the environment model from authoritative sources where possible:

- plant network diagrams;
- asset inventories;
- OT architecture diagrams;
- process descriptions;
- system-owner interviews;
- firewall/routing information;
- remote-access records;
- CMDB or asset-management records;
- vendor documentation;
- cloud architecture;
- observed technical evidence.

Separate documented architecture from observed architecture. A material difference between them is itself useful assessment information.

## 4. Process-to-Technology Mapping

For important production functions, record:

Production Process → Equipment → Control System → Supervisory System → Operations System → Business Dependency → Recovery Dependency

Example:

Packaging → Packaging Line → PLC → HMI/SCADA → MES → ERP order → Maintenance/backup dependency

This is context, not automatically a finding.

## 5. IT vs OT Context

### IT-oriented systems

Common objectives include confidentiality, integrity, availability, identity and access control, data protection and application security.

### OT-oriented systems

Assessment must additionally consider deterministic operation, process continuity, equipment behavior, operational availability, safety, maintenance constraints, legacy technology and vendor dependencies.

Do not copy IT security practices into OT without operational review.

## 6. Remote and External Dependencies

Identify:

- vendor remote access;
- VPN;
- remote desktop/jump hosts;
- cloud connectivity;
- managed services;
- support gateways;
- IIoT platforms;
- external APIs;
- software-update infrastructure.

CISA maintains ICS recommended practices covering remote access, defense in depth, patch management and control-system incident response.

## 7. Assessment Hypotheses

Useful hypotheses include:

- a business system may have an unintended path toward manufacturing systems;
- a vendor access path may provide broader reach than intended;
- a management interface may cross an expected boundary;
- cloud integration may create an undocumented path;
- a critical process may have an undocumented technical dependency;
- documented architecture may differ materially from observed architecture.

Do not test these hypotheses invasively until E001 authorization and E006 safety requirements permit the activity.

## 8. Evidence

Useful evidence includes:

- architecture diagrams;
- asset records;
- system/function mapping;
- approved network diagrams;
- sanitized screenshots;
- configuration references;
- interview records;
- observed communication paths;
- ownership information;
- dependency records.

Avoid copying unnecessary production information into the reusable KB.

## 9. Finding Logic

A missing or inaccurate environment model is not automatically a vulnerability.

Possible outcomes:

- Documented and verified
- Documented but not verified
- Observed but undocumented
- Conflicting information
- Unknown
- Not applicable

A finding becomes appropriate when the discrepancy represents an assessed security or control weakness and sufficient evidence exists.

## 10. Defensive Questions

For important processes ask:

- Would unauthorized access be visible?
- Are important control-system connections monitored?
- Are remote sessions attributable?
- Can operations identify who owns a critical asset?
- Can the organization detect unexpected communication between IT and OT?
- Can the organization reconstruct relevant events after an incident?

## 11. Exit Criteria

E002 is complete when the assessor can explain:

1. what the plant produces;
2. which production processes are relevant;
3. which technology supports those processes;
4. where IT and OT interact;
5. which systems are externally connected;
6. which systems are safety-relevant;
7. which dependencies could affect production;
8. which architecture facts are verified versus assumed.

## Sources

- NIST SP 800-82 Rev. 3 — Guide to Operational Technology Security.
- ISA-95 — Enterprise-Control System Integration.
- NIST IR 8183 Rev. 1 — Cybersecurity Framework Version 1.1 Manufacturing Profile.
- CISA ICS Recommended Practices.

**Boundary:** E002 explains the environment. It does not own asset classification (E003), process mapping detail (E004), trust-boundary analysis (E005), or safety-gate decisions (E006).
