# The Geometry of Truth: Emergent Linear Structure in LLM Representations of True-False Datasets

***

## Abstract

- The paper discusses the issue of large language models (LLMs) generating false information.
- Recent research has explored methods to determine if an LLM is telling the truth by training probes on the model's internal activations.
- This line of research has faced controversy due to concerns about the probes' failures to generalize and other conceptual issues.
- The paper presents curated datasets of true and false statements to investigate the structure of LLM representations of truth.
- The study provides evidence through three approaches:
  1. Visualizations of LLM representations of true and false statements, revealing a clear linear structure.
  2. Transfer experiments where probes trained on one dataset generalize to different datasets.
  3. Causal evidence obtained by intervening in an LLM's forward pass, making it treat false statements as true and vice versa.
- The findings suggest that language models linearly represent the truth or falsehood of factual statements.
- The paper introduces a novel technique called "mass-mean probing," which offers better generalization and has a stronger causal connection to model outputs compared to other probing techniques.

***

## Visualizations

![truth1](https://github.com/afurkank/nlp-paper-notes/assets/62884181/377836f4-094c-4785-833f-122c3a2cfcb2)

![truth2](https://github.com/afurkank/nlp-paper-notes/assets/62884181/a6910fa8-5934-4305-8e21-d513f94acf66)

![truth3](https://github.com/afurkank/nlp-paper-notes/assets/62884181/103d38aa-59d5-4ccc-aa98-ab2174ee8072)

***

Paper link: https://arxiv.org/abs/2310.06824
