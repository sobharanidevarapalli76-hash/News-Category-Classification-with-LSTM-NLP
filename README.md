# News Category Classification Using LSTM

## Project Overview
This project implements a Natural Language Processing (NLP) model using Long Short-Term Memory (LSTM) networks to classify news articles into different categories.

The model predicts the category of a news article based on its title and description.

## Categories
- World
- Sports
- Business
- Science/Technology

## Objective
Build a multiclass text classification system that automatically identifies the category of a news article from textual content.

## Dataset
Dataset: AG News Dataset

Features:
- Title
- Description

Target:
- News Category

## Project Workflow

### 1. Data Loading
- Load training and testing datasets.
- Inspect data structure and classes.
 ![News Category Classification](Screenshot 2026-06-23 173659.png)

 
### 2. Text Preprocessing
- Combine Title and Description.
- Clean and prepare text data.
- Convert labels into numerical format.

### 3. Exploratory Data Analysis
- Analyze document length distribution.
- Visualize dataset characteristics.

### 4. Baseline Model
A baseline model is built using:
- TF-IDF Vectorization
- Logistic Regression

Evaluation Metric:
- Accuracy
- Precision
- Recall
- F1 Score

### 5. LSTM Model
Deep Learning model built using:
- Embedding Layer
- LSTM Layer
- Dropout Layer
- Dense Layers
- Softmax Output Layer

### 6. Model Training
- Tokenization
- Sequence Padding
- Training with validation data
- Performance monitoring

### 7. Evaluation
Metrics used:
- Accuracy
- Classification Report
- Macro F1 Score

### 8. Visualization
- Document Length Distribution
- Training Accuracy Curve
- Validation Accuracy Curve
- Training Loss Curve
- Validation Loss Curve

## Project Screenshot

![News Category Classification](images.jpg)

## Technologies Used

- Python
- NumPy      
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn
- TensorFlow / Keras

## Project Structure

```
AG_News_LSTM_Project/
│
├── train.csv
├── test.csv
├── AG_News_LSTM_Project.ipynb
├── README.md
└── requirements.txt
```

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/News-Category-Classification-with-LSTM-NLP.git
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Run the Project

Open the notebook:

```bash
jupyter notebook AG_News_LSTM_Project.ipynb
```

or

```bash
Google Colab
```

## Results

The LSTM model successfully learns textual patterns and classifies news articles into their respective categories with high accuracy.

## Future Improvements

- Bidirectional LSTM
- GRU Networks
- Attention Mechanism
- BERT-based Classification
- Hyperparameter Tuning

## Author

Sobharani Devarapalli

## License

This project is created for educational and academic purposes.
