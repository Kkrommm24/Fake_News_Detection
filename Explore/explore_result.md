# Explore Result
## ISOT dataset
### Data Overview
- The dataset contains 4 columns and 44898 rows (Both true & fake).
- Label column is the target variable, which has two classes: `True` and `Fake`. The dataset is balanced with 21417 True and 23481 Fake news.
- There are no missing values in the dataset.
- There are 38729 unique news title and 38646 unique news text out of 44898 examples.
### Preprocess check list
- Remove the `date` column as it is not useful for the classification task.
- Combine the `title` and `text` columns or treat them as separate features.
- Remove duplicate news(title and text).
- Remove outliers.
  - Example with title "Homepage" (Crawl error)
  - Examples that contain youtube url only (text length = 43)
  - Examples with only spaces (text length <=2)
- Remove punctuation, special characters, and stopwords.
- Split the data into training and testing sets.
## UTK dataset
### Data overview

