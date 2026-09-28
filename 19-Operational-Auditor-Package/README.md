# Operational Auditor Package

This layer turns the Manufacturing VAPT Knowledge Base into a practical engagement workflow. It is additive to the v1.8.0 knowledge base and preserves the full 23-family / 406-asset scope.

## Core workflow

Authorization & ROE → Scope & Asset Inventory → Architecture/Trust Boundaries → Safety Gate → Phase Planning → Test Execution → Observation → Evidence → Finding/Risk → Reporting → Remediation → Retest → Closure / Risk Acceptance.

## Scope rule

The master asset matrix remains authoritative. Every in-scope asset must receive a status: Not Started, In Progress, Tested, Finding, Not Applicable, Out of Scope, Not Tested, Unknown, Retest Pending, or Retested. Never silently omit an asset.

## OT/ICS rule

Default to passive/read-only assessment for production OT. Any active, state-changing, disruptive, exploitative, or process-impacting activity requires explicit authorization, safety approval, defined stop conditions, controlled windows, and preferably lab/digital-twin validation.

## Included artifacts
- Engagement operating workflow
- Auditor operating procedure
- Master assessment workbook
- Asset coverage tracker for all 406 assets
- Phase execution tracker
- Evidence / observation / finding / retest registers
- Risk and exception registers
- OT safety gate
- Coverage and QA dashboard
- Professional VAPT report framework
- Report finding template
- Engagement closeout checklist
