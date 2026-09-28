# Step 5 — Tool → Asset → Phase → Test Mapping

This layer operationalizes the complete manufacturing asset scope without replacing the master scope matrix. Every one of the 406 master asset/technology entries is represented in `MFG-TOOL-ASSET-PHASE-TEST-MAPPING.csv`.

## Data flow

`Asset → Applicable VAPT Phase → Knowledge Units → Recommended Tool/Tool Class → Test Coverage → Evidence → Finding → Retest`

## Files

- `MFG-TOOL-REGISTRY.csv` — 100 tools/tool classes with purpose, use, safety mode and standards context.
- `MFG-TEST-CASE-CATALOG.csv` — repeatable phase-level test cases covering reconnaissance, enumeration, vulnerability assessment, identity, application/API, OT/ICS, validation/business impact and reporting/retest.
- `MFG-TOOL-TEST-MAPPING.csv` — tool-to-test relationships.
- `MFG-TOOL-ASSET-PHASE-TEST-MAPPING.csv` — all 406 manufacturing assets mapped to phases, knowledge units, tools, tests, preconditions, evidence and safety guardrails.
- `MFG-TOOL-MAPPING-QA-REPORT.md` — coverage and consistency checks.

## Scope preservation rule

The master asset taxonomy remains authoritative. No asset is removed because a particular tool does not apply. An auditor must use `Not Applicable`, `Out of Scope`, `Not Tested`, or `Unknown` rather than silently omitting an asset. Tool selection is contextual: a listed tool is a recommended capability/tool class, not a mandatory product.

## Safety

OT/ICS, safety systems, production equipment, utilities and cyber-physical assets default to passive/read-only or tightly controlled validation. Disruptive testing belongs in an approved lab, digital twin, maintenance window or explicitly engineered production test. Never treat a scanner result or version match as proof of compromise.
