---
docType: knowledge_unit
answerType: assessment_methodology
knowledgeId: E001
sector: manufacturing_industrial
phase: Foundation
topic: Scope Authorization Rules Of Engagement
assetTags: ["governance", "scope", "authorization", "rules-of-engagement", "safety"]
safety: controlled
status: working-rebuild
version: 2.0
---

# E001: Scope, Authorization & Rules of Engagement

## 1. Assessment Question

**How does an authorized manufacturing-sector VAPT team establish, verify, maintain and enforce the boundaries within which security assessment activity may be performed?**

This unit governs the assessment boundary. It does **not** grant permission to test a system, replace a contract, or override plant, safety, legal, regulatory, vendor or operational requirements.

NIST defines Rules of Engagement (ROE) as detailed guidelines and constraints for executing security testing; the ROE is established before testing and gives the test team authority to conduct the defined activities without obtaining additional permission for each activity. [NIST SP 800-115]

---

## 2. Purpose

E001 establishes the **pre-test control plane** for the entire Manufacturing VAPT Knowledge Base.

Before reconnaissance, scanning, authentication testing, web/API testing, OT protocol testing, cloud assessment, physical assessment or validation begins, the assessment team must be able to answer:

- Who authorized this assessment?
- What legal entity and business unit authorized it?
- Which assets, locations, identities, applications, networks and environments are in scope?
- Which activities are explicitly permitted?
- Which activities are prohibited or conditionally permitted?
- Where and when may testing occur?
- Who can approve a scope change?
- Who owns the affected operational process?
- What safety and operational controls must exist before testing?
- What happens if an unexpected critical condition is discovered?
- What happens if the assessor accidentally reaches an out-of-scope asset?
- Who must be contacted if testing produces an operational or safety concern?
- What evidence may be collected, where may it be stored, and who may access it?

The result is a **testable, auditable assessment boundary**, not merely a paragraph stating that the assessor has permission.

---

## 3. Scope of This Knowledge Unit

### In scope

- assessment authorization
- statement of work and engagement documentation
- scope definition and asset identification
- production, staging, laboratory and development environments
- network, application, API, cloud and OT boundaries
- physical locations and facilities where explicitly authorized
- third-party and supplier dependencies
- identities and test accounts
- permitted assessment techniques
- prohibited and conditionally permitted techniques
- testing windows and operational constraints
- safety and operational approvals
- communications and escalation
- scope-change control
- out-of-scope discovery
- accidental access
- unexpected critical findings
- evidence ownership and handling requirements
- emergency stop and test termination
- close-out and scope reconciliation

### Out of scope

E001 does not prescribe:

- a specific exploit;
- a particular scanning product;
- a plant's functional-safety design;
- an organization's legal advice;
- a universal risk score;
- a universal maintenance-window duration;
- vendor-specific operating procedures;
- a substitute for the facility's emergency response or safety procedures.

Those matters belong to the relevant engagement documents or later knowledge units.

---

## 4. Core Principle

### Authorization is not the same as scope.

A signed engagement does not automatically authorize every action against every system discovered during the assessment.

The assessor must maintain a distinction between:

1. **Engagement authorization** — the organization has authorized an assessment.
2. **Scope** — the assets, environments, people, locations and functions included.
3. **ROE** — the permitted methods, constraints and operating rules.
4. **Operational approval** — the responsible operational authority has accepted the activity for the relevant environment/time.
5. **Safety approval** — required safety authorities have reviewed the activity where safety-relevant systems or processes could be affected.
6. **Technical readiness** — prerequisites for safe execution exist.
7. **Evidence authority** — collection, retention and handling of evidence are defined.
8. **Scope-change authority** — a named person/process can approve changes.

A VAPT team must not treat one of these as silently substituting for another.

---

## 5. Manufacturing-Specific Security Context

Manufacturing environments are cyber-physical environments. NIST SP 800-82 Rev. 3 specifically addresses OT security while accounting for performance, reliability and safety requirements.

Therefore, a scope boundary must not be expressed only as:

`10.10.10.0/24`

or:

`app.example.com`

The assessor should understand what the technical boundary represents operationally.

For each relevant in-scope area, establish relationships such as:

