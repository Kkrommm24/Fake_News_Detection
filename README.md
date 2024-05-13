# Fake news detection

## Introduction
- This project is a part of the course "Intro to Machine Learning" at HUST.
- The problem is to detect fake news from real news.

## Members
- Pham Phan Anh - 20210039 (Leader)
- Nguyen Dinh Hieu – 20215049
- Hoang Đuc Gia Hung – 20215062
- Tran Đang Phuc – 20215120
- Mai Minh Khoi – 20210492

## Dataset
### [Fake news competition by UTK Machine Learning Club](https://www.kaggle.com/c/fake-news/data)
Competition run by the UTK Machine Learning Club on Kaggle.
Data overview:
- train.csv: A full training dataset with the following attributes:
  - `id`: unique id for a news article
  - `title`: the title of a news article
  - `author`: author of the news article
  - `text`: the text of the article; could be incomplete
  - `label`: a label that marks the article as potentially unreliable
    - 1: unreliable
    - 0: reliable
- test.csv: A testing training dataset with all the same attributes at train.csv without the label.
- submit.csv: A sample submission to submit on Kaggle in the format id, label.
### [Liar dataset](https://paperswithcode.com/dataset/liar)
A decade-long of 12.8K manually labeled short statements were collected in various contexts from POLITIFACT.COM, which provides detailed analysis report and links to source documents for each case
Data overview:
- Column 1: the ID of the statement ([ID].json).
- Column 2: the label.
  - pants-fire: The statement is a clear lie or grossly inaccurate.
  - false: The statement is false.
  - half-true: The statement is partially true.
  - mostly-true: The statement is mostly true.
  - true: The statement is true.
- Column 3: the statement.
- Column 4: the subject(s) of the statement.
- Column 5: the speaker.
- Column 6: the speaker's job title.
- Column 7: the state info.
- Column 8: the party affiliation.
- Column 9-13: the total credit history count, including the current statement.
  - 9: barely true counts.
  - 10: false counts.
  - 11: half true counts.
  - 12: mostly true counts.
  - 13: pants on fire counts.
- Column 14: the context (venue / location of the speech or statement).
### [ISOT Fake News Dataset](https://www.kaggle.com/datasets/emineyetm/fake-news-detection-datasets)
The dataset contains two types of articles fake and real News. This dataset was collected from realworld sources; the truthful articles were obtained by crawling articles from Reuters.com (News website). As for the fake news articles, they were collected from different sources. The fake news articles were collected from unreliable websites that were flagged by Politifact (a fact-checking organization in the USA) and Wikipedia. The dataset contains different types of articles on different topics, however, the majority of articles focus on political and World news topics.
Data overview:
- True.csv: A dataset containing real news articles.
  - `title`: the title of the article.
  - `text`: the text of the article.
  - `subject`: the subject of the article.
  - `date`: the date the article was published.
- Fake.csv: A dataset containing fake news articles. Columns are the same as True.csv.
### [FakeNewsNet](https://github.com/KaiDMML/FakeNewsNet)
FakeNewsNet is a data repository with news content, social context, and spatiotemporal information for studying fake news on social media. The repository contains two datasets: politifact and gossipcop.
Data overview:
 - `id` - Unique identifider for each news
 - `url` - Url of the article from web that published that news 
 - `title` - Title of the news article
 - `tweet_ids` - Tweet ids of tweets sharing the news. This field is list of tweet ids separated by tab.
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