# Facebook_Posts_Classification
Introduction:
How can I best reach people and make an impact on Facebook? This a question that is often asked by people like retail sellers, influencers, and advertising companies. It is beneficial for them to determine the types of posts their consumers would be responsive to, therefore helping them decide how to advertise on Facebook. 

Goal: 
Develop a classification model to predict the type of Facebook post (photo, video, status, or link) based on the number of likes, comments, shares, and more that the post receives.

Data:
The dataset has Thailand Facebook post information from ten Thai fashion and cosmetics retail sellers from 2012 to 2018. The purpose of this dataset was intended to analyze the variability of consumer engagement, highlighting the changes induced by the use of Facebook Live. 
Pre-processed data acquired from the UCI Machine Learning Repository
7,051 rows
12 attributes
status ID
status type  (photo, video, status, link)
status published (date and time)
number of reactions, comments, shares, likes, loves, wows, hahas, sads, angrys

Visualizatioons:
Count plots showing the status type vs the  count of status type
Histogram of all numerical attributes num of likes, comments, and reactions 
Boxplot showing the type of posts vs the number of likes
Scatterplots for all numeric data to show correlations
Plot model showing the accuracy vs the number of neighbours 

Model:

Data Cleaning
Checked for missing values and outliers
No missing values in the data
Deleted unnecessary columns (last 4 columns empty)
Feature construction
Changed status type to numeric
Exploratory Data Analysis
Basic statistics
Attribute descriptions
Correlation
Attributes Used in Model: number of reactions, comments, shares, likes, loves, wows, hahas, sads, angrys

Model - Tree Based Classification
Split the data into training and test sets using 80% for training and 20% for testing
Used a Tree-based classifier for model building
Used metrics to evaluate the Accuracy evaluation
Used Confusion matrix for evaluation
Model - K-Nearest Neighbors Classification
Split data into training and test sets
Applied KNN classification to training model and then to testing model using k=5
Used Confusion matrix to evaluate the model

Results:
Compare results from Tree based and KNN:
Accuracy evaluation for Tree-Based :
Train set Accuracy:  93%
Test set Accuracy:  76%
Accuracy evaluation for KNN:
Train set Accuracy:  82%
Test set Accuracy:  77%
Findings:

We can conclude that using tree-based classification results in a higher accuracy rate than using K-NN based classification  

Conclusion:
There were a total number of 4288 photos, 2334 videos, 365 statuses and 63 links.
The attributes we used in our models, including the number of reactions, comments, shares, likes, loves, wows, hahas, sads, and angrys that a Facebook post receives, were able to classify the type of Facebook post with a fairly high accuracy rate.
According to this data, it seems like video posts and then photo posts receive the most response on Facebook (shown in bar chart above).
Videos receive the most comments.
Photos receive the most reactions and likes


