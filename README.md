# Project Title

## Problem Statement
Aimed to fine-tune the Llama-2-7b model on a specific dataset to create a chatbot. The goal is to leverage the PEFT library from Hugging Face and QLoRA for efficient fine-tuning.

## Results Interpretation
The fine-tuned model successfully generates responses based on the provided dataset. The results show improved performance in generating contextually relevant and accurate responses.

## Methodology
1. Setup: Install the required libraries including accelerate, peft, transformers, datasets, and TRL
2. Dataset Loading: Load the dataset from Hugging Face Hub
3. Data Preparation: Process the dataset to create a text field combining the prompt and output
4. Model Loading: Load the Llama-2-7b model and configure it for 4-bit quantization
5. Fine-Tuning: Use the SFTTrainer from TRL to fine-tune the model on the dataset
6. Evaluation: Evaluate the model's performance and save the fine-tuned model

## Steps Done
1. Install Libraries: Installed necessary libraries using pip
2. Load Dataset: Loaded the dataset using load_dataset from Hugging Face
3. Prepare Data: Mapped the dataset to create a combined text field
4. Load Model: Loaded the Llama-2-7b model and configured it for 4-bit quantization
5. Fine-Tune Model: Used SFTTrainer to fine-tune the model on the dataset
6. Save Model: Saved the fine-tuned model and pushed it to Hugging Face Hub

## Dataset
The dataset used for this project is nisaar/Articles_Constitution_3300_Instruction_Set from Hugging Face. It contains 3311 rows with features like instruction, input, output, and prompt. The dataset is used to train the model to generate responses based on legal case summaries and instructions.
