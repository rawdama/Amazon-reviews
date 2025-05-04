# Amazon-reviews
## Overview
This project implements an end-to-end sentiment analysis of Amazon product reviews, utilizing Natural Language Processing (NLP) techniques to classify customer feedback. The goal is to automate the classification process and uncover patterns in customer sentiments.

## Features
Sentiment analysis of over 10,000 Amazon product reviews
Automated sentiment scoring using VADER
Logistic regression model for classification
Comprehensive evaluation metrics and visualizations

## Dataset (Google Drive)
you can download it from here [https://drive.google.com/file/d/19oFAs2pIX0wscPOYJmkWBtja9Wsfc7PZ/view?usp=drive_link]

## Data Collection
The dataset consists of 10,000+ Amazon product reviews, which were collected for sentiment analysis.

## Model Details
Sentiment Scoring with VADER  

Utilized NLTK’s SentimentIntensityAnalyzer to handle tokenization, lowercasing, stop-word filtering, and scoring.  
Logistic Regression Model  

Input features: Three VADER scores (positive, neutral, negative).  
Implemented class_weight='balanced' to address class imbalance.  
Training: 90% of the data; Testing: 10%.  
Evaluation & Results    
Accuracy: 93%  
Neutral/Negative Recall: Improved from 0% to 100%  
Visualized results with a confusion matrix and a sentiment distribution pie chart.  
## Key Findings
Approximately 90% of reviews were positive, but VADER missed some Neutral/Negative groups.  
The balanced weights strategy successfully captured all Neutral and Negative reviews.    
A few Positive reviews were shifted into minority classes, which is an acceptable trade-off to eliminate blind spots.  
