# Think before you speak: Training Language Models with Pause Tokens
***
## Abstract

- The paper explores the idea of allowing a language model to manipulate more hidden vectors before generating each token in a sequence.
- This is achieved by introducing a "pause token" that is appended to the input prefix, and the model delays generating the next token until it encounters the last pause token.
- The approach is referred to as "pause-training," and it is applied to decoder-only language models with varying numbers of parameters (1B and 130M) that were pre-trained on C4 data.
- Empirical evaluations of pause-training are conducted on various downstream tasks, including reasoning, question-answering, general understanding, and fact recall.
- The main finding is that introducing inference-time delays during both pre-training and fine-tuning improves performance on several tasks. Notably, there is an 18% gain in EM score on the SQuAD QA task, an 8% improvement on CommonSenseQA, and a 1% accuracy increase on the GSM8k reasoning task for the 1B model.
- The paper suggests that this approach opens up new possibilities and raises questions for future research regarding delayed next-token prediction as a novel paradigm in language modeling.

***

## How it's Applied

![think1](https://github.com/afurkank/nlp-paper-notes/assets/62884181/2968e09b-7dea-4a88-ae96-f970e5102705)

![think2](https://github.com/afurkank/nlp-paper-notes/assets/62884181/04ed6bad-650c-4bd4-9831-638a46f66ec4)
***
## Results

![think3](https://github.com/afurkank/nlp-paper-notes/assets/62884181/10f68434-c131-4054-badd-9dd10e6ba6eb)
***

Paper: https://arxiv.org/abs/2310.02226
