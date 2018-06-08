# TalkingAd-Solution
Kaggle - TalkingData AdTracking Fraud Detection Challenge Solution (Public LB: 0.9810276, Private LB: 0.9819337)

Event rate of target variable was less than 1%, so one of the many challanges was Class imbalance. So decided to give Downsampling a shot and it worked wonders for me.

The original training set had more than 180 million rows. After downsampling, my new training set was 940K rows only which had almost equal proportion of positive and negative samples. Other than that, lots of feature engineering was done and all the  features were generated using BigQuery, since it turned out to be lightning quick and moreover python gives a huge memory spike when you are merging datframes and in turn memory issues. But that doesn't affect my love for Python, not even a bit.

Boosting algorithm used - LightGBM with lots of hyperparameter tuning


