# Twitter Sentiment Analysis Using Machine Learning

# Project Purpose
Our project aims to analyze tweets posted by Twitter users to detect the overall sentiment and mood of the public. This capability allows brands to receive real-time feedback to enhance customer satisfaction, politicians to respond more swiftly to the public's needs, and content creators to understand their followers' opinions in real-time.

# Pushing the Boundaries of Technology
Equipped with machine learning and deep learning algorithms, this project accurately identifies the emotional tones of tweets. For instance, by analyzing tweets about a new product from a brand, we can quickly determine whether users like the product. Such insights provide a tremendous advantage in shaping strategic decisions.

# Future of Analysis Methods
In today's rapidly evolving digital world, sentiment analysis to gauge social media trends is becoming indispensable for both individuals and businesses. This project aims not only to analyze data but also to understand the human emotions behind it.

# DataSet Story
The dataset comprises two main files:

tweets_labeled.csv: Contains tweets from 2022, including tweet IDs, content, timestamps, and manually labeled sentiments (-1 for negative, 0 for neutral, and 1 for positive).
tweets_21.csv: Contains tweets from 2021 with similar structure, but without sentiment labels.

# Data Fields
## tweets_labeled.csv

tweet_id: Tweet's unique identifier

tweet: Content of the tweet

date: Timestamp of when the tweet was posted


label: Manually entered sentiment label (-1: negative, 0: neutral, 1: positive)

## tweets_21.csv
tweet_id: Tweet's unique identifier

tweet: Content of the tweet

date: Timestamp of when the tweet was posted

# Methodology
In this project, we conducted a comprehensive Natural Language Processing (NLP) process to analyze and predict the emotional tendencies of Twitter users. The steps include:

## Data Preprocessing
Text Cleaning: Converted tweet texts to lowercase, handled missing values, and removed URLs, mentions, hashtags, and special characters.

Tokenization: Split text into individual words or tokens.

Stop Words Removal: Eliminated common words that do not contribute to sentiment.

Stemming/Lemmatization: Reduced words to their base or root form.

## Feature Engineering

Date Features: Created new variables based on season, day, and four-hour periods from the date information.

TF-IDF Vectorization: Transformed text data into numerical vectors using the TF-IDF (Term Frequency-Inverse Document Frequency) method.

## Model Training and Evaluation

Logistic Regression: Trained a logistic regression model using the TF-IDF matrix, achieving 67% accuracy.

Cross-Validation: Used k-fold cross-validation to evaluate model performance and ensure robustness.

Hyperparameter Tuning: Applied grid search for hyperparameter tuning to optimize the logistic regression model.

Evaluation Metrics: Assessed models using accuracy, precision, recall, F1-score, and ROC-AUC to gauge performance.

## Advanced Techniques

AutoGluon: Implemented AutoGluon for automated machine learning, comparing its performance with traditional logistic regression.

Performance Metrics: AutoGluon achieved an MSE of 8.4797 and an R² score of 0.8862, outperforming the logistic regression model with an MSE of 21.5174 and an R² score of 0.7112.


# Conclusion
This project demonstrates how advanced machine learning techniques can be employed for sentiment analysis of social media data. Working with text data is challenging due to the inherent complexity and ambiguity of natural language. Especially on social media platforms, where language is informal and filled with abbreviations, improving accuracy rates for tasks like sentiment analysis requires sophisticated algorithms and large datasets.
