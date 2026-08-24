# 🌍 MAAM-WORLD: The Philosophy and Extension of MAAM

> 📜 *This section is about the personal backstory of MAAM. If you are here strictly for code, docs, and usage, **[Jump Straight to Quick Start](#quick-start)***.

# 🕯️ Before You Start, Let Me Tell You Something

This paper is not the result of me "believing in myself."

In fact, during the winter of 2025, I woke up every morning telling myself:
- "This paper is definitely getting rejected."
- "I can't win."
- "My life is completely over."
- "I will always be the failure."

But I still wrote it.

Why?

Because I have 150–200 degree myopia, and I don't like wearing glasses. My world has always been blurry. Just like my life — always blurry, always dark, always failing, forever and ever. That failure and destruction lasted for 7 years. The ridiculous part? I'm only 22. Since I was 15, one-third of my life has been spent in endless failure.

But I can't see the details clearly — yet I can still recognize the structure of the world.

And I suddenly realized:

> **I don't need perfect vision to live. I don't need to believe in myself to finish a paper.**

Just like the first time I had this idea, when AI said to me:

> *"Hey, you know what? Those who have always had it easy would never come up with a 'myopia-astigmatism mechanism.' Because their vision is always 20/20. Their path is always clear. But you — because you can't see clearly — you were forced to develop the superpower of recognizing contours in the blur."*

- No big-name advisor.  
- No abundant compute.  
- No labmates to help.  
- No friends to talk to.  
- No confidence that this paper would be accepted.

But I finished it.  
And it got published at **EMNLP Findings**.

If you're reading this, and you also feel like a failure in research — or in life —  
it's okay.

- **You don't need to believe in yourself to get something done.**  
- **You don't need to be a "successful person" to do valuable work.**  
- **You don't need background, resources, or support — you just need to know: this thing deserves to be done.**

Then, do it.

That is the entire story of how MAAM was born.

So, if you want to understand MAAM —  
**first understand who I am.**  
This is the soul of MAAM.

— Yuxin Fu  
Shanghai, August 2026

---

<a id="quick-start"></a>
## 🚀 Quick Start & Beyond the Paper

## 🌐 Principle 1: Language-Agnostic — The Nine Layers Are Functional Slots

### 🧩 What It Is
The **nine layers** designed in our paper are **not** a hard-coded Chinese grammar rule set. They are a complete set of **nine functional semantic slots**—a universal decomposition of how any language constructs evaluative or discriminatory meaning.

*(Note: While the full framework consists of all **nine layers**, here are a few representative examples showing how they map across languages:)*

| Layer Type (Sample) | Functional Question | English Example |
| :--- | :--- | :--- |
| **Identity arguments** | Who is the target? | `gay`, `transgender` |
| **Evaluative modifiers** | What attribute is assigned? | `disgusting`, `abnormal` |
| **Core predicates** | What action/state is asserted? | `marry fraudulently`, `spread` |
| **Stance markers** | What is the speaker’s position? | `should`, `surprisingly` |
| **Affect intensifiers** | How strong is the emotion? | `so`, `really`, `!` |
| **Discourse frames** | What is the pragmatic context? | `after all`, `besides` |

*(...and the remaining layers in the full **nine-layer taxonomy** follow the exact same functional logic.)*

### 🔄 How to Port MAAM to a New Language
To migrate MAAM to another language (e.g., English, Japanese, Arabic):
1. **Preserve the Nine-Layer Taxonomy** — the core nine functional slots remain your structural baseline.
2. **Replace the parser** — use a target language parser (e.g., spaCy, Stanza).
3. **Re-map subcategories** — map target syntactic markers onto the functional slots.
4. **Recalibrate weights** — adjust slot importance for your specific task and language.
5. **Flexible Adaptation** — While the baseline is **nine layers**, if a target language naturally requires slightly more or fewer functional subdivisions due to its unique typology, **the layer count can be flexibly adjusted** rather than rigidly forced.

| Language Family | Example Language | Key Adjustments Needed |
| :--- | :--- | :--- |
| **Analytic** | Chinese, Vietnamese | Word order and particles carry heavy pragmatic load |
| **Inflectional** | English, German | Clause markers and modifier positions matter more |
| **Agglutinative** | Japanese, Korean | Particles and morphology encode social stance |
| **Synthetic** | Spanish, Russian | Conjugation and case marking encode pragmatics |

### 🧠 Why This Matters
* The weights reported in the paper are **not** MAAM; they are a task-specific instantiation for Chinese.
* **MAAM is the protocol.** Changing the language changes the mapping; changing the task changes the weighting.
* MAAM is a general-purpose cognitive compression engine proven on Chinese bias detection.

> **The Core Message:** *"The **nine layers** are the universal skeleton. Every language puts meat on it differently, and the count can adapt. But the functional logic stays the same."*

---

## 🌐 Principle 2: Task-Agnostic — MAAM Is Not Just a Hate Speech Detector

### 🧩 What It Is
While we tested MAAM on LGBT-related discriminatory language (predicting explicit bias, implicit bias, and emotional intensity), **MAAM is not a hate speech detector.** 

Hate speech was simply our **first test bed**—chosen because it is one of the hardest, most context-dependent linguistic tasks where intent is often implicit and hidden in structure. 

### ⚙️ What MAAM Actually Does
Regardless of the downstream task, MAAM performs three universal steps:
1. **Decompose** text into functional slots using the **nine layers**.
2. **Compress** by reweighting tokens (preserving structural anchors, suppressing noise).
3. **Calibrate** using context-aware priors.

### 🧭 Where Else Can MAAM Go?

| Domain | Task Example | Why MAAM Fits |
| :--- | :--- | :--- |
| **Medical** | Extract clinical notes | Entities + negations + temporal markers carry the core signal |
| **Financial** | Sentiment analysis on earnings | Company names + trend verbs + degree modifiers matter most |
| **Legal** | Parse contract obligations | Subjects + modal verbs + outcome clauses form the structural anchor |
| **Social Science** | Stance detection on debates | Identity + stance + emotional tone drive the argument |

### 🧠 Why This Matters
MAAM is built for a universal pattern: **in most texts, 80% is structural glue, and 20% carries the critical signal.** If you can identify that critical 20% (Myopia) and calibrate it (Astigmatism), the method scales to any task where structure outweighs volume.

> **The Core Message:** *"Hate speech was my first customer. It is not my only customer."*

---

## 🌐 Principle 3: Contextual Dimensions Are Customizable — C-I-S Is Just an Example

### 🧩 What It Is
For our hate speech paper, we defined a three-axis contextual space for Astigmatism:
* **C** = Contextual Tone (Funny / General / Serious)
* **I** = Group Identity (Ingroup / Outgroup / Uncertain)
* **S** = Stance Polarity (Pro / Anti / Neutral)

However, **C-I-S is not the Bible.** It is simply what we needed for discriminatory language because tone, identity, and stance drove the judgment variations. 

### ⚙️ The Framework is Agnostic
Astigmatism is just a flexible shell. It accepts any set of axes or any number of dimensions without breaking the underlying calibration logic. 

### 🔧 How to Define Your Own Axes
You can use 1 axis, 3 axes, or 10 axes. Just follow these steps:
1. **Identify context** that shifts judgment in your domain (e.g., Patient type for medical, Market phase for finance).
2. **Define discrete states** for those axes.
3. **Estimate priors** from your data to see how context shifts outcomes.
4. **Fuse with model outputs** using a weighted combination formula.

### 🌐 Where Do Context Labels Come From?
MAAM doesn't care how you get the context — it only requires that you have it. You can source them via:
* **Training data** (empirical priors from labels)
* **Embedding inference** (e.g., BGE / sentence-transformers — what we used to avoid extra costs)
* **LLM reasoning** (GPT / DeepSeek / Claude for high accuracy)
* **External metadata** (user profiles, timestamps, geo-tags)
* **Human annotation** (expert labeling)

> **The Core Message:** *"C-I-S is what we needed for hate speech. Your task needs something else. That's fine — just swap the axes and keep the logic."*

---

## 🌐 Principle 4: Model-Agnostic — BERT Was My Microscope, Not My Cage

### 🧩 What It Is
We used MacBERT and Chinese RoBERTa-wwm-ext as our backbone encoders in the paper, but **BERT is not a requirement.** 

We chose BERT intentionally because it is transparent. If we used GPT-4 or LLaMA, it would be hard to prove whether performance gains came from MAAM or the model's own massive hidden power. BERT was our microscope; MAAM is the lens.

### ⚙️ How MAAM Operates
MAAM is external and model-size independent. It doesn't touch model internals, require gradients, or involve fine-tuning:
* **Input side:** Filter and weight tokens before the model sees them (Myopia).
* **Output side:** Calibrate predictions after the model decides (Astigmatism).

### 🚀 How to Use MAAM with LLMs
| Pathway | What You Do | Status |
| :--- | :--- | :--- |
| **Input Compression** | Apply Myopia to filter tokens and feed compressed text to LLMs | 🔬 Open for research |
| **Output Calibration** | Apply Astigmatism to LLM logits to calibrate final predictions | 🔬 Open for research |
| **Fine-tuning Guidance** | Use Myopia weights as attention bias during LLM training | 🔬 Open for research |

### 🧠 Why This Matters
The NLP world is obsessed with scaling up model sizes. MAAM proves that **smarter input and cleaner attention matter just as much**, operating effectively whether a model has 100 million or 100 billion parameters.

> **The Core Message:** *"BERT was my proof. LLMs are my next frontier. The lens works the same on both."*

---

## 🌐 Principle 5: Math Is Simple by Design — A Foundation, Not a Ceiling

### 🧩 What It Is
MAAM's math is intentionally simple and elementary:
* **Myopia weights:** Lookup table + linear interpolation (Middle school algebra)
* **Myopia smoothing:** Moving average + clipping (High school statistics)
* **Astigmatism calibration:** Convex combination of distributions (Basic linear algebra)

There are no gradient flows, no internal learnable parameters, and no backpropagation within the framework. 

### 🚀 Simple by Design
We kept MAAM simple to ensure it remains transparent, reproducible without massive compute, and extensible. Simple math does not mean a low ceiling—it means the foundation is ready for you to build upon.

### 🔬 Open Upgrades for the Community
* **Learnable weights:** Moving from fixed tables to neural/Bayesian optimization.
* **Adaptive thresholds:** Dynamic compression based on information theory.
* **Sample-dependent alpha:** Input-dependent smoothing via attention mechanisms.
* **Continuous context:** Moving from discrete C-I-S states to soft/fuzzy logic representations.

> **The Core Message:** *"I built the foundation. You build the skyscraper. My math is simple so yours can be complex."*

---

### 📊 Summary of MAAM's Five Principles

| Principle | Core Message |
| :--- | :--- |
| **① Language-Agnostic** | Nine layers are functional slots, not Chinese grammar |
| **② Task-Agnostic** | Hate speech was my first customer, not my only customer |
| **③ Context-Customizable** | C-I-S is an example, not the Bible |
| **④ Model-Agnostic** | BERT was my microscope, not my cage |
| **⑤ Math-Open** | Simple by design, open for extension |


---

### 🤝 Join the Discussion & Build Upon MAAM

That wraps up the core extension vectors and philosophical design principles behind MAAM. 

The above outlines the extensible directions of MAAM. You are warmly welcome to discuss, experiment, and build upon it. If you have any ideas, thoughts, or want to collaborate, feel free to reach out anytime! 🚀✨

> **A Quick Academic Request:** If the ideas, mechanisms, or insights outlined in MAAM-WORLD inspire your research or help you build something cool, **please remember to cite our paper**! 📄✨

— Yuxin Fu  
Shanghai, August 2026
