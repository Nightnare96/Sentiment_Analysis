# Sentiment Analysis of Amazon Reviews

A Natural Language Processing (NLP) project for analyzing Amazon customer reviews using **VADER**, **RoBERTa**, and **Hugging Face Transformers**.

## 📌 Project Overview

Customer reviews contain valuable information about customer satisfaction and product perception. This project performs sentiment analysis on Amazon reviews using both traditional lexicon-based NLP techniques and modern transformer-based models.

The project compares the sentiment predictions from **VADER** and **RoBERTa** and explores cases where textual sentiment differs from the Amazon star rating.

## 📊 Dataset

The project uses the **Dataset:** [Amazon Fine Food Reviews – Kaggle](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews)

The original dataset contains:

- **568,454 reviews**
- **10 columns**

For computational efficiency, the analysis in this notebook is performed on the first **500 reviews**.

### Important Features

| Feature | Description |
|---|---|
| `Id` | Review ID |
| `ProductId` | Product identifier |
| `UserId` | User identifier |
| `ProfileName` | Reviewer name |
| `HelpfulnessNumerator` | Number of helpful votes |
| `HelpfulnessDenominator` | Total number of votes |
| `Score` | Amazon star rating |
| `Time` | Review timestamp |
| `Summary` | Review summary |
| `Text` | Full review text |

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NLTK
- VADER Sentiment Analyzer
- Hugging Face Transformers
- RoBERTa
- SciPy
- tqdm
- Google Colab

## 🔄 Project Workflow

```text
Amazon Reviews Dataset
        ↓
Data Loading
        ↓
Exploratory Data Analysis
        ↓
Text Tokenization
        ↓
POS Tagging
        ↓
   ┌───────────────┐
   │               │
   ↓               ↓
 VADER          RoBERTa
   │               │
   └───────┬───────┘
           ↓
   Sentiment Comparison
           ↓
    Review Analysis
           ↓
Transformers Pipeline# Sentiment_Analysis
