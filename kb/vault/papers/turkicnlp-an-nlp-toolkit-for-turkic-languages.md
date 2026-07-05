---
kb_id: "arxiv:2602.19174"
type: "paper"
title: "TurkicNLP: An NLP Toolkit for Turkic Languages"
arxiv_id: "2602.19174"
doi: null
hf_repo: null
year: 2026
topics: ["turkic-kyrgyz-non-kazakh-turkic-nlp-land", "turkic-other-langs-non-kazakh-turkic-nlp", "turkic-pan-benchmarks-non-kazakh-turkic", "turkic-pan-models"]
claims: 5
uncertain_claims: 0
verdicts: []
aliases: ["TurkicNLP: An NLP Toolkit for Turkic Languages", "arXiv:2602.19174", "arxiv:2602.19174"]
tags: ["paper", "topic/turkic-kyrgyz-non-kazakh-turkic-nlp-land", "topic/turkic-other-langs-non-kazakh-turkic-nlp", "topic/turkic-pan-benchmarks-non-kazakh-turkic", "topic/turkic-pan-models"]
---
# TurkicNLP: An NLP Toolkit for Turkic Languages

[arXiv](https://arxiv.org/abs/2602.19174)
**Topics:** [[turkic-kyrgyz-non-kazakh-turkic-nlp-land]], [[turkic-other-langs-non-kazakh-turkic-nlp]], [[turkic-pan-benchmarks-non-kazakh-turkic]], [[turkic-pan-models]]

> [!abstract]
> Natural language processing for the Turkic language family, spoken by over 200 million people across Eurasia, remains fragmented, with most languages lacking unified tooling and resources. We present TurkicNLP, an open-source Python library providing a single, consistent NLP pipeline for Turkic languages across four script families: Latin, Cyrillic, Perso-Arabic, and Old Turkic Runic. The library …

## Claims

> [!note] CLAIM — turkic-kyrgyz-non-kazakh-turkic-nlp-land
> [ky][kk][uz][ug][tt][ba][az][tr][sah][alt][tyv][kjh][chv][kaa][nog][krc][crh][gag][tk] TurkicNLP is a 2026 unified toolkit covering 24 Turkic languages (Oghuz/Kipchak/Karluk/Siberian/Oghur/historical branches) offering tokenization, morphology, POS/dependency parsing, NER, transliteration, cross-lingual embeddings, and MT via one API. For Kyrgyz specifically: Apertium FST morphology ('Stable', 60% sentence-detection, 100% analysis coverage, 76% feature coverage), Stanza/Glot500 POS+parsing (79.0% UPOS, 63.8% UAS, 40.9% LAS), Cyrillic+transliteration, NLLB-200 embeddings/MT — but NO NER support, unlike Kazakh which has KazNERD-backed NER and clearly stronger parsing (88.8% UPOS, 71.5% UAS).
>
> **Numbers:** Kyrgyz: 60% morph detection, 100%/76% analysis/feature coverage, 79.0% UPOS/63.8% UAS/40.9% LAS, no NER. Kazakh: 88.8% UPOS/71.5% UAS, has NER (KazNERD)
> **Relevance:** Directly answers decision (3): a broad pan-Turkic TOOLING umbrella already exists (24 languages, unified API) so a 'yet another Turkic toolkit' artifact has no unclaimed territory — but it explicitly has NO embedding/retrieval benchmark layer, confirming that axis remains open for a lab contribution (Turkic-MTEB-mini).
> **Source:** arXiv 2602.19174v4 (TurkicNLP toolkit, Hakimov et al.) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-other-langs-non-kazakh-turkic-nlp
> [pan-turkic] No native MTEB-style or KazQAD-style retrieval/STS/reranking benchmark was found for ANY Turkic language except Turkish. TurkicNLP (arXiv:2602.19174), the most comprehensive Turkic NLP toolkit found (24 languages across Oghuz/Kipchak/Karluk/Siberian/Oghur/Arghu/Historical branches, Apertium FSTs for 20 langs, neural pipelines with UD treebanks for only 8), offers ONLY generic NLLB-200 cross-lingual sentence embeddings for retrieval/clustering across all 24 languages — no fine-tuned or evaluated native retrieval benchmark. Kazakh is explicitly named as one of the best-resourced languages in this toolkit alongside Turkish (full pipeline incl. NER trained on KazNERD, 112,702 tokens/25 entity classes).
>
> **Numbers:** 24 languages, 7 genetic branches; morphology via Apertium for 20 langs; neural dep-parsing UD treebanks for 8 langs; KazNERD 112,702 tokens, 25 entity classes; embeddings = NLLB-200 only, all 24 langs
> **Relevance:** Directly confirms decision (3): a pan-Turkic native retrieval benchmark built on the lab's pinned KazQAD-style protocol would be genuinely unclaimed and would extend naturally from a Kazakh-first kk-MTEB effort — the toolkit paper itself only offers a generic multilingual-embedding fallback, not a benchmark, which is exactly the gap to fill.
> **Source:** arXiv:2602.19174 (TurkicNLP), fetched directly (html v1-v5) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-pan-benchmarks-non-kazakh-turkic
> TurkicNLP toolkit (2026) maps resource tiers across 24 Turkic languages in 4 branches (Oghuz: tr, az, tk, gagauz; Kipchak: kk, ky, tt, ba, crh, kaa, Nogai, Kumyk, Karachay-Balkar; Karluk: uz, ug; Siberian: sah/Sakha, Altai, Tuvan, Khakas; Oghur: cv/Chuvash). Only Turkish + Kazakh have production-quality NER; neural POS/parsing (Stanza+UD) exists for only 8 of 24 languages; Bashkir/Chuvash have morphology-only (beta/prototype Apertium FST) with NO POS/parsing/NER; Sakha has morphology+NLLB embeddings but no syntax/NER; Karakalpak is prototype-morphology-only.
>
> **Numbers:** 24 langs, 4 branches; NER production-quality: tr+kk only; neural pipeline: 8/24 langs; NLLB-200 embeddings/translation: all 24
> **Relevance:** Direct answer to 'which Turkic languages have NO benchmark presence at all': Nogai, Kumyk, Karachay-Balkar, Gagauz, Altai, Tuvan, Khakas have ZERO MMLU/MTEB-style benchmark and only NLLB-translation-level embedding support — these are outside any realistic near-term porting target for the lab's protocols.
> **Source:** arXiv:2602.19174 (TurkicNLP), https://arxiv.org/html/2602.19174v2/v4 · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-pan-models
> [pan-turkic] TurkicNLP toolkit covers 24 Turkic languages across 4 genetic branches (Oghuz/Kipchak/Karluk/Siberian/Oghur) with a single pipeline (tokenization, morph analysis, POS, lemmatization, dep parsing, NER, transliteration, sentence embeddings, MT). Only Turkish [tr] and Kazakh [kk] get full production-quality pipelines. Ten languages ([tr],[kk],[ky],[ug],ottoman-tr,[uz],[az],[tk],[tt],[ba]) have dedicated Stanza neural models. Apertium FST covers 20 languages. Glot500 neural morph analyzer covers 23. All 24 get NLLB-200 embeddings/MT as a floor.
>
> **Numbers:** 24 languages; neural backend 68% detection acc/88% feature coverage vs Apertium FST 53%/54% (20-sentence eval); Glot500 zero-shot Karakalpak-via-Uzbek-proxy 82.1% UPOS acc despite no target training data; avg UPOS 84.9%, UAS 76.8%, LAS 63.6%
> **Relevance:** Direct resource-tier map for where the lab's KazQAD/MTEB-style protocols and Less-is-More recipe can port with existing tooling vs need to build from scratch. Confirms Uzbek/Kyrgyz/Azerbaijani/Tatar/Bashkir sit in a 'moderately-resourced, has neural models but no production pipeline' tier — plausible next targets after Kazakh.
> **Source:** arXiv:2602.19174 (TurkicNLP: An NLP Toolkit for Turkic Languages, 2026) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-pan-models
> [pan-turkic] TurkicNLP's own resource-tier ranking: Turkish [tr] highest-resourced (82,000 UD treebank sentences, multiple BERTurk variants, Zemberek-NLP); Kazakh [kk] well-resourced via ISSAI ecosystem (KazNERD 112,702 tokens/25 classes, KazQAD, KazParC 371,902 parallel sentences kk-en-ru-tr, 1,200+ hrs multilingual Turkic speech); Kyrgyz/Uyghur/Uzbek [ky],[ug],[uz] moderately-resourced (UD treebanks + dedicated LMs + speech corpora; Kyrgyz has 10,900 annotated NER sentences); Sakha/Tuvan/Khakas/Altai/Karakalpak/Kumyk/Karachay-Balkar/Nogai/Gagauz/Khalaj [sah]+others prototype-tier, Apertium coverage thin, zero-shot transfer required.
>
> **Numbers:** Turkish UD 82,000 sentences; Kazakh KazNERD 112,702 tokens; KazParC 371,902 sentences; Kyrgyz NER 10,900 sentences; multilingual Turkic speech 1,200+ hours
> **Relevance:** Directly answers decision (2): resource ranking places Kazakh in the SECOND tier (behind Turkish, ahead of Uzbek/Kyrgyz/Uyghur, far ahead of Sakha/Karakalpak/Tuvan). Gives the atlas a citable 4-tier resource hierarchy.
> **Source:** arXiv:2602.19174 · **Sweep:** `turkic-landscape`

[[Home]]
