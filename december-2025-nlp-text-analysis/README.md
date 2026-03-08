# December 2025 — Natural Language Processing

**Month:** December 2025  
**Program:** Pursuit AI Fellowship — Level 2  
**Author:** Paula Lawton

---

## Description

This project introduces Natural Language Processing (NLP), covering the core techniques for working with unstructured text data. Projects ranged from classic text preprocessing and sentiment analysis to working with pre-trained transformer models via the Hugging Face `transformers` library.

## Topics Covered

- Text preprocessing: tokenization, stopword removal, stemming, lemmatization
- Bag-of-Words and TF-IDF vectorization
- Sentiment analysis (rule-based with `TextBlob` and ML-based with logistic regression)
- Named Entity Recognition (NER)
- Introduction to transformer models (BERT) using `transformers` and `pipeline` API
- Word embeddings: Word2Vec concepts and pre-trained vectors

## Project Highlights

- **Movie Review Sentiment Classifier:** Trained a TF-IDF + Logistic Regression model on the IMDB movie review dataset to classify reviews as positive or negative (93% accuracy).
- **News Headline Summarizer:** Used a pre-trained `facebook/bart-large-cnn` model from Hugging Face to generate abstractive summaries of news articles.
- **NER Demo:** Used `spaCy` to extract named entities (people, organizations, locations) from news text and visualized them with displaCy.

## Skills Demonstrated

- End-to-end NLP pipeline from raw text to predictions
- Leveraging pre-trained models for zero-shot and few-shot tasks
- Evaluation of text models: accuracy, confusion matrices, and manual error analysis

## How to Run

```bash
pip install transformers torch spacy textblob scikit-learn jupyter

# Download spaCy English model
python -m spacy download en_core_web_sm

jupyter notebook
```

## Key Takeaways

Pre-trained transformer models have dramatically lowered the barrier to building effective NLP applications. Understanding classical NLP (TF-IDF, bag-of-words) remains important for building intuition about what these models are doing under the hood.
