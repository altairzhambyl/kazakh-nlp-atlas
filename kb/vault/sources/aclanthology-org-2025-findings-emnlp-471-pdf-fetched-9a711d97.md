---
kb_id: "title:aclanthology org 2025 findings emnlp 471 pdf fetched primary pdf table 1 read directly"
type: "source"
title: "aclanthology.org/2025.findings-emnlp.471.pdf (fetched primary PDF, Tab…"
doi: null
hf_repo: null
year: null
topics: ["turkic-uzbek-non-kazakh-turkic-nlp-lands"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:aclanthology org 2025 findings emnlp 471 pdf fetched primary pdf table 1 read directly"]
tags: ["source", "topic/turkic-uzbek-non-kazakh-turkic-nlp-lands"]
---
# aclanthology.org/2025.findings-emnlp.471.pdf (fetched primary PDF, Tab…

**Topics:** [[turkic-uzbek-non-kazakh-turkic-nlp-lands]]

## Source URLs
- aclanthology.org/2025.findings-emnlp.471.pdf (fetched primary PDF, Table 1 read directly)

## Findings

> [!note] CLAIM — turkic-uzbek-non-kazakh-turkic-nlp-lands
> [tr] TR-MTEB built a 34.2M-pair weakly-supervised Turkish sentence-pair training corpus (filtered down from 62.5M raw candidate pairs via a fine-tuned multilingual-e5-base filter model at a 0.4 cosine-similarity threshold, sourced from >50 public Turkish/translated/synthetic datasets), then contrastively pretrained + supervised fine-tuned both BERTurk-base and multilingual-e5-base. Results (Table 1, internal small-scale comparison): fine-tuned multilingual-e5-base scored Mean(Task)=62.73 / Mean(TaskType)=67.96, beating its own contrastive-pretrain-only checkpoint (57.77/65.92) and both BERTurk-base variants (uncased 53.62/53.38, cased 53.73/53.43).
>
> **Numbers:** corpus 34.2M pairs (from 62.5M raw, threshold 0.4); Mean(Task)/Mean(TaskType): mE5-base contrastive 57.77/65.92, mE5-base fine-tuned 62.73/67.96, BERTurk-uncased 53.62/53.38, BERTurk-cased 53.73/53.43
> **Relevance:** This IS the lab's planned 'Less-is-More' mE5 continued-fine-tuning recipe, already executed and published for Turkish with exact numbers — a directly reusable methodology template (filter-then-contrastive-pretrain-then-supervised-finetune on mE5-base) for the kk/uz embedding pipeline, and independent validation that continued fine-tuning of mE5-base beats both the untouched mE5-base and from-scratch monolingual BERT encoders for a Turkic language.
> **Source:** aclanthology.org/2025.findings-emnlp.471.pdf (fetched primary PDF, Table 1 read directly) · **Sweep:** `turkic-landscape`

[[Home]]
