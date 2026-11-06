---
kb_id: "title:mteb abstasks task metadata py 462 492 in embeddings benchmark mteb 2 16 3"
type: "source"
title: "mteb/abstasks/task_metadata.py:462-492 in embeddings-benchmark/mteb@2.…"
doi: null
hf_repo: null
year: null
topics: ["mteb-upstream-task-api"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:mteb abstasks task metadata py 462 492 in embeddings benchmark mteb 2 16 3"]
tags: ["source", "topic/mteb-upstream-task-api"]
---
# mteb/abstasks/task_metadata.py:462-492 in embeddings-benchmark/mteb@2.…

**Topics:** [[mteb-upstream-task-api]]

## Source URLs
- mteb/abstasks/task_metadata.py:462-492 in embeddings-benchmark/mteb@2.16.3 (

## Findings

> [!note] CLAIM — mteb-upstream-task-api
> `TaskMetadata` is a Pydantic `BaseModel` with `model_config = ConfigDict(extra="forbid")` (unknown kwargs raise). The genuinely REQUIRED fields (no default value) are: `dataset` (MetadataDatasetDict), `name`, `description`, `type` (TaskType literal), `eval_langs` (Languages), `main_score`. All other fields have defaults: `prompt=None`, `modalities=["text"]`, `category=None`, `reference=None`, `eval_splits=["test"]`, `date=None`, `domains=None`, `task_subtypes=None`, `license=None`, `annotations_creators=None`, `dialect=None`, `sample_creation=None`, `bibtex_citation=None`, `adapted_from=None`, `is_public=True`, `contributed_by=None`, `superseded_by=None`, `is_beta=False`.
> **Source:** mteb/abstasks/task_metadata.py:462-492 in embeddings-benchmark/mteb@2.16.3 (https://github.com/embeddings-benchmark/mteb/blob/2.16.3/mteb/abstasks/task_metadata.py) · **Sweep:** `2026-07-mteb-upstream-recon`

[[Home]]
