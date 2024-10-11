# Amazon Kindle Store Reviews Dataset Analysis

## About Dataset

### Context
This repository contains analysis on a small subset of book reviews from the Amazon Kindle Store category.

### Content
The dataset includes a 5-core subset of product reviews from the Amazon Kindle Store category, spanning from May 1996 to July 2014. It contains a total of 982,619 entries. In this dataset, each reviewer has at least 5 reviews, and each product has at least 5 reviews.

### Columns
- `asin`: ID of the product (e.g., B000FA64PK)
- `helpful`: Helpfulness rating of the review (e.g., 2/3)
- `overall`: Rating of the product
- `reviewText`: Text of the review (heading)
- `reviewTime`: Time of the review (raw)
- `reviewerID`: ID of the reviewer (e.g., A3SPTOKDG7WBLN)
- `reviewerName`: Name of the reviewer
- `summary`: Summary of the review (description)
- `unixReviewTime`: Unix timestamp

## Acknowledgements
This dataset is taken from the Amazon product data compiled by Julian McAuley, UCSD. The original data can be found at [http://jmcauley.ucsd.edu/data/amazon/](http://jmcauley.ucsd.edu/data/amazon/). License to the data files belongs to the original authors.

## Analysis Performed

As a beginner in data analysis, I have performed the following:

1. **Bag of Words (BoW) with Naive Bayes Gaussian**: 
   - Achieved 58% accuracy

2. **TF-IDF with Naive Bayes Gaussian**:
   - Achieved slightly higher accuracy than BoW
   - Improved confusion matrix scores

These methods were chosen because they work well on sparse matrices, which is characteristic of text data.
