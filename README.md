# 📄 Resume Analyzer

A simple web-based application that predicts the job category of a given resume and performs sentiment analysis on its content.

---

## 🚀 Features

- Predicts job domain from resume content using a K-Nearest Neighbors classifier.
- Performs text preprocessing using NLTK and custom cleaning steps.
- Includes sentiment analysis using TextBlob.
- Web interface built with Flask.
- Uses TF-IDF vectorization and an LDA model for topic modeling (trained but not displayed in UI).

---

## 🛠️ Tech Stack

- **Python**
- **Flask**
- **scikit-learn**
- **NLTK**
- **TextBlob**
- **spaCy**
- **joblib**

---

## 🧪 Model Training

- Trained a OneVsRest KNN classifier on a labeled resume dataset.
- Applied TF-IDF vectorization on cleaned resume text.
- LDA model trained for topic modeling (not used in frontend).
- Achieved reasonable accuracy on test set (value printed during training).

---

## 📦 Files

- `app.py` – Flask application handling routing and prediction logic.
- `train.py` – Script to train TF-IDF, KNN classifier, and LDA model.
- `clf.pkl`, `tfidf.pkl`, `lda.pkl` – Saved models for inference.
- `UpdatedResumeDataSet.csv` – Input dataset used for training.

---

## ▶️ Running the App

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
Run the Flask app:

python app.py

Open your browser and visit:

http://127.0.0.1:5000/
📁 Dataset
The project uses UpdatedResumeDataSet.csv, which contains labeled resume text and job categories.

