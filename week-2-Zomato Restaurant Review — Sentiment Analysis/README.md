# Zomato Restaurant Review — Sentiment Analysis

A machine learning project that reads restaurant reviews and predicts whether the customer was happy, neutral, or unhappy.

---

## What this project does

Instead of manually reading thousands of reviews, this model automatically labels each one as **Positive**, **Neutral**, or **Negative** based on the text the customer wrote.

---

## Dataset

- Source: Zomato Restaurant Reviews CSV
- ~26,000 reviews
- Columns: Restaurant, Reviewer, Review, Rating, Metadata, Time, Pictures

---

## How sentiment labels were created

| Rating | Sentiment |
|--------|-----------|
| 4 or 5 | Positive  |
| 3      | Neutral   |
| 1 or 2 | Negative  |

---

## Steps followed

1. Cleaned and explored the data
2. Created 15 charts to understand patterns
3. Ran 3 hypothesis tests to confirm findings
4. Preprocessed the review text (lowercase, remove stopwords, lemmatization)
5. Converted text to numbers using TF-IDF
6. Trained 3 ML models and picked the best one

---

## Models used

- Logistic Regression
- Multinomial Naive Bayes
- Linear SVM

All three were tuned using GridSearchCV.

---

## Libraries

```
pandas, numpy, matplotlib, seaborn, nltk, sklearn, scipy, wordcloud, joblib
```

---

## How to run

1. Clone the repo
2. Install dependencies — `pip install -r requirements.txt`
3. Open `Zomato_Sentiment_Analysis_Completed.ipynb` in Jupyter
4. Run all cells from top to bottom

---

## Result

The best model can correctly identify the sentiment of a restaurant review and is saved as a `.pkl` file for reuse.

---

## Why this is useful

Restaurant owners get hundreds of reviews. This system helps them quickly spot the negative ones and act on them — without reading every single review manually.
