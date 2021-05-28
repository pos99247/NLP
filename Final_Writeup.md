# Amazon Product Review Topic Modeling

---

Brian Nam

## Abstract

---
The goal of this project is to use TV reviews from Amazon to have a general understanding of the common problems in various brands. Reviews were cleaned with natural language process methods and then put into a latent dirichlet allocation model for topic modeling. Topic modeling was done from a smaller dataset(by brand) to the entire set for better comparison.

## Design

---
The dataset was divided into brands and ratings. For reviews with overall rating of greater than or equal to four was given 1 for their rating column and 0 for the rest. Rating 1 is good reviews and rating 0 is bad reviews. Then for each brand the LDA model is ran twice. Once for the bad reviews and once for the entire brand. Final LDA will be ran on the entire dataset at the end.

## Data

---
Data was acquired from Jianmo Ni at UCSD that already had the full amazon review dataset. The dataset started with 376,892 data points of TV reviews from 2001 to 2018 with 30 features. After extracting the data we needed the data set was with 66,102 data points and 17 features. 


## Algorithms

---
**Feature Engineering**
Using the overall column in the original dataset, divided the dataset into two sentiments:positive and negative.

**Models**
Non-negative matrix factorization with tf-idf vectorizer was used initially. To improve coherence, latent dirichlet allocation and count vectorizor was chosen as a final modeling tool.


## Tools

---

* Pandas and numpy for data manipulation
* Seaborn and matplotlib for data visualization
* Spacy and Gensim for Natural Language Processing
* Sklearn  for Latent Dirichlet Allocation modeling
* PyLDAvis for data visualization

## Communication

---

Slides were made for the presentation to give a better understanding of the model.