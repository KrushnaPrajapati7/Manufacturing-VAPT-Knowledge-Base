# MFG RAG Chunking & Ingestion Specification

## Purpose
Convert the complete Manufacturing VAPT Knowledge Base into retrievable units without losing manufacturing safety, scope, standards, evidence, or cross-layer relationships.

## Non-negotiable scope
- Preserve all 23 asset families and all 406 master asset/technology rows.
- Preserve all 474 logical knowledge units. Duplicate source copies of the same knowledge ID are retained in the document catalog and represented once in the logical knowledge index.
- Preserve all eight VAPT phases.
- Preserve standards, tool/test, finding/evidence, auditor checklist and threat/attack-path layers.
- Never ingest client-specific credentials, secrets, production evidence, internal IP inventories or confidential engineering material.

## Chunk hierarchy
1. Document-level metadata chunk.
2. Question/Description/Overview chunk.
3. Assessment Objectives + Manufacturing Context chunk.
4. Scope & Preconditions chunk.
5. Assessment methodology chunks, split by meaningful heading.
6. Evidence + Expected Output chunk.
7. Safety / Stop Conditions chunk — never detached from the parent assessment.
8. Common Pitfalls + Related Knowledge chunk.
9. Standards / References chunk.

## Chunk rules
- Prefer semantic heading boundaries over fixed token cuts.
- If a section exceeds the implementation's context limit, split only at paragraph/list boundaries and repeat critical metadata.
- Every chunk must carry knowledgeId, phase, asset family/asset tags, safety, source path and source hash.
- Safety/stop-condition text must be attached to every chunk describing an active test or OT validation.
- Do not merge unrelated assets merely to increase chunk size.
- Do not create a chunk that contains only a tool name without its assessment objective.

## Retrieval units
Use the logical knowledge index for authoritative knowledge-unit identity; use the document catalog when exact source files are required.

## Embeddings
The repository intentionally does not commit model-specific embeddings. Generate embeddings in the deployment environment using the organization's approved model and record model/version, dimensions, distance metric and indexing date in the deployment manifest.
