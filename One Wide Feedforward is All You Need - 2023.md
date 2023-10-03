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

![nomenclature](https://github.com/afurkank/paper-notes/assets/62884181/bfc2a3cd-7fee-4ca4-bd20-1f3d01ae7957)

### Sharing FFNs

![sharing ffns](https://github.com/afurkank/paper-notes/assets/62884181/b316425d-814f-4f2e-b548-ac4eaab884b1)

### Dropping FFNs

![1](https://github.com/afurkank/paper-notes/assets/62884181/e2d6f621-c040-4e4d-aaeb-eaa97d957427)

### One Wide FFN Model

![2](https://github.com/afurkank/paper-notes/assets/62884181/b7f3c206-48e1-43ec-86d7-6af2cf109abd)

### Results for Different Architectures and Languages

![3](https://github.com/afurkank/paper-notes/assets/62884181/9f979a8e-f5ad-48f3-aa5d-3bdcd9b97eb9)

***

Paper link: https://arxiv.org/abs/2309.01826
