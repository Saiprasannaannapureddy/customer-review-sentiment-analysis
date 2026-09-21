# Customer Review Sentiment Analysis

## 📌 Project Overview

Customer Review Sentiment Analysis is a Natural Language Processing (NLP) project that analyzes customer reviews and classifies them into three sentiment categories:

* Positive
* Negative
* Neutral

The project uses **TF-IDF** for converting text into numerical features and **Logistic Regression** for sentiment classification.

---

## 🎯 Objectives

* Analyze customer reviews using NLP.
* Clean and preprocess review text.
* Convert text into numerical features using TF-IDF.
* Train a Logistic Regression classification model.
* Classify reviews into Positive, Negative, and Neutral categories.
* Evaluate the model using accuracy, classification report, and confusion matrix.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Jupyter Notebook
* TF-IDF
* Logistic Regression

---

## 📊 Dataset

The project uses a customer review dataset containing two columns:

```text
review
sentiment
```

The sentiment column contains three classes:

```text
Positive
Negative
Neutral
```

The dataset contains 90 customer reviews.

---

## 🧠 Methodology

The project follows these steps:

```text
Customer Reviews
       ↓
Data Loading
       ↓
Text Preprocessing
       ↓
Train-Test Split
       ↓
TF-IDF Feature Extraction
       ↓
Logistic Regression
       ↓
Sentiment Prediction
       ↓
Model Evaluation
```

### 1. Text Preprocessing

The review text is:

* Converted to lowercase
* Cleaned by removing special characters and numbers
* Extra spaces are removed
* Leading and trailing spaces are removed

### 2. TF-IDF Feature Extraction

TF-IDF (Term Frequency-Inverse Document Frequency) converts customer review text into numerical features that can be processed by the machine learning model.

The implementation uses:

* Maximum 5000 features
* Unigrams and bigrams
* Sublinear TF scaling

### 3. Machine Learning Model

The project uses **Logistic Regression** for sentiment classification.

The model is trained using the TF-IDF features and classifies reviews into:

* Positive
* Negative
* Neutral

---

## 📈 Model Performance

The Logistic Regression model achieved an accuracy of:

**77.8%**

on the test dataset.

The model is also evaluated using:

* Accuracy
* Classification Report
* Confusion Matrix

> The reported accuracy should be updated if the notebook is rerun and produces a different result.

---

## 🔍 Example Predictions

The model can be tested with new customer reviews such as:

```text
"Amazing product, I really loved the quality!"
```

```text
"The product is terrible and stopped working."
```

```text
"The package arrived today."
```

The trained model predicts the sentiment for each new review.

---

## 📁 Project Structure

```text
customer-review-sentiment-analysis/
│
├── sentiment.ipynb
├── customer_reviews.csv
├── README.md
└── .gitignore
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/customer-review-sentiment-analysis.git
```

Open the project folder:

```bash
cd customer-review-sentiment-analysis
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib scikit-learn jupyter
```

---

## ▶️ Run the Project

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
sentiment.ipynb
```

Run the notebook cells from top to bottom.

---

## ⚠️ Limitations

The model may produce incorrect predictions for:

* Sarcasm
* Mixed opinions
* Unfamiliar words
* Reviews containing both positive and negative opinions

For example:

```text
"The delivery was fast, but the product quality was terrible."
```

A simple text classification model may focus on individual words and incorrectly classify the overall sentiment.

---

## 🚀 Future Improvements

Possible improvements include:

* Larger datasets
* Advanced NLP preprocessing
* Word embeddings
* Transformer-based models
* Hyperparameter tuning
* Larger and more diverse customer reviews
* Real-time sentiment analysis
* Web-based sentiment prediction interface

---

## 📌 Conclusion

This project demonstrates how Natural Language Processing and Machine Learning can be used to analyze customer opinions. Customer reviews are cleaned and converted into numerical features using TF-IDF, after which a Logistic Regression model performs sentiment classification.

The project provides a basic and understandable workflow for building an NLP-based sentiment analysis system.

