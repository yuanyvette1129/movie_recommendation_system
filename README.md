# movie recommendation system

Check this link:
https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/1055051710907192/2338663335629870/842309477568637/latest.html

Summary: I used Spark ML-based tools to build a a recommendation system that uses over 100,000 data points to predict movie ratings for users, with an RMSE of 0.883.

Motivation: Recommendation has become an essential part in digital life. In terms of movie, people like to get suggestions when they are searching for a movie to watch. Like Netflix, it is important to have a robust recommendation system in order to attract more users and improve user experience.

Steps:
1. Extracted movie rating data from MovieLens and conducted OLAP with Spark SQL. The dataset contains more than 100000 ratings across 9724 movies that were rated by 610 users between 1996 and 2018.
2. Used an Alternating Least Square algorithm to train a recommendation model, and I used cross validation to get optimal parameters.
3. Evaluated the recommendation model by measuring the root-mean-square error of rating prediction. The final model reached a RMSE (root mean square error) of 0.883.
4. Recommended movies for a given user and computed similar movies for a given movie based on cosine similarity
