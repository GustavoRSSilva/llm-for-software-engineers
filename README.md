# LLM for Software Engineers

Inspired by [Google Interview University](https://github.com/jwasham/coding-interview-university), [Machine Learning for Software Engineers](https://github.com/ZuzooVn/machine-learning-for-software-engineers), [Blockchain for Software Engineers](https://github.com/benstew/blockchain-for-software-engineers)

> "Software is eating the world, but AI is eating software." - Jensen Huang

## What is it?

A collection of resources I've gathered while going deep into the world of Large Language Models, as a software engineer trying to understand not just how to *use* LLMs, but how they actually work from the ground up.

This list is centered on the end goal of building production-quality LLM applications and understanding the models that power them. From the math foundations through transformer architecture, fine-tuning, deployment, and safety. All contributions welcome!

## About me

My name is Gustavo Silva and my background is in software engineering. I'm currently on a journey from a beginner to someone who genuinely understands how language models work and how to build reliable systems on top of them.

LinkedIn: [https://www.linkedin.com/in/GustavoRSSilva/](https://www.linkedin.com/in/GustavoRSSilva/)

## Goal

Create and curate a list of resources for software engineers who want to go beyond API wrappers and deeply understand — and build with — Large Language Models.

## Table of Contents

- [What is it?](#what-is-it)
- [About me](#about-me)
- [Goal](#goal)
- [Covering the Material](#covering-the-material)
- [How to use it](#how-to-use-it)
- [Mathematics Foundations](#mathematics-foundations)
  - [Linear Algebra](#linear-algebra)
  - [Calculus](#calculus)
  - [Probability & Statistics](#probability--statistics)
  - [Information Theory](#information-theory)
- [Machine Learning Fundamentals](#machine-learning-fundamentals)
- [Deep Learning](#deep-learning)
- [Natural Language Processing](#natural-language-processing)
- [The Transformer Architecture](#the-transformer-architecture)
- [Large Language Models](#large-language-models)
  - [Pre-training](#pre-training)
  - [Alignment & Fine-tuning](#alignment--fine-tuning)
  - [Efficient Fine-tuning](#efficient-fine-tuning)
  - [Scaling Laws](#scaling-laws)
- [Inference & Deployment](#inference--deployment)
  - [Quantization & Distillation](#quantization--distillation)
  - [Serving & Optimization](#serving--optimization)
- [Practical LLM Engineering](#practical-llm-engineering)
  - [Prompt Engineering](#prompt-engineering)
  - [Retrieval-Augmented Generation](#retrieval-augmented-generation)
  - [Agents & Tool Use](#agents--tool-use)
  - [Frameworks & Libraries](#frameworks--libraries)
  - [Evaluation](#evaluation)
- [Safety & Alignment](#safety--alignment)
- [Multimodal Models](#multimodal-models)
- [LLM Blogs](#llm-blogs)
- [Forums and Threads](#forums-and-threads)
- [Podcasts](#podcasts)
- [Additional Curated Lists](#additional-curated-lists)
- [Getting a Job](#getting-a-job)
- [Job Boards](#job-boards)

## Covering the Material

I found it useful to pick a subject from the list below, read it thoroughly, take notes, and implement or experiment with it. I prefer a top-down, hands-on approach — get something working, then go deeper on the internals. Building and pushing understanding daily is what makes this stick.

## How to use it

Everything below is a prioritized outline and you should work from the top to the bottom.

- Create a new branch so you can check items like this, just put an x in the brackets: [x]

---

## Mathematics Foundations

LLMs are math. Understanding the foundations is the difference between cargo-culting API calls and genuinely knowing what is happening inside the model.

### Linear Algebra

The language of tensors, embeddings, and weight matrices.

- [ ] [Essence of Linear Algebra — 3Blue1Brown](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)
- [ ] [Linear Algebra — Gilbert Strang (MIT OCW)](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/)
- [ ] [The Matrix Calculus You Need for Deep Learning](https://arxiv.org/abs/1802.01528)

### Calculus

Gradients drive everything in neural network training.

- [ ] [Essence of Calculus — 3Blue1Brown](https://www.youtube.com/playlist?list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr)
- [ ] [Calculus for Machine Learning — fast.ai](https://explained.ai/matrix-calculus/index.html)

### Probability & Statistics

LLMs are probabilistic models — every output is a distribution over tokens.

- [ ] [Probability Theory: The Logic of Science — Jaynes](https://bayes.wustl.edu/etj/prob/book.pdf)
- [ ] [Seeing Theory — Brown University](https://seeing-theory.brown.edu/)
- [ ] [Statistical Rethinking — Richard McElreath](https://xcelab.net/rm/statistical-rethinking/)

### Information Theory

Cross-entropy loss, perplexity, KL divergence — these are all information-theoretic concepts.

- [ ] [Visual Information Theory — Chris Olah](https://colah.github.io/posts/2015-09-Visual-Information/)
- [ ] [A Short Introduction to Entropy, Cross-Entropy, and KL-Divergence — Aurélien Géron](https://www.youtube.com/watch?v=ErfnhcEV1O8)

---

## Machine Learning Fundamentals

Before you can understand LLMs, you need to understand supervised learning, loss functions, gradient descent, and regularization.

- [ ] [An Introduction to Statistical Learning](https://www.statlearning.com/)
- [ ] [Machine Learning — Andrew Ng (Coursera)](https://www.coursera.org/specializations/machine-learning-introduction)
- [ ] [Machine Learning Glossary — Google](https://developers.google.com/machine-learning/glossary)

---

## Deep Learning

Neural networks, backpropagation, CNNs, RNNs — the building blocks before transformers.

- [ ] [Neural Networks: Zero to Hero — Andrej Karpathy](https://youtube.com/playlist?list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ)
- [ ] [Practical Deep Learning for Coders — fast.ai](https://course.fast.ai/)
- [ ] [Deep Learning — Goodfellow, Bengio, Courville](https://www.deeplearningbook.org/)
- [ ] [Dive into Deep Learning](https://d2l.ai/)

---

## Natural Language Processing

The field that LLMs grew out of. Understanding classic NLP helps you appreciate what transformers replaced and why.

- [ ] [CS224N: NLP with Deep Learning — Stanford](https://web.stanford.edu/class/cs224n/)
- [ ] [Speech and Language Processing — Jurafsky & Martin](https://web.stanford.edu/~jurafsky/slp3/)
- [ ] [The Illustrated Word2Vec — Jay Alammar](https://jalammar.github.io/illustrated-word2vec/)

---

## The Transformer Architecture

The architecture that powers all modern LLMs. Understanding this deeply is non-negotiable.

- [ ] [Attention Is All You Need](https://arxiv.org/abs/1706.03762)
- [ ] [The Illustrated Transformer — Jay Alammar](https://jalammar.github.io/illustrated-transformer/)
- [ ] [The Annotated Transformer — Harvard NLP](https://nlp.seas.harvard.edu/2018/04/03/attention.html)
- [ ] [Let's build GPT from scratch — Andrej Karpathy](https://www.youtube.com/watch?v=kCc8FmEb1nY)
- [ ] [Positional Encoding in Transformers](https://kazemnejad.com/blog/transformer_architecture_positional_encoding/)
- [ ] [Flash Attention](https://arxiv.org/abs/2205.14135)

---

## Large Language Models

### Pre-training

How LLMs are trained on massive text corpora to predict the next token.

- [ ] [Language Models are Few-Shot Learners (GPT-3)](https://arxiv.org/abs/2005.14165)
- [ ] [BERT: Pre-training of Deep Bidirectional Transformers](https://arxiv.org/abs/1810.04805)
- [ ] [Improving Language Understanding by Generative Pre-Training (GPT-1)](https://openai.com/research/language-unsupervised)
- [ ] [LLaMA: Open and Efficient Foundation Language Models](https://arxiv.org/abs/2302.13971)
- [ ] [Mistral 7B](https://arxiv.org/abs/2310.06825)
- [ ] [The Pile: An 800GB Dataset of Diverse Text](https://arxiv.org/abs/2101.00027)

### Alignment & Fine-tuning

Making a pre-trained model useful, safe, and instruction-following.

- [ ] [Training Language Models to Follow Instructions (InstructGPT)](https://arxiv.org/abs/2203.02155)
- [ ] [Direct Preference Optimization (DPO)](https://arxiv.org/abs/2305.18290)
- [ ] [Constitutional AI: Harmlessness from AI Feedback](https://arxiv.org/abs/2212.08073)
- [ ] [LIMA: Less Is More for Alignment](https://arxiv.org/abs/2305.11206)
- [ ] [RLHF — Lilian Weng](https://lilianweng.github.io/posts/2023-10-25-adv-attack-llm/)

### Efficient Fine-tuning

Full fine-tuning is expensive. These techniques let you adapt large models on consumer hardware.

- [ ] [LoRA: Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2106.09685)
- [ ] [QLoRA: Efficient Finetuning of Quantized LLMs](https://arxiv.org/abs/2305.14314)
- [ ] [Practical Guide to Fine-tuning LLMs — Sebastian Raschka](https://magazine.sebastianraschka.com/p/practical-tips-for-finetuning-llms)
- [ ] [Hugging Face PEFT library](https://github.com/huggingface/peft)

### Scaling Laws

How model capability grows with compute, data, and parameters.

- [ ] [Scaling Laws for Neural Language Models — Kaplan et al.](https://arxiv.org/abs/2001.08361)
- [ ] [Training Compute-Optimal Large Language Models (Chinchilla)](https://arxiv.org/abs/2203.15556)
- [ ] [Emergent Abilities of Large Language Models](https://arxiv.org/abs/2206.07682)

---

## Inference & Deployment

### Quantization & Distillation

Reducing model size and compute cost for production use.

- [ ] [A Gentle Introduction to 8-bit Matrix Multiplication](https://huggingface.co/blog/hf-bitsandbytes-integration)
- [ ] [GPTQ: Accurate Post-Training Quantization](https://arxiv.org/abs/2210.17323)
- [ ] [Knowledge Distillation — Hinton et al.](https://arxiv.org/abs/1503.02531)
- [ ] [llama.cpp](https://github.com/ggerganov/llama.cpp)

### Serving & Optimization

Making LLMs fast and cost-efficient at scale.

- [ ] [vLLM: Efficient Memory Management for LLM Serving](https://arxiv.org/abs/2309.06180)
- [ ] [Continuous Batching — Orca paper](https://www.usenix.org/conference/osdi22/presentation/yu)
- [ ] [Speculative Decoding](https://arxiv.org/abs/2211.17192)
- [ ] [TensorRT-LLM — NVIDIA](https://github.com/NVIDIA/TensorRT-LLM)

---

## Practical LLM Engineering

### Prompt Engineering

Getting the most out of models through careful input design.

- [ ] [Prompt Engineering Guide](https://www.promptingguide.ai/)
- [ ] [Chain-of-Thought Prompting Elicits Reasoning](https://arxiv.org/abs/2201.11903)
- [ ] [Tree of Thoughts](https://arxiv.org/abs/2305.10601)
- [ ] [Self-Consistency Improves Chain of Thought Reasoning](https://arxiv.org/abs/2203.11171)
- [ ] [Anthropic Prompt Library](https://docs.anthropic.com/en/prompt-library/library)

### Retrieval-Augmented Generation

Grounding LLMs with external knowledge to reduce hallucination and extend context.

- [ ] [Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks](https://arxiv.org/abs/2005.11401)
- [ ] [FAISS — Facebook AI Similarity Search](https://github.com/facebookresearch/faiss)
- [ ] [Chunking Strategies for LLM Applications](https://www.pinecone.io/learn/chunking-strategies/)
- [ ] [Advanced RAG Techniques — LlamaIndex](https://docs.llamaindex.ai/en/stable/optimizing/advanced_retrieval/advanced_retrieval/)
- [ ] [Sentence Transformers](https://www.sbert.net/)

### Agents & Tool Use

LLMs that can reason, plan, and take actions.

- [ ] [ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/abs/2210.03629)
- [ ] [Toolformer: Language Models Can Teach Themselves to Use Tools](https://arxiv.org/abs/2302.04761)
- [ ] [AgentBench: Evaluating LLMs as Agents](https://arxiv.org/abs/2308.03688)
- [ ] [Claude's Tool Use Documentation](https://docs.anthropic.com/en/docs/build-with-claude/tool-use)
- [ ] [OpenAI Function Calling](https://platform.openai.com/docs/guides/function-calling)

### Frameworks & Libraries

- [ ] [Hugging Face Transformers](https://github.com/huggingface/transformers)
- [ ] [LangChain](https://github.com/langchain-ai/langchain)
- [ ] [LlamaIndex](https://github.com/run-llama/llama_index)
- [ ] [DSPy — Programming, not prompting](https://github.com/stanfordnlp/dspy)
- [ ] [Instructor — Structured outputs via Pydantic](https://github.com/jxnl/instructor)
- [ ] [Weights & Biases](https://wandb.ai)
- [ ] [Ollama — Run LLMs locally](https://ollama.ai/)

### Evaluation

Measuring what your LLM application actually does.

- [ ] [MMLU: Measuring Massive Multitask Language Understanding](https://arxiv.org/abs/2009.03300)
- [ ] [Holistic Evaluation of Language Models (HELM)](https://crfm.stanford.edu/helm/)
- [ ] [LLM-as-a-Judge](https://arxiv.org/abs/2306.05685)
- [ ] [RAGAS: Evaluation Framework for RAG](https://github.com/explodinggradients/ragas)
- [ ] [Evals — OpenAI](https://github.com/openai/evals)

---

## Safety & Alignment

Building models that are helpful, harmless, and honest.

- [ ] [Constitutional AI: Harmlessness from AI Feedback](https://arxiv.org/abs/2212.08073)
- [ ] [Red Teaming Language Models with Language Models](https://arxiv.org/abs/2202.03286)
- [ ] [Jailbroken: How Does LLM Safety Training Fail?](https://arxiv.org/abs/2307.02483)
- [ ] [Representation Engineering: A Top-Down Approach to AI Transparency](https://arxiv.org/abs/2310.01405)
- [ ] [AI Safety Fundamentals — BlueDot Impact](https://course.aisafetyfundamentals.com/)
- [ ] [Anthropic's Model Specification](https://www.anthropic.com/claude/model-spec)

---

## Multimodal Models

Extending language models to images, audio, and video.

- [ ] [Learning Transferable Visual Models From Natural Language (CLIP)](https://arxiv.org/abs/2103.00020)
- [ ] [Flamingo: a Visual Language Model for Few-Shot Learning](https://arxiv.org/abs/2204.14198)
- [ ] [GPT-4 Technical Report](https://arxiv.org/abs/2303.08774)
- [ ] [LLaVA: Large Language and Vision Assistant](https://arxiv.org/abs/2304.08485)
- [ ] [Whisper: Robust Speech Recognition via Large-Scale Weak Supervision](https://arxiv.org/abs/2212.04356)

---

## LLM Blogs

- [Lilian Weng's Blog](https://lilianweng.github.io/)
- [Jay Alammar's Blog](https://jalammar.github.io/)
- [Sebastian Raschka's Ahead of AI](https://magazine.sebastianraschka.com/)
- [The Gradient](https://thegradient.pub/)
- [Hugging Face Blog](https://huggingface.co/blog)
- [Anthropic Research](https://www.anthropic.com/research)
- [Google DeepMind Research](https://deepmind.google/research/)
- [Eugene Yan's Blog](https://eugeneyan.com/)
- [Simon Willison's Weblog](https://simonwillison.net/)
- [Arxiv Sanity Preserver](https://arxiv-sanity-lite.com/)

---

## Forums and Threads

- [r/LocalLLaMA](https://www.reddit.com/r/LocalLLaMA/)
- [r/MachineLearning](https://www.reddit.com/r/MachineLearning/)
- [Hugging Face Forums](https://discuss.huggingface.co/)
- [LessWrong](https://www.lesswrong.com/)
- [AlignmentForum](https://www.alignmentforum.org/)
- [Papers With Code](https://paperswithcode.com/)

---

## Podcasts

- [Latent Space](https://www.latent.space/podcast)
- [Lex Fridman Podcast](https://lexfridman.com/podcast/)
- [The TWIML AI Podcast](https://twimlai.com/)
- [Gradient Dissent — W&B](https://wandb.ai/fully-connected/gradient-dissent)
- [No Priors](https://www.sequoiacap.com/podcast/no-priors/)
- [Practical AI](https://practicalai.fm/)

---

## Additional Curated Lists

- [Awesome LLM](https://github.com/Hannibal046/Awesome-LLM)
- [Awesome LLM Apps](https://github.com/Shubhamsaboo/awesome-llm-apps)
- [LLM Course — Maxime Labonne](https://github.com/mlabonne/llm-course)

---

## Getting a Job

- [How to Get a Job in AI/ML — Eugene Yan](https://eugeneyan.com/writing/how-to-get-a-job-in-ai-ml/)
- [ML Engineer Roadmap](https://github.com/chris-chris/ml-engineer-roadmap)

## Job Boards

- [AI Jobs — Hugging Face](https://huggingface.co/jobs)
- [Anthropic Careers](https://www.anthropic.com/careers)
- [OpenAI Careers](https://openai.com/careers)
- [Work at a Startup (YC)](https://www.workatastartup.com/)
- [Levels.fyi AI/ML Jobs](https://www.levels.fyi/jobs?jobType=AI_ML_DATA_SCIENCE)
- [LinkedIn — "LLM Engineer"](https://www.linkedin.com/jobs/search/?keywords=LLM%20engineer)
- [AIJobs.net](https://aijobs.net/)

---

*Pull requests welcome. If you have a resource that genuinely improved your understanding of LLMs, open a PR.*
