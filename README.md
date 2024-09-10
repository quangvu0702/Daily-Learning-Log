# Daily-Learning-Log

## Sep 9, 2024: Soft Prompting vs LoRA

### Soft Prompting:

- How it works: Soft prompting modifies the input by adding a learned prefix to guide the model's behavior. The model isn't retrained from scratch but is influenced by the added prompt.
- Training: It usually doesn't involve retraining the entire model. Instead, you adjust how the input is processed, making it efficient in terms of time and resources.
- Use cases: It's often used for tasks where you want to influence model behavior without fine-tuning the model itself. It’s popular in natural language processing (NLP) tasks like text classification and language generation.

### LoRA (Low-Rank Adaptation):

- How it works: LoRa adjusts the internal weights of a model by learning low-rank matrix updates. These updates are added to the model's parameters, allowing it to adapt to new tasks without changing the entire model.
- Training: LoRa focuses on fine-tuning specific layers (like attention layers in transformers) and is more computationally efficient than traditional full fine-tuning.
- Use cases: It's effective when you need to adapt a model to new tasks while keeping memory and computational costs low. It's commonly used in NLP and other machine learning fields where models need to be adapted efficiently.

### Summary:

- Soft Prompting: Modifies input, efficient, NLP tasks
- LoRA: Adjusts weights, fine-tunes specific layers, efficient, various tasks

## Sep 10, 2024: 

### [No Priors Ep. 80 | With Andrej Karpathy from OpenAI and Tesla](https://www.youtube.com/watch?v=hM_h0UA7upI&t=207s)

- Hardware problem vs software problem: hardware problem is hard to solve, software problem is easy to solve. 
- Tesla is not a software company, it's an robot company.
- Define what is the bottleneck? Model is not the bottleneck, loss function and data are the bottleneck.
- Training chat-transformer: The data in the internet is not what we want, we need more high quality data: reasoning dataset, how people reason about things. 
- The distribution of chat-transformer is silently collapsing, the distribution of what people want to chat about is not being explored: only few samples output per question.
- What we really need is a cognition core. It will be surprisingly small - 1B parameters is enough. (distill the knowledge)
- AI-chatGPT will empower people. (cheap and powerful)
- Learning supposes to be hard.
- What children should learn: Math, physics, CS.

### [Neural and Non-Neural AI, Reasoning, Transformers, and LSTMs](https://www.youtube.com/watch?v=DP454c1K_vQ&t=68s)