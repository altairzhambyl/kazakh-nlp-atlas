---
kb_id: "title:aclanthology org 2025 findings emnlp 471 pdf table 2 read directly"
type: "source"
title: "aclanthology.org/2025.findings-emnlp.471 (PDF, Table 2, read directly)"
doi: null
hf_repo: null
year: null
topics: ["turkic-embeddings-retrieval-non-kazakh-t"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:aclanthology org 2025 findings emnlp 471 pdf table 2 read directly"]
tags: ["source", "topic/turkic-embeddings-retrieval-non-kazakh-t"]
---
# aclanthology.org/2025.findings-emnlp.471 (PDF, Table 2, read directly)

**Topics:** [[turkic-embeddings-retrieval-non-kazakh-t]]

## Source URLs
- aclanthology.org/2025.findings-emnlp.471 (PDF, Table 2, read directly)

## Findings

> [!note] CLAIM — turkic-embeddings-retrieval-non-kazakh-t
> [tr] TR-MTEB (Baysan & Güngör, Boğaziçi Univ., EMNLP 2025 Findings, aclanthology.org/2025.findings-emnlp.471) is the first large-scale Turkish embedding benchmark: 26 datasets across 6 tasks (8 classification, 2 clustering, 3 pair classification, 1 bitext mining, 1 STS, 11 retrieval — 4 are Turkish-translated BEIR sets: SQuAD-TR/MS MARCO-TR/XQuAD/Turkish QA plus 7 newly LLM-translated BEIR sets: NFCorpus-TR, ArguAna-TR, CQADupstack-TR, FiQA-TR, Quora-TR, SCIDOCS-TR, SciFact-TR). Full Table 2 leaderboard confirms mE5 dominance with EXACT numbers: multilingual-e5-large Mean(Task)=66.82/Mean(Type)=73.07 (retrieval 57.21, STS 81.18) is #1; their own best from-scratch-trained Turkish model (BERTurk-init, 34.2M weak pairs, contrastive-pretrain+fine-tune) reaches only 63.42/70.25 (retrieval 52.75), 3.4pt below mE5-large.
>
> **Numbers:** mE5-large 66.82/73.07 (retr 57.21, STS 81.18); mE5-large-instruct 65.92/72.78 (retr 57.51); gte-multilingual-base 64.49/71.96; mE5-base 64.26/70.98 (retr 58.29); text-embedding-3-small 66.61/69.52 (retr 64.99, HIGHEST retrieval of any model); their fine-tuned turkish-embedding-model 63.42/70.25 (retr 52.75); contrastive-only version 59.84/59.49 (bitext catastrophically low 37.7); LaBSE 57.60/66.60; bert-base-turkish-uncased 49.54/47.07 (bitext 7.07 — monolingual encoders fail cross-lingual bitext entirely)
> **Relevance:** Directly extends KB's TurkEmbed finding with the EXACT primary-source leaderboard: a dedicated 34.2M-pair Turkish embedding effort still loses to off-the-shelf mE5-large by 3.4pt Mean(Task) and 4.5pt on retrieval specifically — same lesson as Kazakh's kazembed-v5/SozKZ, now with a second independent Turkic-family confirmation. Also: monolingual encoders score near-zero on bitext mining (7.07 vs mE5 99.43) — validates evallab's choice to measure retrieval/STS, not bitext, as the primary axis for a monolingual Kazakh/Uzbek model.
> **Source:** aclanthology.org/2025.findings-emnlp.471 (PDF, Table 2, read directly) · **Sweep:** `turkic-landscape`

[[Home]]
