# Neural Network and Deep Learning Assignment (CS5720)

## Overview

This repository contains implementations of four key tasks in Neural Network and Deep Learning for the course CS5720. The tasks include:

1. **Basic Autoencoder**
2. **Denoising Autoencoder**
3. **RNN for Text Generation**
4. **RNN for Sentiment Classification**

---

## Task 1: Basic Autoencoder

### Objective

Build a simple autoencoder using fully connected (Dense) layers to reconstruct the MNIST dataset images.

### Model Architecture

- Encoder: Input layer (784), Hidden layer (32)
- Decoder: Hidden layer (32), Output layer (784)
- Loss Function: Binary Cross-Entropy
- Optimizer: Adam

### Results

Visual comparison between original and reconstructed images showed good reconstruction quality. Latent dimension size experiments (16, 32, 64) were conducted.

---

## Task 2: Denoising Autoencoder

### Objective

Train a denoising autoencoder to remove Gaussian noise from the MNIST dataset images.

### Model Architecture

- Encoder: Input layer (784), Hidden layer (32)
- Decoder: Hidden layer (32), Output layer (784)
- Loss Function: Binary Cross-Entropy
- Optimizer: Adam

### Results

The model effectively removed noise from the images, preserving essential features. This technique is useful in **medical imaging** to enhance low-quality scans.

---

## Task 3: RNN for Text Generation

### Objective

Train an LSTM-based Recurrent Neural Network to generate text from a corpus of Shakespeare's Sonnets.

### Model Architecture

- Embedding Layer: 256 units
- LSTM Layer 1: 512 units
- LSTM Layer 2: 512 units
- Dense Output Layer with Softmax Activation
- Loss Function: Sparse Categorical Cross-Entropy
- Optimizer: Adam

### Results

Generated text was mostly random due to insufficient training. Increasing training epochs improves coherence.

---

## Task 4: Sentiment Classification Using RNN

### Objective

Train an LSTM-based Recurrent Neural Network to classify movie reviews from the IMDB dataset as Positive or Negative.

### Model Architecture

- Embedding Layer: 128 units
- LSTM Layer 1: 128 units
- LSTM Layer 2: 128 units
- Dense Output Layer with Sigmoid Activation
- Loss Function: Binary Cross-Entropy
- Optimizer: Adam

### Results

- Test Accuracy: **83.61%**
- Classification Report and Confusion Matrix generated to evaluate performance.

### Precision-Recall Tradeoff

The model performs well but can be tuned further by adjusting the decision threshold or enhancing architecture.

---

## Submission

- Ensure all code files are pushed to this repository.
- Include a short demonstration video explaining the code and its functionality.

---

## Author

- **Student Name:** Akash Pegada
- **Course:** CS5720 Neural Network and Deep Learning
- **University:** University of Central Missouri


