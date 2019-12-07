Project Title: Yelp Rating Prediction

Our research focused on analyzing Yelp data to predict Pittsburgh 
restaurant’s ratings. We obtained data using Yelp API and web-scrapping. 
In our research, we performed prediction task using SVM, Logistic Regression 
and Support Vector Machine. After performing cross-validation and 
parameter tuning, SVM turned out to be the best model with accuracy of 
approximately 60 percent. This paper also identifies set of features that 
customers value the most in their evaluation of restaurants. 
Finally, we have performed clustering to identify how ratings could be 
grouped based on the reviews

We divided our codes into three different jupyter files:

File#1: "Yelp!Scraping.ipynb"
This file contains collects data from Yelp API and use python Beautiful Soup
to scrape reviews from the restaurant's site. As an output this file writes
all the collected data into json file. One thing to note here is that Yelp API
can be accessed using user's unique API key. 

File#2:"Yelp!Data_pre_processing.ipynb"
This chunk of codes takes in json file containing restaurants and reviews data
and performing following tasks: Tokenizing reveiws, Feature extraction from
reviews, One Hot Encoding of the features, Principal Component Analysis (PCA), 
and TSNE.

File#3: "Yelp_models.ipynb"
This chunk takes in processed data and apply Logistic Regression, SVM, and 
Random Forest model on the data. It performs cross validation, grid search,
and performanc evaluation of the models.   