# Restaurant-Recommendation-System

A recommendation system for restaurants using collaborative filtering (CF). We will be using the Yelp Dataset for this. 

The project is divided in 3 jupyter notebooks

## 1. Getting Data Ready
Here we explore data. Do some simple null handling and type casting. As the data size is too big to load on RAM, we send data into a SQLite database chunk by chunk. This database can be later used for EDA and Modelling. We are using yelp dataset for this project. The Yelp dataset is a subset of yelp's businesses, reviews, and user data for use in personal, educational, and academic purposes.

## 2. Exploratory Data Analysis (EDA)
With the database created we explore created tables. We study distribution of data. We see some interesting patterns and observations. This step helps us get a better understanding about our data. 

## 3. Modelling
In modelling, we write our restaurant recommendation engine. We first get a baseline score from an average model. Then to improve on baseline we build a neural network that uses embeddings to represent users and restaurants. We predict rating a user would have given if he had been to a particular restaurant. We use collaborative filtering for the same. We also deploy our recommendation engine by creating a recommend function, which takes user as input and recommends new restaurants for that user. 