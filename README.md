# Neural Network and Deep Learning Assignment (CS5720)

This repository contains implementations for various neural network tasks as part of the CS5720 Neural Network and Deep Learning assignment. The assignment is divided into four questions:

- **Q1: Implementing a Basic Autoencoder**
- **Q2: Implementing a Denoising Autoencoder**
- **Q3: Implementing an RNN for Text Generation**
- **Q4: Implementing an RNN for Sentiment Classification**

## Table of Contents
- [Q1: Basic Autoencoder](#q1-basic-autoencoder)
- [Q2: Denoising Autoencoder](#q2-denoising-autoencoder)
- [Q3: RNN for Text Generation](#q3-rnn-for-text-generation)
- [Q4: Sentiment Classification Using RNN](#q4-sentiment-classification-using-rnn)
- [Installation](#installation)
- [Usage](#usage)
- [Future Improvements](#future-improvements)

## Q1: Basic Autoencoder
### Overview
This task involves building a simple autoencoder using the MNIST dataset to compress and reconstruct images. The model is trained using binary cross-entropy loss.

### Files
- `home_assignment3_q124.py`

### Usage
- Define an autoencoder model using `tf.keras.Sequential`.
- Train the model on MNIST dataset.
- Visualize the reconstruction of images using `matplotlib`.

### Observations
- Compression quality depends on the size of the latent space.
- Higher latent dimension size improves reconstruction but reduces compression efficiency.

---

## Q2: Denoising Autoencoder
### Overview
This task involves building a denoising autoencoder to remove noise from images. Gaussian noise is added to the MNIST dataset before training.

### Files
- `home_assignment3_q124.py`

### Usage
- Build an autoencoder model similar to Q1.
- Train the model on noisy MNIST images.
- Visualize denoising results using `matplotlib`.

### Observations
- The model effectively learns to remove noise and restore the original digit shapes.

---

## Q3: RNN for Text Generation
### Overview
This task involves building an LSTM-based RNN to generate Shakespearean text character-by-character.

### Files
- `home_assignment_q3.py`

### Usage
- Train the model on a text dataset (Shakespeare Sonnets).
- Save model weights using `model.save_weights()`.
- Generate text by loading the model weights and using a text generation function.

### Explanation of Temperature Scaling
- Lower temperature values make the model more predictable and repetitive.
- Higher temperature values make the model produce more creative and random text.

---

## Q4: Sentiment Classification Using RNN
### Overview
This task involves building an LSTM-based model for binary sentiment classification using the IMDB dataset.

### Files
- `home_assignment3_q124.py`

### Usage
- Load and preprocess the IMDB dataset.
- Train an LSTM model for sentiment analysis.
- Generate classification report and confusion matrix.

### Observations
- The model successfully classifies text reviews as positive or negative.

---

## Installation
1. Clone the repository:
```bash
$ git clone <repository-url>
```
2. Install dependencies:
```bash
$ pip install -r requirements.txt
```

---

## Usage
Run the Python files for each question using:
```bash
$ python home_assignment3_q124.py  # For Q1, Q2, and Q4
$ python home_assignment_q3.py      # For Q3
```

---

## Future Improvements
- Improve model accuracy by tuning hyperparameters.
- Add more datasets for generalization.
- Experiment with different architectures (e.g., GRU, Bidirectional LSTM).
- Enhance the text generation model with advanced techniques such as Transformer models.

---

## License
This project is part of the CS5720 Neural Network and Deep Learning course assignment.

---

