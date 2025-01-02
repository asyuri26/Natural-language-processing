# Sentiment Analysis with IMDB Dataset

This project demonstrates a sentiment analysis system using the IMDB dataset for binary classification (positive or negative sentiment). The model is built using Bidirectional LSTMs implemented in Keras.

## Dataset
The dataset used is the IMDB reviews dataset, containing labeled movie reviews.

**Download Link:** [IMDB Dataset](https://drive.google.com/file/d/1bPM_v2Q6tuwJSGCkrQGIfpZMWVykko3L/view?usp=sharing)

## Code Description
The pipeline consists of the following steps:

1. **Data Loading and Preprocessing:**
   - Load the dataset.
   - Remove null values and clean the text data (e.g., remove HTML tags and special characters).
   - Convert sentiment labels to numeric values (0 for negative, 1 for positive).

2. **Text Tokenization and Padding:**
   - Tokenize the text into sequences.
   - Pad sequences to ensure uniform input size for the model.

3. **Model Building:**
   - The model architecture includes:
     - Embedding Layer
     - Bidirectional LSTMs with dropout for regularization
     - Dense layers with L2 regularization

4. **Model Training:**
   - Train the model using `binary_crossentropy` as the loss function.
   - Use `EarlyStopping` to prevent overfitting.

5. **Evaluation:**
   - Evaluate the model on test data and plot accuracy/loss graphs.

## Results
After training the model, the performance metrics (accuracy and loss) on the test data are displayed. Additionally, graphs are generated to visualize training and validation accuracy/loss.

## Visualization
Two plots are generated during training:
1. **Accuracy over epochs:**
   - Displays the model's training and validation accuracy.
2. **Loss over epochs:**
   - Displays the model's training and validation loss.

