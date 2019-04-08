# Milestone 2

- [Milestone 2](#milestone-2)
  - [Naive Bayes Classification](#naive-bayes-classification)
    - [Tokens w/ lowest weight](#tokens-w-lowest-weight)
    - [Tokens w/ highest weight](#tokens-w-highest-weight)
    - [Explanation](#explanation)
  - [Stochastic Gradient Descent](#stochastic-gradient-descent)
    - [Tokens w/ lowest heights](#tokens-w-lowest-heights)
    - [Tokens w/ highest weights](#tokens-w-highest-weights)
    - [Explanation](#explanation-1)

In the previous milestone we started classifying a Kaggle Fake News dataset using a series of different machine learning classifiers. We achieved a range of accuracies, from 68% to 96%. The focus of this milestone was to dig into the findings for each of the classifiers that we used, to get a better understanding into how they are weighing features, to then hopefully determine better features and further increase accuracy.

First, we added additional visualization methods to the Jupyter notebook detailing what our false positives and false negatives are. We also added transparency into the weighting of features, detailing the features with the highest and lowest weights.

## Naive Bayes Classification

### Tokens w/ lowest weight

| index | weight   | token |
| :---- | :------- | :---- |
| 0     | -11.9582 | 0000  |
| 1     | -11.9582 | 001   |
| 2     | -11.9582 | 0024  |
| 3     | -11.9582 | 0102  |
| 4     | -11.9582 | 017   |
| 5     | -11.9582 | 018   |
| 6     | -11.9582 | 01pm  |
| 7     | -11.9582 | 020   |
| 8     | -11.9582 | 024   |
| 9     | -11.9582 | 036   |
| 10    | -11.9582 | 039   |
| 11    | -11.9582 | 046   |
| 12    | -11.9582 | 051   |
| 13    | -11.9582 | 052   |
| 14    | -11.9582 | 053   |
| 15    | -11.9582 | 060   |
| 16    | -11.9582 | 061   |
| 17    | -11.9582 | 064   |
| 18    | -11.9582 | 065   |
| 19    | -11.9582 | 066   |

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

### Explanation

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

### Explanation
