# Efficient Streaming Language Models w/ Attention Sinks

***

## Abstract

- The paper addresses the challenges of deploying Large Language Models (LLMs) in streaming applications with long interactions.
- Two main issues: high memory consumption due to caching Key and Value states (KVs) and inability to generalize to texts longer than training sequences.
- Window attention, which only caches the most recent KVs, fails when text length exceeds cache size.
- Introduces the concept of "attention sink," where attention scores are unusually high for initial tokens, even if they aren't semantically important.
- Presents StreamingLLM, an efficient framework that allows LLMs to work with infinitely long sequences without needing fine-tuning.
- Demonstrates that StreamingLLM can make multiple well-known LLMs work efficiently with up to 4 million tokens.
- Finds that adding a placeholder token (for the attention sinks) during pre-training can further improve streaming performance.
- Claims that StreamingLLM outperforms the sliding window recomputation baseline by up to 22.2x in speed. 
- Provides code and datasets for further research.

***

## Comparison to Different Methods

![streamllm1](https://github.com/afurkank/nlp-paper-notes/assets/62884181/64727361-6bae-40d0-be87-6e9ab200d61b)

***

## Visualization of Attention Sinks

![streamllm2](https://github.com/afurkank/nlp-paper-notes/assets/62884181/62bfac38-c554-4944-91c2-4b930ff541b5)

***

Paper link: https://arxiv.org/abs/2309.17453
