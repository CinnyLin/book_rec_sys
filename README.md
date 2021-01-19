# Improving Book Recommender SystemsUsing Reading Tags and Book Covers

## Team

Cinny Lin, Yingrong Mao, and Zhihan Yang

## Abstract

Our project aims to use the available features about users and books to improve recommendation accuracy for books.Initially, we planned to recommend books based on user features. However, after implementing k-means clustering, we realized that the customers purchase habits do not vary significantly according to demographics.

Then, we learned about item-based collaborative filtering, but also its limitation regarding scalability and cold-starts. Therefore, to offer more useful suggestions, we turned our task to a supervised learning problem.

In terms of dimensionality reduction, we tested stochastic gradient descent(SDG), alternating least squares (ALS) and singular vector decomposition (SVD) matrix factorization methods. While for the cold-start problem, we used popularity model and content-based filtering as complement.

Regarding content-based filtering, we built two models. We used Term Frequency-inverse Document Frequency (TF-iDF) on book tags. We also employed neural network models, incorporating the categorical and numerical book features as well as the images of book covers.

The aggregated performance of our models turned out pretty interesting. To our surprise, SVD did not yield very good results. We discovered that neural based model gives the best performance, reducing RMSE by 94% than the basic k-nearest neighbors (kNN) model. This result reveals that we could efficiently reach a larger customer base since we are able to recommend books accurately even when we know very little about our new users. More specifically, considering cover images when making book recommendationscan yield better results than only using text or numbers.
