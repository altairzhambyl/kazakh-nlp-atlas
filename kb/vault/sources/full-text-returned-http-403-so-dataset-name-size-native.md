---
kb_id: "doi:10.1145/3789692.3789784"
type: "source"
title: "full text returned HTTP 403, so dataset name/size/native-language fram…"
doi: "10.1145/3789692.3789784"
hf_repo: null
year: null
topics: ["turkic-non-kazakh-nlp-landscape-targeted"]
claims: 1
uncertain_claims: 1
verdicts: []
aliases: ["doi:10.1145/3789692.3789784"]
tags: ["source", "topic/turkic-non-kazakh-nlp-landscape-targeted"]
---
# full text returned HTTP 403, so dataset name/size/native-language fram…

**Topics:** [[turkic-non-kazakh-nlp-landscape-targeted]]

## Source URLs
- full text returned HTTP 403, so dataset name/size/native-language framing is unconfirmed)

## Findings

> [!warning] UNCERTAIN — turkic-non-kazakh-nlp-landscape-targeted
> [uz] One directly on-topic academic paper exists but is NOT an open-domain/retrieval dataset: 'Development of Uzbek Question-Answering Models through Fine-Tuning Approaches' (Rakhimov, Ochilov, Abdullayeva, Kholmatov, Nasimov; Proc. 9th ICFNDS, ACM DOI 10.1145/3789692.3789784) fine-tunes T5/Flan-T5/mT5/Llama on a 'special domain dataset' of (context, question, answer) triples for RAG-style QA, evaluated with BLEU/ROUGE/METEOR — this is closed-book/reading-comprehension over a domain dataset (e.g. call-center/public-service use case), not an open-domain retrieval benchmark, and the paper does not appear to give the dataset a distinct public name.
>
> **Numbers:** unknown dataset size (paywalled); metrics reported: BLEU, ROUGE, METEOR (exact values not retrieved)
> **Relevance:** Shows Uzbek QA fine-tuning work exists in the literature under Rakhimov et al., but it targets domain-specific RAG, not the KazQAD-style Wikipedia-scale open-domain retrieval protocol the lab needs to port — so it does not preempt the flagship joint deliverable, though it should be cited as related work.
> **Source:** dl.acm.org/doi/10.1145/3789692.3789784 (abstract only — full text returned HTTP 403, so dataset name/size/native-language framing is unconfirmed) · **Sweep:** `turkic-landscape`

[[Home]]
