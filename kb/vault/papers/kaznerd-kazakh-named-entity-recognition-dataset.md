---
kb_id: "arxiv:2111.13419"
type: "paper"
title: "KazNERD: Kazakh Named Entity Recognition Dataset"
arxiv_id: "2111.13419"
doi: null
hf_repo: null
year: 2021
topics: ["non-kazakh-turkic-nlp-landscape-reconcil"]
claims: 1
uncertain_claims: 1
verdicts: []
aliases: ["KazNERD: Kazakh Named Entity Recognition Dataset", "arXiv:2111.13419", "arxiv:2111.13419"]
tags: ["paper", "topic/non-kazakh-turkic-nlp-landscape-reconcil"]
---
# KazNERD: Kazakh Named Entity Recognition Dataset

[arXiv](https://arxiv.org/abs/2111.13419)
**Topics:** [[non-kazakh-turkic-nlp-landscape-reconcil]]

> [!abstract]
> We present the development of a dataset for Kazakh named entity recognition. The dataset was built as there is a clear need for publicly available annotated corpora in Kazakh, as well as annotation guidelines containing straightforward--but rigorous--rules and examples. The dataset annotation, based on the IOB2 scheme, was carried out on television news text by two native Kazakh speakers under the …

## Claims

> [!warning] UNCERTAIN — non-kazakh-turkic-nlp-landscape-reconcil
> [kk][az] Kazakh DOES lead on a different, distinct axis: breadth of the dedicated NLP research/benchmark ECOSYSTEM (count and diversity of native, purpose-built datasets and models), not raw volume or shared-benchmark accuracy. Kazakh has at least 8 dedicated artifacts with papers: KazNERD (112,000+ sentences, 25 entity classes), KazQAD (~6,000 questions, ~12,000 passage-relevance judgments), KazParC (371,902 parallel kk-en-ru-tr sentences), KazMMLU (23,000 MCQs), KazSAnDRA (sentiment), plus THREE dedicated decoder LLMs: Sherkala-8B/Sherkala-Chat (adapted Llama-3.1), SozKZ (587M from-scratch), KazByte (byte-adapter Qwen). The comparable Azerbaijani effort found (aLLMA family, arXiv:2407.02337) is ENCODER-ONLY (aLLMA-Small 45.9M / Base 135.2M / Large 369.5M params, still training at publication) trained on the DOLLMA corpus (651.1M words) with benchmarks AZE-SCI (5.76k), AZE-NSP (9.15k), CB-MCQ (released but 'all tested models failed to learn this... even at a basic level' per the authors), WikiANN-az NER (12k), plus MOSTLY TRANSLATED tasks (SQuAD-az 54.1k, MRPC-az 3.67k) rather than natively authored ones — no dedicated Azerbaijani DECODER/generative LLM was found in this search.
>
> **Numbers:** kk: KazNERD 112K sent/25 classes; KazQAD 6K Q/12K judgments; KazParC 371,902 pairs; KazMMLU 23K Q; 3 decoder LLMs (8B, 587M, adapter). az: DOLLMA 651.1M words; aLLMA 45.9M/135.2M/369.5M (encoder-only); AZE-SCI 5.76K; AZE-NSP 9.15K; SQuAD-az 54.1K (translated); 0 dedicated decoder LLMs found.
> **Relevance:** This is Kazakh's genuinely defensible leadership claim for the atlas — narrowly scoped to 'dedicated benchmark/model ecosystem breadth,' not to raw data volume or shared-benchmark accuracy, where Azerbaijani leads. This scoping is what makes the atlas claim falsification-proof.
> **Source:** KazNERD/KazQAD/KazParC/KazMMLU per KB (arXiv:2111.13419, 2404.04487, 2403.19399, 2502.12829); Sherkala arXiv:2503.01493; SozKZ arXiv:2603.20854 (KB); KazByte arXiv:2603.27859 (KB, title only); Azerbaijani: 'Open foundation models for Azerbaijani language' arXiv:2407.02337, fetched directly. · **Sweep:** `turkic-landscape`

**Cited KB notes:** [[open-foundation-models-for-azerbaijani-language]], [[sherkala-chat-building-a-state-of-the-art-llm-for-kazakh-in-a-moderately]], [[sozkz-training-efficient-small-language-models-for-kazakh-from-scratch]], [[kazbyte-adapting-qwen-models-to-kazakh-via-byte-level-adapter]]

[[Home]]
