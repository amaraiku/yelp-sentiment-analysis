# Yelp Sentiment Analysis - Hospitality Reviews

A lexicon-based NLP project applying VADER sentiment analysis to 3,000 Yelp 
hospitality reviews to extract actionable service insights.

## Overview

This project investigates whether sentiment analysis of Yelp reviews can provide 
reliable, actionable insights for hospitality businesses to improve service quality 
and customer satisfaction.

## Dataset

- **Source:** Yelp Review Full dataset via HuggingFace
- **Sample size:** 3,000 reviews (subsampled from 650,000+ for reproducibility)
- **Fields:** review text, star rating (1–5), derived sentiment label

## Methodology

1. **Data loading and subsampling** - reproducible random sample (seed = 42)
2. **Preprocessing pipeline** - tokenisation (RegexpTokenizer), stopword removal 
   (NLTK), stemming (PorterStemmer)
3. **Sentiment scoring** - VADER applied to raw text to preserve punctuation, 
   capitalisation, and intensifiers
4. **Exploratory analysis** - histograms, boxplots, frequency distributions, 
   wordclouds for positive, negative, and neutral classes

## Key Findings

- **Sentiment distribution:** 78% positive, 22% negative, <1% neutral
- **Operational pain points (negative reviews):** wait times, food temperature, 
  pricing concerns
- **Service strengths (positive reviews):** friendliness, food quality, atmosphere
- Positive reviews showed wider review-length distributions, suggesting richer 
  qualitative content for theme extraction

## Business Application

Designed framework for automated sentiment monitoring to help hospitality 
businesses detect service failures early and reinforce successful service patterns.

## Tools and Libraries

- Python 3
- NLTK (VADER, stopwords, PorterStemmer, RegexpTokenizer, FreqDist)
- pandas, numpy
- matplotlib, seaborn
- wordcloud
- HuggingFace datasets

## Files

- `yelp_sentiment_analysis.ipynb` — full analysis notebook
- `requirements.txt` — Python dependencies

## How to Run

1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Open the notebook in Jupyter or Google Colab
4. Run all cells sequentially

## Author

Amarachukwu Iku - MSc Data Science, University of Salford
