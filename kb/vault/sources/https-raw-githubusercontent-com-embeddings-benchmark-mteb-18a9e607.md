---
kb_id: "title:https raw githubusercontent com embeddings benchmark mteb main github workflows dataset loading yml"
type: "source"
title: "https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/.gith…"
doi: null
hf_repo: null
year: null
topics: ["mteb-upstream-pr-precedents"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:https raw githubusercontent com embeddings benchmark mteb main github workflows dataset loading yml"]
tags: ["source", "topic/mteb-upstream-pr-precedents"]
---
# https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/.gith…

**Topics:** [[mteb-upstream-pr-precedents]]

## Source URLs
- https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/.github/workflows/dataset_loading.yml

## Findings

> [!note] CLAIM — mteb-upstream-pr-precedents
> mteb runs a dedicated CI job, 'Datasets available on HuggingFace' (.github/workflows/dataset_loading.yml), on every PR that touches mteb/tasks/**.py; it actually calls load_data() for changed/added tasks using an HF_TOKEN secret that only maintainers control. A dataset gated on HF would only load in this CI if the account behind the mteb org's HF_TOKEN has itself accepted that dataset's gate terms on huggingface.co beforehand — a PR author cannot make their own gate-acceptance count for CI.
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/.github/workflows/dataset_loading.yml · **Sweep:** `2026-07-mteb-upstream-recon`

[[Home]]
