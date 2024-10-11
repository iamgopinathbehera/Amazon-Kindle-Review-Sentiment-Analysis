# Amazon Kindle Store Reviews Dataset Analysis

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![NLTK](https://img.shields.io/badge/NLTK-%23000000.svg?style=for-the-badge&logo=nltk&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)

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

1. **Text Preprocessing**:
   - Used WordNet Lemmatizer for word normalization

2. **Bag of Words (BoW) with Naive Bayes Gaussian**: 
   - Achieved 58% accuracy

3. **TF-IDF with Naive Bayes Gaussian**:
   - Achieved slightly higher accuracy than BoW
   - Improved confusion matrix scores

These methods were chosen because they work well on sparse matrices, which is characteristic of text data.

## Tools and Technologies Used

- **Python**: Primary programming language used for the analysis
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing tools
- **scikit-learn**: Machine learning library for Naive Bayes, BoW, and TF-IDF
- **NLTK**: Natural Language Toolkit, used for WordNet Lemmatizer
- **Jupyter Notebook**: Interactive development environment for running the analysis

## Getting Started

To run this analysis on your local machine, follow these steps:

1. Clone this repository:
   ```
   git clone https://github.com/iamgopinathbehera/Amazon-Kindle-Review-Sentiment-Analysis.git
   ```

2. Install the required dependencies:
   ```
   pip install pandas numpy scikit-learn nltk jupyter
   ```

3. Download the NLTK WordNet data:
   ```python
   import nltk
   nltk.download('wordnet')
   ```

4. Open the Jupyter Notebook:
   ```
   jupyter notebook
   ```

5. Navigate to the notebook file and run the cells to reproduce the analysis.
