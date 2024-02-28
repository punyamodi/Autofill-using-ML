# Autofill-using-ML Text Generation Project

This project implements a text generation model using LSTM neural networks in TensorFlow.

## Overview

The model is trained on a dataset of frequently asked questions to generate relevant follow-up questions or sentences. It builds vocabulary and learns sequences from the training data.

During inference, the user can input a starting phrase and the model will predict the next word in the sequence. This allows interactively expanding the generated text.

## Model Architecture

The model architecture consists of:

- Embedding layer 
- 2 LSTM layers
- Fully connected output layer with softmax activation

It is trained with categorical cross-entropy loss and adam optimizer.

## Usage

The input phrases need to be tokenized and padded to match the training sequence length before passing to the model.

Sample interaction:

```
User: what
Model: what is 
User: how 
Model: how will
```

## Data

The model was trained on a small dataset of FAQ sentences. More diverse and larger dataset would improve model performance.

## Future Work

- Experiment with model hyperparameters like layer sizes, regularization etc.
- Use a larger and more diverse dataset
- Support loading/saving models to avoid re-training each time