**Asset → Zone/Boundary → Function → Process → Production Dependency → Safety Dependency → Recovery Dependency**

Examples of scope objects include:

- enterprise systems supporting manufacturing;
- MES/MOM;
- historians;
- SCADA;
- DCS;
- PLC/RTU/controller environments;
- HMIs;
- engineering workstations;
- remote-access infrastructure;
- OT network infrastructure;
- industrial gateways;
- IIoT platforms;
- manufacturing APIs;
- cloud services supporting plant operations;
- vendor-maintained systems;
- laboratory/test cells;
- production lines;
- quality systems;
- engineering/IP systems.

The presence of an asset in the same network or facility does **not** by itself make it in scope.

---

# 6. Scope Model

The assessment team should maintain a structured scope register.

| Scope dimension | Minimum question |
|---|---|
| Legal entity | Which organization authorized the work? |
| Business unit | Which division/site/function is included? |
| Facility | Which physical locations are included? |
| Environment | Production, staging, lab, development or other? |
| Network | Which ranges, segments, VLANs, zones or conduits? |
| Host | Which hosts/devices are explicitly included? |
| Application | Which applications and functions? |
| API | Which API hosts, routes or environments? |
| Cloud | Which accounts/subscriptions/projects/resources? |
| OT/ICS | Which control, supervisory and engineering assets? |
| Identity | Which identities/test accounts may be used? |
| Third party | Which suppliers/MSPs/vendors are included? |
| Physical | Which physical testing activities/locations? |
| Wireless | Which wireless infrastructure, if authorized? |
| Social engineering | Which people/channels, if explicitly authorized? |
| Time | When may activity occur? |
| Methods | Which techniques are permitted? |
| Prohibitions | Which techniques/actions are forbidden? |
| Evidence | What may be collected and retained? |
| Escalation | Who must be contacted for exceptions? |

The scope register should use unambiguous identifiers wherever possible.

---

# 7. Scope States

Every discovered target should be placed into an explicit state:

### IN-SCOPE

The target is explicitly authorized and satisfies the applicable technical and operational conditions.

### CONDITIONALLY IN-SCOPE

The target may be tested only after an additional condition is satisfied.

Examples:

- maintenance window;
- operations approval;
- safety review;
- vendor approval;
- dedicated test account;
- backup/restore verification;
- passive-only restriction.

### OUT-OF-SCOPE

The target must not be actively tested.

### UNKNOWN

The assessor cannot determine whether the target is authorized.

**UNKNOWN must not be interpreted as IN-SCOPE.**

### DISCOVERED OUT-OF-SCOPE

The assessor encountered the target during authorized work but has no authorization to continue testing it.

The correct action is to preserve only the minimum information needed to report the discovery according to the ROE and escalate it through the defined process.

---

# 8. Pre-Engagement Authorization Gate

Before technical activity begins, confirm the following.

## 8.1 Engagement identity

Record:

- client/legal entity;
- assessment name or identifier;
- assessment purpose;
- assessment type;
- authorized assessment period;
- assessment team;
- responsible engagement lead;
- client authorization authority.

## 8.2 Authorization evidence

The engagement package should identify the authoritative authorization document(s), such as:

- signed statement of work;
- authorization letter;
- approved assessment order;
- contract/engagement documentation;
- applicable internal authorization record.

The KB should not store confidential client contracts.

Instead, record a reference/identifier in the engagement's private assessment records.

## 8.3 Asset authorization

Verify that the scope identifies the actual target rather than relying on assumptions such as:

- "the plant network";
- "all servers";
- "the corporate environment";
- "all IPs we discover."

Where practical, use exact:

- hostnames;
- IP ranges;
- asset identifiers;
- application names;
- cloud account/resource identifiers;
- site identifiers;
- OT zone identifiers;
- API endpoints;
- physical locations.

---

# 9. Rules of Engagement

The ROE should convert authorization into executable constraints.

At minimum, define:

### 9.1 Permitted activity

Examples may include, where explicitly authorized:

- passive observation;
- configuration review;
- authenticated security assessment;
- controlled service discovery;
- web/API testing;
- vulnerability verification;
- controlled exploitation;
- cloud configuration assessment;
- wireless testing;
- physical security testing;
- social engineering.

The exact permitted activity must be engagement-specific.

