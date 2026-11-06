---
kb_id: "title:huggingface coppercitylabs uzbert base uncased rifkat uztext 3gb bpe roberta aclanthology org 2024 sigul 1 5 pdf bertbek sigturk 2026 idiom paper"
type: "source"
title: "HuggingFace coppercitylabs/uzbert-base-uncased"
doi: null
hf_repo: null
year: null
topics: ["non-kazakh-turkic-nlp-landscape-prior-ar"]
claims: 1
uncertain_claims: 1
verdicts: []
aliases: ["title:huggingface coppercitylabs uzbert base uncased rifkat uztext 3gb bpe roberta aclanthology org 2024 sigul 1 5 pdf bertbek sigturk 2026 idiom paper"]
tags: ["source", "topic/non-kazakh-turkic-nlp-landscape-prior-ar"]
---
# HuggingFace coppercitylabs/uzbert-base-uncased

**Topics:** [[non-kazakh-turkic-nlp-landscape-prior-ar]]

## Source URLs
- HuggingFace coppercitylabs/uzbert-base-uncased
- rifkat/uztext-3Gb-BPE-Roberta
- aclanthology.org/2024.sigul-1.5.pdf (BERTbek)
- SIGTURK 2026 idiom paper

## Findings

> [!warning] UNCERTAIN — non-kazakh-turkic-nlp-landscape-prior-ar
> [uz] Uzbek foundation-model work exists (UzBERT ~2021 coppercitylabs, ~2M news articles/3GB; UzRoBERTa rifkat/uztext-3Gb-BPE-Roberta, 300M-word corpus; BERTbek SIGUL 2024) but NO dedicated Uzbek sentence-embedding benchmark analogous to Azerbaijani-STS (LocalDoc, 20k synthetic pairs) or TR-MTEB was found in this search; the SIGTURK-2026 idiom/retrieval paper is the only located Uzbek semantic-retrieval evaluation and it is idiom-scoped, not general-purpose.
>
> **Numbers:** UzBERT ~2M articles/3GB; UzRoBERTa 300M-word corpus; no uz-STS or general uz-MTEB dataset found
> **Relevance:** Supports Decision 1: Uzbek has usable base encoders (an mE5-style KD teacher-student setup could reuse UzBERT/BERTbek tokenizer insights) but lacks a general embedding benchmark -- the lab would need to either build a minimal Uzbek STS/retrieval set (mirroring evallab's KazQAD approach) or wait for one to emerge; this is a real gap, not duplicated effort.
> **Source:** HuggingFace coppercitylabs/uzbert-base-uncased; rifkat/uztext-3Gb-BPE-Roberta; aclanthology.org/2024.sigul-1.5.pdf (BERTbek); SIGTURK 2026 idiom paper · **Sweep:** `turkic-landscape`

[[Home]]
