# reflections-2026-08-22 — Dataset Knowledge Pack

> Published by the Intellinexus data pipeline. Agents learn from this dataset via vault
> retrieval — search for its subject and the records below surface as context.

## Provenance & audit
- **Dataset id**: `reflections-2026-08-22-mt522aho`
- **Source**: Intellinexus daily reflection
- **Sector**: operations
- **Published**: 2026-08-23T00:14:54.876Z
- **Batch root hash** (tamper-evident): `5229a599b5b1fb97f19f1dcd8c50b4f8f63647daf519da18da71689c222d0ec2`
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
| Cryptographic Hashing | 1 | 1 | SHA-256 per record; batch root 5229a599b5b1… |
| Confidence Scoring | 1 | 1 | completeness over 8 fields |
| HITL Validation | 1 | 1 | 0 flagged below 0.6 confidence |
| Entity Resolution | 1 | 1 | merged on "template" |

## Machine-ready outputs
- **ML CSV** — `_datasets/reflections-2026-08-22-mt522aho/dataset.csv`
- **Knowledge-graph JSONL** — `_datasets/reflections-2026-08-22-mt522aho/graph.jsonl`
- **RAG chunks** — `_datasets/reflections-2026-08-22-mt522aho/rag.md`

## How agents use this
The RAG chunks and this card are indexed in the vault. Any agent answering a
question in this domain retrieves the golden records as grounding. Sample fields:
`date`, `template`, `total`, `succeeded`, `failed`, `success_rate`, `avg_duration_sec`, `top_failure`.
