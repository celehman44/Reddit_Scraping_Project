# Problem Statement:
In this project, I am attempting to answer the question: Do republicans and democrats discuss different topics? I think this is an interesting question, because it essentially judges how insular each political community is by finding out if their are inherent preferences towards only discussing certain topics (such as gun control, perhaps). If this is the case, then we can further investigate, and find out which topics divide the country politically. To achieve this, I will scrape posts from both republican and democratic subreddits, and then create a classification model to see if I can predict which subreddit the post came from. If I am able to do so with a high degree of accuracy, then it follows that democrats and republicans discuss different topics, or discuss the same topics but with differing sentiments. I will also look at word histograms of popular words form both subreddits, and perform t-tests between top words that appear in both subreddits to see if there is a statistically significant difference between the mean frequencies of the top words.

# Conclusion:
Here are the best scores for the three models I tried out:

Logistic Regression: $64.2\%$

K-nearest neighbors: $60.3\%$

Random forest: $65.9\%$

None of my models achieved an accuracy above $66%$, implying that democrats and republicans discuss similar topics and with similar sentiments. My best model was a random forest model on count vectorized data. I ran 7 t-tests between the top overlapping words, to find that 4/7 of the tests did not have evidence to reject the null hypothesis (which is that word x has the same mean frequency for democrat and republican subreddits), since this is a majority, it is further evidence that Republicans and Democrats discuss the same topics. One thing that was interesting to find was that sentiment analysis did not help my models at all. I believe this is the case because a majority of the posts were just news headlines that were void of sentiment. Further analysis should look at the comments in addition to the text/title of the post, because comments should contain more sentiment and thus help differentiate between the subreddits.

# Technologies used:

Python:

  sklearn
  Pandas
  numpy

GitHub

Reddit's API

Google slides
