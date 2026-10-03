---
docType: knowledge_unit
knowledgeId: E008
sector: manufacturing_industrial
phase: Foundation
topic: Assessment Preconditions and Readiness
safety: controlled
status: working-rebuild
---

# E008: Assessment Preconditions and Readiness

## Assessment Question

**Is the environment, engagement team and operational context ready for the planned assessment activity?**

## Purpose

Authorization alone does not make an assessment ready to execute.

E008 verifies prerequisites such as scope, contacts, access, monitoring, backups, maintenance windows, test accounts and operational coordination.

## 1. Readiness Categories

### Governance

- authorization available;
- ROE approved;
- scope current;
- scope-change process defined.

### People

- engagement lead identified;
- technical contacts available;
- operational owner available;
- safety contact identified where required;
- emergency escalation available.

### Technical

- approved test connectivity works;
- approved test accounts work;
- required tooling is ready;
- time synchronization is understood;
- logging/monitoring contacts are known.

### Operational

- maintenance window confirmed;
- production state known;
- active incidents known;
- change freeze considered;
- operational constraints understood.

### Recovery

- backup status known;
- rollback responsibility known;
- recovery process identified;
- vendor support available where required.

## 2. Readiness State

Use:

- READY
- READY WITH CONDITIONS
- NOT READY
- UNKNOWN

Do not start an activity marked NOT READY or UNKNOWN merely because the assessment schedule is tight.

## 3. Readiness Checklist

| Question | Status |
|---|---|
| Authorization verified? | |
| Scope current? | |
| ROE current? | |
| Production status known? | |
| OT relevance known? | |
| Safety review completed if needed? | |
| Test accounts available? | |
| Monitoring contact available? | |
| Emergency contact available? | |
| Testing window confirmed? | |
| Recovery path understood? | |
| Third-party coordination complete? | |
| Evidence storage ready? | |

## 4. Technical Readiness

Validate only what is necessary.

Examples:

- Can the approved assessment workstation reach the approved target?
- Does the test identity authenticate as expected?
- Are required VPN/jump-host controls functioning?
- Is the test environment the intended environment?
- Are required logs available?

Do not perform broad discovery merely to prove connectivity.

## 5. Operational Readiness

Ask:

- Is production running?
- Is maintenance active?
- Is an unusual production event occurring?
- Is another assessment already active?
- Are plant personnel aware of the test?
- Are there known fragile systems?
- Is a vendor activity occurring concurrently?

Unexpected operational conditions can change the safe testing decision.

## 6. Monitoring Readiness

Determine, where required:

- who watches the environment;
- which telemetry is available;
- who receives alerts;
- how the assessor identifies test traffic;
- how abnormal behavior is escalated.

A SIEM being installed does not prove that relevant activity will be detected.

## 7. Offensive Questions

- Can the planned test be executed without violating a readiness condition?
- Is the intended identity authorized?
- Is the intended target confirmed?
- Is the environment actually the one approved?

## 8. Defensive Questions

- Can defenders distinguish authorized testing from an incident?
- Are monitoring teams informed?
- Are relevant logs available?
- Can the organization correlate test activity?

## 9. Failure Conditions

Pause when:

- target identity is uncertain;
- authorization changed;
- production state changed materially;
- operational owner is unavailable where required;
- safety approval is missing;
- monitoring/recovery prerequisites are missing for the planned activity;
- test access is broader than approved.

## 10. Exit Criteria

The assessment can proceed when all prerequisites required by the engagement are verified and documented.

## Sources

- NIST SP 800-115.
- NIST SP 800-82 Rev. 3.

**Boundary:** E008 owns readiness. It does not redefine authorization (E001) or detailed safety controls (E006).