### 9.2 Restricted activity

Activities may require explicit additional approval.

Examples:

- active scanning of production OT;
- authentication testing against shared operational accounts;
- exploit validation;
- changes to device configuration;
- service restart;
- controlled failover;
- firmware interaction;
- PLC/HMI interaction;
- testing of safety-related systems;
- vendor remote-access testing;
- physical interruption;
- denial-of-service simulation.

### 9.3 Prohibited activity

Examples may include:

- destructive actions;
- uncontrolled denial-of-service;
- deliberate process disruption;
- unauthorized safety-function manipulation;
- deletion or alteration of production data;
- unauthorized persistence;
- unauthorized credential harvesting;
- testing third-party assets without their authorization;
- accessing unrelated personal or proprietary information;
- expanding scope based only on discovery.

The list must be tailored to the engagement rather than copied blindly from this KB.

---

# 10. Production vs Non-Production

The ROE must explicitly distinguish:

- production;
- pre-production/staging;
- development;
- test;
- laboratory;
- digital-twin/simulation;
- training environments.

A technique acceptable in a laboratory may be unacceptable in production.

The assessor must not infer that a production control is safe to test merely because the same technology was safely tested elsewhere.

For OT, NIST SP 800-82 Rev. 3 emphasizes the unique performance, reliability and safety considerations of OT.

---

# 11. OT Safety and Operational Gate

E001 establishes the **authorization gate**; E006 will define the detailed OT safety-gate methodology.

For E001, the required decision is:

`Can this activity proceed under the current authorization, operational state and safety conditions?`

If any required authorization or operational condition is missing:

**STOP / DO NOT PROCEED**

At minimum, establish:

- operational owner;
- safety owner where applicable;
- maintenance window;
- process criticality;
- known operational constraints;
- monitoring responsibility;
- abort authority;
- emergency contact;
- rollback/recovery expectations;
- required vendor involvement.

Safety requirements are not satisfied by the pentester's own judgment.

---

# 12. Scope by Network and Trust Boundary

The scope should identify relevant boundaries, not only address ranges.

Document, where applicable:

- enterprise network;
- industrial DMZ;
- OT zones;
- safety-related zones;
- engineering zones;
- vendor-access zones;
- wireless networks;
- cloud connectivity;
- remote-access gateways;
- management networks;
- data exchange paths.

A target may be technically reachable but still outside the authorized assessment boundary.

Conversely, an in-scope asset may have dependencies outside scope. The assessor must document the dependency rather than silently testing through it.

---

# 13. Third-Party and Supplier Scope

Manufacturing assessments frequently involve:

- OEMs;
- system integrators;
- managed service providers;
- remote-support vendors;
- cloud providers;
- software vendors;
- equipment vendors.

Client authorization does not automatically authorize testing a third party.

For each third-party dependency determine:

- whether it is in scope;
- who owns the authorization;
- whether separate authorization is required;
- what interfaces may be tested;
- whether testing must be coordinated;
- who receives emergency notifications;
- whether vendor support is required;
- whether evidence contains third-party confidential information.

CISA's ICS guidance specifically addresses secure management of remote access to industrial control environments, reinforcing the need to treat remote/vendor access as an explicit security boundary rather than an incidental detail.

---

# 14. Identity and Test Account Scope

Define:

- named assessor identities;
- client-provided test accounts;
- privilege level;
- allowed systems;
- authentication method;
- MFA requirements;
- credential delivery method;
- credential expiration;
- emergency/break-glass restrictions;
- service-account restrictions.

Do not use privileged production identities simply because they are available.

If an identity is outside the agreed test model, stop and obtain clarification.

---

# 15. Physical Testing

If physical testing is authorized, define separately:

- facility/location;
- dates and hours;
- permitted entry methods;
- permitted areas;
- badge/access-control testing;
- equipment interaction;
- photography;
- removable media;
- social engineering;
- personnel interaction;
- safety/PPE requirements;
- escort requirements;
- emergency procedures.

Physical authorization must not be inferred from cyber authorization.

---

# 16. Social Engineering

If social engineering is included, the ROE should define:

- target population;
- approved scenarios;
- communication channels;
- timing;
- prohibited scenarios;
- data collection boundaries;
- credential handling;
- escalation;
- stop conditions;
- notification requirements.

