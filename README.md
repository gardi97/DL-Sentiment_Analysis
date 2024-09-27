# Anti-Hate Filter for Social Networks (Sentiment Analysis)

## Introduction

This project focuses on developing a filter to detect and prevent hate speech on social networks. By utilizing natural language processing (NLP) techniques, the model can analyze text data to identify harmful content. The main objective is to create an effective classifier that can flag hate speech while minimizing false positives.

The project employs deep learning techniques, specifically Long Short-Term Memory (LSTM) networks, to classify social network text data. The goal is to improve the safety of online interactions by identifying and filtering hateful content.

## Features

- Text preprocessing using tokenization and padding sequences.
- Utilizes a dataset split for training, validation, and testing purposes.
- Implementation of LSTM networks for text classification.
- Performance evaluation with metrics such as accuracy, precision, recall, and AUC.
- Models comparisons and optimization of the threeshold for each label

## Project Workflow

1. **Text Preprocessing**: The text data undergoes preprocessing, including tokenization, sequence padding, and splitting into training and test sets.
2. **Model Building**: An LSTM model is created using TensorFlow’s Keras API, with options for bidirectional layers and dropout for regularization.
3. **Training**: The model is trained on a labeled dataset of social media posts to detect hate speech.
4. **Evaluation**: The model is evaluated using various metrics to ensure its performance in a real-world scenario.



## Model Overview

- **Text Tokenization**: The text data is tokenized and transformed into sequences, which are then padded to ensure uniform input size.
- **LSTM Network**: A Long Short-Term Memory network is employed to handle sequential text data, learning patterns over time to classify input text.
- **Bidirectional Layers**: The model includes bidirectional layers to improve the understanding of context in both directions of the sequence.
- **Evaluation Metrics**: The model is evaluated using classification reports, accuracy scores, precision-recall curves, and AUC values to ensure reliable performance.

## Configuration

The model's configuration, including hyperparameters such as learning rate, batch size, and the number of LSTM units, can be customized in the notebook. Additionally, options for handling class imbalances through techniques such as class weights are included.

## Conclusion
Five models were trained and evaluated using different metrics; the threesholds which maximize the F1-score were identified for each label of every models.
The selected model includes two LSTM bi-dirictional layers and it shows good performances on the most represented labels and disappointed performances on the leas represented labels.
Better overall performances could be reached using more complex neural networks and oversampling in order to obtain a more balanced dataset.




## Contributors
[Francesco Gardini](https://github.com/gardi97)
