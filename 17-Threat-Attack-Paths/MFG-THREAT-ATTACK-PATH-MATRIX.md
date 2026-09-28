# Manufacturing Threat & Attack-Path Matrix

This is the human-readable control layer for the machine-readable attack-path catalogs.

## Core path families

| Domain | Representative paths | Main concern | Default validation |
|---|---|---|---|
| External exposure | AP-001, AP-002 | Public services, remote access, internet reachability | Controlled active + manual |
| Identity | AP-003, AP-005, AP-030 | Privilege, service accounts, vendor access, PKI/time | Read-only/config review |
| IT/OT boundaries | AP-006, AP-007 | Segmentation, zones/conduits, dual-homing | Passive/read-only |
| Engineering | AP-008, AP-009, AP-032 | Project integrity, controller access, IP | Passive + lab validation |
| OT/control | AP-010–AP-015 | Protocols, HMI/SCADA/DCS/PLC, safety | Passive/read-only; lab for active |
| Wireless/physical | AP-016, AP-017, AP-026, AP-027 | Plant access, removable media, facility systems | Controlled |
| Cloud/edge/API | AP-018–AP-021, AP-035 | Trust bridging, IAM, APIs, gateways | Non-destructive |
| Supply chain | AP-022, AP-023, AP-034 | Source/build/update/firmware integrity | Review + lab |
| Resilience | AP-024, AP-025, AP-036 | Backup, ransomware, recovery | Review/tabletop/lab |
| Monitoring | AP-029, AP-030 | Detection, telemetry, time | Read-only + approved test events |
| Business/quality | AP-020, AP-038, AP-039 | ERP/MES/QMS/WMS/traceability | Non-destructive |
| AI/analytics | AP-031 | Data/model/API integrity and exposure | Controlled |

## Path interpretation
Each attack path must be traced from **entry condition → identity/privilege → network/trust boundary → target asset → capability → potential impact → detection/response → recovery**. A path may contain multiple assets and multiple VAPT phases.

## Scope preservation
The path layer does not replace the master matrix, auditor checklist, tools, findings/evidence or standards layers. It cross-references them.
