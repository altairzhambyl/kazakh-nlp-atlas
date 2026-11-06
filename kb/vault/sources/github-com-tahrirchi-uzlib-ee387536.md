---
kb_id: "hf:murodbek/mmlu-uz"
type: "source"
title: "github.com/tahrirchi/uzlib"
doi: null
hf_repo: "murodbek/MMLU-uz"
year: null
topics: ["turkic-non-kazakh-nlp-landscape-targeted"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["hf:murodbek/mmlu-uz"]
tags: ["source", "topic/turkic-non-kazakh-nlp-landscape-targeted"]
---
# github.com/tahrirchi/uzlib

**Topics:** [[turkic-non-kazakh-nlp-landscape-targeted]]

## Source URLs
- github.com/tahrirchi/uzlib
- huggingface.co/datasets/murodbek/MMLU-uz

## Findings

> [!note] CLAIM — turkic-non-kazakh-nlp-landscape-targeted
> [uz] Existing Uzbek 'QA-like' resources are multiple-choice knowledge/linguistics quizzes or machine-translated multitask benchmarks, NOT open-domain QA with passage retrieval: (a) UzLiB (tahrirchi/uzlib, GitHub) sources MC questions from Telegram quiz channels on Uzbek linguistics, converts to Latin script, shuffles answer choices — no passages, no retrieval component; (b) MMLU-uz (HF: murodbek/MMLU-uz) is a machine translation of Global-MMLU-Lite done via the 'sayqalchi' model (Tilmoch platform) plus an LLM polishing pass, explicitly 'not undergone human review' — again MC knowledge, not retrieval/ODQA.
>
> **Numbers:** MMLU-uz: machine-translated, 2-stage pipeline, no human QC; UzLiB: Telegram-sourced MC quiz format
> **Relevance:** Rules out these as disguised UzQAD equivalents — neither has a Wikipedia-passage corpus or relevance judgments, so they cannot substitute for the KazQAD-style retrieval protocol the lab's evallab needs to port to Uzbek.
> **Source:** github.com/tahrirchi/uzlib; huggingface.co/datasets/murodbek/MMLU-uz · **Sweep:** `turkic-landscape`

[[Home]]
