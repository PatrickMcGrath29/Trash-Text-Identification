# Document Bias and Misinformation Identification

## Team Composition

Our team consists of Julien Cherry and Patrick McGrath.

## Problem

We would like to identify bias and misinformation in articles and other online sources. We plan on building a service that enables articles to be analyzed, with the purpose of exposing underlying information about those articles.

To accomplish this we plan on using machine learning with a suite of different models, trained over large datasets. Models will be trained for different purposes (identifying bias, coherency, etc.), and will each return a result that will then contribute to an overall report for that article.

We have found several models that can identify fake news articles, and we plan on looking into whether those models could supplement this information, in providing a robust analysis on our input. We are also considering focusing more on building a reliable model for identifying fake news articles, perhaps extending existing implementations.


Some example characteristics that we plan to look at include:
- **Likelihood of being fake news**
- Political bias
- Level of coherency
- Reputability of author, organization

A successful outcome for this project would entail building a service that analyzes articles, returning a series of ratings relating to different data points, that will then enable the user to establish informed opinions about the reputability of the article. We hope to have accurate models that offer valuable information about articles, and therefore we will likely be devoting most of our time to building high quality models for this classification process.

## Topics / Libraries / Platforms

We plan on using a machine learning library to train models over large sets of data. We’re currently leaning towards Tensorflow.

We’ll also be looking at naïve Bayes classifiers to see whether we’d be able to use it to get better categorization of fake news (briefly outlined in second resource in the Existing Research section).

The interface of the misinformation identifier could be a website or browser extension.

## Existing Research

* [Evaluating machine learning algorithms for fake news detection](https://ieeexplore.ieee.org/document/8305411)
* [Machine Learning tackles the Fake News problem](https://towardsdatascience.com/machine-learning-tackles-the-fake-news-problem-c3fa75549e52)

## Datasets

For credibility of articles, we could use a dataset like [CREDBANK](https://github.com/compsocial/CREDBANK-data) compiled by [Mitra and Gilbert (2015)](http://comp.social.gatech.edu/papers/icwsm15.credbank.mitra.pdf).

To report on the political leaning of articles, we could create our own dataset using online news articles from various sources tagged with the appropriate bias from [AllSides](https://www.allsides.com), a website which rates American news sources on a five-point left-to-right scale.

## Milestones and Week-by-Week Plan

| Week № or Deadline | Plan                                                                                             |
|--------------------|--------------------------------------------------------------------------------------------------|
| 9                  | Discuss ideas for project; create proposal.                                                      |
| February 26th      | Submit proposal.                                                                                 |
| 10                 | Research problem further; decide on relevant data set and methodology.                           |
| 11                 | Compile data set if necessary; understand and finalize methodology.                              |
| 12                 | Implement and evaluate first method to solve problem (extending fake news categorization tools). |
| March 22nd         | Milestone 1                                                                                      |
| 13                 | Implement and evaluate second method to solve problem (working on alternative characteristics)   |
| 14                 | Review two approaches; adjust trajectory as necessary.                                           |
| April 15th         | Milestone 2                                                                                      |
| 15                 | Finalize results; develop interface; prepare presentation.                                       |
| April 12th or 16th | Present project.                                                                                 |
| 16                 | Document results and prepare draft report                                                        |
| April 19th         | Submit draft report.                                                                             |
| 17                 | Finish documenting results and finalize report.                                                  |
| April 26th         | Submit final report.                                                                             |
