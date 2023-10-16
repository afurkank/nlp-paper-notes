# Small-scale proxies for large-scale Transformer training instabilities

***

## Abstract

- The paper addresses training instabilities observed when training large Transformer-based models at scale.
- These instabilities are challenging to investigate due to the high resource requirements for reproducing them.
- The study aims to reproduce and study training stability and instability at smaller scales.
- It focuses on two sources of training instability mentioned in previous work: the growth of logits in attention layers and the divergence of output logits from log probabilities.
- By analyzing the relationship between learning rate and loss across different scales, the paper demonstrates that these instabilities also occur in small models when trained with high learning rates.
- Mitigations that were effective at large scales are found to work equally well in addressing these instabilities at smaller scales.
- The research explores various optimizer and model interventions, including warm-up, weight decay, and the μParam, to assess their impact on the sensitivity of the final loss to changes in the learning rate.
- By combining techniques, the study achieves training of small models with similar losses across a wide range of learning rate values.
- The paper also investigates cases where instabilities can be predicted by examining the scaling behavior of model activation and gradient norms before they emerge.

***

## Results

![training1](https://github.com/afurkank/nlp-paper-notes/assets/62884181/d20b8650-c978-449f-bb9d-32bd5a9415c2)

![training2](https://github.com/afurkank/nlp-paper-notes/assets/62884181/a7127d46-3626-4254-b139-367401b527dd)

![training3](https://github.com/afurkank/nlp-paper-notes/assets/62884181/64b8f5b2-609a-4e10-be52-51db672192f4)

![training4](https://github.com/afurkank/nlp-paper-notes/assets/62884181/d098618f-cead-44c2-83ed-2078040b4980)

![training5](https://github.com/afurkank/nlp-paper-notes/assets/62884181/f376cf9e-38b5-4f6c-8ae8-2abb728b0849)

***

Paper link: https://arxiv.org/abs/2309.14322
