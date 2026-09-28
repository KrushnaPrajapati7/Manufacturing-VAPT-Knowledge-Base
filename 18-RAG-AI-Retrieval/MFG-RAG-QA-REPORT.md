# RAG Layer QA Report

Version target: 1.7.0

## Coverage
- Source Markdown documents indexed: 591
- Logical knowledge units: 474 (expected 474)
- Master asset rows: 406 (expected 406)
- Relationship edges: 15519
- Evaluation queries: 24
- Asset rows missing knowledge-unit IDs: 0
- Knowledge IDs with multiple source copies: 80

## Duplicate handling
Duplicate source copies are not discarded. They remain in the document catalog, while the logical index represents each knowledge ID once and lists all source paths. This prevents duplicate retrieval while preserving source traceability.

## Phase distribution
- unspecified: 193
- Data / Privacy / IP: 18
- Engineering / IIoT / Cloud: 25
- Foundation: 10
- Identity / Authentication / Authorization: 20
- Internal / OT / ICS: 28
- Monitoring / Detection: 17
- Network / Remote / Supply Chain: 20
- Reconnaissance: 34
- Reporting / Remediation / Retest: 16
- Scanning & Enumeration: 26
- Validation / Business Impact: 14
- Vulnerability Assessment: 26
- Web / API / Application / Infrastructure: 27
- application_security: 1
- enumeration: 1
- identity_access: 1
- ot_ics: 1
- reconnaissance: 1
- reporting: 1
- validation_impact: 1
- vulnerability_assessment: 1

## Required retrieval invariants
- 23/23 asset families retained.
- 406/406 asset rows retained.
- 474/474 logical knowledge IDs retained.
- 8 VAPT phases represented in the existing repository.
- Safety and unknown-state metadata preserved.
- Client-specific data remains prohibited.

## QA conclusion
The RAG layer is an index/ingestion layer, not a replacement knowledge source. It preserves the existing scope and adds deterministic identifiers, metadata, relationships, source hashes and retrieval evaluation cases.
