---
kb_id: "title:git diff 6b21b5a origin main stat"
type: "source"
title: "`git diff 6b21b5a origin/main --stat`"
doi: null
hf_repo: null
year: null
topics: ["mteb-upstream-task-api"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:git diff 6b21b5a origin main stat"]
tags: ["source", "topic/mteb-upstream-task-api"]
---
# `git diff 6b21b5a origin/main --stat`

**Topics:** [[mteb-upstream-task-api]]

## Source URLs
- `git diff 6b21b5a origin/main --stat`

## Findings

> [!note] CLAIM — mteb-upstream-task-api
> GitHub main branch tip (2026-07-03T19:17:01Z, commit 9d21470a, 'fix por benchmark (#4844)') is exactly ONE commit ahead of the 2.16.3 tag, and that commit only touches Dockerfile, README.md, a leaderboard workflow file, benchmarks.py, and a new model file (sionic_models.py) — it does NOT touch abstasks/, task_metadata.py, retrieval.py, or any task files. So for task-API purposes, mteb 2.16.3 == current main (no API drift to account for).
> **Source:** https://api.github.com/repos/embeddings-benchmark/mteb/commits/main ; `git diff 6b21b5a origin/main --stat` · **Sweep:** `2026-07-mteb-upstream-recon`

[[Home]]
