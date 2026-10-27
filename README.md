# MAAM and ChLGBT


[![EMNLP 2026 Accepted](https://img.shields.io/badge/EMNLP%202026-Accepted%20(Findings)-emerald.svg)](https://2026.emnlp.org/)
[![arXiv](https://img.shields.io/badge/arXiv-2606.09114-b31b1b.svg)](http://arxiv.org/abs/2606.09114)
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

> ## 🎉 **News (August 21, 2026)**
> 
> Our paper **"MAAM: Anchor-Preserving Compression and Contextual Calibration for Chinese Discriminatory Language Detection"** has been officially accepted to **EMNLP 2026 (Findings)**!
> 


## 🕊️ [2026-10-27 Update] Retrospective on EMNLP & The End of MAAM


After attending the conference, I still find myself overwhelmed with complex emotions. Standing on the stage of a top-tier conference for the first time, it is inevitable to leave with both theoretical pride and a touch of regret.

I was deeply moved when the very first attendee at my poster session said to me: 
> *"This work should have made it into the main conference."*

In truth, how could I not have thought the same? The solitary courage of youth and unadulterated talent could only carry me this far.

> **“少年之孤勇与悲痛并非能被大众所热烈推崇之作。”**  
> *(The raw courage and grief of youth are rarely works that the broad public warmly embraces.)*

The chapter of **MAAM** comes to its close here. Though there remains so much left unsaid, it has officially reached its conclusion (2025.12.15 – 2026.10.27).

Even if it didn't reach a higher pedestal, nor commanded grander applause, it at least allowed me to step out of being a *nobody* and begin carving out my own voice in the field.


Anyway, stay tuned for my next work — **coming soon**.

This will be the second installment of the series (MAAM was the first). Success in research demands far more than raw talent alone. Fortunately, this time around, I will no longer be as completely empty-handed — left with nothing but talent — as I was back in December 2025.

<br>

<div align="left">
  <p><em>Written in Budapest, Hungary</em></p>
  <p><em>October 2026</em></p>
</div>



 
---

## 📢 [2026-09-23 Update] Note on System-1 Synergy (e.g., Jev) & Call for Collaborators 🚀

Recently, ultra-fast System-1 decision controllers (such as Jev)) have gained significant traction in the community. Although **MAAM** (*Anchor-Preserving Compression and Contextual Calibration*) was originally evaluated on classical BERT-style encoders to guarantee rigorous, noise-free pragmatic baselines, its core methodology is fundamentally **architecture-agnostic**.

Conceptually, MAAM serves as a near-perfect pre-processing and noise-filtering engine for fast System-1 controllers:
- **Noise Suppression**: Dynamically filters context redundancy while retaining essential semantic anchors.
- **Context Calibration**: Restores implicit pragmatic nuances (e.g., sarcasm, indirect discrimination) before hitting the decision layer.

Integrating MAAM as an anchor-preserved pre-processor for Jev-like controllers can potentially achieve much higher accuracy and inference throughput than traditional encoders. 

As I am currently shifting my focus toward a **completely new, independent research direction that goes beyond MAAM (stay tuned for the upcoming series!)** in NLP/AI Safety, I won't have the bandwidth to write a dedicated MAAM + Jev hybrid paper. However, I warmly invite and encourage interested researchers and developers to explore this promising direction!

> 💡 **Call for Collaborators:**
> As an independent researcher with limited compute resources and team support, I am actively seeking collaborators, compute sponsors, and lab partners for my upcoming research series. If you are passionate about pioneering novel, sharp angles in NLP, AI Safety, and Pragmatics, feel free to open an Issue, PR, or reach out via email! Let's build something impactful together! 🌟



---

# 🤝 **Let's Connect & Build Together!**

🔥 **Primary Goal: Seeking Ph.D. Opportunities**

I am actively looking for **Ph.D. positions**! My core background is anchored in the **AI Bias, Safety, and Ethics** track, and I am eager to expand into next-generation research directions. If you are a professor, researcher, or lab leader looking for a fiercely independent student with a proven track record (and the ability to deliver top-tier work single-handedly), I would love to chat! 
👉 **Personal Site**: [yuxinfu-nlp.github.io](https://yuxinfu-nlp.github.io)
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


# 📖 Three Ways to Read This Repository

> **🧭 [Read the Philosophy & MAAM's WORLD](./README（MAAM%27s%20WORLD）.md)** — Why this method exists, the personal story, the five universal principles, and how to extend it to any language, task, or model.
>
> **⚙️ [Read the instructions for the Dataset](./README（ChLGBT）.md)** — Details of ChLGBT.
> 
> **🎨 [View / Download my Hand-Crafted Poster PDF here](MAAM-Poster.pdf)** — Come check out what true handmade poster looks like.

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


*For institutional or administrative correspondence:*
- **Shijing Si** (co-author): shijing.si@outlook.com
