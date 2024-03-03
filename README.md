# BERT
# Difference between pretraining and finetuning 

In pretraining, model is trained on a lage dataset can take a significant amount of time and computational resources, often requiring specialized hardware like GPUs or TPUs. Fine-tuning involves taking a pretrained model and further training it on a smaller, task-specific dataset with labeled examples. The goal is to adapt the pretrained model's knowledge to the specific task at hand, such as text classification, named entity recognition, or machine translation.

In summary, pretraining involves training a model on a large dataset(wikipedia data) without task-specific labels to learn general-purpose representations, while fine-tuning involves further training the pretrained model on a smaller task-specific dataset with labeled examples to adapt its knowledge to a specific task. Fine-tuning leverages the knowledge captured during pretraining and tailors it to the specific requirements of the target task, resulting in improved performance on the task at hand.
# Pretraining BERT Model
BERT is pretrained on two different tasks: NSP(Next seq prediction) and MLM(Masked Language Modelling).
Dataset prep in NSP. My name is sayanteka. I am working as data scientist. 2nd sentence follows first sentence.
Therefore, it is lablelled as yes. On the other hand, My name is sayanteka. Sun rises in east. 2nd sentence doesn't follow 1st sentence. It will be labelled as No.
