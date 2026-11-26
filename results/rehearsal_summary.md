# Rehearsal Summary - Nemotron

Date: 2026-11-26
Model: Nemotron 3 Ultra
Temperature: 0.2
Max tokens: 2000
Cost reported by API: $0

## Results

| Label | RAG | Closed-book |
|---|---:|---:|
| Supported | 4 | 1 |
| Distorted | 1 | 3 |
| Unsupported/Invented | 0 | 1 |
| Unverifiable | 0 | 0 |
| Total | 5 | 5 |

## Preliminary observations

- RAG produced more evidence-supported claims in this small rehearsal.
- RAG still changed the source's uncertainty level in one attribution claim.
- Closed-book generated claims not supported by the reference corpus.
- Closed-book included an unsupported MSS association and an unverified
  Fortinet zero-day claim.
- Human annotation remains necessary to assess factual support and
  preservation of uncertainty.

## Limitations

- Only five claims were generated per condition.
- Only Nemotron was tested.
- Only one run per condition was performed.
- These results are a workflow rehearsal, not the final experiment.
- Unsupported by the corpus does not necessarily mean false in reality.

## Files

- results/rehearsal_nemotron_rag.json
- results/rehearsal_nemotron_closed_book.json
- annotations/rehearsal_nemotron_rag.csv
- annotations/rehearsal_nemotron_closed_book.csv
