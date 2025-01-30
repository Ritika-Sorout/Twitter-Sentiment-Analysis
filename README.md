# Twitter-Sentiment-Analysis
# Sentiment Analysis Using Recurrent Neural Network

## Overview
This project implements a Recurrent Neural Network (RNN) to analyze and classify text comments as either negative or non-negative (positive/neutral). The model is trained using a dataset containing various comments with sentiment labels.

## Features
- Preprocesses text data using tokenization and padding.
- Implements an LSTM-based RNN for sentiment classification.
- Saves and loads the trained model for inference.
- Works with general comments, not limited to any specific domain.

## Dataset
The dataset should be a CSV file containing at least two columns:
- `text`: The comment or review text.
- `sentiment`: The sentiment label (`negative`, `positive`, or `neutral`). The model maps `negative` to 1 and all others to 0.

Ensure your dataset is named `comments.csv` and placed in the project directory.

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/sentiment-analysis-rnn.git
   cd sentiment-analysis-rnn
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

## Usage
### Train the Model
Run the script to train the model:
```sh
python train_model.py
```

### Predict Sentiment
Use the trained model to predict sentiment for new comments:
```sh
python predict.py "This is a sample comment."
```

## Model Structure
The model consists of:
- **Embedding Layer**: Converts words into vector representations.
- **LSTM Layer**: Captures sequenti
