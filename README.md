# code_gen_with_LoRA_finetuning

A research project to finetune the Llama 2 7B large language model (LLM) and improve its coding ability, specifically Python code in algorithm and data structure related programs.
LLMs have revolutionary productivity in modern workflows, particularly in code generation. However, a lot of more widely used open-source models still focus on traditional
tasks. They do little training and optimization for code generation tasks. Llama 2 underperforms on code generation, as indicated by the Human-Eval pass@k code benchmark below (only 12.8% acceptance rate at 1st code generation and 45.6% acceptance rate after 100 instances). The Human-Eval pass@k metric [link][https://www.github.com/openai/human-eval] is an improved way of evaluating code correctness from the traditional match-based methods. The project uses finetuning on the LLM instead of training a completely new machine learning model to take advantage of its reduced requirement on memory and time, while achieving similar performance with less finetuning dataset. 


Tools used: 
1. Parameter-Efficient Fine-Tuning (PEFT): Low-Rank Adaptation(LoRA) technique
2. AlphaCode and Evol-Instruct-Code-80k-v1 to obtain and generate the dataset
3. Python programming language and packages including torch, transformers, peft, and accelerate 
