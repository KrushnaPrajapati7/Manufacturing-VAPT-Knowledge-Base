# v1.8.0 — Final QA / Coverage Audit / Release

- Added `00-Foundation/MFG-FINAL-QA-RELEASE-AUDIT-v1.8.0.md`.
- Audited the complete 23-family / 406-asset master scope across auditor, tool, threat and RAG asset layers.
- Validated 474 logical RAG knowledge units, structured catalog IDs, CSV parsing and release metadata.
- Confirmed OT safety/assessment-state requirements remain represented.
- Confirmed no master asset scope was removed by later layers.
- Marked v1.8.0 as the final release for the original eight-step architecture; future changes are versioned enhancements rather than missing core layers.

# v1.7.0 — RAG / AI Retrieval Layer

- Added `18-RAG-AI-Retrieval/` with document, knowledge, asset and relationship indexes.
- Added deterministic JSONL ingestion export for 474 logical knowledge units.
- Added semantic chunking and metadata rules that preserve safety/OT context.
- Added retrieval policy, query routing and evaluation dataset.
- Added RAG QA report and machine-readable RAG schema.
- Preserved the complete 23-family / 406-asset manufacturing scope and existing 474 knowledge units.


## [1.6.0] - Threat / Attack-Path & MITRE ICS Layer

- Added `17-Threat-Attack-Paths/`.
- Added 12 MITRE ATT&CK for ICS tactic records.
- Added a manufacturing-relevant MITRE ICS technique catalog.
- Added 40 reusable manufacturing attack-path scenarios spanning external, IT, identity, IT/OT, engineering, OT/ICS, industrial, wireless, physical, cloud, API, supply chain, backup/DR, monitoring, utilities, business applications, data and AI.
- Added threat/attack-path mappings for all 406 asset/technology entries.
- Added attack-path assessment methodology, evidence guidance and OT safety constraints.
- Preserved the complete 23-family/406-asset master scope.
# Changelog

## 1.4.0
- Added `13-Standards/MFG-STANDARDS-REGISTRY.csv`.
- Added `13-Standards/MFG-STANDARDS-CONTROL-MAPPING.csv` with 51 assessment mappings.
- Added standards mapping guidance and QA report.
- Updated project summary and repository version to 1.4.0.


## 1.0.0 — 2026-09-28
- Master manufacturing asset taxonomy.
- Master VAPT scope matrix.
- Eight VAPT phases.
- 281 structured knowledge units.
- Metadata and finding schemas.
- Standards and tooling guidance.
- GitHub workflow documentation.

## 1.2.0 — Master Asset × VAPT Knowledge Matrix
- Added authoritative 406-entry asset-to-phase-to-knowledge-unit matrix.
- Added standards, assessment mode, prerequisites and evidence columns.
- Preserved original scope matrix for compatibility.

## 1.3.0 — Findings & Evidence Layer
- Added the standardized Observation → Evidence → Finding → Retest lifecycle.
- Added manufacturing-specific finding, evidence, observation and retest templates.
- Added finding lifecycle QA guidance.
- Added machine-readable observation, evidence, finding and retest schemas.
- Added a traceability catalog for record-level QA.
- Preserved explicit OT/ICS safety gates and production-impact handling.


## v1.5.0 — Tool → Asset → Phase → Test Mapping

- Added complete tool/test mapping layer covering all 406 master asset entries.
- Added 100-tool/tool-class registry with safety and usage guidance.
- Added phase-level repeatable test-case catalog.
- Added tool-to-test relationships.
- Added QA coverage report.
- Preserved the master scope as the authoritative completeness baseline.
## 2.0.0 — Operational Auditor Package
- Added end-to-end manufacturing VAPT auditor workflow and operating procedure.
- Added practical assessment workbook preserving all 23 asset families and 406 asset/technology entries.
- Added asset, phase, test execution, observation, evidence, finding, retest, exception, OT safety and coverage registers.
- Added professional VAPT report framework and finding template.
- Added engagement closeout checklist.
- No existing scope layer removed.
