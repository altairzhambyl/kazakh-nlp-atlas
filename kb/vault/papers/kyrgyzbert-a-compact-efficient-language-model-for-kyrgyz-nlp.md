---
kb_id: "arxiv:2511.20182"
type: "paper"
title: "KyrgyzBERT: A Compact, Efficient Language Model for Kyrgyz NLP"
arxiv_id: "2511.20182"
doi: null
hf_repo: null
year: 2025
topics: ["turkic-kyrgyz-non-kazakh-turkic-nlp-land", "turkic-other-langs-non-kazakh-turkic-nlp", "turkic-pan-models", "non-kazakh-turkic-nlp-landscape-prior-ar"]
claims: 4
uncertain_claims: 0
verdicts: []
aliases: ["KyrgyzBERT: A Compact, Efficient Language Model for Kyrgyz NLP", "arXiv:2511.20182", "arxiv:2511.20182"]
tags: ["paper", "topic/turkic-kyrgyz-non-kazakh-turkic-nlp-land", "topic/turkic-other-langs-non-kazakh-turkic-nlp", "topic/turkic-pan-models", "topic/non-kazakh-turkic-nlp-landscape-prior-ar"]
---
# KyrgyzBERT: A Compact, Efficient Language Model for Kyrgyz NLP

[arXiv](https://arxiv.org/abs/2511.20182)
**Topics:** [[turkic-kyrgyz-non-kazakh-turkic-nlp-land]], [[turkic-other-langs-non-kazakh-turkic-nlp]], [[turkic-pan-models]], [[non-kazakh-turkic-nlp-landscape-prior-ar]]

> [!abstract]
> Kyrgyz remains a low-resource language with limited foundational NLP tools. To address this gap, we introduce KyrgyzBERT, the first publicly available monolingual BERT-based language model for Kyrgyz. The model has 35.9M parameters and uses a custom tokenizer designed for the language's morphological structure. To evaluate performance, we create kyrgyz-sst2, a sentiment analysis benchmark built by …

## Claims

> [!note] CLAIM — turkic-kyrgyz-non-kazakh-turkic-nlp-land
> [ky] KyrgyzBERT is the first published monolingual Kyrgyz BERT: 35.9M params, custom WordPiece tokenizer (vocab 30,522), hidden 512, 8 attention heads, 6 layers, trained from scratch on a PRIVATE corpus of >1.5M Kyrgyz sentences on a single RTX 3090. Fine-tuned on kyrgyz-sst2 (SST-2 translated + manually-annotated gold test set of 1,821 sentences) it reaches weighted F1 0.8280 vs fine-tuned mBERT (177M) 0.8401 — only 1.2pp gap at 5x fewer params. Zero-shot base models are near-random: mBERT F1 0.3509, XLM-R F1 0.3221.
>
> **Numbers:** 35.9M params; vocab 30,522; hidden 512; 6L/8H; >1.5M sentences private corpus; kyrgyzbert_sst2 F1 0.8280 vs mbert-kyrgyz-sst2-finetuned F1 0.8401 (177M); zero-shot mBERT F1 0.3509, XLM-R F1 0.3221
> **Relevance:** Directly analogous small-scale case: a 35.9M compact monolingual encoder nearly matches a 5x-larger multilingual model on Kyrgyz sentiment — supports the lab's own bet that a small purpose-built model can be competitive with big multilingual baselines on a Kipchak Turkic language. Also a template for a Kyrgyz-analog benchmark the lab could reuse/extend.
> **Source:** arXiv:2511.20182 (Metinov, Kudakeeva, Kabaeva, KSTU Bishkek, Nov 2025) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-other-langs-non-kazakh-turkic-nlp
> [ky] KyrgyzBERT (arXiv:2511.20182), the first monolingual Kyrgyz BERT, is compact (35.9M params, custom tokenizer) and reaches F1 0.828 on a translated-SST2 sentiment benchmark, 'competitive with a fine-tuned mBERT model five times larger' — but KyrText's own MLM-loss comparison shows kyrgyz-bert has by far the worst XNLI accuracy of any tested model (0.47) and the highest MLM loss (6.4), confirming monolingual-from-scratch-at-this-scale loses cross-lingual reasoning capability even when it wins narrow single-task benchmarks.
>
> **Numbers:** KyrgyzBERT 35.9M params; sentiment F1 0.8280; KyrText's independent eval: kyrgyz-bert BoolQ 0.60, News 0.83, PAWS-X 0.58, SST 0.82, XNLI 0.47 (worst of all 11 models compared), MLM loss 6.4 (worst)
> **Relevance:** Corroborates KB's SozKZ finding at a second Kipchak language: small from-scratch monolingual models can win narrow lexical/sentiment tasks but lose badly on reasoning/entailment tasks vs multilingual-adapted peers — reinforces the lab's own decision to prefer continual-PT-on-multilingual-base over from-scratch for the ≤600M Kazakh model.
> **Source:** arXiv:2511.20182 abstract; corroborated by ACL 2026.loreslm-1.39 Table 6 · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-pan-models
> [ky] KyrgyzBERT (Nov 2025) is the first monolingual Kyrgyz BERT: 35.9M params, custom tokenizer (vocab 30,522), trained on >1.5M Kyrgyz sentences. On a translated+manually-annotated SST2-style sentiment benchmark (kyrgyz-sst2), fine-tuned KyrgyzBERT scores F1 0.8280 vs fine-tuned mBERT (177M, 5x larger) 0.8401 — only a 1.2pp gap. Zero-shot (no Kyrgyz fine-tuning) XLM-R and mBERT collapse to F1 0.3221 / 0.3509.
>
> **Numbers:** 35.9M params, vocab 30,522, >1.5M sentences; F1: KyrgyzBERT 0.8280, mBERT-FT 0.8401, XLM-R zero-shot 0.3221, mBERT zero-shot 0.3509
> **Relevance:** Directly mirrors the lab's SozKZ-vs-Qwen debate for a sister Kipchak language: a tiny (36M) monolingual model nearly matches a 5x-larger multilingual model when BOTH are fine-tuned, but the multilingual model catastrophically fails zero-shot. Supports the case that dedicated small models are worth building IF fine-tuning data exists, but general multilingual models need task adaptation regardless of scale — same lesson QymyzLM should generalize to 'from-scratch small vs adapted general' framing in the atlas.
> **Source:** arXiv:2511.20182 (KyrgyzBERT: A Compact, Efficient Language Model for Kyrgyz NLP) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — non-kazakh-turkic-nlp-landscape-prior-ar
> [ky] KyrgyzBERT (arXiv:2511.20182, Nov 2025) is the first publicly available monolingual Kyrgyz language model: 35.9M params, 6 layers, 8 heads, hidden dim 512, custom morphology-aware tokenizer. Evaluated only on kyrgyz-sst2 (translated SST-2, manually re-annotated test set) sentiment classification, F1=0.828, competitive with a ~5x larger fine-tuned mBERT. No embedding/retrieval benchmark or KD work exists for Kyrgyz.
>
> **Numbers:** 35.9M params; 6L/8H/d512; F1 0.828 vs mBERT (~5x larger)
> **Relevance:** Kyrgyz is at an even earlier stage than Azerbaijani/Uzbek (no embedding model at all, only a small encoder + one classification benchmark) -- confirms Kyrgyz is unclaimed for embedding work, but also signals it may be too resource-poor for the lab's Less-is-More recipe to find good synthetic-pair source data without first securing a parallel corpus.
> **Source:** arXiv:2511.20182 abstract · **Sweep:** `turkic-landscape`

[[Home]]
