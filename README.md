📰 News Authenticity Classification using NLP & Machine Learning

📌 Project Overview

This project develops a machine learning pipeline to classify news
articles as Real or Fake using Natural Language Processing (NLP).

The project analyzes nearly 45,000 news articles, applies text
preprocessing and TF-IDF vectorization, and benchmarks four machine
learning classifiers. The best-performing classifier achieved
approximately 99.6% test accuracy.

🎯 Problem Statement

The objective is to build an automated classification system capable of
distinguishing between real and fake news articles based on textual
content.

The project focuses on: - Cleaning and preprocessing raw news text -
Converting text into numerical features - Training multiple
classification algorithms - Comparing model performance - Testing
predictions on unseen news articles

📊 Dataset

The Fake and Real News Dataset contains 44,898 news articles: -
Fake News: 23,481 - Real News: 21,417 - Total: 44,898

A small set of articles was reserved for manual prediction testing,
while the remaining data was used for model development.

Dataset Source

Fake and Real News Dataset --- Clément Bisaillon, Kaggle

https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset

🔄 Project Workflow

Raw News Articles → Data Cleaning → Regex-based Text Preprocessing →
TF-IDF Vectorization → Train-Test Split → Model Training → Model
Evaluation → Model Comparison → Unseen Article Prediction

🧹 Text Preprocessing

Regex-based preprocessing was used to remove: - URLs and HTML content -
Punctuation and special characters - Numeric noise - Unnecessary
formatting

🔢 Feature Engineering with TF-IDF

TF-IDF (Term Frequency-Inverse Document Frequency) transforms
cleaned news text into numerical feature vectors suitable for machine
learning models.

🤖 Machine Learning Models

Logistic Regression

Decision Tree Classifier

Gradient Boosting Classifier

Random Forest Classifier

📈 Model Performance

Model                            Test Accuracy

Logistic Regression                     98.49%
Decision Tree Classifier            99.61%
Gradient Boosting Classifier            99.55%
Random Forest Classifier                98.64%

The Decision Tree Classifier achieved approximately 99.6% test
accuracy, the highest among the four evaluated classifiers.

🔍 Unseen Article Testing

An inference pipeline was implemented to: 1. Accept raw news text 2.
Apply the same preprocessing 3. Transform text using the trained TF-IDF
vectorizer 4. Generate predictions using trained classifiers 5. Compare
predictions across models

💡 Key Findings

Processed nearly 45K news articles

Used TF-IDF for text feature engineering

Benchmarked 4 machine learning classifiers

Achieved approximately 99.6% best test accuracy

Built an inference workflow for unseen news articles

🛠️ Tech Stack

Programming: Python

Data Processing: Pandas, NumPy

NLP: Regex, TF-IDF

Machine Learning: Scikit-learn

Models: Logistic Regression, Decision Tree, Gradient Boosting,
Random Forest

Visualization: Matplotlib

Environment: Jupyter Notebook

📁 Project Structure

news-authenticity-classification/
├── Fake_News_Detection.ipynb
├── README.md
├── requirements.txt
├── dataset_source.txt
└── LICENSE-DATASET.md

⚙️ Installation & Usage

git clone https://github.com/Aditya01110/news-authenticity-classification.git
cd news-authenticity-classification
pip install -r requirements.txt

Open Fake_News_Detection.ipynb and run the notebook cells
sequentially.

📦 Requirements

pandas
numpy
scikit-learn
matplotlib

🚀 Future Improvements

Add Precision, Recall, and F1-score based comparison

Implement cross-validation

Perform hyperparameter tuning

Explore word embeddings and transformer-based NLP models

Build a web interface for real-time classification

👤 Author

Aditya Kumar Rawani
B.Tech, Indian Institute of Technology Guwahati
