# Manufacturing VAPT — Master Auditor Checklist

**Version:** 1.2.0 checklist layer
**Purpose:** Standardized assessment workflow derived from the asset/phase matrix and existing Manufacturing VAPT KB.

> This checklist is a planning and assessment-control instrument. It is not authorization to test any organization or production system. Production OT/ICS and safety-related testing requires explicit written authorization and safety controls.

## Status values
`Not Started` · `In Progress` · `Tested` · `Finding` · `Not Applicable` · `Out of Scope` · `Not Tested` · `Unknown` · `Retest Pending` · `Retested`

## Engagement-level gates
- [ ] **Authorization & Scope:** Written authorization, explicit assets/systems, testing window, production identification, third-party inclusion/exclusion, separate OT scope, safety restrictions.
- [ ] **Asset ownership:** Record asset owner, business owner, technical owner, environment, criticality and business process.
- [ ] **Architecture & trust boundaries:** Document Internet, corporate IT, IT/OT DMZ, OT network, industrial control network, cloud/edge and other relevant trust boundaries.
- [ ] **Safety gate:** Confirm production/OT status, safety-system restrictions, stop conditions, emergency contact and approved test mode.
- [ ] **Evidence plan:** Define evidence types, timestamps, retention, access control and sensitive-data minimization.
- [ ] **Status discipline:** Use only: In Scope, Out of Scope, Not Applicable, Not Tested, Unknown, Tested, Finding, Retest Pending, Retested.

## Phase checklists
### Reconnaissance

- [ ] **Scope discovery:** Confirm authorized domains, IP ranges, applications, cloud accounts, remote access, facilities and third parties.
- [ ] **External attack surface:** Identify domains, subdomains, DNS, public IPs, internet gateways, firewalls, WAF, load balancers, reverse proxies and exposed applications.
- [ ] **Application discovery:** Identify web applications, admin panels, cPanel/hosting, portals, ERP/MES/QMS/WMS/CMMS/CRM/HRMS and mobile/API surfaces where applicable.
- [ ] **Engineering discovery:** Identify CAD/CAM/PLM, engineering workstations, repositories, design/IP stores and engineering integrations.
- [ ] **OT discovery:** Identify OT zones, SCADA/DCS/PLC/HMI/RTU/historian/engineering stations/gateways using approved passive or controlled methods.
- [ ] **Cloud/IIoT discovery:** Identify cloud platforms, object storage, IAM, APIs, edge gateways, IIoT platforms, brokers and device-management services.
- [ ] **Remote/third-party discovery:** Identify VPN, jump/bastion, RDP/SSH/VNC, vendor support, MSP/MSSP, integrators and supplier connections.
- [ ] **Data discovery:** Identify PII, financial, production, quality, recipe, CAD/IP, source/firmware, credentials, keys, tokens, certificates and backup data classes.
- [ ] **Recon evidence:** Record source, timestamp, confidence and authorization status; distinguish observation from inference.
### Scanning & Enumeration

- [ ] **Host/service enumeration:** Enumerate authorized hosts, ports, services, protocols and management interfaces without unsafe disruption.
- [ ] **Technology identification:** Identify OS, application, middleware, database, device and protocol technologies; do not equate version identification with a vulnerability.
- [ ] **Network enumeration:** Assess routing, segmentation, firewall exposure, trust boundaries and management-plane exposure.
- [ ] **Application/API enumeration:** Map endpoints, methods, parameters, authentication schemes, documentation, schemas and integrations.
- [ ] **Identity enumeration:** Review authorized directory, SSO, MFA, RBAC, privileged, service, machine and cloud identities.
- [ ] **Cloud enumeration:** Review accounts/projects/subscriptions, networks, IAM, storage, databases, compute, containers, serverless and exposed endpoints.
- [ ] **OT enumeration:** Prefer passive/read-only methods for sensitive OT; identify assets and protocols with safety gates.
- [ ] **Wireless/mobile enumeration:** Assess approved corporate/industrial Wi-Fi, mobile, RFID/BLE/NFC and handheld environments where in scope.
- [ ] **Evidence:** Capture enumerated asset/service inventory, timestamps, source and confidence.
### Vulnerability Assessment

- [ ] **Vulnerability identification:** Assess known vulnerabilities, unsupported software, missing patches and insecure configurations using approved methods.
- [ ] **Configuration review:** Review hardening, default settings, exposed management services, insecure protocols and security controls.
- [ ] **Credential/security control review:** Assess password policy, MFA, secrets handling, certificates, keys and service accounts where authorized.
- [ ] **Application/API weaknesses:** Assess injection, access control, session/token issues, file handling, business logic, information exposure and API-specific weaknesses.
- [ ] **Cloud weaknesses:** Assess IAM, network controls, storage exposure, security groups/NACLs, secrets, logging and service configuration.
- [ ] **OT/ICS weaknesses:** Review firmware/software exposure, insecure protocols, remote administration, segmentation, configuration and logging with OT safety constraints.
- [ ] **Engineering/IP weaknesses:** Assess CAD/PLM repositories, engineering workstations, source/firmware stores and access controls.
- [ ] **False-positive validation:** Manually verify material findings before reporting; document evidence and limitations.
- [ ] **Risk dimensions:** Consider confidentiality, integrity, availability, safety, production, quality and recovery impact.
### Identity / Authentication / Authorization

