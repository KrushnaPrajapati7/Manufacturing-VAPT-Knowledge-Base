# 16 — Findings & Evidence

This layer connects the auditor checklist to defensible assessment records:

**Checklist → Observation → Evidence → Finding → Risk → Recommendation → Retest**

The templates are reusable and intentionally exclude client-specific credentials, IPs, screenshots, secrets, proprietary data, or exploit payloads.

## Record lifecycle

1. Start from an asset/checklist item and knowledge unit.
2. Record the expected state and observed state as an **Observation**.
3. Attach one or more controlled **Evidence** records.
4. Promote a validated observation into a **Finding** when a security weakness is supported by sufficient evidence.
5. Assess technical, business, operational, recovery, and safety impact.
6. Assign severity/risk using the engagement's approved methodology; CVSS is a technical severity input, not a substitute for manufacturing context.
7. Record remediation and compensating controls.
8. Track owner/status/target date.
9. Perform and document a **Retest** against the original finding.
10. Record residual risk and closure/reacceptance decision.

## Status discipline

Use explicit states such as `Not Started`, `In Progress`, `Tested`, `Finding`, `Not Applicable`, `Out of Scope`, `Not Tested`, `Unknown`, `Retest Pending`, and `Retested` for checklist coverage. A finding itself should additionally use its lifecycle status: `Open`, `Remediation In Progress`, `Retest Pending`, `Fixed`, `Partially Fixed`, `Risk Accepted`, or `Closed`.

## Manufacturing safety rule

For OT/ICS and cyber-physical assets, evidence collection and validation must follow the approved rules of engagement and safety gate. Default to passive/read-only validation unless controlled testing is explicitly authorized. Do not use generic finding templates as authorization to manipulate process state, safety functions, production logic, or availability.

## Machine-readable schemas

- `schemas/observation-schema.yaml`
- `schemas/evidence-schema.yaml`
- `schemas/finding-schema.yaml`
- `schemas/retest-schema.yaml`
- `schemas/finding-evidence-catalog.csv`

## Human-use templates

- `MFG-OBSERVATION-RECORD-TEMPLATE.md`
- `MFG-EVIDENCE-RECORD-TEMPLATE.md`
- `MFG-FINDING-TEMPLATE.md`
- `MFG-RETEST-RECORD-TEMPLATE.md`
- `MFG-FINDING-LIFECYCLE.md`

## Required quality gates

A finding should not be closed merely because a scanner no longer reports it. The reviewer should verify the original weakness, the remediation claim, the relevant asset/environment, evidence sufficiency, manufacturing impact, and residual risk.
