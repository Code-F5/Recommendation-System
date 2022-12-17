# Recommendation-System
Recommendation System with NLP &amp; KNN 
Anime Recommendation System (INFO7390 Advances Data Sci/Architecture)



Goal:

Recommender systems ain to predict users interests and recommend product items that quite likely are interesting for them. They are among the most powerful machine learning systems that online retailers implement in order to drive sales.

Dataset:

We have picked the dataset from Kaggle. This Dataset includes various columns such as anime name, genre, duration, rating, aired, etc which help us in carrying out analysis and 
helping us deploy the desired anime recommendation system.

Link: https://www.kaggle.com/datasets/azathoth42/myanimelist
Content:
The dataset contains 3 files:
•	AnimeList.csv contains list of anime, with title, title synonyms, genre, studio, licensor, producer, duration, rating, score, airing date, episodes, source (manga, light novel etc.) and many other important data about individual anime providing sufficient information about trends in time about important aspects of anime. Rank is in float format in csv, but it contains only integer value. This is due to Nan values and their representation in pandas.
•	UserList.csv contains information about users who watch anime, namely username, registration date (join date), last online date, birth date, gender, location, and lots of aggregated values from their anime lists.
•	UserAnimeList.csv contains anime lists of all users. Per each record, here is username, anime ID, score, status and timestamp when was this record last updated.
The dataset as a whole contains: 
•	302 675 unique users
•	302 573 of them with some demographic data
•	80 076 112 records in anime lists
•	46 358 322 of them have ratings
•	14 478 unique anime
There is filtered version of dataset is contained in files animefiltered.csv, animelistsfiltered.csv and users_filtered.csv. It consists of users who have birth date, location and gender filled. So, it contains lot less animalists data.
But all-important characteristics like rating mean and variation, or genres in animalists is unchanged when omitting users with some missing data, so even with filtered data we should get same information.



The filtered dataset contains:
•	116 133 unique users with demographic data
•	35 802 010 records in anime lists
•	20 726 794 of them have ratings
•	14 474 unique anime


Problem Statement: 

The anime universe is vast and has an even larger fanbase. After getting done with one anime one is always curious to start another one but also in fear of wasting time watching something which is outside of their area of liking.
Every streaming content has its own viewers and each content has its rating. Viewers leave some good ratings for the content if they like it. But where does it apply? Viewers can spend hours scrolling through hundreds, sometimes thousands of anime's never finding a content they like. Business need to be provided suggestions based on their likes and needs in order to create a better streaming environment that boosts revenue and increases the time spent on a website.

Solution:

It is an unsupervised learning algorithm (one that does not have a target variable to measure accuracy against) mostly used to aid in consumer decision making. I’m sure you have seen them while online shopping. They also appear in places like streaming apps (aka Netflix and Hulu) to help you select a TV show or movie to watch next and on journalism/media websites like Medium to suggest other articles you may like to read, among many other uses. Obviously, many e-retailers like Amazon have already been using recommender algorithms for quite some time, but many smaller or newer sites are still in need. There are different varieties of recommenders that base their predictions on different features.
Our recommendation system makes use of different algorithms such as KNN, NLP with LDA and LSA to recommend the user, anime with relevant anime as per their liking.
This helps the users to not spend time on deciding on the next anime without having to try each other anime they know.
In the first recommendation system we use the KNN algorithm which stands for K Nearby Neighbours which uses the ‘Euclidean Distance’ to find out the distance of the given data point from each core.
After it finds out the distance, the data point is allocated in the cluster of whose core is nearest to the data point. This process is carried out on all of the data points and then the clusters of data points having similar characteristics is formed.
In the second approach we are using the LSA algorithm, the acronym stands for Latent Semantic Analysis. It uses the meaning of the word and considers that words with similar meaning are bound to appear together. It is a mathematical method of modelling and simulation of meanings of words by analysis of representative corpora of natural text. 
The third approach was by using the LDA which stands for Linear Discriminant Analysis. In order to avoid the curse of dimensionality, as well as to save resources and minimize dimensional expenses, LDA projects features from higher dimensional space onto a lower dimensional space.

