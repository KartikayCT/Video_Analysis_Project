# Yelp Review Sentiment Classification

## About the Project

This project focuses on classifying Yelp reviews into three sentiment categories using classical Natural Language Processing (NLP) and Machine Learning techniques.

The project was built to understand the complete NLP classification workflow, from text preprocessing and TF-IDF vectorization to model training, evaluation, and error analysis.

Two classification models were trained and compared:

- Multinomial Naive Bayes
- Multinomial Logistic Regression

---

## Project Goal

The objective is to predict the sentiment of a Yelp review based on its text.

The original Yelp Review Dataset contains reviews rated from 1 to 5 stars. For this project, only 1-star, 3-star, and 5-star reviews were used.

The ratings were mapped as follows:

- 1-star → Negative
- 3-star → Neutral
- 5-star → Positive

2-star and 4-star reviews were removed.

To maintain class balance, 50,000 reviews were randomly sampled from each class, resulting in a final dataset of 150,000 reviews.

---

## NLP Pipeline

The project follows these main steps:

1. Filter and balance the dataset
2. Clean the review text
3. Handle negation
4. Tokenize the text
5. Remove stopwords
6. Apply lemmatization
7. Split the data into training and testing sets
8. Convert text into numerical features using TF-IDF
9. Train Multinomial Naive Bayes
10. Train Multinomial Logistic Regression
11. Evaluate both models
12. Analyze classification errors using confusion matrices

The TF-IDF vectorizer was fitted only on the training data before transforming the test data to prevent data leakage.

---

## Model Performance



Multinomial Naive Bayes | Accuracy=82.08% | Precision=82.45% | Recall=82.08% | F1-Score=82.18% |
| Multinomial Logistic Regression | Accuracy=86.05% | Precision=86.02% | Recall=86.05% | F1-Score=86.03% |

Multinomial Logistic Regression performed better than Multinomial Naive Bayes across all major evaluation metrics.

---

## Error Analysis

The confusion matrix analysis showed that the models had the most difficulty distinguishing between Neutral and Positive reviews.

Multinomial Naive Bayes made 5,377 incorrect predictions, while Multinomial Logistic Regression made 4,185 incorrect predictions.

Logistic Regression therefore made 1,192 fewer errors, representing approximately a 22.17% reduction in classification errors.

The largest error category for Naive Bayes was Positive reviews being classified as Neutral.

For Logistic Regression, the largest error category was Neutral reviews being classified as Positive.

---

## Key Findings

- Multinomial Logistic Regression was the best-performing model.
- Logistic Regression achieved an accuracy of 86.05%.
- Logistic Regression improved accuracy by approximately 3.97 percentage points over Naive Bayes.
- The Neutral sentiment class was more difficult to classify than Negative and Positive sentiments.
- Neutral and Positive reviews were the most commonly confused sentiment pair.
- Traditional NLP models can achieve strong results when combined with appropriate preprocessing and TF-IDF features.

---

## Libraries Used

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- NLTK
- Joblib
- Jupyter Notebook

---

## Author

Kartikay Chandra Tiwari

B.Tech Computer Science Engineering

GB Pant Institute of Engineering and Technology

GitHub: https://github.com/KartikayCT