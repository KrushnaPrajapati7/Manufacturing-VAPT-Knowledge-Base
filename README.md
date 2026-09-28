# Manufacturing & Industrial VAPT Knowledge Base

**Version:** 1.7.0 — RAG/AI retrieval-ready release

## Purpose
Reusable knowledge library for authorized manufacturing-sector VAPT planning, assessment, validation, reporting and future AI/RAG retrieval.

## Eight VAPT phases
1. Reconnaissance
2. Scanning & Enumeration
3. Vulnerability Assessment
4. Identity / Authentication / Authorization
5. Web / API / Application / Infrastructure
6. Internal / OT / ICS
7. Validation / Business Impact
8. Reporting / Remediation / Retest

Foundation and cross-cutting domains support all phases.

## Repository contents
- `00-Foundation/` — taxonomy, scope matrix and architecture
- `01-...` through `12-...` — phase/domain knowledge units
- `13-Standards/` — standards/reference families
- `14-Tools/` — tooling guidance
- `schemas/` — machine-readable metadata and finding schemas

## Knowledge-unit format
Each unit follows the supplied E32/E40 reference pattern: metadata, question, description, overview, objectives, manufacturing context, scope/preconditions, evidence, expected output, safety/stop conditions, pitfalls, related knowledge and references.

## Safety
This repository is methodology, not authorization. Test only explicitly authorized assets. Avoid destructive testing, denial-of-service, uncontrolled malware, intentional data destruction and unsafe OT manipulation. For OT/ICS, prefer passive/read-only validation and lab/digital-twin validation for disruptive actions.

## Data separation
Never commit client credentials, secrets, private keys, personal data, production screenshots, internal asset lists or confidential engineering evidence. Keep engagement-specific material in a protected engagement repository.

## GitHub
```bash
git init
git add .
git commit -m "Initial manufacturing VAPT knowledge base"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/Manufacturing-VAPT-Knowledge-Base.git
git push -u origin main
```

## RAG-ready design
```text
Markdown/YAML -> Parser/Chunker -> Embeddings -> Vector DB -> RAG/Agent
```

## Quality rules
- Never infer a vulnerability from a version alone.
- Separate facts, observations and analyst conclusions.
- Do not assume every manufacturer has the same architecture.
- Treat IT and OT differently.
- Version external standards.
- Keep client-specific findings outside this repository.
- Require OT safety gates before potentially disruptive actions.


## Completeness principle

This repository is designed for **category completeness**, not a false promise of universal product-by-product completeness. Manufacturing environments vary by process, plant, vendor, geography, regulation and maturity. Unknown, not-applicable, out-of-scope and not-tested states are therefore first-class assessment outcomes.

The final coverage audit is in `00-Foundation/MFG-FINAL-COVERAGE-AUDIT.md`.


## Auditor Checklists
The `15-Auditor-Checklists/` layer converts the master asset/phase matrix into engagement, phase and asset-level assessment trackers. It includes a 406-asset machine-readable checklist and QA report.

## Findings & Evidence Layer

Version 1.3.0 adds `16-Findings-Evidence/`, connecting auditor checklist coverage to observations, evidence, findings, remediation and retesting. Machine-readable record schemas are maintained under `schemas/`.


## Threat, Attack-Path & MITRE ICS Layer
The `17-Threat-Attack-Paths/` layer connects the full 406-asset manufacturing scope to 40 reusable attack paths, MITRE ATT&CK for ICS tactics/techniques, safety guardrails, evidence and impact analysis. It is additive to—not a replacement for—the master asset/phase matrix.


## RAG / AI Retrieval Layer
The `18-RAG-AI-Retrieval/` layer provides a machine-readable document catalog, 474-logical-unit knowledge index, 406-asset index, cross-layer relationship graph, chunking rules, retrieval policy, query routing and evaluation dataset. It preserves the full manufacturing scope and does not commit model-specific embeddings.


## Final QA
The v1.8.0 release includes the final coverage and release audit at `00-Foundation/MFG-FINAL-QA-RELEASE-AUDIT-v1.8.0.md`. The audit preserves the full 23-family / 406-asset scope and treats future work as versioned enhancements.


## v2.0 Operational Auditor Package
The repository now includes `19-Operational-Auditor-Package/`, which operationalizes the complete v1.8.0 knowledge base into an engagement workflow, assessment workbook, evidence/finding tracking, OT safety gate, reporting framework and closeout process. The 23-family / 406-asset scope remains authoritative and intact.
