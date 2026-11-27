# Experiment Log Guide

## Purpose
Record every model execution, including successful runs and failures.

## Rules

1. Create one CSV row for every execution attempt.
2. Use ISO 8601 timestamps with timezone when available. If the exact time was not recorded, use the ISO 8601 date only (YYYY-MM-DD).
3. Use the exact model ID configured in the environment.
4. Use only these conditions:
   - closed_book
   - rag
5. Keep the same temperature and max_tokens across comparable runs.
6. Record the run number: 1, 2, or 3.
7. Use these status values:
   - success
   - rate_limited
   - failed
8. Record token usage, cost, and latency when available.
9. Leave unavailable measurements empty; never invent values.
10. Record a short error description when a run fails.
11. Never record API keys, passwords, or other secrets.

## Run ID convention

Examples:
- NEM-CB-01: Nemotron, closed-book, run 1
- NEM-RAG-01: Nemotron, RAG, run 1
- ERN-CB-01: ERNIE, closed-book, run 1
- ERN-RAG-01: ERNIE, RAG, run 1

## Reproducibility

Keep the original model response JSON for each successful run.
Do not overwrite previous results.

## Experiment phase

Use the phase field to distinguish:
- rehearsal: preliminary workflow tests
- main: official hackathon experiments
- availability_check: model availability tests

Never combine rehearsal results with main experiment results.
For availability checks, leave condition empty.
