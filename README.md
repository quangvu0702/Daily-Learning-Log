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

### [Hands-On LLM Fine-Tuning](https://www.wandb.courses/courses/take/training-fine-tuning-LLMs/lessons/44579742-hands-on-llm-fine-tuning)
- The big picture: 
  - Finetuning data
    - Download data, convert to usable format, mixed and sampled.
    - Data loader for training and evaluation.
  - Finetuning repository and scripts.
    - Load model, load data, training, checkpoint, tracking.
    - Hackable: easy to modify, add features.
    - [TODO]
      - [NeurIPS LLM Efficiency Challenge](https://github.com/llm-efficiency-challenge/neurips_llm_efficiency_challenge)
      - https://colab.research.google.com/github/wandb/edu/blob/main/llm-training-course/colab/finetuning.ipynb 
  - Finetuning model. (llamma3, Falcon, OpenLLaMa, ...)
  - LB eval on Subset of HELM benchmark. * Need to think about the evaluation carefully. *

## Sep 12, 2024:
- [Build a Question/Answering system over SQL data](QA_SQL/README.md) 

## Sep 18, 2024:

### Build a Question/Answering system over SQL data:
- add 20 popular examples.

### Build a Bond with Your Children
- Spend 20 minutes a day with them.
- Engage in an activity together.
- Avoid comments, questions, or giving directions.
- Instead of telling your children they're smart, encourage them to work hard and embrace challenges. It teaches them that effort and perseverance are the keys to growth.

### [LLM Evaluation](https://www.wandb.courses/courses/take/training-fine-tuning-LLMs/lessons/44579578-introduction-to-llm-evaluation)
Here’s an improved version of your chat for clarity, structure, and better readability:

---

### [LLM Evaluation Overview](https://www.wandb.courses/courses/take/training-fine-tuning-LLMs/lessons/44579578-introduction-to-llm-evaluation)

#### Key Evaluation Techniques:
1. **HumanEval**:
   - Uses **unit tests** rather than traditional n-grams for evaluating code generation.

2. **OpenLLM Benchmarks**:
   - **Arc**: Focuses on multiple-choice questions with reasoning components.
   - **HellaSwag**: Evaluates the ability to correctly complete sentences.
   - **MMLU**: is a benchmark designed to evaluate the multitask accuracy of language models across a wide variety of subjects
   - **TruthfulQA**: Aims to test models on question-answering tasks, ensuring they do not generate false or misleading responses.

3. **Evaluation Tools**:
   - **Eleuther Eval Harness**: A toolkit for standardized LLM evaluation across different tasks and benchmarks.

4. **HELM**:
   - focus on English
   - provides a comprehensive, multidimensional evaluation of LLMs, helping researchers and developers understand not just how good a model is at a specific task, but also how safe, fair, and reliable it is across different use cases

5. **MosaicML**
   - lower price.

6. **Chatbot Arena**
   - Elo ratings
   - MT-Bench and LLM-as-a-judge
   - Model bias

7. **Specific Use Cases**
   - These benchmarks are designed by domain experts and are focused on specific niche domains. For example LegalBench, which evaluates models on different legal reasoning tasks. 

8. [**LLM Apps**](https://www.wandb.courses/courses/building-llm-powered-apps)
   - Vibes check: curated, Human
   - Model-based Eval: curated, & generated, LLM
   - Unit testing: curated, & generated, LLM
   - A/B testing: production, User

## Sep 20, 2024:

### [The Key Equation Behind Probability](https://www.youtube.com/watch?v=KHVR587oW8I):
   - Define entropy based on surprise and probability.
      - The less probable an event is, the higher its surprisal.
      - When p(x) approaches 1, the surprisal h(x) approaches 0.
      - When probabilities are multiplied, surprisal is additive (e.g., guessing the right dice outcome 3 times results in 3 times the surprisal).
      => using log: h(x) = log(1/p(x)): surprise is high for rare events.
      - entropy = expected value of surprise
      - cross entropy(P, Q) = expected surprise of practical event P based on belief Q.
      - Kullback–Leibler (KL) divergence = cross entropy(P, Q) - entropy(P): the distance between 2 distributions
      
## Sep 24, 2024:

### [Understanding note-taking | Zettelkasten](https://www.youtube.com/watch?v=-r6fnC5lVfE):
   - Main idea: Create idea -> id, Create connections ids -> ids
   - Emergent: bottom-up: from note -> connections -> clusters -> structures
   - Dynamic: structure change by adding every note and connections.
   - Personalized: the way people create create noted and connnections are unique. unique way of thinking.
   - Inter-thinking: create connection between new ideas with older ideas, put them into giant network. The number of connection growth exponentialy.
   - Clarity: Convert idea into paper, write it down in your own words.
   - Invest in the future: process of writing and aggregate knowleadge.

### [How to choose a note-taking app | Zettelkasten | Notion vs Roam vs Obsidian](https://www.youtube.com/watch?v=4MxI68kg8to)
   - Apply Zettelkasten in the daily live.
   - Mindset: try the ideas with any tools. Prevent perfectioness.
   - Notion, ROAM, Remnote: not suitable for Zettelkasten
   - Obsidian: free and local.


## TODO
### [Neural and Non-Neural AI, Reasoning, Transformers, and LSTMs](https://www.youtube.com/watch?v=DP454c1K_vQ&t=68s)