Sensitive personal information collected during testing should be minimized and handled under the engagement's evidence/data-handling requirements.

---

# 17. Cloud and SaaS Scope

Cloud authorization should identify the relevant:

- organization;
- tenant;
- account/subscription/project;
- regions;
- resources;
- workloads;
- APIs;
- identities;
- logging/security services;
- third-party SaaS integrations.

Do not infer cloud scope from a corporate domain or from ownership of a parent organization.

Where cloud provider testing restrictions or notification requirements apply, they must be checked before testing.

---

# 18. Scope Change Control

Scope must be treated as a controlled configuration.

A scope change should identify:

1. requested change;
2. reason;
3. target;
4. requested activities;
5. potential impact;
6. operational owner;
7. safety implications;
8. authorization authority;
9. approval/rejection;
10. effective time;
11. assessor notification;
12. evidence of the decision.

**Discovery is not authorization.**

If an assessor discovers a potentially vulnerable system outside scope, the correct sequence is:

**Discover → Record minimally → Do not actively test → Escalate → Obtain explicit authorization if testing is desired → Update scope → Proceed only after approval**

---

# 19. Accidental Access

Accidental access can occur through:

- shared infrastructure;
- routing;
- DNS;
- inherited credentials;
- shared management platforms;
- vendor gateways;
- misconfigured segmentation;
- cloud trust relationships;
- redirected applications.

The assessor must not convert accidental access into implied authorization.

Record enough information to establish what occurred, avoid unnecessary interaction, and follow the ROE's escalation procedure.

---

# 20. Unexpected Critical Condition

Define the escalation path before testing begins.

Examples include:

- unexpected production instability;
- safety-system concern;
- loss of monitoring;
- controller instability;
- unexplained process change;
- evidence of active compromise;
- access to sensitive safety or proprietary information;
- unexpected access to a high-criticality asset.

The assessor should have:

- stop authority;
- client emergency contact;
- operational contact;
- safety contact where applicable;
- engagement lead;
- evidence-preservation instructions.

The ROE should state whether the assessor must immediately stop all activity or only activity affecting the suspected condition.

---

# 21. Emergency Stop

Every engagement involving production or OT should define a practical stop mechanism.

At minimum:

**Trigger → Assessor Action → Client Notification → Operational Response → Evidence Preservation → Restart Authorization**

The assessor must know who can authorize resumption.

A test must not automatically resume because the immediate symptom disappeared.

---

# 22. Evidence Boundaries

E001 defines what evidence the assessor is permitted to collect; E007 defines the detailed evidence-management methodology.

The ROE should establish:

- permitted evidence types;
- prohibited data;
- credential handling;
- personal-data handling;
- production-data handling;
- proprietary engineering information;
- PLC logic;
- recipes;
- CAD/engineering drawings;
- network diagrams;
- packet captures;
- screenshots;
- logs;
- API requests/responses;
- cloud configuration exports.

The reusable KB must never contain client evidence.

---

# 23. Offensive and Defensive Interpretation

E001 should establish two questions for every boundary.

### Offensive

**What unauthorized capability would become possible if this boundary were weak or incorrectly defined?**

Examples:

- access from an unauthorized network;
- supplier access beyond intended scope;
- test credentials reaching production;
- an assessor reaching an unintended management interface;
- a compromised enterprise system reaching OT.

### Defensive

**Would the organization know that the boundary was crossed or violated?**

Consider:

- access logging;
- authentication records;
- firewall/segmentation telemetry;
- VPN logs;
- OT monitoring;
- EDR/NDR/IDS telemetry;
- SIEM correlation;
- operational alerts;
- escalation workflows.

The defensive question does not turn E001 into a detection module; it ensures that scope boundaries can be operationally enforced and observed.

---

# 24. Scope Validation Procedure

Use the following sequence before technical testing:

`Authorization`
↓
`Scope Register`
↓
`Asset/Environment Validation`
↓
`Production vs Non-Production Decision`
↓
`OT/Safety Relevance Check`
↓
`Permitted/Restricted/Prohibited Technique Check`
↓
`Operational Approval`
↓
`Testing Window`
↓
`Monitoring + Escalation Ready`
↓
`Test`

