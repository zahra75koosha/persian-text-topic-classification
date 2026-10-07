# Persian Text Topic Classification

A deep learning project for classifying Persian text into eight topic categories using LSTM, GRU, and Bidirectional LSTM neural networks.

## Overview

This project investigates recurrent neural network architectures for Persian text classification.

The models classify Persian text into eight topic categories:

- Social
- Economic
- International
- Political
- Scientific/Technology
- Cultural/Artistic
- Sports
- Medical

The project compares three neural network architectures:

- Long Short-Term Memory (LSTM)
- Gated Recurrent Unit (GRU)
- Bidirectional LSTM (BiLSTM)

## Text Preprocessing

Persian text is preprocessed using the Hazm library. The preprocessing pipeline includes text normalization and tokenization before converting the text into numerical sequences.

The sequences are padded to a fixed length before being passed to the neural networks.

## Models

### LSTM

The LSTM model uses:

- Embedding layer
- LSTM layer
- Global Max Pooling
- Dropout
- Fully connected layer
- Softmax output layer

Test accuracy: **94.76%**

### GRU

The GRU model uses:

- Embedding layer
- GRU layer
- Global Max Pooling
- Dropout
- Fully connected layer
- Softmax output layer

Test accuracy: **96.65%**

### Bidirectional LSTM

The Bidirectional LSTM model processes the input sequence in both forward and backward directions.

The architecture includes:

- Embedding layer
- Bidirectional LSTM
- Global Max Pooling
- Dropout
- Fully connected layer
- Softmax output layer

Test accuracy: **96.29%**

## Results

| Model | Test Accuracy |
|---|---:|
| LSTM | 94.76% |
| GRU | **96.65%** |
| Bidirectional LSTM | 96.29% |

Among the three models, the GRU architecture achieved the highest test accuracy.

## Technologies

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Hazm
- Natural Language Processing
- Deep Learning

## Project Structure

```text
persian-text-topic-classification/
│
├── lstm_final_persian.ipynb
├── GRU_final_persian.ipynb
├── blstm_final_persian.ipynb
└── README.md
