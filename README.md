# Amazon Fine Food Reviews - Sentiment Analysis

## Project Overview
This project applies an end-to-end machine learning workflow to the Amazon Fine Food Reviews dataset.

The goal is to classify customer reviews into three sentiment classes:

- Negative: Scores 1-2
- Neutral: Score 3
- Positive: Scores 4-5

The project also includes unsupervised clustering to explore the structure of the review data.

## Project Workflow

### Data Preparation
- Data Cleaning & Preprocessing
- Missing-value handling
- Duplicate removal
- Text cleaning
- Tokenization
- Stopword removal
- Lemmatization

### Exploratory Data Analysis
- Score distribution
- Sentiment distribution
- Review length analysis
- Data visualization

### Supervised Learning
- Logistic Regression
- Multinomial Naive Bayes
- Decision Tree
- Support Vector Machine (SVM)
- Random Forest
- Bagging
- Boosting (AdaBoost)

### Unsupervised Learning
- K-Means Clustering
- Hierarchical Clustering

### Evaluation
Models are evaluated using:
- Accuracy
- Precision
- Recall
- Macro F1-score
- Weighted F1-score
- Confusion Matrix

Clustering is evaluated using:
- Silhouette Score
- Adjusted Rand Index (ARI)
- Normalized Mutual Information (NMI)

## Dataset
Amazon Fine Food Reviews.

The project uses a reproducible sample of 50,000 reviews for development in Google Colab.

## Text Representation
TF-IDF is used to represent review text numerically.

For tree-based models and clustering, Truncated SVD is used to reduce the high-dimensional TF-IDF representation.

## Important Note
The dataset is imbalanced, with Positive reviews being the majority class. Therefore, Macro F1-score is considered an important metric in addition to accuracy.

## How to Run
1. Open the notebook in Google Colab.
2. Install the packages listed in `requirements.txt` if needed.
3. Run the notebook cells from top to bottom.
4. Review the model comparison and final insights.

## Project Structure

```text
ML/
├── Amazon_Food_Review_Sentiment_Analysis.ipynb
├── README.md
└── requirements.txt
```
