# AI Text Detection Project

This project uses BERT to classify text as either AI-generated or human-written.

## Requirements

- Python 3.x
- Required packages:
  ```
  transformers==4.51.3
  pandas
  scikit-learn
  torch
  numpy
  tqdm
  ```

## Setup

1. Install dependencies:
   ```bash
   pip install transformers==4.51.3 pandas scikit-learn torch numpy tqdm
   ```

2. Place your training data in `train_data.csv` with columns:
   - `text`: The text content
   - `label`: Classification label ('meta' or 'haiku')

## Usage

1. Open `AI_Detection.ipynb` in Jupyter Notebook or Google Colab
2. Run cells sequentially to:
   - Load and preprocess data
   - Train BERT model
   - Evaluate model performance
   - Make predictions on new text

## Data Format

The training data should be in CSV format with two columns:
- `text`: The text to classify
- `label`: Binary classification ('meta' or 'haiku')

## Model

The project uses BERT (Bidirectional Encoder Representations from Transformers) for text classification, fine-tuned on the provided dataset. 