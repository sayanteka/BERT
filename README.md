# BERT
# Difference between pretraining and finetuning 

In pretraining, model is trained on a lage dataset can take a significant amount of time and computational resources, often requiring specialized hardware like GPUs or TPUs. Fine-tuning involves taking a pretrained model and further training it on a smaller, task-specific dataset with labeled examples. The goal is to adapt the pretrained model's knowledge to the specific task at hand, such as text classification, named entity recognition, or machine translation.

In summary, pretraining involves training a model on a large dataset(wikipedia data) without task-specific labels to learn general-purpose representations, while fine-tuning involves further training the pretrained model on a smaller task-specific dataset with labeled examples to adapt its knowledge to a specific task. Fine-tuning leverages the knowledge captured during pretraining and tailors it to the specific requirements of the target task, resulting in improved performance on the task at hand.
# Pretraining BERT Model
BERT is pretrained on two different tasks: NSP(Next seq prediction) and MLM(Masked Language Modelling).
Dataset prep in NSP. My name is sayanteka. I am working as data scientist. 2nd sentence follows first sentence.
Therefore, it is  yes when it comes to isnext. On the other hand, My name is sayanteka. Sun rises in east. 2nd sentence doesn't follow 1st sentence. It will be  No when it comes to isnext.

BERT Heads: NSP & MLM

In NSP, Feed forward NN is applied on CLS Token.
In MLM, Feed forward NN applied on Masked Token.


In MLM, random tokens get masked in input sentences. I am [masked] boy. She is at [masked]. I just texted her. Above masking done for 80% of total input seq. 10% below alterations were done. Replace any token with random token from vocab. He is car best friend. instead using word my, car is used. Car love each other. Instead using they  car is used and so on. Rem 10% no alterations. So, in total there are 3 cases in MLM. 


