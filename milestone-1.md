# Milestone 1

## Report

Our initial work tackles the problem of identifying misinformation. We used a [fake news dataset on Kaggle](https://www.kaggle.com/c/fake-news/data) that consists of a training set of 20,800 articles annotated as either reliable or unreliable. With Python and the `scikit-learn` library, we cleaned and vectorized the data, weighted it using tf–idf, and used one of two classifiers. Employing a naïve Bayes classifier achieves 77% accuracy with a test dataset of 5,200 articles. A support-vector machine classifier is even more accurate—achieving 92% accuracy.

## Reflect

We’ve made significant progress and have implemented two methods of classifying misinformation. This is about what we expected to complete for this milestone, although we didn’t specify that we would use more than one classifier.

## Replan

Per our week-by-week plan, we are on track. Upcoming, we’d like to tweak our feature engineering for this first problem, perhaps achieving higher accuracy, and move onto another problem such as classifying articles based on political bias. So, our plan stays more or less the same.
