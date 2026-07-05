---
kb_id: "title:and"
type: "source"
title: "and"
doi: null
hf_repo: null
year: null
topics: ["mteb-upstream-contrib-process"]
claims: 2
uncertain_claims: 0
verdicts: []
aliases: ["title:and"]
tags: ["source", "topic/mteb-upstream-contrib-process"]
---
# and

**Topics:** [[mteb-upstream-contrib-process]]

## Source URLs
- and

## Findings

> [!note] CLAIM — mteb-upstream-contrib-process
> CI runs a dedicated dataset-loading workflow keyed off changes to mteb/tasks/**.py, executed via `make dataset-load-test-pr` (or `make dataset-load-test` on push to main), which resolves to a pytest run restricted to the `test_datasets` marker; the base `make test` used for general PR CI explicitly EXCLUDES that marker.
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/.github/workflows/dataset_loading.yml and https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/Makefile · **Sweep:** `2026-07-mteb-upstream-recon`

> [!note] CLAIM — mteb-upstream-contrib-process
> Required local dev commands before a PR: `make install` (uv sync --extra image --group dev), `make lint` (ruff format/check, typos), `make typecheck` (mypy mteb), `make test` (pytest -n auto excluding test_datasets/leaderboard_stability/test_reference_models); combined shortcut is `make pr` = lint + test.
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/Makefile and https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/docs/CONTRIBUTING.md · **Sweep:** `2026-07-mteb-upstream-recon`

[[Home]]
