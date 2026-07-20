# Poetry Generation using RNN and LSTM

A Deep Learning project that generates poetry using **Recurrent Neural Networks (RNN)** and **Long Short-Term Memory (LSTM)** networks implemented in **PyTorch**.

---

## Overview

This project explores sequence modeling for Natural Language Processing (NLP) by training neural networks to generate poetry. Two different architectures are implemented and compared:

- Vanilla RNN with One-Hot Encoding
- LSTM with Word Embeddings

The models learn language patterns from a poetry dataset and generate new poems based on a user-provided seed text.

---

## Features

- Text preprocessing and tokenization
- Vocabulary creation
- Sequence generation for next-word prediction
- One-Hot encoded RNN implementation
- Embedding-based LSTM implementation
- Automatic poem generation
- Comparison between RNN and LSTM architectures
- Training loss monitoring

---

## Models Implemented

### One-Hot RNN

- One-Hot encoded input vectors
- Vanilla Recurrent Neural Network
- Fully Connected Output Layer

### Embedding-based LSTM

- Learnable Embedding Layer
- Long Short-Term Memory (LSTM)
- Fully Connected Output Layer

---

## Dataset

The project uses a poetry corpus (`poems-100.csv`) containing English poems.

Dataset preprocessing includes:

- Reading the dataset
- Tokenization
- Vocabulary generation
- Word-to-index mapping
- Index-to-word mapping
- Sequence generation
- Target word creation

---

## Project Workflow

```text
Poetry Dataset
      │
      ▼
Text Preprocessing
      │
      ▼
Tokenization
      │
      ▼
Vocabulary Creation
      │
      ▼
Sequence Generation
      │
      ▼
Model Training
 ┌──────────────┐
 │              │
 ▼              ▼
One-Hot RNN    LSTM
 │              │
 └──────┬───────┘
        ▼
Next Word Prediction
        │
        ▼
Poem Generation
```

---

## Technologies Used

### Programming Language

- Python

### Deep Learning

- PyTorch

### Libraries

- Torch
- NumPy
- CSV
- Matplotlib (optional for visualization)

---

## Model Configuration

| Parameter | Value |
|----------|------:|
| Sequence Length | 10 |
| Embedding Dimension | 100 |
| Hidden Dimension | 128 |
| Optimizer | Adam |
| Loss Function | CrossEntropyLoss |
| Epochs | 100 |

---

## Project Structure

```text
Poem-Generation/
│
├── text_generation.py
├── poems-100.csv
├── generated_poems.txt
├── README.md
└── requirements.txt
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/Dark3302/Poetry-Generation-RNN-LSTM.git

cd Poetry-Generation-RNN-LSTM
```

Install dependencies:

```bash
pip install torch
```

---

## Running the Project

Execute:

```bash
python text_generation.py
```

The program will:

1. Load the poetry dataset
2. Build the vocabulary
3. Train the One-Hot RNN
4. Train the LSTM
5. Compare training performance
6. Generate poems using a seed sentence

---

## Sample Output

**Input Seed**

```text
I look up to
```

**Generated Poem (LSTM)**

```text
I look up to a love
You see in the tongue
I hear the violoncello,
It glides quickly through my ears,
It shakes sweet melodies
Across my heart and soul...
```

---

## Results

- Successfully trained both RNN and LSTM models for poem generation.
- Compared sequence modeling performance between One-Hot RNN and Embedding-based LSTM.
- Observed that the LSTM generated more coherent and context-aware poems than the vanilla RNN.
- Demonstrated the effectiveness of embedding layers in capturing semantic relationships between words.

---

## Future Improvements

- Train on larger poetry datasets
- Implement GRU architecture
- Add Transformer-based text generation
- Improve decoding using Beam Search
- Deploy as a web application

---

## Learning Outcomes

Through this project, the following concepts were explored:

- Natural Language Processing
- Sequence Modeling
- Word Embeddings
- Recurrent Neural Networks
- Long Short-Term Memory Networks
- Language Modeling
- Text Generation using Deep Learning

