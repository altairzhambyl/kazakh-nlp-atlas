---
kb_id: "arxiv:2605.04948"
type: "paper"
title: "Adapting Large Language Models to a Low-Resource Agglutinative Language: A Comparative Study of LoRA and QLoRA for Bashkir"
arxiv_id: "2605.04948"
doi: null
hf_repo: null
year: 2026
topics: ["turkic-other-langs-non-kazakh-turkic-nlp", "turkic-pan-benchmarks-non-kazakh-turkic"]
claims: 2
uncertain_claims: 0
verdicts: []
aliases: ["Adapting Large Language Models to a Low-Resource Agglutinative Language: A Comparative Study of LoRA and QLoRA for Bashkir", "arXiv:2605.04948", "arxiv:2605.04948"]
tags: ["paper", "topic/turkic-other-langs-non-kazakh-turkic-nlp", "topic/turkic-pan-benchmarks-non-kazakh-turkic"]
---
# Adapting Large Language Models to a Low-Resource Agglutinative Language: A Comparative Study of LoRA and QLoRA for Bashkir

[arXiv](https://arxiv.org/abs/2605.04948)
**Topics:** [[turkic-other-langs-non-kazakh-turkic-nlp]], [[turkic-pan-benchmarks-non-kazakh-turkic]]

> [!abstract]
> This paper presents a comparative study of parameter-efficient fine-tuning (PEFT) methods, including LoRA and QLoRA, applied to the task of adapting large language models to the Bashkir language, a low-resource agglutinative language of the Turkic family. Experimental evaluation is conducted on a Bashkir text corpus of 71k documents (46.9M tokens) using models of various architectures: DistilGPT2, …

## Claims

> [!note] CLAIM — turkic-other-langs-non-kazakh-turkic-nlp
> [ba] The only controlled from-scratch-vs-adaptation study for Bashkir (arXiv:2605.04948, LoRA/QLoRA comparison) used a small corpus (71,567 docs / 46.9M tokens, only 10,000 docs actually used for experiments) and found QLoRA rank sensitivity is severe: DeepSeek-7B QLoRA at r=8 catastrophically fails (PPL 129.55) while r=16 on the same model recovers to PPL 8.98 — a >14x perplexity swing from one LoRA-rank hyperparameter change. Best overall: GPT-2-medium full fine-tune PPL 3.34; best PEFT: Mistral-7B QLoRA r=16 PPL 3.79 and Phi-2 QLoRA r=8 PPL 3.81, 'with over 40x fewer trainable parameters' than full FT.
>
> **Numbers:** Corpus: 71,567 docs, 46.9M tokens (10,000 docs used); GPT-2-medium full FT PPL 3.34±0.01; Mistral-7B QLoRA r16 PPL 3.79±0.02; Phi-2 QLoRA r8 PPL 3.81±0.03; DeepSeek-7B QLoRA r8 PPL 129.55±1.06 vs r16 PPL 8.98±0.10
> **Relevance:** Directly transferable warning for the lab's own QLoRA-CPT-on-Qwen3-0.6B plan: LoRA rank choice can produce catastrophic (not just suboptimal) failure on a low-resource agglutinative Turkic language at 7B+ scale — the lab's design-panel should treat rank as a swept hyperparameter, not a fixed default, before committing paid compute.
> **Source:** arXiv:2605.04948v1, fetched directly · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-pan-benchmarks-non-kazakh-turkic
> A Turkic multilingual ASR study found Bashkir [ba] has consistently HIGHER word-error-rates than Kazakh, Tatar, or Kyrgyz despite Bashkir's larger raw MT parallel-corpus (see finding above) — a small-scale from-scratch Bashkir LM comparison (71,567 docs / ~46.9M tokens assembled from 16 sources, subsampled to 10,000 docs) further shows QLoRA rank-16 on Mistral-7B reaches 3.79 perplexity vs full-fine-tune GPT-2-medium's 3.34, i.e. '40x fewer trainable params for comparable quality.'
>
> **Numbers:** Bashkir corpus: 71,567 docs / ~46.9M tokens; QLoRA(r16)/Mistral-7B PPL 3.79 vs full-FT GPT-2-medium PPL 3.34; ~40x fewer trainable params
> **Relevance:** Bashkir's ~46.9M-token assembled corpus is roughly 200x smaller than the lab's own ~9-10B-token Kazakh corpus (SozKZ scale) — quantifies just how far behind Bashkir sits versus Kazakh even among fellow Kipchak languages, useful concrete data point for the atlas's resource-ratio table.
> **Source:** arXiv:2605.04948 (Adapting LLMs to Bashkir: LoRA vs QLoRA) · **Sweep:** `turkic-landscape`

[[Home]]
