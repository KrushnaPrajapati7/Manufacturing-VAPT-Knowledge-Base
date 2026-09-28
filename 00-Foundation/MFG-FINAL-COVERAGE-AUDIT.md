# Manufacturing VAPT — Final Coverage & Completeness Model

## Purpose

This document is the quality gate for the reusable Manufacturing & Industrial VAPT Knowledge Base. It defines what must be represented before a release is considered professionally usable.

A manufacturing VAPT library cannot truthfully claim that every possible technology or regulatory requirement is universal. Instead, this model aims for **complete category coverage** and requires engagement-specific tailoring.

## 1. Manufacturing architecture coverage

The KB must account for:

- ISA-95 Level 0: physical production processes.
- ISA-95 Level 1: sensing and manipulation.
- ISA-95 Level 2: monitoring and supervisory/automated control.
- ISA-95 Level 3: manufacturing operations management.
- ISA-95 Level 4: business planning and logistics.
- Enterprise/cloud integration layers where implemented.
- Purdue-style hierarchical architectures where used.
- Zones, conduits and industrial DMZs.
- IT/OT boundaries and trust relationships.

ISA-95 explicitly defines Levels 0–4 and the interfaces between manufacturing control and enterprise functions. The actual implementation varies by manufacturer.

## 2. Manufacturing type coverage

The KB must support different operating models:

- Discrete manufacturing.
- Continuous/process manufacturing.
- Batch manufacturing.
- Hybrid manufacturing.
- Assembly/workcell environments.
- Multi-site manufacturing.
- Contract manufacturing.
- Highly automated plants.
- Plants with substantial manual operations.

## 3. Asset coverage

The master taxonomy covers:

- Internet-facing assets.
- Corporate IT.
- Identity.
- Enterprise applications.
- ERP.
- MES/MOM.
- QMS/WMS/CMMS/LIMS/SCM.
- Engineering/CAD/CAM/CAE/PLM/PDM.
- SCADA/DCS/PLC/HMI/RTU/historians.
- Safety systems.
- Industrial machines.
- Robots/CNC/AGV/AMR.
- Sensors/actuators/drives.
- Industrial networks/protocols.
- IIoT/edge.
- Cloud.
- APIs/integration.
- Remote access.
- Third parties.
- Data/IP.
- Backup/DR.
- Security monitoring.
- Wireless/mobile.
- Physical/facility systems.
- DevSecOps/software supply chain.
- AI/analytics.

## 4. Security-control coverage

Every applicable asset should be considered against:

- Asset inventory.
- Ownership.
- Authentication.
- Authorization.
- Least privilege.
- MFA.
- Network segmentation.
- Secure configuration.
- Vulnerability/patch management.
- Malware protection.
- Application allowlisting where appropriate.
- File integrity.
- Change management.
- Logging.
- Monitoring.
- Detection.
- Backup.
- Recovery.
- Encryption.
- Secrets/key management.
- Secure remote access.
- Third-party access.
- Software/firmware update security.
- Incident response.

## 5. VAPT coverage

The eight standard phases are:

1. Reconnaissance.
2. Scanning & Enumeration.
3. Vulnerability Assessment.
4. Identity / Authentication / Authorization.
5. Web / API / Application / Infrastructure.
6. Internal / OT / ICS.
7. Validation / Business Impact.
8. Reporting / Remediation / Retest.

Cross-cutting activities must not be forced into one phase. Social engineering, physical security, wireless, cloud, supply chain, resilience, threat modeling and GRC can span multiple phases.

## 6. Human and physical coverage

Where explicitly authorized, the methodology must support:

- Phishing/social engineering.
- Physical access review.
- Badge/access-control systems.
- Visitor controls.
- Removable media.
- Control-room/server-room/engineering-area security.
- Security awareness.
- Human error and insider-risk controls.

These activities require their own rules of engagement and must not be silently assumed to be part of a technical VAPT.

## 7. Safety coverage

OT testing must explicitly consider:

- Worker safety.
- Process safety.
- Availability.
- Reliability.
- Physical consequences.
- Safety Instrumented Systems.
- Emergency-stop systems.
- Safety PLCs/controllers.
- Maintenance windows.
- Stop conditions.
- Escalation paths.
- Lab/digital-twin validation.

Production OT is not treated as ordinary IT.

