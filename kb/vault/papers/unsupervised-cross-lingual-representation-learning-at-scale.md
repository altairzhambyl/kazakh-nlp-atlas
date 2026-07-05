---
kb_id: "arxiv:1911.02116"
type: "paper"
title: "Unsupervised Cross-lingual Representation Learning at Scale"
arxiv_id: "1911.02116"
doi: null
hf_repo: null
year: 2019
topics: ["turkic-embeddings-retrieval-non-kazakh-t", "turkic-nlp-landscape-uzbek-monolingual-p", "non-kazakh-turkic-nlp-landscape-reconcil"]
claims: 4
uncertain_claims: 1
verdicts: []
aliases: ["Unsupervised Cross-lingual Representation Learning at Scale", "arXiv:1911.02116", "arxiv:1911.02116"]
tags: ["paper", "topic/turkic-embeddings-retrieval-non-kazakh-t", "topic/turkic-nlp-landscape-uzbek-monolingual-p", "topic/non-kazakh-turkic-nlp-landscape-reconcil"]
---
# Unsupervised Cross-lingual Representation Learning at Scale

[arXiv](https://arxiv.org/abs/1911.02116)
**Topics:** [[turkic-embeddings-retrieval-non-kazakh-t]], [[turkic-nlp-landscape-uzbek-monolingual-p]], [[non-kazakh-turkic-nlp-landscape-reconcil]]

> [!abstract]
> This paper shows that pretraining multilingual language models at scale leads to significant performance gains for a wide range of cross-lingual transfer tasks. We train a Transformer-based masked language model on one hundred languages, using more than two terabytes of filtered CommonCrawl data. Our model, dubbed XLM-R, significantly outperforms multilingual BERT (mBERT) on a variety of cross-lin …

## Claims

> [!warning] UNCERTAIN — turkic-embeddings-retrieval-non-kazakh-t
> [pan-turkic][kk][az][ky][uz] Raw web-crawl volume (CC-100, used to train XLM-R) ranks Turkic languages DIFFERENTLY than curated-resource surveys: Azerbaijani 783M tokens/6.5GiB > Kazakh 476M tokens/6.4GiB > Kyrgyz 94M tokens/1.2GiB > Uzbek 91M tokens/0.7GiB. This means Azerbaijani, not Kazakh, has the largest raw pretraining-corpus footprint among these four in the exact corpus that trained XLM-R/mE5's tokenizer vocabulary.
>
> **Numbers:** az 783M tok/6.5GiB; kk 476M tok/6.4GiB; ky 94M tok/1.2GiB; uz 91M tok/0.7GiB
> **Relevance:** Creates tension with arXiv:2407.05006's qualitative ranking (Kazakh='Rising Star' > Uzbek='Hopeful' > Kyrgyz/Turkmen='Scraping-Bys') which is based on curated task-dataset counts, not raw pretraining volume. The atlas should explicitly distinguish 'curated/task-dataset resourcing' (Kazakh clearly ahead) from 'raw web-crawl pretraining volume' (Azerbaijani ahead) as two DIFFERENT axes when positioning Kazakh in the family — do not conflate them into a single ranking.
> **Source:** CC-100 corpus statistics (via XLM-R paper arXiv:1911.02116), figures synthesized from search results, not directly read from a table — needs primary-source re-verification · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-nlp-landscape-uzbek-monolingual-p
> [uz][kk] CC-100 (the XLM-R paper's corpus) reports Uzbek at 91M tokens / 0.7 GiB, built from a single 2018 CommonCrawl snapshot via cc-net; the same table gives Kazakh 476M tokens / 6.4 GiB in the same era-matched pipeline — i.e. Uzbek was ~5.2x smaller than Kazakh in this single-snapshot 2019-era source.
>
> **Numbers:** uz: 91M tokens, 0.7 GiB; kk: 476M tokens, 6.4 GiB (ratio kk:uz = 5.2x)
> **Relevance:** Confirms the Kazakh-KB-known 'Kazakh 5.8x smaller than Turkish' framing extends consistently: in this OLDER single-snapshot corpus family Uzbek trails Kazakh by a similar multiplier region (~5x), but this era is now superseded by FineWeb2 below.
> **Source:** Conneau et al. 2019, 'Unsupervised Cross-lingual Representation Learning at Scale' (XLM-R), arXiv:1911.02116, Table 7; corroborated by data.statmt.org/cc-100/ (uz.txt.xz listed as 155M compressed) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — non-kazakh-turkic-nlp-landscape-reconcil
> [az][kk] On the CC-100 web-crawl corpus (2018 Common Crawl snapshot, the XLM-R training data), Azerbaijani has MORE raw tokens than Kazakh: az=783M tokens/6.5 GiB vs kk=476M tokens/6.4 GiB. GiB is nearly tied but tokens diverge 1.64x because Azerbaijani is predominantly Latin-script (post-1991 alphabet, low byte-per-token) while Kazakh is Cyrillic (higher byte premium), so the near-tied GiB figure understates Azerbaijani's real content lead. Also for reference: tr=2,736M tok/20.9 GiB (5.7x Kazakh), uz=91M tok/0.7 GiB (5.2x SMALLER than Kazakh), ky=94M tok/1.2 GiB, ug(Uyghur)=27M tok/0.4 GiB. Tatar, Bashkir, Turkmen, Chuvash, Sakha, Karakalpak have NO CC-100 entry at all (fell below the 100-language crawl threshold).
>
> **Numbers:** az 783M tok/6.5GiB; kk 476M tok/6.4GiB; tr 2736M/20.9GiB; uz 91M/0.7GiB; ky 94M/1.2GiB; ug 27M/0.4GiB
> **Relevance:** Directly answers the raw-web-volume axis with the primary source table (not a secondhand quote); establishes Azerbaijani > Kazakh on CC-100 by 1.64x tokens, contradicting a 'Kazakh ahead on all axes' framing.
> **Source:** Conneau et al. 2020, 'Unsupervised Cross-lingual Representation Learning at Scale' (arXiv:1911.02116), Table 6, Appendix A — verified directly from the PDF appendix table. · **Sweep:** `turkic-landscape`

> [!note] CLAIM — non-kazakh-turkic-nlp-landscape-reconcil
> [kk][az][uz] RECONCILED single-axis verdict: Kazakh is NOT ahead of Azerbaijani when reduced to one axis at a time on data volume or accuracy — Azerbaijani leads Kazakh on CC-100 tokens (1.64x), FineWeb2 2024-snapshot volume (1.65-2.17x), Wikipedia total words (1.93x), and TUMLU-mini native-benchmark accuracy (ahead on all 5 tested models, +1.4 to +4.6pp). Kazakh's only defensible lead is ecosystem breadth (dedicated dataset/model count), which is a research-output metric, not a resource-volume or capability metric. The previously-considered 'Kazakh is the most-resourced non-Turkish Turkic language' claim is FALSE as stated and must be rewritten as: 'Kazakh has the most extensive dedicated NLP research/benchmark ecosystem among non-Turkish Turkic languages, but trails Azerbaijani on both raw text volume (all three corpora checked) and shared native-benchmark accuracy (TUMLU-mini).'
>
> **Numbers:** Volume ratios az:kk = 1.64x (CC-100 tok), 1.65-2.17x (FineWeb2), 1.93x (Wikipedia words); accuracy az>kk on 5/5 TUMLU models by 1.4-4.6pp
> **Relevance:** This is the falsifiable, defensible ranking statement Decision 2 needs — it survives a reviewer holding the CC-100 table AND the FineWeb2/Wikipedia/TUMLU tables, because all four independent sources agree on direction.
> **Source:** Synthesis of the four findings above (arXiv:1911.02116 Table 6; HF fineweb-2 datasets-server; live Wikipedia API; arXiv:2502.11020 Table 2). · **Sweep:** `turkic-landscape`

**Cited KB notes:** [[tumlu-a-unified-and-native-language-understanding-benchmark-for-turkic-languages]]

[[Home]]
