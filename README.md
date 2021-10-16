# Boston Airbnb Listing 2021

## Table of Contents
- Project Background
- Data Source
- Libraries Used
- Motivation for The Project
- Files
- Summary of the results
- Acknowledgment


Project Background
This project is to analyze Airbnb listing data on Boston 2021. (Latest scraped data from Airbnb OpenData at the time of writing)

Data Source
[http://insideairbnb.com/get-the-data.html][1]
[http://data.insideairbnb.com/united-states/ma/boston/2021-09-19/data/listings.csv.gz][2] (19 September, 2021)

Libraries Used
- numpy
- pandas
- matplotlib
- sklearn
- (Python 3.9 / Jupyter Notebook)

Motivation for The Project
The main goal is to build a Airbnb Listing Price Estimator model by implementing machine learning from Boston 2021 data to generate a LinearRegression model. 
Host, agency, or end user can use this model to estimate / predict  listing prices by inputing some independent variables. 
I also tried to find out what most recent amenities are listed in Boston listing that new host might considering for his/her new listing. And some others like: most demanded/popular districts; price ranges distribution.

Files
- /files/Boston_airbnb_2021/listings.csv
- boston_airbnb_2021_refactor.ipynb_

Summary of the results
The Boston Airbnb Price Estimator/Predictor model I built based on this dataset is able to achieve 0.62 R-squared for training score, and 0.6 r-squared score for test score. The model can explain at least 60% of the variabilities of the data. 


Acknowledgment
- Code snipped used about the function of train_test_split, coef_weights, and train test from udacity example. _
- Plot on price range distribution inspired by the book “Data Science from Scratch” - Visualization chapter. 
- Some helper functions solution founds on StackOverflow. 

[1]:	http://insideairbnb.com/get-the-data.html
[2]:	http://data.insideairbnb.com/united-states/ma/boston/2021-09-19/data/listings.csv.gz