# MAAM and ChLGBT


[![EMNLP 2026 Accepted](https://img.shields.io/badge/EMNLP%202026-Accepted%20(Findings)-emerald.svg)](https://2026.emnlp.org/)
[![arXiv](https://img.shields.io/badge/arXiv-2606.09114-b31b1b.svg)](http://arxiv.org/abs/2606.09114)
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

> ## 🎉 **News (August 21, 2026)**
> 
> Our paper **"MAAM: Anchor-Preserving Compression and Contextual Calibration for Chinese Discriminatory Language Detection"** has been officially accepted to **EMNLP 2026 (Findings)**!  
> 
> We look forward to seeing you in Budapest, Hungary!

## 📢 A Quick Note & A First-Timer's Honesty (September 1, 2026)

First of all, thank you all so much for checking out MAAM and ChLGBT! 

As we officially step into September 1st, I realize there might have been some misunderstandings due to my initial, rather formal notice. To be completely honest, **this is my very first time having a paper accepted to such a large-scale international conference (EMNLP 2026), and I am still getting familiar with its post-acceptance workflow.** 

Because I have no prior experience navigating a venue of this scale, and no senior lab mates to guide me through the administrative and risk controls, **I was extra anxious and wanted to make sure everything was 100% secure before releasing the raw dataset**—which is why I pushed the public release of **ChLGBT** to **early September 2026**.

To make matters even more "adventurous": **I am flying solo to Budapest all by myself!** This will be my very first time traveling to Europe, my first time taking such a long-haul international flight, and honestly, **the first time I'm leaving Asia**. I am basically a complete novice when it comes to travel of this scale, and to be a little vulnerable—**I am quite nervous!**

---

### 🤝 Let's Break the Ice & Connect!

Since we've cleared the air, **please don't hesitate to reach out to me!** 

🔥 **Primary Goal / PhD Opportunities & Research Direction:**  
**I am actively looking for Ph.D. positions / opportunities starting soon!** My core research background is anchored in the **AI Bias & Safety** track, and I am currently looking forward to exploring and expanding into exciting new research directions. If you are a professor, a researcher, or a lab looking for a motivated student with a proven track record in this domain, **please reach out to me via email!** I would love to discuss potential Ph.D. openings and how I can contribute to your group.

**Other ways to connect (I'd love to hear from you!):**
* Chat about the **MAAM methodology**, discuss the **Bias & Safety** landscape, or brainstorm new cross-domain tracks.
* Share any advice, **visa tips, or conference survival guides** for Budapest (I am all ears!).
* Connect as **conference buddies** if you are also attending EMNLP 2026!

You can drop me an email anytime. Let’s connect, clear up any misunderstandings, and hopefully start a wonderful academic journey together!

> **Best regards,**  
> **Yuxin Fu**  
> yuxinfuNLP@outlook.com  
> *(Author of MAAM & ChLGBT)*
---

This repository contains project materials for **MAAM: Anchor-Preserving Compression and Contextual Calibration for Chinese Discriminatory Language Detection**.

Chinese discriminatory-language detection is challenging because harmful intent is often implicit and context-dependent. We propose **MAAM (Myopia--Astigmatism Anchor Mechanism)**, a lightweight, model-agnostic framework inspired by functional visual blur: rather than preserving every token equally, MAAM retains discrimination-relevant semantic anchors and calibrates them with C--I--S contextual priors (Contextual Tone, Group Identity, and Stance Polarity). We also introduce **ChLGBT**, to our knowledge the first Chinese LGBT-focused discriminatory-language dataset, with 8,120 manually annotated samples and three ordinal labels: explicit bias, implicit bias, and emotional intensity. Across strong encoder baselines, MAAM improves all three prediction dimensions, with consistent gains in accuracy, F1, Brier score, and expected calibration error. Compared with frontier LLM baselines under zero-shot and few-shot prompting protocols, MAAM remains competitive while offering stronger compactness and stability. These results suggest that interpretable anchor preservation and contextual calibration provide a practical alternative to heavier model scaling for Chinese discriminatory-language assessment.

> **Important:** We do **not** release the original raw social-media texts of ChLGBT because they may contain sensitive personal expression, harmful language, and content that could be linked back to individual users. The non-identifying ChLGBT dataset will be made public after the paper is formally accepted (by early September 2026); at this stage, this repository only provides project information and dataset documentation.


# 📖 Two Ways to Read This Repository

> **🧭 [Read the Philosophy & MAAM's WORLD](./README（MAAM%27s%20WORLD）.md)** — Why this method exists, the personal story, the five universal principles, and how to extend it to any language, task, or model.
>
> **⚙️ [Read the Technical Paper & Experiments](#)** — The EMNLP 2026 Findings paper, ChLGBT dataset and experimental results.

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
