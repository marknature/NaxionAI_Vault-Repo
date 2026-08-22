# reflections-2026-08-21 — Dataset Knowledge Pack

> Published by the Intellinexus data pipeline. Agents learn from this dataset via vault
> retrieval — search for its subject and the records below surface as context.

## Provenance & audit
- **Dataset id**: `reflections-2026-08-21-mt3v01of`
- **Source**: Intellinexus daily reflection
- **Sector**: operations
- **Published**: 2026-08-22T04:09:26.655Z
- **Batch root hash** (tamper-evident): `ba2a9c05cfbb037e12e26ebd113733f2d07ef8743a1e411bda92f4ca522aa325`
- **Records**: 1 golden (1 raw in) · **avg confidence**: 87.5%
- **HITL review queue**: 0 records flagged below confidence threshold

## Fields
- `date`
- `template`
- `total`
- `succeeded`
- `failed`
- `success_rate`
- `avg_duration_sec`
- `top_failure`

## Pipeline stages
| Stage | In | Out | Note |
|---|---|---|---|
| Normalization | 1 | 1 | canonical keys, trimmed + type-coerced values |
| Cryptographic Hashing | 1 | 1 | SHA-256 per record; batch root ba2a9c05cfbb… |
| Confidence Scoring | 1 | 1 | completeness over 8 fields |
| HITL Validation | 1 | 1 | 0 flagged below 0.6 confidence |
| Entity Resolution | 1 | 1 | merged on "template" |

## Machine-ready outputs
- **ML CSV** — `_datasets/reflections-2026-08-21-mt3v01of/dataset.csv`
- **Knowledge-graph JSONL** — `_datasets/reflections-2026-08-21-mt3v01of/graph.jsonl`
- **RAG chunks** — `_datasets/reflections-2026-08-21-mt3v01of/rag.md`

## How agents use this
The RAG chunks and this card are indexed in the vault. Any agent answering a
question in this domain retrieves the golden records as grounding. Sample fields:
`date`, `template`, `total`, `succeeded`, `failed`, `success_rate`, `avg_duration_sec`, `top_failure`.
