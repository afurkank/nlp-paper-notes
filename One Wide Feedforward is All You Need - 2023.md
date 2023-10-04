# One Wide Feedforward is All You Need

***

## Abstract

- The paper investigates the role of the Feed Forward Network (FFN) in the Transformer architecture.
- Despite being a significant part of the model's complexity, the FFN is found to be highly redundant.
- Removing the FFN from the decoder layers and using a single shared FFN for the encoder leads to a minor loss in accuracy but a significant reduction in complexity.
- When the simplified model is scaled back to its original size by enlarging the hidden dimension of the shared FFN, it outperforms the original Transformer Big model in terms of accuracy and speed.

***

## Findings

### Nomenclature

![4](https://github.com/afurkank/nlp-paper-notes/assets/62884181/b616ca39-7949-42f9-a50d-cf4bb20d7073)


### Sharing FFNs

![sharing ffns](https://github.com/afurkank/nlp-paper-notes/assets/62884181/789f8122-04da-4139-ac75-2abd2c2acd49)


### Dropping FFNs

![1](https://github.com/afurkank/nlp-paper-notes/assets/62884181/ee8be3e2-2e97-47a3-b721-5722e2eb4c6d)


### One Wide FFN Model

![2](https://github.com/afurkank/nlp-paper-notes/assets/62884181/4316f35d-855a-45c8-916c-b507de4eeb45)


### Results for Different Architectures and Languages

![3](https://github.com/afurkank/nlp-paper-notes/assets/62884181/831fdb8c-4006-4fa8-b0b6-83d24d3d9f2c)

***

Paper link: https://arxiv.org/abs/2309.01826
