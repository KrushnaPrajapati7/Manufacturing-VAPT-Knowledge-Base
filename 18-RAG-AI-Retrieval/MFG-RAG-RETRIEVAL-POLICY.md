# MFG RAG Retrieval & Safety Policy

## Retrieval priority
1. Exact knowledgeId / asset / test / finding identifiers.
2. Asset + VAPT phase.
3. Manufacturing process + asset type.
4. Threat/attack path + MITRE ICS.
5. Standards/control mapping.
6. General semantic similarity.

## Mandatory filters
- sector = manufacturing_industrial for manufacturing methodology queries.
- Apply phase filter when supplied.
- Apply asset family/asset filter when supplied.
- Preserve safety level and stop conditions.
- Prefer authoritative repository records over generated summaries.

## Cross-layer expansion
A high-quality answer should be able to traverse:
Asset → Phase → Knowledge Unit → Tool/Test → Standard → Threat/Attack Path → Evidence/Finding → Retest.
Do not substitute a generic IT answer when a manufacturing-specific record exists.

## Safety gate
If retrieved content concerns OT/ICS, safety systems, physical processes, utilities, robotics or other cyber-physical assets, surface the applicable authorization, ROE, passive/read-only default and stop conditions before describing active validation.

## Unknown-state discipline
The system must be able to return Unknown, Not Applicable, Out of Scope and Not Tested instead of inventing coverage or findings.

## Answer provenance
Responses should cite the knowledgeId/source path used by the application layer. If multiple records disagree, surface the conflict for review rather than silently merging them.