- [ ] **Identity inventory:** Identify human, privileged, vendor, contractor, service, machine, API, cloud and break-glass accounts.
- [ ] **Authentication:** Assess password controls, MFA, SSO, certificates, device identity and authentication flows.
- [ ] **Authorization:** Assess RBAC/least privilege, object-level access, segregation of duties and server-side enforcement.
- [ ] **Privileged access:** Review PAM, administrator paths, privileged sessions and emergency/break-glass access.
- [ ] **Lifecycle:** Review joiner/mover/leaver, dormant/excessive access, credential rotation and revocation.
- [ ] **Remote/vendor access:** Assess time-bounded access, MFA, least privilege, session logging and revocation.
- [ ] **Machine/API identities:** Review non-human identities, tokens, secrets, certificates and service accounts.
- [ ] **Evidence:** Record role matrices, approved test accounts, access outcomes and relevant logs without collecting unnecessary secrets.
### Web / API / Application

- [ ] **Application inventory:** Identify business-critical applications, portals, mobile apps, admin interfaces and integrations.
- [ ] **Authentication/session:** Assess authentication, session management, token handling, logout, timeout and recovery flows.
- [ ] **Authorization:** Test server-side authorization, horizontal/vertical access boundaries and object-level access controls.
- [ ] **Input/output handling:** Assess input validation, injection classes, encoding, deserialization where applicable and error handling.
- [ ] **File handling:** Assess upload/download, path handling, file type controls, storage and access boundaries.
- [ ] **Business logic:** Assess workflow abuse, state transitions, approval controls, quantity/price/production/quality logic where applicable.
- [ ] **API security:** Assess API authentication, authorization, object-level access, rate limiting, schema validation, sensitive data and error handling.
- [ ] **Configuration:** Review security headers, TLS, CORS, exposed documentation, debug settings and secrets exposure.
- [ ] **Data exposure:** Assess PII, employee, supplier, customer, production, quality, recipe and engineering/IP exposure.
### Internal / OT / ICS

- [ ] **OT architecture:** Map ISA-95/Purdue-aligned levels where applicable, zones/conduits, industrial DMZ and IT/OT trust boundaries.
- [ ] **OT asset inventory:** Identify PLC, HMI, SCADA, DCS, RTU, historian, engineering station, industrial gateway and network assets.
- [ ] **OT protocol review:** Assess applicable industrial protocols such as Modbus/TCP, OPC UA, EtherNet/IP, PROFINET, MQTT and vendor protocols using safe methods.
- [ ] **Segmentation:** Review firewall rules, routing, conduits, remote paths and management interfaces.
- [ ] **OT identity:** Assess operator/engineer/admin/service accounts, remote access, vendor access and privileged paths.
- [ ] **Configuration/firmware:** Review authorized configurations, firmware/software versions, hardening, backups and change controls.
- [ ] **Safety systems:** Identify SIS/safety PLC/interlocks/emergency systems and apply dedicated safety restrictions.
- [ ] **Passive-first validation:** Prefer observe/identify/passive/read-only validation for sensitive production assets.
- [ ] **Monitoring:** Assess OT logging, alerting, IDS/NDR and SIEM integration where applicable.
- [ ] **Incident/recovery:** Review OT incident response, backup/restore, golden images and recovery readiness.
### Validation / Business Impact

- [ ] **Finding validation:** Verify material findings manually where safe; document false-positive reasoning and limitations.
- [ ] **Attack path analysis:** Assess realistic paths across identity, IT, cloud, engineering, vendor access and IT/OT boundaries.
- [ ] **Business process mapping:** Map findings to procurement, inventory, production, quality, maintenance, warehouse, engineering and customer processes as applicable.
- [ ] **Impact dimensions:** Assess technical, confidentiality, integrity, availability, safety, production, quality, financial, IP and recovery impact.
- [ ] **Controlled exploit validation:** Only perform controlled validation within ROE; use lab/digital twin for disruptive OT validation where possible.
- [ ] **Detection validation:** Where authorized, assess whether relevant activity is logged/detected by SIEM/EDR/OT monitoring.
- [ ] **Recovery implications:** Assess backup, restore, RTO/RPO and single points of failure where relevant.
### Reporting / Remediation / Retest

- [ ] **Finding record:** Use standardized ID, title, asset, description, evidence, impact, severity, root cause, remediation, references and retest status.
- [ ] **Risk scoring:** Use CVSS where appropriate and supplement with manufacturing-specific operational/safety context.
- [ ] **Evidence quality:** Ensure evidence is reproducible, timestamped, minimized and linked to the finding.
- [ ] **Remediation:** Provide actionable technical and process remediation plus compensating controls where appropriate.
- [ ] **Management reporting:** Provide executive summary, scope, methodology, risk summary, operational impact and recommendations.
- [ ] **Retest:** Validate remediation, record residual risk and distinguish fixed/partially fixed/not fixed/not retested.
- [ ] **QA/peer review:** Review scope coverage, evidence, severity rationale, references, duplicates and sensitive-data handling before release.

## Asset-by-asset control rule
For every in-scope asset, the auditor should consult the Master Asset × VAPT × Knowledge matrix and record the applicable phase status. Do not mark a phase as tested solely because the asset exists; record the actual assessment activity and evidence.

## Minimum asset record
`Asset ID | Family | Asset/Technology | Owner | Environment | Location/Zone | Business Process | Criticality | Exposure | Phase | Status | Knowledge Unit IDs | Evidence | Finding IDs | Safety Mode | Notes`
