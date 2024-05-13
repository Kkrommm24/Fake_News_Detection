# Fake news detection
## Introduction
- This project is a part of the course "Intro Machine Learning" at HUST.
- The problem is to detect fake news from real news.    
## Members
- Pham Phan Anh - 20210039 (Leader)
- Nguyen Dinh Hieu – 20215049
- Hoang Đuc Gia Hung – 20215062
- Tran Đang Phuc – 20215120
- Mai Minh Khoi – 20210492

## Dataset
### [Fake news competition by UTK Machine Learning Club](https://www.kaggle.com/c/fake-news/data)
### [Liar dataset](https://paperswithcode.com/dataset/liar)
### [ISOT Fake News Dataset](https://www.kaggle.com/datasets/emineyetm/fake-news-detection-datasets)
### [FakeNewsNet](https://github.com/KaiDMML/FakeNewsNet)

## Methods
### 1. Data Exploration
- Check missing values
- Check duplicates
- Check distribution of labels
- Check distribution of text length
- Check distribution of word count
- Use WordCloud to visualize the most common words in the dataset
- Use K-Means to cluster the dataset
- Use PCA to visualize the dataset
### 2. Data Preprocessing
- Remove missing values
- Remove duplicates
- Remove special characters
- Remove stopwords
- Lemmatization
- Tokenization
- Vectorization
### 3. Model
- Machine Learning
  - Logistic Regression
  - Random Forest
  - Gradient Boosting
  - Support Vector Machine
  - Naive Bayes
  - XGBoost
- Deep Learning
  - LSTM
  - Bi-LSTM
  - CNN
  - Bi-LSTM + CNN
- Ensemble Learning
  - Voting Classifier
  - Stacking Classifier
  - Bagging Classifier 
### 4. Evaluation
- Accuracy
- F1 score
### 5. Deployment
- Streamlit: Create a simple web app to predict fake news