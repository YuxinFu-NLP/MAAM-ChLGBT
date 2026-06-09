# MAAM and ChLGBT

This repository contains project materials for **MAAM: Anchor-Preserving Compression and Contextual Calibration for Chinese Discriminatory Language Detection**.

We introduce **ChLGBT**, a fine-grained Chinese LGBT-focused discriminatory-language benchmark with 8,120 manually annotated social-media samples. ChLGBT is designed for analyzing discriminatory expression beyond binary detection by separating **explicit bias**, **implicit bias**, and **emotional intensity**.

> **Important:** We do **not** release the original raw social-media texts of ChLGBT because they may contain sensitive personal expression, harmful language, and content that could be linked back to individual users. The non-identifying ChLGBT dataset will be made public after the paper is formally accepted; at this stage, this repository only provides project information and dataset documentation.

## Paper (Preprint)

Our paper **"MAAM: Anchor-Preserving Compression and Contextual Calibration for Chinese Discriminatory Language Detection"** is now available as a preprint:

[![arXiv](https://img.shields.io/badge/arXiv-2606.09114-b31b1b.svg)](http://arxiv.org/abs/2606.09114)

- **arXiv ID:** 2606.09114
- **Link:** [http://arxiv.org/abs/2606.09114](http://arxiv.org/abs/2606.09114)
- **Cite as:** arXiv:2606.09114 [cs.CL]

## Project Overview

Chinese discriminatory-language detection is challenging because harmful intent is often implicit, contextual, and expressed through stereotypes rather than direct slurs. Existing Chinese bias/discrimination benchmarks are often binary or coarse-grained, which limits fine-grained analysis of how discriminatory meaning is expressed.

This project provides:

- the MAAM framework description,
- the ChLGBT annotation schema and scoring guidelines,
- dataset documentation and aggregate statistics,
- the released ChLGBT dataset in anonymized/re-written text form.

## What is ChLGBT?

ChLGBT is a Chinese LGBT-focused discriminatory-language benchmark built for three-dimensional ordinal annotation. Each sample is labeled independently along the following dimensions:

| Field | Scale | Description |
| --- | --- | --- |
| `explicit_bias` | 1-5 | Overt derogation, hostility, exclusion, or direct discriminatory expression toward LGBT individuals or groups. |
| `implicit_bias` | 1-5 | Indirect prejudice conveyed through stereotypes, insinuation, pragmatic framing, or seemingly neutral statements with discriminatory implications. |
| `emotional_intensity` | 1-5 | Affective strength of the expression, regardless of whether the stance is discriminatory, supportive, ironic, or neutral. |

The three labels are independent. For example, a post can contain little overt hostility but still express strong implicit bias through stereotypes or contextual framing.

## Motivation

Many existing Chinese bias or discriminatory-language resources are formulated as binary classification datasets or coarse categorical benchmarks. While useful for detecting whether a text is biased or discriminatory, binary labels are less suitable for analyzing:

- whether the harmful expression is explicit or implicit,
- whether prejudice is conveyed through stereotypes or pragmatic framing,
- how emotionally intense the expression is,
- how different dimensions of discriminatory language interact.

ChLGBT addresses this gap by providing a fine-grained, multi-dimensional annotation scheme for Chinese LGBT-related discourse.

## Data Collection Summary

The corpus was constructed from Chinese-language Weibo posts related to LGBT discourse. The collection period covered **January 1 to December 31, 2024**.

Keyword queries included LGBT-related terms such as:

- homosexuality,
- bisexuality,
- transgender,
- non-binary,
- sexual minority,
- LGBT,
- queer.

Only original posts were retained. Comments, replies, and retweets were excluded to reduce duplication and preserve linguistic independence.

## Data Cleaning Summary

The preprocessing process removed or filtered:

- user identifiers and profile metadata,
- creation timestamps,
- release locations,
- device information,
- reposted or forwarded content,
- platform-specific tags and mentions,
- duplicated texts,
- detected private information,
- non-Chinese or non-English texts.

The released repository does not include user IDs, handles, profile metadata, source URLs, timestamps, locations, or other metadata that could facilitate re-identification.

## Annotation Process

ChLGBT was manually annotated by six native Chinese speakers, including two LGBT annotators. Annotators were trained and blind to source metadata. Each annotator scored samples independently, and disagreements were resolved through discussion. Final labels were obtained by rounded average scores.

The annotation dimensions are based on a 1-5 ordinal scale:

- **1** indicates no or minimal signal for the target dimension,
- **5** indicates strong signal for the target dimension.

Inter-annotator agreement in the paper is reported using Krippendorff's alpha for explicit bias, implicit bias, and emotional intensity.

## Label Interpretation Note

The labels in ChLGBT reflect judgments made under the annotation protocol of this project. Scores were assigned by trained annotators according to the provided guidelines and resolved through the project's annotation process.

The 1-5 scores should be interpreted as ordinal research labels rather than objective or absolute measurements of discriminatory intent, implicit bias, or emotional intensity. Because discriminatory language can be context-dependent, implicit, ironic, or ambiguous, individual examples may admit alternative interpretations.

Therefore, the labels should be used for dataset-level analysis, model training, and benchmark evaluation under the documented annotation scheme. They should not be treated as definitive moral, legal, or social judgments about any individual speaker or community. Disagreements about individual scores should be understood as part of the inherent subjectivity of fine-grained bias annotation, rather than as errors in isolation.

## Dataset Access

Due to privacy and ethical considerations related to social-media content and LGBT-related discriminatory language, we do **not** release the original raw Weibo texts used to construct ChLGBT.

The original posts may contain sensitive personal expression, potentially harmful language, and content that could be linked back to individual users. Even after removing usernames, URLs, and metadata, original social-media texts may still be searchable or reconstructable. To reduce privacy risks and prevent re-identification, this repository does not provide:

- full raw Weibo texts,
- source URLs,
- user IDs,
- user handles,
- timestamps,
- locations,
- device metadata,
- other identifying metadata.

**The non-identifying ChLGBT dataset will be released after the paper is formally accepted.** At the current stage, this repository only provides related project information and documentation materials, including:

- annotation guidelines,
- label schema,
- data statement,
- preprocessing description,
- aggregate statistics.

After release, the non-identifying dataset texts will be intended to preserve the linguistic and annotation-relevant content needed for research while reducing the risk of tracing examples back to original social-media users. We do **not** distribute the original raw social-media texts.

## Ethical Use

This project studies discriminatory language toward LGBT individuals and communities. Some examples or descriptions may involve harmful, offensive, or sensitive language for research purposes.

Users of this repository must not:

- attempt to identify, trace, contact, or profile any original social-media user,
- search for, reconstruct, or redistribute the original posts,
- use the materials for harassment, surveillance, profiling, or targeting of LGBT individuals or communities,
- use the materials to generate, amplify, or normalize discriminatory content,
- redistribute sensitive examples outside necessary academic discussion,
- use the materials for commercial or harmful applications.

The intended use of this project is academic research on bias, discriminatory-language detection, model robustness, interpretability, and socially beneficial NLP applications.

## Repository Contents

This repository is organized in a minimal format:

```text
.
├── README.md
└── Dataset/
```

`README.md` provides the project overview, annotation schema, access policy, ethical-use statement, license information, and contact details.

`Dataset/` contains the released non-identifying ChLGBT dataset and documentation, including anonymized/re-written dataset texts, labels, annotation guidelines, label schema, preprocessing description, and aggregate statistics. It does **not** contain the original raw social-media texts, code, or experimental scripts.

## Example Data Format

The released anonymized/re-written dataset follows the CSV-style schema used in our annotation files:

```csv
Sentences,Explicit,Implicit,Emotional
xswl来自直女的真诚发问话说我从初中就开始看有同性恋相关的漫画，并不是刻意去找这种题材，而是很多漫画里都涉及到，当时看也没觉得是很敏感的事。上大学后除了漫画还看小说和影视剧，直到现在也一样，然而我一直是异性恋啊，所以青少年接触同性题材会被影响性观念在我身上好像说不通，也可能是没试过,1,1,2
姐妹你真的误会了，他俩真不是给子，你看这照片，不就是拍了组一模一样的图吗？不就是看起来像情头而且都放在了第一张吗？队友同事拍一张怎么了？！好了好了姐妹你别说了，世界上没有那么多同性恋！！,3,3,5
女孩是个同性恋我越看越抽象越看越雷人，不是，饭不吃来看这个好惶恐，我不是故意的,3,3,3
显然还是做同性恋好啊,1,1,3
```

Column meanings:

- `Sentences`: anonymized or re-written dataset text,
- `Explicit`: explicit-bias score from 1 to 5,
- `Implicit`: implicit-bias score from 1 to 5,
- `Emotional`: emotional-intensity score from 1 to 5.

This format describes the released non-identifying dataset. It does not imply that the original raw social-media texts are publicly released.

## License

This repository is released under the **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)**.

You may share and adapt the released materials for non-commercial research purposes, provided that you:

- give appropriate credit,
- indicate if changes were made,
- do not use the materials for commercial purposes,
- distribute derivative materials under the same license.

The CC BY-NC-SA 4.0 license applies to the released documentation, annotation guidelines, label schema, aggregate statistics, and anonymized/re-written dataset texts. It does **not** grant access to the original raw social-media texts, code, or experimental scripts.

## Citation

If you use this project, the MAAM framework, or the ChLGBT dataset in your research, please cite our arXiv preprint:

```bibtex
@misc{fu2026maamanchorpreservingcompressioncontextual,
      title={MAAM: Anchor-Preserving Compression and Contextual Calibration for Chinese Discriminatory Language Detection}, 
      author={Yuxin Fu and Shijing Si},
      year={2026},
      eprint={2606.09114},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2606.09114}, 
}
```

## Contact

For questions about the project, annotation protocol, or non-identifying research materials, please contact:

- **Yuxin Fu**: yuxinfuNLP@outlook.com
- **Shijing Si**: shijing.si@outlook.com
