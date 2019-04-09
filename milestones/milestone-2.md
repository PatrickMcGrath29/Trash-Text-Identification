# Milestone 2

- [Milestone 2](#milestone-2)
  - [Introduction](#introduction)
  - [Naive Bayes Classification](#naive-bayes-classification)
    - [Tokens w/ lowest weight](#tokens-w-lowest-weight)
    - [Tokens w/ highest weight](#tokens-w-highest-weight)
    - [Analysis](#analysis)
  - [Stochastic Gradient Descent](#stochastic-gradient-descent)
    - [Tokens w/ lowest heights](#tokens-w-lowest-heights)
    - [Tokens w/ highest weights](#tokens-w-highest-weights)
    - [Analysis](#analysis-1)
  - [Passive Aggressive](#passive-aggressive)
    - [Tokens w/ lowest weights](#tokens-w-lowest-weights)
    - [Tokens w/ highest weights](#tokens-w-highest-weights-1)
    - [Analysis](#analysis-2)
  - [Next Steps](#next-steps)

## Introduction

In the previous milestone we started classifying a Kaggle Fake News dataset using a series of different machine learning classifiers. We achieved a range of accuracies, from 68% to 96%. The focus of this milestone was to dig into the findings for each of the classifiers that we used, to get a better understanding into how they are weighing features, to then hopefully determine better features and further increase accuracy.

First, we added additional visualization methods to the Jupyter notebook detailing what our false positives and false negatives are. We also added transparency into the weighting of features, detailing the features with the highest and lowest weights.

## Naive Bayes Classification

### Tokens w/ lowest weight

| Weight   | Token |
| :------- | :---- |
| -11.9582 | 0000  |
| -11.9582 | 001   |
| -11.9582 | 0024  |
| -11.9582 | 0102  |
| -11.9582 | 017   |
| -11.9582 | 018   |
| -11.9582 | 01pm  |
| -11.9582 | 020   |
| -11.9582 | 024   |
| -11.9582 | 036   |
| -11.9582 | 039   |
| -11.9582 | 046   |
| -11.9582 | 051   |
| -11.9582 | 052   |
| -11.9582 | 053   |
| -11.9582 | 060   |
| -11.9582 | 061   |
| -11.9582 | 064   |
| -11.9582 | 065   |
| -11.9582 | 066   |

### Tokens w/ highest weight
| Weight    | Token   |
| :-------- | :------ |
| -7.341644 | hillary |
| -7.326587 | be      |
| -7.267753 | by      |
| -7.259368 | with    |
| -7.218171 | as      |
| -7.203357 | are     |
| -7.192496 | trump   |
| -7.187729 | this    |
| -7.184327 | you     |
| -7.094942 | on      |
| -7.067222 | clinton |
| -6.980072 | it      |
| -6.927019 | for     |
| -6.618096 | is      |
| -6.546371 | that    |
| -6.301768 | in      |
| -5.995318 | and     |
| -5.947999 | of      |
| -5.880526 | to      |
| -5.177399 | the     |

### Analysis

The accuracy when using Naive Bayes classification is roughly 68%. When looking at the weights associated with specific tokens, it is clear that there is not much of a correlation between the weight and the likelihood that a word would be in a corpus of text classified as fake news.

## Stochastic Gradient Descent

### Tokens w/ lowest heights

| Weight    | Token     |
| :-------- | :-------- |
| -0.077192 | said      |
| -0.071631 | breitbart |
| -0.063136 | twitter   |
| -0.056375 | 2017      |
| -0.055649 | follow    |
| -0.051476 | mr        |
| -0.046095 | ms        |
| -0.035301 | added     |
| -0.034659 | president |
| -0.033361 | mrs       |
| -0.033050 | its       |
| -0.031165 | milo      |
| -0.030118 | saturday  |
| -0.029957 | friday    |
| -0.028999 | tillerson |
| -0.028256 | former    |
| -0.026728 | sunday    |
| -0.026449 | thursday  |
| -0.026413 | week      |
| -0.026063 | an        |

### Tokens w/ highest weights

| Weight   | Token    |
| :------- | :------- |
| 0.025720 | being    |
| 0.025847 | tpp      |
| 0.027083 | fact     |
| 0.028952 | via      |
| 0.029833 | are      |
| 0.030305 | however  |
| 0.030922 | clinton  |
| 0.031632 | 11       |
| 0.032910 | old      |
| 0.036262 | source   |
| 0.041281 | elect    |
| 0.044610 | self     |
| 0.046667 | us       |
| 0.047127 | 2016     |
| 0.048166 | co       |
| 0.055459 | non      |
| 0.056147 | november |
| 0.060869 | october  |
| 0.063116 | hillary  |
| 0.072100 | anti     |

### Analysis

Stochastic Gradient Descent gives us an accuracy rate of roughl;y 95%. Here we start to see tokens with perhaps more meaning associated to high and low weights. The token `fact` shows up in the set of words with highest weights which is reasonable, however words like `mrs`, `mr`, `ms`, and `an` have a very low weighting when they don't in themselves represent whether content is factual or not.

## Passive Aggressive

### Tokens w/ lowest weights
| Weight    | Token     |
| :-------- | :-------- |
| -6.562925 | breitbart |
| -6.382216 | said      |
| -6.183251 | twitter   |
| -5.887345 | follow    |
| -5.867927 | 2017      |
| -4.939482 | mr        |
| -3.908291 | ms        |
| -3.077843 | mrs       |
| -2.990358 | president |
| -2.986703 | sunday    |
| -2.875207 | march     |
| -2.868521 | its       |
| -2.576587 | democrats |
| -2.441469 | on        |
| -2.432432 | dr        |
| -2.398569 | milo      |
| -2.277705 | that      |
| -2.259361 | an        |
| -2.163066 | pamkeynen |
| -2.095076 | last      |

### Tokens w/ highest weights
| Weight   | Token    |
| :------- | :------- |
| 2.567435 | via      |
| 2.572235 | related  |
| 2.640190 | however  |
| 2.678863 | print    |
| 2.764005 | clinton  |
| 2.912111 | al       |
| 2.997316 | snip     |
| 3.203991 | share    |
| 3.328805 | this     |
| 3.565803 | self     |
| 3.628204 | source   |
| 3.736768 | non      |
| 3.830771 | co       |
| 4.216531 | elect    |
| 4.544882 | us       |
| 4.835506 | hillary  |
| 4.893513 | november |
| 5.133547 | 2016     |
| 5.675274 | october  |
| 6.181697 | anti     |

### Analysis

Passive Aggressive achieves an accuracy rate of above 96%. The weights on tokens is similar to those in Stochastic Gradient Descent, with what appears to be slightly more relevance (words like `tpp` and `l1` are no longer as negatively weighted). In all, the weights for tokens does not appear to have a direct corelation to whether or not an article is fake news or not.


## Next Steps

Using individual words as features proved to be fairly effective in identifying whether an article is fake news or not **in this dataset**, however we have concerns that the model is too fit to this specific dataset, to the point where it is not actually determining whether an article is reliable or not. The context behind these words is lost when they are used individually as features, meaning logical flow in sentences is not taken into account. To accomodate this, we will likely use Word2Vec and n-grams (and possibly sentiment analysis) to gain additional context into the structure and meaning of sentences, as opposed to individual words. We think this will prove to be a more reliable method of identifying whether a corpus of text is reliable or not, on a wider range of data.
