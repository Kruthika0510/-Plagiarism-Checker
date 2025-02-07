Plagiarism Detection Project 

Overview

This project focuses on detecting plagiarism between text pairs using the BLEU similarity method. It analyzes sentence similarity and classifies whether a given text pair is plagiarized.

Features
- Uses **BLEU Score** to measure similarity.
- Power BI Dashboard for visualization.
- Additional attributes like sentence length ratio, word overlap, etc.
- Supports thresholding for classification.

Dataset
- The dataset consists of sentence pairs with a **PAWS  (Paraphrase Adversaries from Word Scrambling)** indicating plagiarism.
- Columns:id,sentence1,sentence2,label 

Libraries Required:   
pandas   
numpy  
nltk   
spacy   
scikit-learn

Usage
Load and Preprocess Data(tokenisation):
Use pandas to load text data, clean  it with nltk/spacy, and convert it into numerical representations using TF-IDF or BERT embeddings.
Train the Model: Apply XGBoost, SVM, or deep learning models (BERT/LSTM) to learn patterns of paraphrased and plagiarized text.
Detect Plagiarism: Compare input text with stored documents using cosine similarity or fuzzy matching to identify similarities.

A BLEU (BiLingual Evaluation Understudy) score is a metric that measures how similar a machine-translated text is to a reference translation. It's a number between 0 and 1, with 0 indicating no overlap and 1 indicating perfect overlap.

Generate Reports: Highlight copied content, provide similarity scores, and visualize results via Flask/Streamlit.
