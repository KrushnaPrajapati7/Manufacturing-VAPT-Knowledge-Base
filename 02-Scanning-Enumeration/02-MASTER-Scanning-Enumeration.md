---
docType: guide
answerType: guide
guideType: pentest
knowledgeId: MFG-P02
sector: manufacturing_industrial
phase: enumeration
---

# MFG-P02: Scanning & Enumeration

## Question

How should an authorized VAPT team perform the **Scanning & Enumeration** phase in a manufacturing environment?

## Description

Identify reachable hosts, ports, services, applications, protocols, versions, identities and architecture.

## Standard Workflow

1. Confirm authorization, scope, safety and assessment window.
2. Identify relevant assets and business processes.
3. Select the applicable knowledge units.
4. Use the least disruptive valid method.
5. Record evidence and separate facts, observations and conclusions.
6. Validate material findings.
7. Map technical exposure to business/operational impact.
8. Hand findings to reporting/remediation.

## Coverage

This phase can involve external assets, corporate IT, ERP/MES/QMS/WMS/CMMS, engineering/CAD/PLM, OT/ICS, IIoT/edge, cloud, APIs, networks, third parties, data and monitoring.

## Safety

Manufacturing security testing must account for availability, reliability and safety. OT/ICS should default to passive/read-only techniques and require explicit authorization for potentially disruptive actions.

## References

- NIST SP 800-82 Rev. 3
- ISA-95 / IEC 62264
- ISA/IEC 62443
- MITRE ATT&CK for ICS
- NIST SP 800-115
- OWASP WSTG / OWASP Top 10 / OWASP API Security where applicable
