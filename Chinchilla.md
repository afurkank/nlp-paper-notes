# Abstract

- The paper explores the best combination of model size and training data size for transformer language models within a fixed compute budget.
- The study finds that current large language models are not trained to their full potential due to the trend of scaling up model size without increasing the amount of training data.
- Extensive experiments were conducted using various sizes of models and training datasets. 
- The authors propose that for optimal training, the size of the model and the size of the training dataset should be scaled up equally.
- A new model named Chinchilla is introduced, which is trained following this optimal scaling hypothesis. It performs better than other well-known large models on various evaluation tasks while using the same compute budget.
- Chinchilla is also more efficient for fine-tuning and inference, making it easier to use for downstream applications.
- The model sets a new benchmark in accuracy on the MMLU benchmark, outperforming its closest competitor, Gopher, by a significant margin.

***

## 3.4. Optimal Model Scaling

- The paper discusses three different methodologies to predict the optimal scaling of model size and training data within a fixed computational budget.
- All three approaches agree that as the computational budget goes up, both the model size and the amount of training data should increase in roughly equal proportions.
- Among the methods, slight differences in predicting optimal model sizes exist. The third method predicts even smaller models as ideal when computational budgets are larger.
- The paper also provides estimates on the amount of computational resources (FLOPs) and training data (tokens) needed for training models of various sizes optimally.
- According to these estimates, most current large language models are "over-sized" relative to their computational budgets. For example, a model with 175 billion parameters ideally needs far more computational power and training data than what's generally used.
- The findings underscore the need for not just engineering improvements to scale models but also a focus on dataset collection.
- Overall, the paper suggests that smaller models could achieve better performance if trained on more tokens, given the compute resources currently available to most large language models.

***

## Chinchilla Tokens and FLOPs Scaling

Table A3 from the paper:

![chinchilla2](https://github.com/afurkank/paper-notes/assets/62884181/b1580b74-ccb1-4ab8-ba9b-0fda23c7dc7a)

***

## Chinchilla Parameter Scaling

Table A9 from the paper:

![chinchilla](https://github.com/afurkank/paper-notes/assets/62884181/197465ae-78dd-4bb6-9b28-db5d5c1da68d)

***

Paper link: https://arxiv.org/pdf/2203.15556.pdf
