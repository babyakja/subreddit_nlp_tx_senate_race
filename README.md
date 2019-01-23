# NLP on the 2018 Texas Race using the Reddit API
## Objective
Using the tools learned in General Assembley's Data Science Immersive course, we will collect data via an API request and then building a binary predictor.
In particular, we will apply this in the realm of Reddit. Using NLP, what characteristics of a post on Reddit contribute most to which subreddit it belongs to? Our data will focus on Texas Senate race between Ted Cruz (R) and Beto O'Rourke (D).

Python Packages Used:
  - Pandas
  - Numpy
  - Scikit-Learn
  
## Data Collection

Build function to scrape reddit with inputs of _subreddit name_ and _number of pages to pull_
Reddit's API is limited to the last 1000 post for any subreddit, so how active a subreddit is can determine how frequently it is necessary to pull pages.

Clean data into useful corpus and assign each with a label of it's subreddit source. This creates domain specific training data that then can be used to classify new data.

## Modeling
Classification
- Use GridSearch and Pipelines to find best predictive model
  Run through different model types and GridSearch hyperparameters to tune for best performance
- Metric Targeted: __Accuracy__

## Findings
We can apply our model to a different Reddit subreddit to gauge the pulse and discussion of untagged posts. We will reference r/Texas with politic flags to see what this 'neutral' space is discussing more in terms of candidates.

After supplying r/texas data into the model, 69% of posts were geared toward Beto while 31% was geared towards Cruz. This initially indicates an advantage for Beto being the center of discussion but the sentiment for each post needs to be factored in as well.



## Conclusion

Although we had a model that performed at a accuracy of 94%, the context of the discussion was heavily negative for both candidates for classification with a high probability.
