---
kb_id: "arxiv:2501.10107"
type: "paper"
title: "BBPOS: BERT-based Part-of-Speech Tagging for Uzbek"
arxiv_id: "2501.10107"
doi: null
hf_repo: null
year: 2025
topics: ["turkic-nlp-landscape-uzbek-monolingual-p"]
claims: 1
uncertain_claims: 1
verdicts: []
aliases: ["BBPOS: BERT-based Part-of-Speech Tagging for Uzbek", "arXiv:2501.10107", "arxiv:2501.10107"]
tags: ["paper", "topic/turkic-nlp-landscape-uzbek-monolingual-p"]
---
# BBPOS: BERT-based Part-of-Speech Tagging for Uzbek

[arXiv](https://arxiv.org/abs/2501.10107)
**Topics:** [[turkic-nlp-landscape-uzbek-monolingual-p]]

> [!abstract]
> This paper advances NLP research for the low-resource Uzbek language by evaluating two previously untested monolingual Uzbek BERT models on the part-of-speech (POS) tagging task and introducing the first publicly available UPOS-tagged benchmark dataset for Uzbek. Our fine-tuned models achieve 91% average accuracy, outperforming the baseline multi-lingual BERT as well as the rule-based tagger. Nota …

## Claims

> [!warning] UNCERTAIN — turkic-nlp-landscape-uzbek-monolingual-p
> [uz] The '~5B tokens' TahrirchiBERT figure is NOT a comparable web-crawl-only number: it draws on tahrirchi/uz-crawl (1,618,035 docs = 1,250,018 news + 368,017 Telegram-blog docs, 5.1GB total disk, sourced from 57 news sites + 128 curated Telegram channels — proprietary scraping, not CommonCrawl) plus a Latin-normalized subset of tahrirchi/uz-books (~40,000 OCR'd books, 16.98GB downloaded / 32.95GB generated across Cyrillic-OCR and Latin versions, with acknowledged noisy Tesseract OCR quality).
>
> **Numbers:** uz-crawl: 1,618,035 docs (1,250,018 news + 368,017 Telegram), 5.1GB. uz-books: ~40,000 books, 16.98GB downloaded / 32.95GB generated. Combined training subset cited as ~5B tokens / ~18.5GB.
> **Relevance:** The 5B-token number should NOT be used as 'Uzbek's true monolingual pretraining corpus size' for a web-crawl-style port (KazQAD-style retrieval / Less-is-More recipe assumes CC-style web text); it mixes non-CC proprietary Telegram scraping and noisy OCR'd book text with distinct quality/legal-provenance profiles, and is not license-clear for redistribution the way FineWeb2 (ODC-By) is.
> **Source:** Mamasaidov & Shopulatov 2023 (Tahrirchi), corpus described via HF dataset cards tahrirchi/uz-crawl and tahrirchi/uz-books, and characterized (incl. '5B tokens ≈18.5GB', OCR noise caveat) in Israilova et al. 2025 'BBPOS: BERT-based Part-of-Speech Tagging for Uzbek', arXiv:2501.10107 · **Sweep:** `turkic-landscape`

[[Home]]
