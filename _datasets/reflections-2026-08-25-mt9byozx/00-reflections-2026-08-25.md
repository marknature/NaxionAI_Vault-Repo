# reflections-2026-08-25 — Dataset Knowledge Pack

> Published by the Intellinexus data pipeline. Agents learn from this dataset via vault
> retrieval — search for its subject and the records below surface as context.

## Provenance & audit
- **Dataset id**: `reflections-2026-08-25-mt9byozx`
- **Source**: Intellinexus daily reflection
- **Sector**: operations
- **Published**: 2026-08-26T00:03:07.917Z
- **Batch root hash** (tamper-evident): `338e615f62700608eed50b392bb669f3e541ebf1a32600b8eebc41e499b2debf`
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
| Cryptographic Hashing | 1 | 1 | SHA-256 per record; batch root 338e615f6270… |
| Confidence Scoring | 1 | 1 | completeness over 8 fields |
| HITL Validation | 1 | 1 | 0 flagged below 0.6 confidence |
| Entity Resolution | 1 | 1 | merged on "template" |

## Machine-ready outputs
- **ML CSV** — `_datasets/reflections-2026-08-25-mt9byozx/dataset.csv`
- **Knowledge-graph JSONL** — `_datasets/reflections-2026-08-25-mt9byozx/graph.jsonl`
- **RAG chunks** — `_datasets/reflections-2026-08-25-mt9byozx/rag.md`

## How agents use this
The RAG chunks and this card are indexed in the vault. Any agent answering a
question in this domain retrieves the golden records as grounding. Sample fields:
`date`, `template`, `total`, `succeeded`, `failed`, `success_rate`, `avg_duration_sec`, `top_failure`.
