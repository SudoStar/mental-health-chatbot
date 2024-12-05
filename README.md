# Mental Health Chatbot

This repository contains the Jupyter notebooks for the Mental Health Chatbot project. The code is split into two files:

* **Seq2seq_MentalHealthDataset.ipynb**: this is the first part of the project and demonstrates the development of two simple encoder/decoder models highlighting the issues these models face when the number of training samples is highly limited
* **TinyLlama_PEFT_LoRA_MentalHealthDataset.ipynb**: by building on a foundation model, good results can be achieved although the number of samples is still highly limited

## README for Seq2seq_MentalHealthDataset.ipynb

### Overview

This notebook demonstrates the development of two encoder/decoder models based on the seq2seq architecture. The models are fundumantelly constrained by a very small sample size. Nonetheless, it is interesting to investigate the creation of such models and analyse their performance in view of the mentioned limitation.

### Key Features

    Model architecture: The first model is a seq2seq encoder/decoder model utilizing LSTM, while the second model is a seq2seq encoder/decoder model with an attention mechanism utilizing GRU.
    Mental health dataset: Focused on applications in mental health, containing 97 questions and answers.

### Requirements

The notebook was tested on the HSLU's JupyterHub environment. Simply executing one field after the other should work. After installing the packages from `requirements.txt` a restart of the kernel might be required. Make sure to be in the correct directory when running the notebook. 


## README for TinyLlama_PEFT_LoRA_MentalHealthDataset.ipynb

### Overview

This notebook is designed to demonstrate the application of PEFT (Parameter-Efficient Fine-Tuning) using the LoRA (Low-Rank Adaptation) methodology on a mental health dataset. It showcases how to fine-tune a lightweight language model, TinyLlama, for mental health-related tasks while maintaining efficiency and reducing computational costs.

### Key Features

    Model architecture: Uses the TinyLlama language model, a compact and efficient transformer-based architecture.
    PEFT with LoRA: Demonstrates fine-tuning by freezing most model parameters and adapting select layers for efficient training.
    Mental health dataset: Focused on applications in mental health, containing 97 questions and answers.
    Customizable pipeline: Easily adaptable for other datasets or downstream tasks.

### Requirements

To run the notebook virtually or online, ensure you have the following:

    Kaggle Notebook(Free Version)

To run the notebook locally using Windows with Linux, ensure you have the following:

    WSL2
    VSCode
    Python 3.12 Environment
    Python Virtual Environment
