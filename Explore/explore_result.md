# Explore Result
## ISOT dataset
### 1. Data Overview
- The dataset contains 4 columns and 44898 rows (Both true & fake).
- Label column is the target variable, which has two classes: `True` and `Fake`. The dataset is balanced with 21417 True and 23481 Fake news.
- There are no missing values in the dataset.
- There are 38729 unique news title and 38646 unique news text out of 44898.
### Things to do when preprocessing the data
- Remove the `date` column as it is not useful for the classification task.
- Combine the `title` and `text` columns or treat them as separate features.
- Remove duplicate news(title and text).
- Remove corrupted news that has no text.
- Remove outliers.
- Remove punctuation, special characters, and stopwords.
- Tokenize the text.
- Lemmatize the text.   
- Vectorize the text using TF-IDF.
- Split the data into training and testing sets.