If a required gate fails:

`STOP / ESCALATE`

---

# 25. Scope Validation Record

For each target or target group, maintain a private assessment record similar to:

| Field | Example value |
|---|---|
| Target ID | ENG-OT-001 |
| Asset identifier | Client asset ID |
| Technical identifier | Hostname/IP/resource ID |
| Environment | Production |
| Zone | Client-defined OT zone |
| Function | Engineering workstation |
| Owner | Operational owner |
| Scope state | In-scope / Conditional / Out-of-scope / Unknown |
| Permitted activity | Client-approved activities |
| Restricted activity | Activities requiring approval |
| Prohibited activity | Engagement-specific restrictions |
| Test window | Approved window |
| Safety review | Required / Not required |
| Operational approval | Name/reference |
| Monitoring | Responsible team/system |
| Emergency contact | Engagement reference |
| Evidence restrictions | Engagement-specific |
| Scope version | Version/reference |
| Approval reference | Private engagement reference |

Never populate this reusable KB with real client identifiers.

---

# 26. Finding Logic for Scope Violations

A scope violation is not automatically a vulnerability.

Examples:

- An assessor discovers an out-of-scope host: **not automatically a vulnerability.**
- A firewall exposes an out-of-scope system: **may become an assessment observation, but requires separate authorization before active testing.**
- A vendor account reaches an unauthorized zone: **potential security finding if the condition is within the authorized assessment and can be safely validated.**
- A contract does not name an asset: **authorization gap, not automatically a technical vulnerability.**

Findings must preserve the distinction between:

**Authorization defect → Scope defect → Control weakness → Security weakness → Vulnerability → Exploitability → Manufacturing impact**

---

# 27. Common Failure Modes

### Failure 1 — "The client owns it, so it is in scope."

Ownership does not replace explicit scope.

### Failure 2 — "It is on the same subnet."

Network proximity does not establish authorization.

### Failure 3 — "The client said test everything."

Translate broad language into an explicit scope and ROE before testing.

### Failure 4 — "We found a PLC, so we can enumerate it."

Discovery does not authorize OT interaction.

### Failure 5 — "The system is not production, so anything is allowed."

Non-production status reduces some risks but does not remove authorization, data, safety, vendor or availability constraints.

### Failure 6 — "The scan already started, so finish it."

A newly discovered constraint or operational change can require immediate suspension.

### Failure 7 — "The vulnerability is critical, so we can test it."

Severity does not expand authorization.

### Failure 8 — "We can test the vendor because the customer hired us."

Third-party authorization must be established separately where required.

---

# 28. Minimum Exit Criteria

E001 is complete for an engagement only when:

- authorization is identified;
- scope is explicit;
- scope identifiers are usable;
- production/non-production status is known;
- OT relevance is known;
- safety relevance is known;
- permitted techniques are documented;
- prohibited techniques are documented;
- restricted techniques have an approval path;
- testing windows are known;
- operational ownership is identified;
- escalation contacts are known;
- emergency-stop conditions are defined;
- scope-change authority is defined;
- evidence boundaries are defined;
- third-party dependencies are addressed;
- the assessor can determine whether a discovered target is in, conditionally in, out, or unknown.

---

# 29. Related Foundation Boundaries

E001 owns **authorization and assessment boundaries**.

It deliberately does not own the detailed methodology of:

- E002 — manufacturing architecture/context;
- E003 — asset classification and ownership model;
- E004 — manufacturing business-process mapping;
- E005 — IT/OT trust boundaries and zones/conduits;
- E006 — OT safety gates;
- E007 — evidence/data handling;
- E008 — readiness/preconditions;
- E009 — finding lifecycle/risk decision;
- E010 — assessment lifecycle/KB retrieval.

Those modules may reference E001 but should not reproduce its full content.

---

# 30. Standards and Source Mapping

### Primary sources

**NIST SP 800-115 — Technical Guide to Information Security Testing and Assessment**

Used for:

- planning and conducting security testing;
- assessment constraints;
- ROE concept;
- technical testing methodology;
- analysis and mitigation.

**NIST SP 800-82 Rev. 3 — Guide to Operational Technology (OT) Security**

Used for:

