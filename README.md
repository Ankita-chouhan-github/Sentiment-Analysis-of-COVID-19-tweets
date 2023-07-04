# Sentiment-Analysis-of-COVID-19-tweets

**INTRODUCTION**

The coronavirus disease 2019 (COVID-19) pandemic has influenced the everyday life of people around the globe. In general and during lockdown phases, people worldwide use social media network to state their viewpoints and general feelings concerning the pandemic that has hampered their daily lives. Twitter is one of the most commonly used social media platforms, and it showed a massive increase in tweets related to coronavirus, including positive, negative, and neutral tweets, in a minimal period. The researchers move toward the sentiment analysis and analyze the various emotions of the public toward COVID-19 due to the diverse nature of tweets. Meanwhile, people have expressed their feelings regarding the vaccinations' safety and effectiveness on social networking sites such as Twitter. As an advanced step, in this project, our proposed approach analyzes COVID-19 by focusing on Twitter users who share their opinions on this social media networking site. The proposed approach analyzes collected tweets' sentiments for sentiment classification using various feature sets and classifiers. The early detection of COVID-19 sentiments from collected tweets allow for a better understanding and handling of the pandemic. Tweets are categorized into positive, negative, and neutral sentiment classes. We evaluate the performance of machine learning (ML) classifiers.
The present prediction analysis is based on the tweets done between the months of March and April, 2020 which is the first wave of COVID-19 pandemic disease. Coronavirus disease (COVID-19) is an infectious disease caused by the SARS-CoV-2 virus. Henceforth, due to panic situation people started tweeting on Twitter (it is social media platform) following with different sentiments associated with that. The present provided dataset consist of (41157, 6) numbers of rows and columns. But our present prediction analysis performed using two columns only of original tweets and sentiments. 5 types of sentiments were provided namely: Extremely Positive, Positive, Neutral, Negative and Extremely Negative.

**PROBLEM STATEMENT**

This challenge asks you to build a classification model to predict the sentiment of COVID-19 tweets. The tweets have been pulled from Twitter and manual tagging has been done then.

**OBJECTIVE**

The CoVid-19 pandemic has shaken the very foundation of society wherein people were forced to live inside their houses because of the lockdown being imposed and also the livelihood of almost every section of the society was impacted.

The objective of our analysis revolved around knowing the sentiments of people from their tweets on Twitter as Twitter is one of the prime means of expression over social media.

**APPROACH**

* Text Preprocessing
* Exploratory Data Analysis
* Model Preprocessing
* Model Training

**ALGORITHM USED**

* Logistic Regression with Grid Search CV
* Decision Tree Classifier
* XG Boost
* Random Forest
* KNN for both Count Vector and TF ID Vectorization techniques.

**PROBLEM FACED**

* Text preprocessing.
* Vectorization.
* Model Training and performance improvement

**CONCLUSION**

**On EDA**

* Original dataset contains 6 columns and 41157 rows.

* ‘Location’ column contains approx. 20.87% of Null values.

* The columns such as “UserName” and “ScreenName” does not give any meaningful insights for our analysis.

* In order to analyse the data we required only the following columns "OriginalTweet", "Sentiment", "Location", "TweetAt".

* There are five types of sentiments- Extremely Negative, Negative, Neutral, Positive and Extremely Positive. So, we merged Extremely Positive with positive and Extremely Negative with Negative. And use encoding with value ‘-1’ for negative, ‘0’ for neutral and ‘1’ for positive.

* All tweets data collected between months of March and April 2020 and of around 30 days.

* Most of the tweets came from London followed by U.S.

* Among top 10 mentions in tweets realDonaldTrump was the top mentioned name and "#coronavirus" was most trendiest hashtag that was trending during that period.

**On Model Training**

* We applied 5 different machine learing models namely, Logistic Regression with Grid Search CV, Desision Tree Classifier, XG Boost, RandomForest with GridSearchCV and KNN for both Count Vector And TF IDF Vectorisation techniques.
* All the models are performing better with Count vectoriser compared to TF/IDF vectoriser.
* We conclude that the machine is generating best results for Logistic Regression with Grid Search CV model with and Accuracy score of 79.32% and 78.96% respectively for Count vector and TF/idf Vector, followed by XGBoost and RandomForest. K-NN seems to be performing the worst among all the models.
* Also, we observed that no overfitting is seen for the data, and we can deploy this model.
* The sentiments of future tweets can be easily predicted using this model.
