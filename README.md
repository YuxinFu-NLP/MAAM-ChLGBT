# MAAM and ChLGBT


[![EMNLP 2026 Accepted](https://img.shields.io/badge/EMNLP%202026-Accepted%20(Findings)-emerald.svg)](https://2026.emnlp.org/)
[![arXiv](https://img.shields.io/badge/arXiv-2606.09114-b31b1b.svg)](http://arxiv.org/abs/2606.09114)
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

> ## 🎉 **News (August 21, 2026)**
> 
> Our paper **"MAAM: Anchor-Preserving Compression and Contextual Calibration for Chinese Discriminatory Language Detection"** has been officially accepted to **EMNLP 2026 (Findings)**!  
> 
> We look forward to seeing you in Budapest, Hungary!



# 📢 **A Quick Note & Delivering on My Promise (September 7, 2026)**

First of all, thank you all so much for checking out **MAAM** and **ChLGBT**!

As promised, I am here to honor my word—even if it might feel like a quiet promise in a noisy world. Today, I am officially releasing the complete, authentic **ChLGBT** dataset. 

This dataset carries the weight of my entire undergraduate journey—countless late nights, unyielding persistence, and absolute passion. My original motivation for building **ChLGBT** was to amplify the voices of marginalized communities, fostering a truly equal world where people are never judged or discriminated against by labels.

In that very same spirit, I hope the academic community will look past my educational background, look past the labels, and evaluate my work based purely on **my talent, my logic, and my contribution to the field.**

To be completely honest, this is my very first time having a paper accepted to a venue of this scale (EMNLP 2026), and I am navigating the entire post-acceptance workflow alone. I am also flying solo to Budapest—my first time taking a long-haul flight and leaving Asia! It’s a bit daunting, but I am excited for what lies ahead.

---

# 🤝 **Let's Connect & Build Together!**

🔥 **Primary Goal: Seeking Ph.D. Opportunities**
I am actively looking for **Ph.D. positions**! My core background is anchored in the **AI Bias, Safety, and Ethics** track, and I am eager to expand into next-generation research directions. If you are a professor, researcher, or lab leader looking for a fiercely independent student with a proven track record (and the ability to deliver top-tier work single-handedly), I would love to chat! 

**Other Ways to Connect:**
* Discuss the **MAAM** methodology, dataset replications, or AI Safety landscapes.
* Share any visa tips or conference survival guides for Budapest.
* Connect as conference buddies at EMNLP 2026!

Feel free to drop me an email anytime. The data is now live—let's start this journey!

> **Best regards,**  
> **Yuxin Fu**  
> yuxinfuNLP@outlook.com  
> *(Author of MAAM & ChLGBT)*
---

This repository contains project materials for **MAAM: Anchor-Preserving Compression and Contextual Calibration for Chinese Discriminatory Language Detection**.

Chinese discriminatory-language detection is challenging because harmful intent is often implicit and context-dependent. We propose **MAAM (Myopia--Astigmatism Anchor Mechanism)**, a lightweight, model-agnostic framework inspired by functional visual blur: rather than preserving every token equally, MAAM retains discrimination-relevant semantic anchors and calibrates them with C--I--S contextual priors (Contextual Tone, Group Identity, and Stance Polarity). We also introduce **ChLGBT**, to our knowledge the first Chinese LGBT-focused discriminatory-language dataset, with 8,120 manually annotated samples and three ordinal labels: explicit bias, implicit bias, and emotional intensity. Across strong encoder baselines, MAAM improves all three prediction dimensions, with consistent gains in accuracy, F1, Brier score, and expected calibration error. Compared with frontier LLM baselines under zero-shot and few-shot prompting protocols, MAAM remains competitive while offering stronger compactness and stability. These results suggest that interpretable anchor preservation and contextual calibration provide a practical alternative to heavier model scaling for Chinese discriminatory-language assessment.

> **Data Access & Privacy Note:** 
> To protect sensitive personal expressions and ensure ethical compliance, the original raw social-media texts of **ChLGBT** are not released to prevent any risk to individual users. However, the cleaned, non-identifying, and fully processed **ChLGBT dataset** is **now officially live and available in this repository** (see the attached release files). Enjoy exploring and building upon our work!


# 📖 Two Ways to Read This Repository

> **🧭 [Read the Philosophy & MAAM's WORLD](./README（MAAM%27s%20WORLD）.md)** — Why this method exists, the personal story, the five universal principles, and how to extend it to any language, task, or model.
>
> **⚙️ [Read the Technical Paper & Experiments](./README（ChLGBT）.md)** — The EMNLP 2026 Findings paper, ChLGBT dataset and experimental results.

---


## Paper (Preprint)

Our paper **"MAAM: Anchor-Preserving Compression and Contextual Calibration for Chinese Discriminatory Language Detection"** is now available as a preprint:

[![arXiv](https://img.shields.io/badge/arXiv-2606.09114-b31b1b.svg)](http://arxiv.org/abs/2606.09114)

- **arXiv ID:** 2606.09114
- **Link:** [http://arxiv.org/abs/2606.09114](http://arxiv.org/abs/2606.09114)
- **Cite as:** arXiv:2606.09114 [cs.CL]




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

## Contact & Collaboration

We warmly welcome academic discussions, potential research collaborations, and inquiries regarding the **MAAM** framework or the **ChLGBT** benchmark!

- **Primary Contact (for research collaboration & dataset access):** Yuxin Fu ([yuxinfuNLP@outlook.com](mailto:yuxinfuNLP@outlook.com)) — please direct all project-related correspondence here.
- **GitHub Issues:** Feel free to open an issue in this repository for technical questions or bug reports.
- **Collaboration Note:** If you are interested in extending the ChLGBT benchmark, fine-grained bias analysis, or cross-linguistic discriminatory language detection, please don't hesitate to reach out via email—we'd be happy to connect and discuss ideas.

We also welcome feedback, suggestions, and constructive criticism to help us improve this project.

---

*For institutional or administrative correspondence:*
- **Shijing Si** (co-author): shijing.si@outlook.com
