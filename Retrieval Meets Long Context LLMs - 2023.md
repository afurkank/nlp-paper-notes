# Retrieval Meets Long Context Large Language Models
***
## Abstract

- The paper discusses the popularity of extending the context window of large language models (LLMs).
- It explores the comparison between retrieval-augmentation and long context window extension for LLMs.
- The study uses two pretrained LLMs, the proprietary 43B GPT and LLaMA2-70B, for experimentation.
- Surprisingly, the research finds that a 4K context window LLM with retrieval-augmentation can achieve comparable performance to a finetuned LLM with a 16K context window, while being computationally more efficient.
- Retrieval is shown to significantly enhance the performance of LLMs, regardless of their extended context window sizes.
- The best-performing model in the study is a retrieval-augmented LLaMA2-70B with a 32K context window, outperforming other models in various long context tasks, such as question answering and query-based summarization.
- This retrieval-augmented model also surpasses its non-retrieval baseline while being faster at generation.
- The study offers valuable insights for practitioners on choosing between retrieval-augmentation and long context extension for LLMs.
***
## Results

![ret1](https://github.com/afurkank/nlp-paper-notes/assets/62884181/ba43eaf2-7ab4-4991-8664-881bb648f3e9)

![ret3](https://github.com/afurkank/nlp-paper-notes/assets/62884181/4532739d-abc7-4342-b9e2-62ad658607e9)

![ret2](https://github.com/afurkank/nlp-paper-notes/assets/62884181/413dd052-f958-4bc8-a1a6-21776284afc0)

***

Paper: https://arxiv.org/abs/2310.03025
