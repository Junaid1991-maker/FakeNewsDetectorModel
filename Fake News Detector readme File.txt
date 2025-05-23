# Fake News Detector 🕵️‍♂️📰

A machine learning-based system to classify news articles as real or fake using Natural Language Processing (NLP) and machine learning techniques.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0.2-orange)
![NLTK](https://img.shields.io/badge/NLTK-3.6.7-green)
![Streamlit](https://img.shields.io/badge/Streamlit-1.12.0-red)

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Technical Approach](#technical-approach)
- [Results](#results)
- [Demo](#demo)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
This project demonstrates how to:
- Preprocess textual data using NLP techniques
- Extract features using TF-IDF vectorization
- Train machine learning models (Logistic Regression/Random Forest)
- Deploy as a web app using Streamlit (optional)

## Features
✔️ Text preprocessing (lemmatization, stopword removal)  
✔️ TF-IDF feature extraction  
✔️ Two classifier options (Logistic Regression and Random Forest)  
✔️ Confidence scoring for predictions  
✔️ Streamlit web interface (optional)  

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/fake-news-detector.git
cd fake-news-detector

python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

pip install -r requirements.txt

jupyter notebook Fake_News_Detector.ipynb

Dataset
The project uses the Fake and Real News Dataset from Kaggle:

True.csv: 21,417 real news articles

Fake.csv: 23,481 fake news articles

Dataset columns:

title: News headline

text: News content

subject: News category

date: Publication date

label: 1 for real, 0 for fake (added during preprocessing)

Text Preprocessing:

Lowercasing

Removing URLs and special characters

Lemmatization

Stopword removal

Feature Extraction:

TF-IDF with max 5000 features

Models:

Logistic Regression (default)

Random Forest Classifier

Results
Model	Accuracy	Precision	Recall	F1-Score
Logistic Regression	98.7%	98.6%	98.9%	98.7%
Random Forest	97.2%	97.1%	97.4%	97.2%

Future Improvements
Add BERT/Transformer models

Include sentiment analysis features

Implement fact-checking API integration

Add multilingual support

