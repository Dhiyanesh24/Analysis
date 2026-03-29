# 🧠 Vibe Checker AI: NLP Sentiment Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-Latest-orange)
![Gradio](https://img.shields.io/badge/UI-Gradio-lightgrey)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Overview
Vibe Checker AI is a complete Natural Language Processing (NLP) pipeline built from scratch. It takes raw text (movie reviews, sports reactions, random rants) and uses a trained Machine Learning model to instantly classify the sentiment as **Positive 🟢** or **Negative 🔴**. 

This isn't just a basic script—it features data cleaning, an 80/20 train/test split, data balancing to prevent bias, and a fully interactive web UI.

## 🚀 Tech Stack
* **Core Engine:** Python, Scikit-learn (Machine Learning), NLTK (Natural Language Toolkit)
* **Data Handling:** Pandas, Regex (`re`)
* **Math/Logic:** TF-IDF Vectorizer, Multinomial Naive Bayes
* **Deployment:** Joblib (Model serialization), Gradio (Frontend Web UI)

## ✨ Core Features
1. **Custom TF-IDF Pipeline:** Converts raw English sentences into mathematical feature matrices, filtering out useless stop words.
2. **Naive Bayes Classifier:** A lightweight, highly efficient probabilistic model trained to detect sentiment.
3. **The "Anti-Bias" Fix:** Initially, the model suffered from "Toxic Positivity" due to an imbalanced dataset (80% positive Yelp reviews). I engineered a custom, perfectly balanced dataset encompassing sports (IPL, football), movies, and general life phrases to expand the vocabulary and force neutral baseline predictions.
4. **Production Ready:** The trained model and vectorizer are serialized (`.pkl`) so the UI can run instantly without retraining.
5. **Interactive Web App:** A clean, user-friendly Gradio interface for real-time vibe checking.
