# 📰 Classification of Urdu News Articles

This project is focused on classifying Urdu news articles into predefined categories using custom machine learning models. It addresses the lack of language-specific tools for Urdu and aims to support personalized content delivery by transforming unstructured news data into organized, labeled information.

---

## 📌 Project Overview

The core objective of this project is to:

- Scrape Urdu-language news articles from popular local news websites.
- Preprocess and clean the text data.
- Classify each article into one of the following five categories:
  1. Entertainment
  2. Business
  3. Sports
  4. Science-Technology
  5. International

---

## 🗂️ Repository Contents

| File/Folder           | Description                                                                 |
|-----------------------|-----------------------------------------------------------------------------|
| `Scraping.ipynb`      | Web scraping notebook to extract articles from Urdu news websites           |
| `combined_articles.csv` | Collected dataset (IDs, titles, content, labels)                            |
| `data_cleaning.py`    | Script for preprocessing and cleaning raw text data                         |
| `eda.ipynb`           | Exploratory Data Analysis on the cleaned dataset                            |
| `models/`             | Contains implementations of at least three ML models                        |
| `evaluation.py`       | Evaluation functions to calculate accuracy, precision, recall, F1-score     |
| `report/`             | Project report in ACM format (PDF/DOCX)                                     |
| `README.md`           | This documentation file                                                     |

---

## 🔍 Data Collection

Articles are scraped from the following Urdu news sources:

- [Geo News Urdu](https://urdu.geo.tv)
- [Jang News](https://jang.com.pk)
- [ARY Urdu](https://urdu.arynews.tv)
- [Dunya News Urdu](https://dunya.com.pk)
- [Express News Urdu](https://express.pk)

Each article is saved with the following fields:
- `Article ID`
- `URL`
- `Title`
- `Content`
- `Gold Label` (true category)

---

## 🔧 Preprocessing & EDA

Preprocessing steps include:

- Removing HTML tags and non-Urdu characters
- Tokenization
- Stopword removal (Urdu-specific)
- Handling missing values
- Balancing classes (if necessary)

EDA includes:
- Category distribution
- Word frequency analysis
- Article length statistics

---

## 🧠 Model Implementation

The following models have been implemented **from scratch**:
1. **Naive Bayes Classifier**
2. **Logistic Regression**
3. **Multilayer Perceptron (Neural Network)**

Each model was trained and tested on the dataset, and evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score

(Sklearn models may be used **for comparison only**, not for grading.)

---

## 🏁 Final Report

A detailed report written in **ACM format** is included in the `/report` folder. It contains:

- Abstract
- Introduction
- Data Collection & Cleaning
- Model Descriptions
- Evaluation Results
- Conclusion & Future Work

---

## 📌 Requirements

- Python 3.7+
- BeautifulSoup, Requests (for scraping)
- Pandas, NumPy, Matplotlib (for data handling & EDA)
- Custom ML implementations (no Sklearn for grading)

You can install dependencies using:

```bash
pip install -r requirements.txt
