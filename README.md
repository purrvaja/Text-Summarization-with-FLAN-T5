# Conversation Summarization with FLAN-T5

This project investigates the effectiveness of different techniques to improve the performance of the flan-T5 model, to summarize conversations. 

## Prompt Engineering

* Zero-shot Inference: The model was prompted with an instruction prompt to summarize the conversation without any additional training data. This provides a baseline performance. 

* One-shot Inference: The model is prompted with both an instruction and a single conversation-summary pair as an example. It was observed that the model responses were improved vastly compared to zero-shot inference. 


## Fine Tuning

* Parameter-efficient Fine-tuning: The LoRA (Low Rank Adaptation) method is used to fine-tune the model with reduced parameters. This is a computationaly efficient method compared to performing full fine-tuning on the model.

## Evaluation
* The model was evaluated qualitatively through human evaluation and quantitatively through the ROUGE metric.

