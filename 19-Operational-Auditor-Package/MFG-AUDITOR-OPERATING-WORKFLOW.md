# Manufacturing VAPT Auditor Operating Workflow

## 1. Pre-engagement
1. Confirm written authorization and named owner.
2. Define in-scope/out-of-scope assets, sites, environments, accounts, third parties and testing windows.
3. Establish Rules of Engagement (ROE), emergency contacts and escalation paths.
4. Identify production, quality, safety, regulatory and business constraints.
5. Establish evidence handling, classification, retention and sharing rules.

## 2. Architecture and scope baseline
1. Build the asset inventory using the 23-family / 406-asset master matrix.
2. Map enterprise, plant, cell/area, DMZ, cloud and remote-access boundaries.
3. Identify IT/OT trust boundaries, zones/conduits, critical processes and safety systems.
4. Record unknowns instead of guessing.

## 3. Safety gate
Before testing an OT/ICS or cyber-physical asset confirm: authorization, owner, safety contact, maintenance window, allowed methods, stop conditions, recovery path, backup availability, emergency communications and whether a lab/digital twin is available.

## 4. Phase execution
Use the eight phases: Reconnaissance; Scanning & Enumeration; Vulnerability Assessment; Identity/Auth; Web/API/Application; Internal/OT/ICS; Validation/Business Impact; Reporting/Retest. Use the asset matrix and knowledge-unit mappings to select applicable tests.

## 5. Execution discipline
For every test record: asset, phase, test/knowledge unit, objective, preconditions, authorization state, method, expected result, observed result, safety mode, limitations, evidence IDs and status.

## 6. Evidence and findings
Observation → Evidence → Finding. Preserve timestamps, source, capture method, sensitivity, integrity/hash where applicable, redaction state and chain-of-custody requirements. Do not call a scanner output a confirmed vulnerability without appropriate validation.

## 7. Risk and business impact
Assess technical impact plus confidentiality, integrity, availability, production, quality, safety, recovery, regulatory/customer and intellectual-property consequences. Keep CVSS separate from business/plant risk where appropriate.

## 8. Reporting
Aggregate coverage, findings, exceptions and limitations. Clearly distinguish confirmed, suspected, not tested, unknown and out-of-scope states.

## 9. Remediation and retest
Track owner, action, target date, compensating controls, residual risk, retest evidence and closure/risk-acceptance decision.

## 10. Closeout
Confirm all assets have a final status, all findings have disposition, evidence is stored according to policy, credentials/test accounts are disabled or returned, temporary access is removed, and the client receives the agreed deliverables.
