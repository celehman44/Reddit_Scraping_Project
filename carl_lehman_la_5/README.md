# Problem Statement:
In this project, I am attempting to answer the question: Do republicans and democrats discuss different topics? To do so, I will scrape posts from both republican and democratic subreddits, and then create a classification model to see if I can predict which subreddit the post came from. If I am able to do so with a high degree of accuracy, then it follows that democrats and republicans discuss different topics, or discuss the same topics but with differing sentiments. I will also look at word histograms of popular words form both subreddits, and perform t-tests between top words that appear in both subreddits to see if there is a statistically significant difference between the mean frequencies of the top words.

# Conclusion:
Here are the scores for the three models I tried out:

Logistic Regression: $65.9\%$

K-nearest neighbors: $61.1\%$

Random forest: $60.0\%$

None of my models achieved an accuracy above $65%$, implying that democrats and republicans discuss similar topics and with similar sentiments. My best model turned out to be a simple logistic regression model on a TFIDF matrix, although this model performed only marginally better than my other two models.

# Technologies used:
Python:
  sklearn
  Pandas
  numpy

GitHub

Reddit's API

Google slides
