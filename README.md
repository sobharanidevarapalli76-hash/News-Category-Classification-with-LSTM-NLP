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
 
  
    

    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }


  
    
      
      Class Index
      Title
      Description
    
  
  
    
      0
      3
      Wall St. Bears Claw Back Into the Black (Reuters)
      Reuters - Short-sellers, Wall Street's dwindli...
    
    
      1
      3
      Carlyle Looks Toward Commercial Aerospace (Reu...
      Reuters - Private investment firm Carlyle Grou...
    
    
      2
      3
      Oil and Economy Cloud Stocks' Outlook (Reuters)
      Reuters - Soaring crude prices plus worries\ab...
    
    
      3
      3
      Iraq Halts Oil Exports from Main Southern Pipe...
      Reuters - Authorities have halted oil export\f...
    
    
      4
      3
      Oil prices soar to all-time record, posing new...
      AFP - Tearaway world oil prices, toppling reco...
    
  


    

  
    

  
    
  
    

  
    .colab-df-container {
      display:flex;
      gap: 12px;
    }

    .colab-df-convert {
      background-color: #E8F0FE;
      border: none;
      border-radius: 50%;
      cursor: pointer;
      display: none;
      fill: #1967D2;
      height: 32px;
      padding: 0 0 0 0;
      width: 32px;
    }

    .colab-df-convert:hover {
      background-color: #E2EBFA;
      box-shadow: 0px 1px 2px rgba(60, 64, 67, 0.3), 0px 1px 3px 1px rgba(60, 64, 67, 0.15);
      fill: #174EA6;
    }

    .colab-df-buttons div {
      margin-bottom: 4px;
    }

    [theme=dark] .colab-df-convert {
      background-color: #3B4455;
      fill: #D2E3FC;
    }

    [theme=dark] .colab-df-convert:hover {
      background-color: #434B5C;
      box-shadow: 0px 1px 3px 1px rgba(0, 0, 0, 0.15);
      filter: drop-shadow(0px 1px 2px rgba(0, 0, 0, 0.3));
      fill: #FFFFFF;
    }
  

    
      const buttonEl =
        document.querySelector('#df-477bd961-154a-4d0c-a45c-ba224facdf6e button.colab-df-convert');
      buttonEl.style.display =
        google.colab.kernel.accessAllowed ? 'block' : 'none';

      async function convertToInteractive(key) {
        const element = document.querySelector('#df-477bd961-154a-4d0c-a45c-ba224facdf6e');
        const dataTable =
          await google.colab.kernel.invokeFunction('convertToInteractive',
                                                    [key], {});
        if (!dataTable) return;

        const docLinkHtml = 'Like what you see? Visit the ' +
          '<a target="_blank" href=https://colab.research.google.com/notebooks/data_table.ipynb>data table notebook</a>'
          + ' to learn more about interactive tables.';
        element.innerHTML = '';
        dataTable['output_type'] = 'display_data';
        await google.colab.output.renderOutput(dataTable, element);
        const docLink = document.createElement('div');
        docLink.innerHTML = docLinkHtml;
        element.appendChild(docLink);
      }
    
  


    
  



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
