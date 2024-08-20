### gemma_codeWriter_finetune
Fine-tunes GEMMA-2B using Hugging Face Transformers and BitsAndBytes for optimized code generation tasks.



This repository hosts a jupyternb that fine-tunes the GEMMA-2B model from Google using Hugging Face's Transformers library and BitsAndBytes for efficient 4-bit quantization. The script employs Parameter-efficient Fine-Tuning (PEFT) with LoRA (Low-Rank Adaptation) to minimize the number of trainable parameters, targeting only specific layers for updates while keeping others frozen. It uses a dataset specifically designed for code generation tasks, TokenBender/code_instructions_122k_alpaca_style, to train the model. After training, the model undergoes further optimization for efficient memory and processing use, and is then saved and pushed to Hugging Face's Model Hub for accessibility.
