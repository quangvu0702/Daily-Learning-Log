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

## Sep 10, 2024: [No Priors Ep. 80 | With Andrej Karpathy from OpenAI and Tesla](https://www.youtube.com/watch?v=hM_h0UA7upI&t=207s)

- 

