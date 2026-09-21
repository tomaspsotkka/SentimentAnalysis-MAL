# Sentiment Analysis with Neural Networks

This repository contains a Jupyter Notebook demonstrating sentiment analysis on the IMDb movie review dataset.

The project converts text reviews into numerical representations using a **Bag-of-Words** model and trains a neural network classifier to predict whether each review is positive or negative.

## What the notebook covers

- Splitting the dataset into training, validation, and test sets
- Converting reviews into Bag-of-Words vectors with `CountVectorizer`
- Exploring how individual words and complete reviews are represented
- Training and tuning a one-hidden-layer neural network
- Evaluating the model on unseen test data
- Classifying custom movie reviews

## Results

The final model achieved approximately:

- **Validation accuracy:** 88.6%
- **Test accuracy:** 88.64%

## Requirements

- Python 3
- Jupyter Notebook
- NumPy
- pandas
- scikit-learn

Install the required libraries with:

```bash
pip install numpy pandas scikit-learn jupyter
```

## Dataset

The notebook expects the following files to be in the same directory:

- `reviews.txt`
- `labels.txt`

These files should contain the IMDb reviews and their corresponding sentiment labels.

## Running the notebook

1. Clone or download this repository.
2. Place `reviews.txt` and `labels.txt` in the repository directory.
3. Start Jupyter Notebook:

```bash
jupyter notebook
```

4. Open `5. Neural networks I - Sentiment analysis.ipynb`.
5. Run the notebook cells in order.

## Model

The classifier uses `MLPClassifier` from scikit-learn with:

- One hidden layer containing 150 neurons
- ReLU activation
- Early stopping
- Bag-of-Words input features