- OT context;
- performance, reliability and safety considerations;
- OT architectures and environments;
- OT-specific security considerations.

**NIST IR 8183 Rev. 1 — Cybersecurity Framework Version 1.1 Manufacturing Profile**

Used for:

- manufacturing-sector cybersecurity context;
- risk-based manufacturing security framing.

**CISA ICS Recommended Practices**

Used for:

- practical ICS operational security considerations;
- remote access;
- defense-in-depth;
- control-system operational constraints.

### Secondary / contextual sources

Applicable ISA/IEC standards, contractual requirements, organizational policies, vendor documentation and jurisdiction-specific legal requirements may supplement the primary methodology.

The assessment team must record the exact source/version used when an engagement depends on a specific requirement.

---

# 31. Source Limitations

NIST SP 800-115 is a foundational technical assessment guide published in 2008; it should not be treated as a complete manufacturing/OT methodology by itself.

NIST SP 800-82 Rev. 3 is the current final revision identified by NIST as of this KB rebuild; NIST's page also notes that an initial public draft of Revision 4 is available in 2026. This KB must therefore record the source revision used rather than silently treating a draft as the governing final publication.

NIST IR 8183 Rev. 1 is specifically a CSF 1.1 Manufacturing Profile. It should not be represented as a current replacement for CSF 2.0.

This unit translates source guidance into VAPT methodology; it does not reproduce copyrighted standards or override engagement-specific requirements.

---

# 32. Repository Safety

This repository is reusable methodology.

Never commit:

- client credentials;
- API keys;
- private keys;
- personal data;
- production screenshots;
- internal IP inventories;
- plant diagrams;
- PLC programs;
- recipes;
- proprietary engineering drawings;
- confidential contracts;
- customer findings;
- captured authentication tokens;
- raw production packet captures.

Client-specific material belongs in the controlled engagement evidence system, not the public knowledge base.

---

# 33. E001 Quality Gate

Before E001 is considered approved, reviewers must verify:

### Authorization

- [ ] Authorization and ROE are clearly distinguished.
- [ ] Scope is explicit and testable.
- [ ] Scope-change authority is defined.
- [ ] Third-party authorization is addressed.
- [ ] Accidental access is addressed.
- [ ] Unknown targets are not treated as authorized.

### Manufacturing

- [ ] Production and non-production are distinguished.
- [ ] OT relevance is addressed.
- [ ] Operational ownership is addressed.
- [ ] Safety escalation is addressed.
- [ ] Manufacturing impact is not reduced to IP/host/network identifiers.

### Technical

- [ ] Network, application, cloud and OT scope can be represented.
- [ ] Permitted, restricted and prohibited activity are distinct.
- [ ] Identity/test-account boundaries are addressed.
- [ ] Physical and social-engineering authorization are separate.
- [ ] Cloud and third-party scope are explicit.

### Operational

- [ ] Testing windows are defined.
- [ ] Monitoring responsibility is defined.
- [ ] Emergency stop is defined.
- [ ] Unexpected critical conditions have an escalation path.
- [ ] Restart requires appropriate authorization.

### Evidence

- [ ] Evidence boundaries are defined.
- [ ] Client data is excluded from the reusable KB.
- [ ] Private engagement references are separated from reusable methodology.

### Methodology

- [ ] The unit does not duplicate E006's detailed safety procedure.
- [ ] The unit does not duplicate E007's evidence lifecycle.
- [ ] The unit does not duplicate E009's finding lifecycle.
- [ ] The unit can be used before Reconnaissance.
- [ ] No statement implies that discovery equals authorization.

---

## References

- NIST SP 800-115, *Technical Guide to Information Security Testing and Assessment*
- NIST SP 800-82 Rev. 3, *Guide to Operational Technology (OT) Security*
- NIST IR 8183 Rev. 1, *Cybersecurity Framework Version 1.1 Manufacturing Profile*
- CISA, *ICS Recommended Practices*
- CISA, *Configuring and Managing Remote Access for Industrial Control Systems*
- Applicable ISA/IEC 62443 publications
- Engagement-specific contract, authorization and organizational policies

## Source Traceability Note

For the final release, the Foundation source register must record source title, revision/version, publication date, authoritative URL, sections used, modules using the source, rationale and limitations.

