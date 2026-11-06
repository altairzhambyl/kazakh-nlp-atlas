---
kb_id: "hf:baai/bge-m3"
type: "source"
title: "huggingface.co/BAAI/bge-m3/discussions/29"
doi: null
hf_repo: "BAAI/bge-m3"
year: null
topics: ["turkic-embeddings-retrieval-non-kazakh-t"]
claims: 1
uncertain_claims: 1
verdicts: []
aliases: ["hf:baai/bge-m3"]
tags: ["source", "topic/turkic-embeddings-retrieval-non-kazakh-t"]
---
# huggingface.co/BAAI/bge-m3/discussions/29

**Topics:** [[turkic-embeddings-retrieval-non-kazakh-t]]

## Source URLs
- huggingface.co/BAAI/bge-m3/discussions/29
- github.com/FlagOpen/FlagEmbedding/issues/1228

## Findings

> [!warning] UNCERTAIN — turkic-embeddings-retrieval-non-kazakh-t
> [az][ba][cv][kk][ky][sah][tk][tr][tt][ug][uz] BGE-M3's pretraining language list (from its CC-100/XLM-R-lineage tokenizer/training data, per HF discussion and FlagEmbedding GitHub issue #1228) nominally covers nearly the entire Turkic family already: az, azb, ba (Bashkir), cv (Chuvash), kk, ky, sah (Sakha/Yakut), tk (Turkmen), tr, tt (Tatar), tyv (Tuvan), ug (Uyghur), uz are all present in the raw list of ~170+ supported language codes — but the model card itself warns 'performance may reduce for low-resource languages' and NO per-Turkic-language MTEB score is published to confirm actual quality for any of these except the Kazakh numbers already in KB (Belebele kaz nDCG@10 0.9017).
>
> **Relevance:** Establishes that BGE-M3 (and by extension mE5, same CC-100 lineage) claims broad Turkic coverage at the pretraining-language-list level, but this is an UNVERIFIED quality claim for every Turkic language except Kazakh — any port decision should budget for an explicit BGE-M3/mE5 baseline measurement per target language (as evallab already does for Kazakh) rather than assume family-wide quality parity.
> **Source:** huggingface.co/BAAI/bge-m3/discussions/29; github.com/FlagOpen/FlagEmbedding/issues/1228 · **Sweep:** `turkic-landscape`

[[Home]]
