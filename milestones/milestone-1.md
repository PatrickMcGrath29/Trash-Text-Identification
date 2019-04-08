# Milestone 1

## Report

Our initial work tackles the problem of identifying misinformation. We used a [fake news dataset on Kaggle](https://www.kaggle.com/c/fake-news/data) that consists of a training set of 20,800 articles annotated as either reliable or unreliable. With Python and the `scikit-learn` library, we cleaned and vectorized the data, weighted it using tf–idf, and used one of two classifiers. Employing a naïve Bayes classifier achieves 77% accuracy with a test dataset of 5,200 articles. A support-vector machine classifier is even more accurate—achieving 92% accuracy.

This milestone also involved a great deal of work identifying and cleaning datasets, and learning about industry practices within classification for machine learning. We each took online courses, and spent numerous hours researching methods for text classification. We identified additional approaches for classification, and explored new libraries like TensorFlow.

## Reflect

We’ve made significant progress and have implemented two methods of classifying misinformation. This is about what we expected to complete for this milestone, although we didn’t specify that we would use more than one classifier.

We believe things are going extremely well so far. We established a simpler baseline for the classification of fake news, while gaining more general understanding about what classification involves.

## Replan

Per our week-by-week plan, we are on track. Upcoming, we’d like to tweak our feature engineering for this first problem, perhaps achieving higher accuracy. We expect to now work towards a more complex implementation of text classification (perhaps using TensorFlow deep learning) to achieve better results. After doing so, we will then move towards breaking up our classification into more specific and refined points including political bias and sentiment.
