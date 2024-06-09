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
- The dataset contains 5 columns and 20800 rows
- Label column is the target variable, which has two classes: `1` - unreliable and `0` - reliable. The dataset is balanced with 10413 unreliable and 10387 reliable news.
- There are missing values in `title` and `text` column
- There are 19803 unique news title and 20386 unique news text out of 20800 examples.
### Preprocess check list
- Remove the `author` column as it is not useful for the classification task.
- Combine the `title` and `text` columns or treat them as separate features.
- Remove null values.
- Remove duplicate news(title and text).
- Remove outliers.
  - Examples with only spaces (text length <=2)
  - Examples with text content "source Add To The Conversation Using Facebook Comments" (text length = 54)
  - Examples with non-English text
- Remove punctuation, special characters, and stopwords.
