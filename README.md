
## Twitter Feed - Sentiment Analysis
`Python 3.5` classification of tweets (positive or negative) using `NLTK-3` and `sklearn`.

An analysis of the Twitter feed data incorporated in the `nltk` corpus.

***
## Repository Contents

- [x] `nltk.NaiveBayesClassifier` trained with **1000 tweets**. Implemented in `Train_Classifiers.py`.
- [x] Usage of `sklearn` implementing:
  - [x] **Naive Bayes**
    - [x] `MultinomialNB`
    - [x] `BernoulliNB`
  - [x] **Linear Model**
    - [x] `LogisticRegression`
    - [x] `SGDClassifier`
  - [x] **SVM**
    - [x] `SVC`
    - [x] `LinearSVC`
    - [x] `NuSVC`

Implemented in `Scikit_Learn_Classifiers.py`.

- [x] A voting system to determine the optimal learning method. Implemented in `sentiment_mod.py`.

***

## Accuracy Documentation

The table below outlines the accuracies achieved by various classifiers:

| **Classifiers**                 | **Accuracy achieved** |
|---------------------------------|-----------------------|
| `nltk.NaiveBayesClassifier`     | _73.0%_               |
| **ScikitLearn Implementations** |                       |
| `BernoulliNB`                   | _72.0%_               |
| `MultinomialNB`                 | _75.0%_               |
| `LogisticRegression`            | _71.0%_               |
| `SGDClassifier`                 | _69.0%_               |
| `SVC`                           | _48.0%_               |
| `LinearSVC`                     | _74.0%_               |
| `NuSVC`                         | _75.0%_               |

***

## Requirements & Setup

To set up this project, it's recommended to use either [anaconda](https://www.continuum.io/downloads) or [miniconda](http://conda.pydata.org/miniconda.html) to install the required packages and dependencies.

After that you can execute:

```sh
$ conda update conda
$ conda install scikit-learn nltk
```

***

#### Dataset

The dataset used in this package comes bundled with the `nltk` package.

In your Python interpreter, import `nltk` and download `stopwords` and `movie_reviews`:

```python
>>> import nltk
>>> nltk.download('stopwords')
>>> nltk.download('movie_reviews') 
```

**NOTE**: For instructions specific to your system, refer to the official [`nltk` website](http://www.nltk.org/data.html).

Once completed, run the Python interpreter and verify that the following imports are successful:

```python
>>> import nltk
>>> from nltk.corpus import stopwords, movie_reviews
>>> import sklearn
>>> 
```

***

## Execution

After cloning the repository with the following commands:

```sh
$ git clone https://github.com/suecmd/TwitterSentimentAnalysis-NLP
$ cd TwitterSentimentAnalysis-NLP
```

Run the Python files in the following order:
  1. `NLTK_Naive_Bayes.py`
  2. `Scikit_Learn_Classifiers.py`
  3. `Voting_Algos.py`

After that, you're ready to go!

***

## Next Developments

I'm presently working on a Twitter Sentiment Analysis project which first trains on a given dataset before analyzing live Twitter feeds and visualizing the data.

***

-prepared by SueCMD.