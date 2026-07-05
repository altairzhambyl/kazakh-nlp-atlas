---
kb_id: "title:https raw githubusercontent com embeddings benchmark mteb main docs contributing adding a dataset md"
type: "source"
title: "https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/docs/…"
doi: null
hf_repo: null
year: null
topics: ["mteb-upstream-contrib-process", "mteb-upstream-pr-precedents"]
claims: 12
uncertain_claims: 0
verdicts: []
aliases: ["title:https raw githubusercontent com embeddings benchmark mteb main docs contributing adding a dataset md"]
tags: ["source", "topic/mteb-upstream-contrib-process", "topic/mteb-upstream-pr-precedents"]
---
# https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/docs/…

**Topics:** [[mteb-upstream-contrib-process]], [[mteb-upstream-pr-precedents]]

## Source URLs
- https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/docs/contributing/adding_a_dataset.md

## Findings

> [!note] CLAIM — mteb-upstream-contrib-process
> Adding a task/dataset to mteb requires 4 steps: implement a task subclass, fill out TaskMetadata, calculate descriptive statistics, submit a PR.
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/docs/contributing/adding_a_dataset.md · **Sweep:** `2026-07-mteb-upstream-recon`

> [!note] CLAIM — mteb-upstream-contrib-process
> For retrieval tasks, subclass AbsTaskRetrieval; main_score is ndcg_at_10; example uses mteb.abstasks.retrieval.AbsTaskRetrieval and mteb.abstasks.task_metadata.TaskMetadata.
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/docs/contributing/adding_a_dataset.md · **Sweep:** `2026-07-mteb-upstream-recon`

> [!note] CLAIM — mteb-upstream-contrib-process
> Retrieval task dataset load_data must produce corpus with `id` + text/title (or image/audio), queries with `id` + text, and qrels as dict[query_id][doc_id]=relevance; class example given is MyRetrievalTask(AbsTaskRetrieval) with dataset={'path': 'mteb/CQADupstackAndroidRetrieval', 'revision': ...}.
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/docs/contributing/adding_a_dataset.md · **Sweep:** `2026-07-mteb-upstream-recon`

> [!note] CLAIM — mteb-upstream-contrib-process
> All TaskMetadata fields (description, reference, dataset path+revision, type, category, modalities, eval_splits, eval_langs, main_score, date, domains, task_subtypes, license, annotations_creators, dialect, sample_creation, adapted_from, bibtex_citation) must be filled out for the dataset to be included in mteb; can leave None during dev/PR draft and ask reviewers.
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/docs/contributing/adding_a_dataset.md · **Sweep:** `2026-07-mteb-upstream-recon`

> [!note] CLAIM — mteb-upstream-contrib-process
> File placement: task class goes inside mteb/tasks/ directory and must be imported in that directory's __init__.py.
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/docs/contributing/adding_a_dataset.md · **Sweep:** `2026-07-mteb-upstream-recon`

> [!note] CLAIM — mteb-upstream-contrib-process
> Before opening the PR, must run task.calculate_descriptive_statistics() to detect duplicates/small-sample/short-document issues.
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/docs/contributing/adding_a_dataset.md · **Sweep:** `2026-07-mteb-upstream-recon`

> [!note] CLAIM — mteb-upstream-contrib-process
> Exact PR checklist (verbatim, to paste into PR description).
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/docs/contributing/adding_a_dataset.md · **Sweep:** `2026-07-mteb-upstream-recon`

> [!note] CLAIM — mteb-upstream-contrib-process
> Test commands to verify a new task: python `mteb.evaluate(model, task)` or CLI `mteb run -m mteb/baseline-random encoder -t {name of your task}`.
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/docs/contributing/adding_a_dataset.md · **Sweep:** `2026-07-mteb-upstream-recon`

> [!note] CLAIM — mteb-upstream-contrib-process
> Uploading the dataset to a specific HF org is NOT strictly mandated to open the PR — `dataset.path` can point to any existing HF dataset repo (e.g. third-party org) — but a `push_dataset_to_hub(repo_name)` helper exists and the convention shown in docs uses the `mteb/` org (e.g. `mteb/poem_sentiment`, `mteb/CQADupstackAndroidRetrieval`) after processing, which is recommended so dataset_transform preprocessing doesn't have to be re-run.
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/docs/contributing/adding_a_dataset.md · **Sweep:** `2026-07-mteb-upstream-recon`

> [!note] CLAIM — mteb-upstream-contrib-process
> [UNVERIFIED] Whether the mteb maintainers REQUIRE the final dataset copy to live under the `mteb/` HF org (vs. contributor's own org) before merging a retrieval-task PR — the doc shows `mteb/` as the example prefix but does not state it as a hard requirement, and no separate policy page was found confirming/denying this.
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/docs/contributing/adding_a_dataset.md · **Sweep:** `2026-07-mteb-upstream-recon`

> [!note] CLAIM — mteb-upstream-pr-precedents
> Calculating descriptive statistics via task.calculate_descriptive_statistics() (producing the mteb/descriptive_stats/<Type>/<TaskName>.json file) is stated in mteb's official contributor doc as a required step before submitting a PR, done to catch duplicates, too-small datasets, and too-short documents; every one of the sampled recent PRs (4710, 4487, 4521, 3991, 4226) included this JSON file in its diff, consistent with the doc being enforced in practice, not merely suggested.
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/docs/contributing/adding_a_dataset.md · **Sweep:** `2026-07-mteb-upstream-recon`

> [!note] CLAIM — mteb-upstream-pr-precedents
> mteb's official PR checklist (linked from PR bodies, e.g. #4226) requires: explaining the gap the dataset fills, confirming the dataset loads via the mteb package, running at least mteb/baseline-random-encoder plus one small real model (e.g. intfloat/multilingual-e5-small) and pasting scores into the PR, confirming scores are neither trivial/perfect nor random, reducing dataset size if too large, and reproducing paper scores in the PR description if applicable.
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/docs/contributing/adding_a_dataset.md · **Sweep:** `2026-07-mteb-upstream-recon`

[[Home]]
