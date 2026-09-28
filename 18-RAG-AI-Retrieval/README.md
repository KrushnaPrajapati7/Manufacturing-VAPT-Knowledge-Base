# RAG / AI Retrieval Layer

This layer makes the complete Manufacturing & Industrial VAPT Knowledge Base machine-retrievable while preserving the original scope and safety model.

## Core indexes
- `MFG-RAG-DOCUMENT-CATALOG.csv` — every Markdown source document.
- `MFG-RAG-KNOWLEDGE-INDEX.csv` — 474 logical knowledge units, with duplicate source paths retained.
- `MFG-RAG-KNOWLEDGE-INDEX.jsonl` — ingestion-friendly logical records.
- `MFG-RAG-ASSET-INDEX.csv` — all 406 master assets.
- `MFG-RAG-RELATIONSHIP-INDEX.csv` — cross-layer graph edges.
- `MFG-RAG-EVALUATION-DATASET.csv` — representative retrieval tests.

## Architecture
`Repository → Parse → Metadata normalize → Semantic chunk → Embed → Vector/Hybrid index → Relationship expansion → RAG answer`

Use hybrid retrieval where possible: exact/keyword filters for identifiers plus semantic/vector retrieval for natural-language questions.

## Important
No embeddings are committed because embedding models are deployment-specific. The repository provides stable IDs, metadata, source hashes and relationships so embeddings can be regenerated deterministically.

## Scope guarantee
This layer is additive. It does not replace the 23-family/406-asset master scope, 474 knowledge units, 8 VAPT phases, standards, tools/tests, findings/evidence or threat/attack-path layers.
