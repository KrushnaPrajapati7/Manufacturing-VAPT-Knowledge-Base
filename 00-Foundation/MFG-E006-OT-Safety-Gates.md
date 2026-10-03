---
docType: knowledge_unit
knowledgeId: E006
sector: manufacturing_industrial
phase: Foundation
topic: OT Safety Gates
safety: controlled
status: working-rebuild
---

# E006: OT Safety Gates

## Assessment Question

**Before a cybersecurity test can affect an OT environment, has the activity passed the required operational and safety decision gates?**

## Purpose

E006 is a decision architecture for safe cybersecurity testing. It is not a functional-safety standard and does not replace plant safety procedures, permits, lockout/tagout requirements, emergency procedures or competent safety authority.

NIST SP 800-82 Rev. 3 explicitly addresses OT security while considering performance, reliability and safety requirements.

## 1. Safety Is a Gate, Not a Disclaimer

For an OT target, determine:

1. Is it OT?
2. Is it connected to production?
3. Could the planned activity affect a process, controller, equipment, alarm, monitoring function or availability?
4. Is a safety-related function involved?
5. Is the activity explicitly authorized?
6. Has the responsible operational owner approved it?
7. Has the relevant safety authority reviewed it where required?
8. Is the testing window appropriate?
9. Is monitoring available?
10. Are abort and escalation conditions defined?

If a required answer is unknown, do not assume permission to proceed.

## 2. Test Modes

Classify the intended activity:

- documentation-only;
- passive observation;
- read-only authenticated review;
- low-impact active testing;
- controlled validation;
- intrusive testing;
- exploitation;
- configuration change;
- process-affecting activity.

The higher the potential operational effect, the stronger the approval and control requirements.

## 3. Preferred Testing Order

Where the objective can be achieved without operational interaction, prefer:

Documentation → Passive Observation → Configuration Review → Controlled Read-Only Validation → Limited Active Validation → More Intrusive Validation

Do not use intrusive activity merely because it produces stronger evidence if safer evidence is sufficient.

## 4. Production Decision

Classify the target:

- production;
- production-supporting;
- pre-production;
- laboratory;
- test;
- development;
- simulation/digital twin;
- unknown.

A lab result does not automatically prove that the same technique is safe in production.

## 5. Safety-Relevant Systems

If a target participates in a safety function or safety-related process, establish:

- system identity;
- responsible authority;
- approved test method;
- required permits/procedures;
- testing window;
- monitoring;
- abort authority;
- recovery method.

Cybersecurity testing must not independently modify or disable a safety function unless the engagement and applicable operational/safety process explicitly permit it.

## 6. Abort Conditions

Examples:

- unexpected process behavior;
- controller instability;
- loss of monitoring;
- alarm abnormalities;
- unexplained communication loss;
- equipment instability;
- unexpected production effect;
- safety concern;
- inability to communicate with the operational owner;
- evidence that activity exceeds approved conditions.

Exact thresholds must be engagement-specific.

## 7. Emergency Sequence

STOP TEST → PRESERVE MINIMUM EVIDENCE → NOTIFY DESIGNATED CONTACT → FOLLOW PLANT RESPONSE → WAIT FOR AUTHORIZATION BEFORE RESUMPTION

The assessor should not improvise recovery actions that belong to plant operations or safety personnel.

## 8. Rollback and Recovery

Before controlled changes, establish:

- whether a backup exists;
- whether restoration has been tested;
- who performs rollback;
- expected recovery path;
- whether vendor support is required;
- who authorizes restoration;
- what evidence must be preserved.

“Backup exists” is not equivalent to “recovery is proven.”

## 9. Offensive Questions

- What capability could the test expose?
- Could the activity change state rather than only observe it?
- Could authentication attempts affect an operational account?
- Could scanning load a fragile device?
- Could exploitation affect timing or availability?
- Could an engineering action change process behavior?

## 10. Defensive Questions

- Is testing visible to OT monitoring?
- Can operations identify the assessor?
- Are test activities distinguishable from hostile activity?
- Are alarms and events being monitored?
- Is there a clear stop/escalation path?
- Can the organization determine what changed during the test?

## 11. Evidence

Record:

- target;
- test mode;
- authorization;
- operational approval;
- safety review where applicable;
- window;
- monitoring;
- start/stop times;
- observed effects;
- abort events;
- final disposition.

Do not store client safety documentation in the public KB.

## 12. Finding Logic

Failure to have a safety gate is not automatically a cybersecurity vulnerability.

Possible classifications:

- process deficiency;
- authorization deficiency;
- operational-control weakness;
- cybersecurity control weakness;
- vulnerability;
- not assessed.

The finding must identify the specific requirement and evidence.

## Exit Criteria

Testing proceeds only when the required safety/operational conditions are satisfied and the assessor knows:

- what is permitted;
- what is prohibited;
- what triggers a stop;
- who can stop the test;
- who can authorize resumption;
- how the plant responds to an unexpected condition.

## Sources

- NIST SP 800-82 Rev. 3.
- Applicable plant safety procedures and competent safety authority.
- Applicable ISA/IEC functional-safety and industrial cybersecurity requirements as engagement context.

**Boundary:** E006 defines the testing safety gate. It does not define the plant's functional-safety engineering design.
