# Bag of Words Meets Bags of Popcorn

# Description
In this tutorial competition, we dig a little "deeper" into sentiment analysis. Google's Word2Vec is a deep-learning inspired method that focuses on the meaning of words. Word2Vec attempts to understand meaning and semantic relationships among words. It works in a way that is similar to deep approaches, such as recurrent neural nets or deep neural nets, but is computationally more efficient. This tutorial focuses on Word2Vec for sentiment analysis.

Sentiment analysis is a challenging subject in machine learning. People express their emotions in language that is often obscured by sarcasm, ambiguity, and plays on words, all of which could be very misleading for both humans and computers. There's another Kaggle competition for movie review sentiment analysis. In this tutorial we explore how Word2Vec can be applied to a similar problem.

Deep learning has been in the news a lot over the past few years, even making it to the front page of the New York Times. These machine learning techniques, inspired by the architecture of the human brain and made possible by recent advances in computing power, have been making waves via breakthrough results in image recognition, speech processing, and natural language tasks. Recently, deep learning approaches won several Kaggle competitions, including a drug discovery task, and cat and dog image recognition.

# Tutorial overview
This tutorial will help you get started with Word2Vec for natural language processing. It has two goals:
- Basic Natural Language Processing: Part 1 of this tutorial is intended for beginners and covers basic natural language processing techniques, which are needed for later parts of the tutorial.
- Deep Learning for Text Understanding: In Parts 2 and 3, we delve into how to train a model using Word2Vec and how to use the resulting word vectors for sentiment analysis.
- Since deep learning is a rapidly evolving field, large amounts of the work has not yet been published, or exists only as academic papers. Part 3 of the tutorial is more exploratory than prescriptive; we experiment with several ways of using Word2Vec rather than giving you a recipe for using the output.
- To achieve these goals, we rely on an IMDB sentiment analysis data set, which has 100,000 multi-paragraph movie reviews, both positive and negative.

# Acknowledgements
This dataset was collected in association with the following publication:

Andrew L. Maas, Raymond E. Daly, Peter T. Pham, Dan Huang, Andrew Y. Ng, and Christopher Potts. (2011). "Learning Word Vectors for Sentiment Analysis." The 49th Annual Meeting of the Association for Computational Linguistics (ACL 2011).

# Evaluation
Submissions are judged on area under the ROC curve.

# What is Deep Learning?
The term "deep learning" was coined in 2006, and refers to machine learning algorithms that have multiple non-linear layers and can learn feature hierarchies.

Most modern machine learning relies on feature engineering or some level of domain knowledge to obtain good results. In deep learning systems, this is not the case; instead, algorithms can automatically learn feature hierarchies, which represent objects in increasing levels of abstraction. Although the basic ingredients of many deep learning algorithms have been around for many years, they are currently increasing in popularity for many reasons, including advances in compute power, the falling cost of computing hardware, and advances in machine learning research.

Deep learning algorithms can be categorized by their architecture (feed-forward, feed-back, or bi-directional) and training protocols (purely supervised, hybrid, or unsupervised).

Some good background materials include:
- "Deep Learning for Signal and Information Processing", by Li Deng and Dong Yu (out of Microsoft)
- "Deep Learning Tutorial" (2013 presentation by Yann LeCun and Marc'Aurelio Ranzato)

# Where does Word2Vec fit in?
Word2Vec works in a way that is similar to deep approaches such as recurrent neural nets or deep neural nets, but it implements certain algorithms, such as hierarchical softmax, that make it computationally more efficient.

In this tutorial, we use a hybrid approach to training; consisting of an unsupervised piece (Word2Vec) followed by supervised learning (the Random Forest).

# Libraries and packages
The lists below should in no way be considered exhaustive.

In Python:
- Theano offers very low-level, nuts and bolts functionality for building deep learning systems. You can also find some good tutorials on their site.
- Caffe is a deep learning framework out of the Berkeley Vision and Learning Center.
- Pylearn2 wraps Theano and seems slightly more user friendly.
- OverFeat was used to win the Kaggle Cats and Dogs competition.

In Lua:

Torch is a popular package and comes with a tutorial.

In R:

As of August 2014, there are a few packages just starting to be developed, but none are quite mature enough to be used in a tutorial.

There may be good packages in other languages as well, but we have not researched them.
