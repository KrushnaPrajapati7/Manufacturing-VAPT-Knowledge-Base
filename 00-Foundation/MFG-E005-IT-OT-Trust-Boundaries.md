---
docType: knowledge_unit
knowledgeId: E005
sector: manufacturing_industrial
phase: Foundation
topic: IT OT Trust Boundaries
safety: controlled
status: working-rebuild
---

# E005: IT–OT Trust Boundaries

## Assessment Question

**Where can trust, identity, data or network connectivity cross between enterprise IT, manufacturing OT and external environments, and is that crossing intentional and controlled?**

## Purpose

E005 identifies boundaries that control movement between different security and operational domains.

A network connection is not automatically a trust relationship. A logical trust relationship may exist even when the connection is indirect.

## 1. Boundary Types

Consider:

- enterprise IT ↔ industrial environment;
- Level 4 ↔ Level 3;
- Level 3 ↔ Level 2;
- engineering ↔ controller environment;
- vendor ↔ OT;
- cloud ↔ plant;
- wireless ↔ wired;
- remote-access ↔ OT;
- safety-related ↔ control environment;
- production ↔ laboratory/test;
- user identity ↔ privileged OT function.

ISA-95 provides logical levels and boundaries for manufacturing-control/business integration. These levels should be treated as logical reference points, not as proof that every modern architecture is a strict hierarchy.

## 2. Trust-Boundary Record

For each important boundary record:

- source domain;
- destination domain;
- communication path;
- authentication;
- authorization;
- protocol/service;
- direction;
- allowed purpose;
- owner;
- monitoring;
- logging;
- remote-access dependency;
- failure behavior;
- operational dependency.

## 3. Zones and Conduits

Where ISA/IEC 62443 concepts are used, document the organization's defined zones and conduits.

Do not invent zone assignments simply to fit a diagram.

A zone should represent a meaningful grouping based on security requirements and operational context. A conduit represents controlled communication between zones.

## 4. Boundary Hypotheses

Examples:

- enterprise identity may be trusted by OT systems;
- a vendor gateway may reach more OT assets than intended;
- a management interface may bypass an expected boundary;
- cloud integration may create an undocumented path;
- a firewall rule may permit a service beyond its business purpose;
- a shared account may cross multiple trust domains.

## 5. Offensive Validation

Use the least disruptive method that answers the question.

Possible validation:

- review firewall rules;
- review routing;
- inspect ACLs;
- inspect remote-access configuration;
- validate authorized connectivity;
- test a specific permitted path;
- review authentication/authorization;
- correlate traffic with documented purpose.

Do not turn an observed route into permission for unrestricted lateral movement.

## 6. Defensive Validation

Ask:

- Is crossing logged?
- Is source identity attributable?
- Is unusual traffic detected?
- Are remote sessions monitored?
- Can operations identify which boundary was crossed?
- Are denied attempts visible?
- Can the organization investigate a suspected boundary violation?

## 7. Boundary Failure vs Vulnerability

Examples:

- documented communication path → architecture fact;
- undocumented path → architecture/governance observation;
- firewall rule permits unintended traffic → potential security weakness;
- service is reachable → not automatically a vulnerability;
- boundary can be bypassed to obtain unauthorized capability → potential vulnerability/control failure.

## 8. Manufacturing Impact

For a validated weakness, trace:

Boundary → Reachable Asset → Capability → Process Dependency → Operational Effect

Do not claim physical consequences without evidence or appropriate process-owner input.

## 9. Evidence

Useful evidence:

- sanitized diagrams;
- firewall/ACL rules;
- route information;
- remote-access configuration;
- authentication logs;
- packet metadata where authorized;
- approved test results;
- monitoring evidence.

## 10. Exit Criteria

E005 is complete when important IT/OT/external boundaries are:

- identified;
- owner-associated;
- purpose-defined;
- technically characterized;
- monitoring status known;
- testing constraints known;
- potential attack paths documented.

## Sources

- NIST SP 800-82 Rev. 3.
- ISA-95.
- Applicable ISA/IEC 62443 zone/conduit concepts.
- CISA ICS Recommended Practices.

**Boundary:** E005 owns trust and connectivity boundaries. It does not replace E006's safety gate or E009's risk decision.
