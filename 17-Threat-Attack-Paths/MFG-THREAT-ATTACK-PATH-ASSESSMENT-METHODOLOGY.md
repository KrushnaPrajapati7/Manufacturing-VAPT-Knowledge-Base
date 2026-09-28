# Manufacturing Threat, Attack-Path & MITRE ATT&CK for ICS Assessment Methodology

## Purpose
This layer converts the manufacturing VAPT scope into adversary-oriented assessment paths without replacing the asset/phase matrix. It is a reusable methodology layer for authorized assessments, threat modeling, purple-team exercises, validation, detection engineering and risk reporting.

## Coverage rule
The authoritative scope remains the 23 asset families and 406 asset/technology entries in `00-Foundation/MFG-MASTER-ASSET-VAPT-KNOWLEDGE-MATRIX.csv`. Every asset is mapped in `MFG-ASSET-THREAT-ATTACK-MAPPING.csv`; absence of a specific attack path must be recorded as Not Applicable rather than silently omitted.

## Attack-path construction
1. Identify the starting exposure or trust relationship.
2. Identify identity, network, application, physical or supply-chain prerequisites.
3. Map the next reachable asset/zone/conduit.
4. Map relevant MITRE ATT&CK for ICS tactic/technique behavior.
5. Identify collection, command/control, process-control and impact opportunities.
6. Determine whether the path is technically reachable, administratively permitted, or only theoretical.
7. Validate only the minimum necessary condition under the ROE.
8. Record evidence at each material trust boundary.
9. Assess business, production, quality, recovery, safety and environmental consequences.
10. Map detection and response opportunities.
11. Record limitations, assumptions and untested transitions.

## Path status
- **Observed:** evidence shows the path/relationship exists.
- **Potential:** conditions exist but full path was not validated.
- **Validated:** authorized, controlled validation confirmed the relevant security condition.
- **Blocked:** a control prevented the path at the tested boundary.
- **Not Tested:** validation was prohibited, unsafe, unavailable or outside scope.
- **Not Applicable:** path does not apply to the asset/environment.
- **Unknown:** evidence is insufficient.

## Trust boundaries to assess
- Internet ↔ DMZ
- Internet ↔ remote access
- Corporate IT ↔ OT
- Enterprise ↔ plant/site
- OT DMZ ↔ control zones
- Level 3 ↔ Level 2/1
- Engineering ↔ controller
- Vendor ↔ plant
- Cloud ↔ edge/plant
- API/integration ↔ downstream system
- Wireless ↔ wired/OT
- Physical access ↔ cyber assets
- Backup/recovery ↔ production
- Software supply chain ↔ deployed environment

## Impact dimensions
Evaluate separately where applicable: confidentiality, integrity, availability, authentication/authorization, production continuity, product quality, traceability, engineering IP, data protection, recovery capability, safety, environment, equipment/property, regulatory/contractual obligations and financial/reputation consequences.

## OT safety rules
- Default to passive/read-only collection for production OT.
- Do not change PLC logic, controller modes, setpoints, I/O, firmware, alarm settings, safety functions or physical process parameters as a routine VAPT activity.
- Use a lab, test cell, digital twin or explicitly controlled maintenance window for process-changing validation.
- Require plant owner, OT engineering and safety stakeholders for any activity that could affect production or safety.
- Establish stop conditions, emergency contacts, rollback and recovery procedures before active validation.
- Treat safety, quality and availability as first-class assessment dimensions.

## MITRE ATT&CK for ICS usage
MITRE ATT&CK for ICS is used to describe adversary behavior, not to authorize unsafe emulation. The current MITRE ICS matrix contains 12 tactics and the live technique catalog is maintained by MITRE. This repository records relevant technique mappings and should be refreshed against the authoritative MITRE catalog when the repository is versioned.

## Evidence requirements
Evidence should support the specific transition or control claim: architecture/zone diagram, route/ACL, authentication record, configuration, service/interface inventory, protocol metadata, logs, detection events, project/firmware integrity evidence, backup/restore evidence, approved screenshots, timestamps and finding references. Sensitive evidence must be classified, minimized and redacted as appropriate.

## Reporting
Do not report an attack path as a confirmed compromise merely because an associated technique exists. Distinguish: exposure, reachable path, exploitable condition, validated security weakness, confirmed impact and residual risk.
