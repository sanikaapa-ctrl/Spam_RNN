# Spam Detection Using Recurrent Neural Network (RNN)

## Project Overview
This project focuses on detecting whether a text message is Spam or Ham (Normal Message) using a Recurrent Neural Network (RNN). The model analyzes message text and classifies it into two categories: Spam and Ham.

## Technologies Used
- Python
- Google Colab
- TensorFlow / Keras
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## Dataset
The project uses the SMS Spam Collection dataset (`spam.csv`), which contains two main columns:
- `v1`: Message category (Ham or Spam)
- `v2`: SMS message text

## Data Preprocessing
- Removed missing values.
- Checked duplicate records and empty messages.
- Converted labels into numerical values:
  - Ham = 0
  - Spam = 1
- Applied Tokenization to convert text into sequences.
- Used Padding to make all sequences the same length (50).

## Model Architecture
The RNN model consists of:
- Embedding Layer (16 dimensions)
- SimpleRNN Layer (16 units, tanh activation)
- Dense Layer (1 neuron, sigmoid activation)

## Model Compilation
- Loss Function: Binary Crossentropy
- Optimizer: SGD
- Evaluation Metric: Accuracy

## Model Training
- Train-Test Split: 80% Training and 20% Testing
- Epochs: 30
- Batch Size: 32

## Prediction
The trained model predicts whether a given SMS message is Spam or Ham using a 0.5 threshold.

## Project Objective
The main objective is to develop a text classification model that can automatically identify unwanted spam messages and distinguish them from normal messages.

## Conclusion
This project demonstrates how Recurrent Neural Networks (RNN) can be used for Natural Language Processing (NLP) and text classification tasks. It helps understand text preprocessing, tokenization, sequence padding, model training, and prediction using deep learning.
