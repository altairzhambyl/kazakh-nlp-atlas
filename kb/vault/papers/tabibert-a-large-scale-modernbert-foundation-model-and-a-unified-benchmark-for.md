---
kb_id: "arxiv:2512.23065"
type: "paper"
title: "TabiBERT: A Large-Scale ModernBERT Foundation Model and A Unified Benchmark for Turkish"
arxiv_id: "2512.23065"
doi: null
hf_repo: null
year: 2025
topics: ["turkic-embeddings-retrieval-non-kazakh-t", "non-kazakh-turkic-nlp-landscape-embeddin"]
claims: 2
uncertain_claims: 1
verdicts: []
aliases: ["TabiBERT: A Large-Scale ModernBERT Foundation Model and A Unified Benchmark for Turkish", "arXiv:2512.23065", "arxiv:2512.23065"]
tags: ["paper", "topic/turkic-embeddings-retrieval-non-kazakh-t", "topic/non-kazakh-turkic-nlp-landscape-embeddin"]
---
# TabiBERT: A Large-Scale ModernBERT Foundation Model and A Unified Benchmark for Turkish

[arXiv](https://arxiv.org/abs/2512.23065)
**Topics:** [[turkic-embeddings-retrieval-non-kazakh-t]], [[non-kazakh-turkic-nlp-landscape-embeddin]]

> [!abstract]
> Since the inception of BERT, encoder-only Transformers have evolved significantly in computational efficiency, training stability, and long-context modeling. ModernBERT consolidates these advances by integrating Rotary Positional Embeddings (RoPE), FlashAttention, and refined normalization. Despite these developments, Turkish NLP lacks a monolingual encoder trained from scratch, incorporating such …

## Claims

> [!warning] UNCERTAIN — turkic-embeddings-retrieval-non-kazakh-t
> [tr] TabiBERT (arXiv:2512.23065) is a ModernBERT-architecture Turkish foundation model reported to reach TR-MTEB retrieval NDCG@10 = 75.44, surpassing BERTurk's 74.84; a related ModernBERT-base checkpoint post-trained with a 'BGE-M3 guide' scores 55.67 MTEB/46.36 Legal-domain score, and newmindai/Mursit-Large-TR-Retrieval scores 56.87 MTEB/46.56 Legal.
>
> **Numbers:** TabiBERT NDCG@10 75.44 vs BERTurk 74.84; ModernBERT+BGE-M3-guide 55.67 MTEB/46.36 Legal; Mursit-Large-TR-Retrieval 56.87 MTEB/46.56 Legal
> **Relevance:** Suggests a NEWER (Dec 2025) modern-encoder-architecture Turkish retrieval model may be closing the gap with mE5/BGE-M3 specifically on retrieval, in contrast to TR-MTEB's 2025 finding that mE5-large still leads overall — worth a follow-up primary-source read before citing, since the source numbers here were not independently verified against the paper's own tables.
> **Source:** search-result snippets referencing arxiv.org/pdf/2512.23065 (PDF parsing failed; numbers not independently confirmed from the primary text) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — non-kazakh-turkic-nlp-landscape-embeddin
> [tr] TabiBERT's headline '75.44 NDCG@10, surpassing BERTurk's 74.84' retrieval claim (arXiv:2512.23065) is NOT a counter-example to mE5-large's dominance — it never compares against mE5-large, text-embedding-3-small, BGE-M3, or any dedicated text-embedding model at all. Its retrieval evaluation ('TabiBench', Appendix A.1.6/Table 11) is restricted to 5 BERT-family encoder foundation models: TurkishBERTweet (163M, IR 68.40 weighted-avg... actually per-dataset weighted avg 68.40 total metric not IR-only, see numbers field), YTU-Cosmos-BERT (111M, 74.29), BERTurk (110M, 74.84), TabiBERT (149M, 75.44), mmBERT (307M, higher, exact IR number for mmBERT not fully captured but total-avg 79.26). Dataset set: BiText/MsMarco-TR/Scifact-TR/Fiqa-TR/NFCorpus-TR/Quora-TR (translated BEIR subset via TR-MTEB group).
>
> **Numbers:** IR NDCG@10 weighted avg: TurkishBERTweet 68.40, YTU-Cosmos-BERT 74.29, BERTurk 74.84, TabiBERT 75.44, mmBERT not isolated in extract (total avg 79.26). No mE5/OpenAI/BGE baseline present anywhere in the 33-page paper (grep confirmed zero mentions of 'e5' or 'E5').
> **Relevance:** This resolves the KB's standing flag ('TabiBERT failed PDF verification in every sweep') definitively: TabiBERT is genuinely NOT a valid counter-example to mE5-large's retrieval dominance — it is an encoder-vs-encoder comparison at a different weight class (110-307M BERT-style) that simply never tested against the SOTA embedding models the lab is targeting. Any future lab citation of TabiBERT as 'beating mE5' would be a factual error and should be actively suppressed.
> **Source:** arxiv.org/pdf/2512.23065 (TabiBERT: A Large-Scale ModernBERT Foundation Model and Unified Benchmarking Framework for Turkish), directly downloaded and pdftotext-parsed, Table 11 + prose (lines ~2317-2440 of extracted text) · **Sweep:** `turkic-landscape`

[[Home]]
