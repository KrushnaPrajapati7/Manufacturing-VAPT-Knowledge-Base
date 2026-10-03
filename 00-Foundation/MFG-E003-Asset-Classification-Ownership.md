---
docType: knowledge_unit
knowledgeId: E003
sector: manufacturing_industrial
phase: Foundation
topic: Asset Classification and Ownership
safety: controlled
status: working-rebuild
---

# E003: Asset Classification and Ownership

## Assessment Question

**Can the assessment team identify what each relevant asset is, what it does, who owns it, how important it is, and who can authorize changes to it?**

## Purpose

A manufacturing assessment becomes unreliable when an assessor knows an IP address but cannot establish the asset's function, owner or operational importance.

E003 creates an asset context model for VAPT. It does not attempt to replace a complete CMDB.

## 1. Minimum Asset Record

For each relevant asset, capture where available:

- asset identifier;
- hostname/IP/resource identifier;
- asset type;
- manufacturer/model;
- function;
- environment;
- ISA-95 logical level where useful;
- zone/network;
- business/process dependency;
- operational owner;
- technical owner;
- security owner;
- vendor/support owner;
- criticality;
- safety relevance;
- remote-access status;
- lifecycle status;
- evidence source.

## 2. Asset Types

Use functional categories rather than only device names:

- enterprise server;
- workstation;
- engineering workstation;
- HMI;
- PLC;
- RTU;
- DCS component;
- SCADA server;
- historian;
- MES/MOM;
- industrial switch/router;
- firewall;
- jump server;
- remote-access gateway;
- IIoT gateway;
- industrial sensor/device;
- safety-related system;
- cloud service;
- API;
- database;
- backup/recovery system;
- engineering repository.

## 3. Ownership Model

| Owner | Meaning |
|---|---|
| Operational owner | Accountable for how the asset supports plant operations |
| Technical owner | Responsible for technical administration |
| Security owner | Responsible for cybersecurity requirements |
| Vendor/support owner | External party responsible for support where applicable |
| Safety owner | Relevant authority for safety-related concerns |

One person or team may hold multiple roles, but technical administration must not automatically be treated as operational authority.

## 4. Criticality

Do not assign criticality from asset type alone.

Consider:

- production dependency;
- process dependency;
- safety dependency;
- quality dependency;
- recovery dependency;
- data integrity dependency;
- engineering dependency;
- external/customer dependency;
- single-point-of-failure characteristics.

An asset's importance depends on its role in the specific environment.

## 5. Asset State

Use explicit states:

- confirmed;
- partially verified;
- suspected;
- duplicate;
- retired;
- unknown;
- out-of-scope.

Unknown remains unknown until evidence supports classification.

## 6. Assessment Hypotheses

Examples:

- critical assets may lack accountable ownership;
- technical ownership may not match operational ownership;
- remote-support assets may have unclear responsibility;
- obsolete assets may remain reachable;
- asset inventories may omit OT or IIoT devices;
- cloud-connected assets may not have a clear plant owner.

## 7. Offensive Interpretation

Ask:

**If an attacker compromises this asset, what capability does the asset provide?**

Examples:

- access to engineering functions;
- credential exposure;
- network pivoting;
- process visibility;
- control-system access;
- production-data manipulation;
- access to vendor infrastructure.

## 8. Defensive Interpretation

Ask:

**Would the organization know which asset was affected and who is responsible for it?**

Check for:

- asset inventory;
- owner mapping;
- monitoring coverage;
- alert ownership;
- incident escalation;
- lifecycle status;
- backup responsibility.

## 9. Evidence

Prefer:

- approved asset inventory;
- sanitized architecture records;
- management-system records;
- configuration evidence;
- owner confirmation;
- technical observation;
- vendor documentation.

Record the source of classification. Do not silently convert an interview statement into verified technical fact.

## 10. Finding Logic

Examples:

- Unknown owner alone → governance/asset-management observation.
- Unmanaged critical asset with security exposure → potential finding if validated.
- Duplicate inventory entry → data-quality issue unless it causes a security/control weakness.
- Old asset version → not automatically a vulnerability.
- Asset reachable from an unauthorized zone → potentially significant security weakness, subject to safe validation.

## 11. Exit Criteria

The assessor should be able to answer:

- What is the asset?
- What does it do?
- Where does it operate?
- Who owns it?
- Who administers it?
- What process depends on it?
- Is it safety-relevant?
- How is it monitored?
- How is it recovered?
- Is it actually in scope?

## Sources

- NIST SP 800-82 Rev. 3.
- CISA Cross-Sector Cybersecurity Performance Goals, including asset inventory guidance.
- ISA-95 where manufacturing hierarchy/context is relevant.

**Boundary:** E003 owns asset identity, classification and ownership. It does not own the business-process model (E004) or detailed risk decisions (E009).