## 8. Supply-chain coverage

The KB must cover:

- Equipment suppliers.
- Automation vendors.
- System integrators.
- Managed service providers.
- Remote maintenance vendors.
- Software suppliers.
- Firmware suppliers.
- Cloud providers.
- Third-party APIs.
- Update channels.
- Code/artifact/package repositories.
- Software bills of materials where available.
- Vendor security requirements.

## 9. Resilience coverage

The assessment must be capable of evaluating:

- Backup availability.
- Backup integrity.
- Backup isolation.
- Restore capability.
- Recovery objectives.
- Production recovery.
- Redundancy.
- Failover.
- Single points of failure.
- Ransomware recovery.
- PLC/SCADA/HMI/engineering backups.

## 10. Threat and attack-path coverage

The KB should support mapping from:

**External access → identity → IT → engineering → OT → control → physical process**

and other valid paths, without assuming that a path exists.

MITRE ATT&CK for ICS provides an additional threat-behavior vocabulary and includes ICS-specific tactics such as Inhibit Response Function, Impair Process Control and Impact.

## 11. Detection and response coverage

The assessment should consider:

- What is logged?
- Where is it logged?
- What is monitored?
- What is detected?
- Can SOC/OT personnel distinguish normal plant behavior from suspicious activity?
- Are critical OT events visible?
- Are remote-access events logged?
- Are authentication changes logged?
- Are configuration changes logged?
- Can incidents be safely contained?

## 12. Data coverage

Consider:

- PII.
- Employee data.
- Customer data.
- Supplier data.
- Financial data.
- Production data.
- Quality data.
- Recipes/formulas.
- CAD/design/IP.
- Firmware.
- Source code.
- Credentials.
- API keys.
- Tokens.
- Certificates/private keys.
- Backups.
- Engineering documentation.

## 13. Application lifecycle coverage

Where applicable:

- Requirements.
- Architecture.
- Development.
- Code review.
- SAST.
- DAST.
- Dependency security.
- SBOM.
- CI/CD.
- Artifact integrity.
- Signing.
- Deployment.
- Configuration.
- Runtime.
- Logging.
- Decommissioning.

## 14. Risk coverage

A finding should distinguish:

- Technical severity.
- Exploitability.
- Confidentiality impact.
- Integrity impact.
- Availability impact.
- Business impact.
- Production impact.
- Safety impact.
- Regulatory/contractual impact.
- Recovery impact.

CVSS can support technical severity; it must not replace manufacturing-specific business, operational or safety analysis.

## 15. Evidence coverage

Every finding should be capable of recording:

- Asset.
- Environment.
- Date/time.
- Tester.
- Test action.
- Observation.
- Evidence.
- Reproduction information.
- Technical impact.
- Business/operational impact.
- Remediation.
- Retest status.

Sensitive client evidence remains outside the public reusable KB.

## 16. Standards coverage

The repository should maintain a reference map for:

- NIST SP 800-82.
- NIST SP 800-115.
- NIST SP 1800-10 Manufacturing.
- NIST Manufacturing Profile / applicable CSF version.
- ISA-95 / IEC 62264.
- ISA/IEC 62443.
- MITRE ATT&CK for ICS.
- OWASP WSTG.
- OWASP API Security.
- CVSS.
- Applicable ISO/IEC standards.
- Applicable national, sectoral, contractual and customer requirements.

Standards are references, not automatic proof that a company is compliant or non-compliant.

## 17. Release gate

A release is not considered complete unless:

- Every master asset family has applicable assessment coverage.
- Every VAPT phase has knowledge units.
- OT/ICS safety controls are represented.
- Cross-cutting assessments are represented.
- Evidence and finding schemas exist.
- Standards are referenced and versioned.
- Client-specific information is excluded.
- Missing/unknown areas can be marked as `not_applicable`, `not_in_scope`, `unknown`, or `not_tested`.
- The repository can be queried by phase, asset, technology, business process and risk.

## 18. Important limitation

No generic repository can guarantee coverage of an unknown proprietary machine, vendor-specific protocol, newly released product, newly published vulnerability or jurisdiction-specific obligation. The correct professional design is therefore:

**Complete category taxonomy + standardized methodology + explicit unknown/not-applicable states + engagement-specific tailoring + periodic version review.**
